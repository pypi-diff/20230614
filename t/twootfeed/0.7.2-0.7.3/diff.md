# Comparing `tmp/twootfeed-0.7.2.tar.gz` & `tmp/twootfeed-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twootfeed-0.7.2.tar", last modified: Sat Aug 27 08:38:22 2022, max compression
+gzip compressed data, was "twootfeed-0.7.3.tar", last modified: Wed Jun 14 19:56:39 2023, max compression
```

## Comparing `twootfeed-0.7.2.tar` & `twootfeed-0.7.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2022-08-27 08:38:22.651258 twootfeed-0.7.2/
--rw-r--r--   0 sam       (1000) sam       (1000)     1072 2018-12-23 17:33:37.000000 twootfeed-0.7.2/LICENCE
--rw-r--r--   0 sam       (1000) sam       (1000)       15 2021-10-05 08:39:09.000000 twootfeed-0.7.2/MANIFEST.in
--rw-r--r--   0 sam       (1000) sam       (1000)     2850 2022-08-27 08:38:22.651258 twootfeed-0.7.2/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)     1904 2022-08-27 08:30:17.000000 twootfeed-0.7.2/README.md
--rw-r--r--   0 sam       (1000) sam       (1000)        6 2022-08-27 08:32:00.000000 twootfeed-0.7.2/VERSION
--rw-r--r--   0 sam       (1000) sam       (1000)      297 2022-07-16 10:01:49.000000 twootfeed-0.7.2/pyproject.toml
--rw-r--r--   0 sam       (1000) sam       (1000)     2058 2022-08-27 08:38:22.651258 twootfeed-0.7.2/setup.cfg
--rw-r--r--   0 sam       (1000) sam       (1000)       61 2018-12-23 19:02:28.000000 twootfeed-0.7.2/setup.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2022-08-27 08:38:22.651258 twootfeed-0.7.2/twootfeed/
--rw-r--r--   0 sam       (1000) sam       (1000)     1471 2022-08-27 06:24:00.000000 twootfeed-0.7.2/twootfeed/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1195 2022-07-16 10:01:49.000000 twootfeed-0.7.2/twootfeed/__main__.py
--rwxr-xr-x   0 sam       (1000) sam       (1000)      699 2022-07-16 10:01:49.000000 twootfeed-0.7.2/twootfeed/config.example.yml
--rw-r--r--   0 sam       (1000) sam       (1000)      574 2022-07-16 10:01:49.000000 twootfeed-0.7.2/twootfeed/config.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2022-08-27 08:38:22.651258 twootfeed-0.7.2/twootfeed/mastodon/
--rw-r--r--   0 sam       (1000) sam       (1000)        0 2018-12-23 17:33:37.000000 twootfeed-0.7.2/twootfeed/mastodon/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)     7810 2022-08-27 07:02:29.000000 twootfeed-0.7.2/twootfeed/mastodon/generate_toots_feed.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1095 2022-07-16 10:01:49.000000 twootfeed-0.7.2/twootfeed/mastodon/get_api.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1639 2022-08-27 06:24:00.000000 twootfeed-0.7.2/twootfeed/mastodon/routes.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2022-08-27 08:38:22.651258 twootfeed-0.7.2/twootfeed/twitter/
--rw-r--r--   0 sam       (1000) sam       (1000)        0 2018-12-23 17:33:37.000000 twootfeed-0.7.2/twootfeed/twitter/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)     7071 2022-08-27 06:48:40.000000 twootfeed-0.7.2/twootfeed/twitter/generate_tweets_feed.py
--rw-r--r--   0 sam       (1000) sam       (1000)      777 2022-07-16 10:01:49.000000 twootfeed-0.7.2/twootfeed/twitter/get_api.py
--rw-r--r--   0 sam       (1000) sam       (1000)      548 2022-07-16 10:01:49.000000 twootfeed-0.7.2/twootfeed/twitter/routes.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2022-08-27 08:38:22.651258 twootfeed-0.7.2/twootfeed/utils/
--rw-r--r--   0 sam       (1000) sam       (1000)        0 2018-12-23 17:33:37.000000 twootfeed-0.7.2/twootfeed/utils/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1439 2022-07-16 10:01:49.000000 twootfeed-0.7.2/twootfeed/utils/config.py
--rwxr-xr-x   0 sam       (1000) sam       (1000)     2636 2022-07-16 10:01:49.000000 twootfeed-0.7.2/twootfeed/utils/create_mastodon_client.py
--rw-r--r--   0 sam       (1000) sam       (1000)      554 2022-07-16 10:01:49.000000 twootfeed-0.7.2/twootfeed/utils/decorator.py
--rw-r--r--   0 sam       (1000) sam       (1000)       98 2022-07-16 10:01:49.000000 twootfeed-0.7.2/twootfeed/utils/exceptions.py
--rw-r--r--   0 sam       (1000) sam       (1000)      748 2022-07-16 10:01:49.000000 twootfeed-0.7.2/twootfeed/utils/feed_generation.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2022-08-27 08:38:22.651258 twootfeed-0.7.2/twootfeed.egg-info/
--rw-r--r--   0 sam       (1000) sam       (1000)     2850 2022-08-27 08:38:22.000000 twootfeed-0.7.2/twootfeed.egg-info/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)      847 2022-08-27 08:38:22.000000 twootfeed-0.7.2/twootfeed.egg-info/SOURCES.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        1 2022-08-27 08:38:22.000000 twootfeed-0.7.2/twootfeed.egg-info/dependency_links.txt
--rw-r--r--   0 sam       (1000) sam       (1000)      181 2022-08-27 08:38:22.000000 twootfeed-0.7.2/twootfeed.egg-info/entry_points.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        1 2022-08-27 08:38:22.000000 twootfeed-0.7.2/twootfeed.egg-info/not-zip-safe
--rw-r--r--   0 sam       (1000) sam       (1000)      282 2022-08-27 08:38:22.000000 twootfeed-0.7.2/twootfeed.egg-info/requires.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       10 2022-08-27 08:38:22.000000 twootfeed-0.7.2/twootfeed.egg-info/top_level.txt
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-14 19:56:39.681941 twootfeed-0.7.3/
+-rw-r--r--   0 sam       (1000) sam       (1000)     1072 2018-12-23 17:33:37.000000 twootfeed-0.7.3/LICENCE
+-rw-r--r--   0 sam       (1000) sam       (1000)       15 2021-10-05 08:39:09.000000 twootfeed-0.7.3/MANIFEST.in
+-rw-r--r--   0 sam       (1000) sam       (1000)     2789 2023-06-14 19:56:39.681941 twootfeed-0.7.3/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)     1817 2023-06-14 19:49:28.000000 twootfeed-0.7.3/README.md
+-rw-r--r--   0 sam       (1000) sam       (1000)        6 2023-06-14 19:49:28.000000 twootfeed-0.7.3/VERSION
+-rw-r--r--   0 sam       (1000) sam       (1000)      297 2022-07-16 10:01:49.000000 twootfeed-0.7.3/pyproject.toml
+-rw-r--r--   0 sam       (1000) sam       (1000)     2041 2023-06-14 19:56:39.681941 twootfeed-0.7.3/setup.cfg
+-rw-r--r--   0 sam       (1000) sam       (1000)       61 2018-12-23 19:02:28.000000 twootfeed-0.7.3/setup.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-14 19:56:39.678608 twootfeed-0.7.3/twootfeed/
+-rw-r--r--   0 sam       (1000) sam       (1000)     1471 2022-08-27 06:24:00.000000 twootfeed-0.7.3/twootfeed/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1195 2022-07-16 10:01:49.000000 twootfeed-0.7.3/twootfeed/__main__.py
+-rwxr-xr-x   0 sam       (1000) sam       (1000)      699 2022-07-16 10:01:49.000000 twootfeed-0.7.3/twootfeed/config.example.yml
+-rw-r--r--   0 sam       (1000) sam       (1000)      574 2022-07-16 10:01:49.000000 twootfeed-0.7.3/twootfeed/config.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-14 19:56:39.678608 twootfeed-0.7.3/twootfeed/mastodon/
+-rw-r--r--   0 sam       (1000) sam       (1000)        0 2018-12-23 17:33:37.000000 twootfeed-0.7.3/twootfeed/mastodon/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     7810 2023-06-14 18:52:27.000000 twootfeed-0.7.3/twootfeed/mastodon/generate_toots_feed.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1094 2023-06-14 19:49:28.000000 twootfeed-0.7.3/twootfeed/mastodon/get_api.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1639 2022-08-27 06:24:00.000000 twootfeed-0.7.3/twootfeed/mastodon/routes.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-14 19:56:39.678608 twootfeed-0.7.3/twootfeed/twitter/
+-rw-r--r--   0 sam       (1000) sam       (1000)        0 2018-12-23 17:33:37.000000 twootfeed-0.7.3/twootfeed/twitter/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     7071 2022-08-27 06:48:40.000000 twootfeed-0.7.3/twootfeed/twitter/generate_tweets_feed.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      777 2022-07-16 10:01:49.000000 twootfeed-0.7.3/twootfeed/twitter/get_api.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      548 2022-07-16 10:01:49.000000 twootfeed-0.7.3/twootfeed/twitter/routes.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-14 19:56:39.681941 twootfeed-0.7.3/twootfeed/utils/
+-rw-r--r--   0 sam       (1000) sam       (1000)        0 2018-12-23 17:33:37.000000 twootfeed-0.7.3/twootfeed/utils/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1439 2022-07-16 10:01:49.000000 twootfeed-0.7.3/twootfeed/utils/config.py
+-rwxr-xr-x   0 sam       (1000) sam       (1000)     2560 2023-06-14 19:49:28.000000 twootfeed-0.7.3/twootfeed/utils/create_mastodon_client.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      554 2022-07-16 10:01:49.000000 twootfeed-0.7.3/twootfeed/utils/decorator.py
+-rw-r--r--   0 sam       (1000) sam       (1000)       98 2022-07-16 10:01:49.000000 twootfeed-0.7.3/twootfeed/utils/exceptions.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      747 2023-06-14 19:49:28.000000 twootfeed-0.7.3/twootfeed/utils/feed_generation.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-14 19:56:39.678608 twootfeed-0.7.3/twootfeed.egg-info/
+-rw-r--r--   0 sam       (1000) sam       (1000)     2789 2023-06-14 19:56:39.000000 twootfeed-0.7.3/twootfeed.egg-info/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)      847 2023-06-14 19:56:39.000000 twootfeed-0.7.3/twootfeed.egg-info/SOURCES.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-06-14 19:56:39.000000 twootfeed-0.7.3/twootfeed.egg-info/dependency_links.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)      181 2023-06-14 19:56:39.000000 twootfeed-0.7.3/twootfeed.egg-info/entry_points.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-06-14 19:56:39.000000 twootfeed-0.7.3/twootfeed.egg-info/not-zip-safe
+-rw-r--r--   0 sam       (1000) sam       (1000)      260 2023-06-14 19:56:39.000000 twootfeed-0.7.3/twootfeed.egg-info/requires.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       10 2023-06-14 19:56:39.000000 twootfeed-0.7.3/twootfeed.egg-info/top_level.txt
```

### Comparing `twootfeed-0.7.2/LICENCE` & `twootfeed-0.7.3/LICENCE`

 * *Files identical despite different names*

### Comparing `twootfeed-0.7.2/PKG-INFO` & `twootfeed-0.7.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: twootfeed
-Version: 0.7.2
+Version: 0.7.3
 Summary: generate a rss feed from Twitter or Mastodon search
 Home-page: https://github.com/SamR1/python-twootfeed
 Author: SamR1
 License: The MIT License (MIT)
 Project-URL: Documentation, https://samr1.github.io/python-twootfeed
 Keywords: rss,twitter,mastodon,search
 Platform: linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
+Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doc
 License-File: LICENCE
 
 # python-twootfeed
 **generate an RSS feed from parsed Twitter or Mastodon search and Mastodon bookmarks/favorites/home timeline**  
   
 [![PyPI version](https://img.shields.io/pypi/v/twootfeed.svg)](https://pypi.org/project/twootfeed/)
-[![Downloads](https://pepy.tech/badge/twootfeed)](https://pepy.tech/project/twootfeed)
-[![Python Version](https://img.shields.io/badge/python-3.7+-brightgreen.svg)](https://python.org) 
-[![Flask Version](https://img.shields.io/badge/flask-2.2-brightgreen.svg)](http://flask.pocoo.org/)
+[![Python Version](https://img.shields.io/badge/python-3.8+-brightgreen.svg)](https://python.org) 
+[![Flask Version](https://img.shields.io/badge/flask-2.3-brightgreen.svg)](http://flask.pocoo.org/)
 [![code style: black](https://img.shields.io/badge/code%20style-black-black)](https://black.readthedocs.io/en/stable/) 
 [![type check: mypy](https://img.shields.io/badge/type%20check-mypy-blue)](http://mypy-lang.org/)  
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/14d1c00121c04cd2b81453c597639ca6)](https://www.codacy.com/app/SamR1/python-twootfeed) 
 [![Coverage Status](https://coveralls.io/repos/github/SamR1/python-twootfeed/badge.svg?branch=master)](https://coveralls.io/github/SamR1/python-twootfeed?branch=master) 
 [![pipeline status](https://gitlab.com/SamR1/python-twootfeed/badges/master/pipeline.svg)](https://gitlab.com/SamR1/python-twootfeed/commits/master)
 
 ---
```

### Comparing `twootfeed-0.7.2/README.md` & `twootfeed-0.7.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # python-twootfeed
 **generate an RSS feed from parsed Twitter or Mastodon search and Mastodon bookmarks/favorites/home timeline**  
   
 [![PyPI version](https://img.shields.io/pypi/v/twootfeed.svg)](https://pypi.org/project/twootfeed/)
-[![Downloads](https://pepy.tech/badge/twootfeed)](https://pepy.tech/project/twootfeed)
-[![Python Version](https://img.shields.io/badge/python-3.7+-brightgreen.svg)](https://python.org) 
-[![Flask Version](https://img.shields.io/badge/flask-2.2-brightgreen.svg)](http://flask.pocoo.org/)
+[![Python Version](https://img.shields.io/badge/python-3.8+-brightgreen.svg)](https://python.org) 
+[![Flask Version](https://img.shields.io/badge/flask-2.3-brightgreen.svg)](http://flask.pocoo.org/)
 [![code style: black](https://img.shields.io/badge/code%20style-black-black)](https://black.readthedocs.io/en/stable/) 
 [![type check: mypy](https://img.shields.io/badge/type%20check-mypy-blue)](http://mypy-lang.org/)  
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/14d1c00121c04cd2b81453c597639ca6)](https://www.codacy.com/app/SamR1/python-twootfeed) 
 [![Coverage Status](https://coveralls.io/repos/github/SamR1/python-twootfeed/badge.svg?branch=master)](https://coveralls.io/github/SamR1/python-twootfeed?branch=master) 
 [![pipeline status](https://gitlab.com/SamR1/python-twootfeed/badges/master/pipeline.svg)](https://gitlab.com/SamR1/python-twootfeed/commits/master)
 
 ---
```

### Comparing `twootfeed-0.7.2/setup.cfg` & `twootfeed-0.7.3/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -12,52 +12,51 @@
 classifiers = 
 	Development Status :: 4 - Beta
 	Framework :: Flask
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Internet :: WWW/HTTP
 project_urls = 
 	Documentation = https://samr1.github.io/python-twootfeed
 
 [options]
 packages = find:
+python_requires = >=3.8.1
 zip_safe = false
 setup_requires = pytest-runner
 install_requires = 
-	beautifulsoup4==4.11.1
-	feedgenerator==2.0.0
-	Flask==2.2.2
+	beautifulsoup4==4.12.2
+	feedgenerator==2.1.0
+	Flask==2.3.2
 	gunicorn==20.1.0
-	Mastodon.py==1.5.1
-	pytz==2022.2.1
+	Mastodon.py==1.8.1
+	pytz==2023.3
 	PyYAML==6.0.0
-	tweepy==4.10.1
+	tweepy==4.14.0
 tests_require = 
-	flake8<5.0.0
+	flake8
 	mypy
 	pytest-cov
-	pytest-flake8
 	pytest-isort
 	pytest-black
 	types-pytz
 	types-PyYAML
 include_package_data = True
 
 [options.extras_require]
 test = 
-	flake8<5.0.0
+	flake8
 	mypy
 	pytest-cov
-	pytest-flake8
 	pytest-isort
 	pytest-black
 	types-pytz
 	types-PyYAML
 doc = 
 	sphinx
 	sphinx_rtd_theme
```

### Comparing `twootfeed-0.7.2/twootfeed/__init__.py` & `twootfeed-0.7.3/twootfeed/__init__.py`

 * *Files identical despite different names*

### Comparing `twootfeed-0.7.2/twootfeed/__main__.py` & `twootfeed-0.7.3/twootfeed/__main__.py`

 * *Files identical despite different names*

### Comparing `twootfeed-0.7.2/twootfeed/config.example.yml` & `twootfeed-0.7.3/twootfeed/config.example.yml`

 * *Files identical despite different names*

### Comparing `twootfeed-0.7.2/twootfeed/config.py` & `twootfeed-0.7.3/twootfeed/config.py`

 * *Files identical despite different names*

### Comparing `twootfeed-0.7.2/twootfeed/mastodon/generate_toots_feed.py` & `twootfeed-0.7.3/twootfeed/mastodon/generate_toots_feed.py`

 * *Files identical despite different names*

### Comparing `twootfeed-0.7.2/twootfeed/mastodon/get_api.py` & `twootfeed-0.7.3/twootfeed/mastodon/get_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,14 @@
         mastodon_param = param['mastodon']
         client_file = default_directory + mastodon_param['client_id_file']
         access_token_file = (
             default_directory + mastodon_param['access_token_file']
         )
 
         if os.path.isfile(client_file) and os.path.isfile(access_token_file):
-
             mastodon_url = param['mastodon'].get(
                 'url', 'https://mastodon.social'
             )
             mastodon_api = Mastodon(
                 client_id=client_file,
                 access_token=access_token_file,
                 api_base_url=mastodon_url,
```

### Comparing `twootfeed-0.7.2/twootfeed/mastodon/routes.py` & `twootfeed-0.7.3/twootfeed/mastodon/routes.py`

 * *Files identical despite different names*

### Comparing `twootfeed-0.7.2/twootfeed/twitter/generate_tweets_feed.py` & `twootfeed-0.7.3/twootfeed/twitter/generate_tweets_feed.py`

 * *Files identical despite different names*

### Comparing `twootfeed-0.7.2/twootfeed/twitter/get_api.py` & `twootfeed-0.7.3/twootfeed/twitter/get_api.py`

 * *Files identical despite different names*

### Comparing `twootfeed-0.7.2/twootfeed/twitter/routes.py` & `twootfeed-0.7.3/twootfeed/twitter/routes.py`

 * *Files identical despite different names*

### Comparing `twootfeed-0.7.2/twootfeed/utils/config.py` & `twootfeed-0.7.3/twootfeed/utils/config.py`

 * *Files identical despite different names*

### Comparing `twootfeed-0.7.2/twootfeed/utils/create_mastodon_client.py` & `twootfeed-0.7.3/twootfeed/utils/create_mastodon_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,15 +62,14 @@
         scopes=['read'],
     )
 
     click.echo('\nVerifying credentials...')
     try:
         mastodon.account_verify_credentials()
         click.secho("Credentials look good", fg='green')
-        click.echo("Client reports user\'s account name is: {res['acct']}")
         click.echo(
             f"Configuration complete, app should appear at: "
             f"{mast_cfg['url']}/oauth/authorized_applications"
         )
         click.echo(
             'You should not need to log in again unless this app is '
             'removed or credentials expire.'
```

### Comparing `twootfeed-0.7.2/twootfeed/utils/decorator.py` & `twootfeed-0.7.3/twootfeed/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `twootfeed-0.7.2/twootfeed/utils/feed_generation.py` & `twootfeed-0.7.3/twootfeed/utils/feed_generation.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import feedgenerator
 
 
 def generate_feed(
     title: str, link: str, param: Dict, description: Optional[str] = None
 ) -> feedgenerator.Rss201rev2Feed:
-
     return feedgenerator.Rss201rev2Feed(
         title=title,
         link=link,
         description=(
             description if description else param['twitter']['description']
         ),
         language=param['feed']['language'],
```

### Comparing `twootfeed-0.7.2/twootfeed.egg-info/PKG-INFO` & `twootfeed-0.7.3/twootfeed.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: twootfeed
-Version: 0.7.2
+Version: 0.7.3
 Summary: generate a rss feed from Twitter or Mastodon search
 Home-page: https://github.com/SamR1/python-twootfeed
 Author: SamR1
 License: The MIT License (MIT)
 Project-URL: Documentation, https://samr1.github.io/python-twootfeed
 Keywords: rss,twitter,mastodon,search
 Platform: linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
+Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doc
 License-File: LICENCE
 
 # python-twootfeed
 **generate an RSS feed from parsed Twitter or Mastodon search and Mastodon bookmarks/favorites/home timeline**  
   
 [![PyPI version](https://img.shields.io/pypi/v/twootfeed.svg)](https://pypi.org/project/twootfeed/)
-[![Downloads](https://pepy.tech/badge/twootfeed)](https://pepy.tech/project/twootfeed)
-[![Python Version](https://img.shields.io/badge/python-3.7+-brightgreen.svg)](https://python.org) 
-[![Flask Version](https://img.shields.io/badge/flask-2.2-brightgreen.svg)](http://flask.pocoo.org/)
+[![Python Version](https://img.shields.io/badge/python-3.8+-brightgreen.svg)](https://python.org) 
+[![Flask Version](https://img.shields.io/badge/flask-2.3-brightgreen.svg)](http://flask.pocoo.org/)
 [![code style: black](https://img.shields.io/badge/code%20style-black-black)](https://black.readthedocs.io/en/stable/) 
 [![type check: mypy](https://img.shields.io/badge/type%20check-mypy-blue)](http://mypy-lang.org/)  
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/14d1c00121c04cd2b81453c597639ca6)](https://www.codacy.com/app/SamR1/python-twootfeed) 
 [![Coverage Status](https://coveralls.io/repos/github/SamR1/python-twootfeed/badge.svg?branch=master)](https://coveralls.io/github/SamR1/python-twootfeed?branch=master) 
 [![pipeline status](https://gitlab.com/SamR1/python-twootfeed/badges/master/pipeline.svg)](https://gitlab.com/SamR1/python-twootfeed/commits/master)
 
 ---
```

### Comparing `twootfeed-0.7.2/twootfeed.egg-info/SOURCES.txt` & `twootfeed-0.7.3/twootfeed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

