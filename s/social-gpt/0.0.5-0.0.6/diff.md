# Comparing `tmp/social_gpt-0.0.5.tar.gz` & `tmp/social_gpt-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "social_gpt-0.0.5.tar", last modified: Wed Jun 14 08:00:10 2023, max compression
+gzip compressed data, was "social_gpt-0.0.6.tar", last modified: Wed Jun 14 08:03:02 2023, max compression
```

## Comparing `social_gpt-0.0.5.tar` & `social_gpt-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-14 08:00:10.640282 social_gpt-0.0.5/
--rw-r--r--   0 dineshsingh   (501) staff       (20)     1072 2023-06-13 14:09:04.000000 social_gpt-0.0.5/LICENSE
--rw-r--r--   0 dineshsingh   (501) staff       (20)      400 2023-06-14 08:00:10.640156 social_gpt-0.0.5/PKG-INFO
--rw-r--r--   0 dineshsingh   (501) staff       (20)       12 2023-06-13 14:08:39.000000 social_gpt-0.0.5/README.md
--rw-r--r--   0 dineshsingh   (501) staff       (20)       99 2023-06-13 14:09:35.000000 social_gpt-0.0.5/pyproject.toml
--rw-r--r--   0 dineshsingh   (501) staff       (20)       38 2023-06-14 08:00:10.640318 social_gpt-0.0.5/setup.cfg
--rw-r--r--   0 dineshsingh   (501) staff       (20)      716 2023-06-14 07:59:56.000000 social_gpt-0.0.5/setup.py
-drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-14 08:00:10.638537 social_gpt-0.0.5/social_gpt/
--rw-r--r--   0 dineshsingh   (501) staff       (20)       21 2023-06-13 14:49:17.000000 social_gpt-0.0.5/social_gpt/__init__.py
-drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-14 08:00:10.639400 social_gpt-0.0.5/social_gpt/ingestion/
--rw-r--r--   0 dineshsingh   (501) staff       (20)        0 2023-06-07 11:16:57.000000 social_gpt-0.0.5/social_gpt/ingestion/__init__.py
--rw-r--r--   0 dineshsingh   (501) staff       (20)     1650 2023-06-13 10:34:27.000000 social_gpt-0.0.5/social_gpt/ingestion/indexer.py
--rw-r--r--   0 dineshsingh   (501) staff       (20)      515 2023-06-13 14:23:25.000000 social_gpt-0.0.5/social_gpt/ingestion/ingestion.py
-drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-14 08:00:10.639815 social_gpt-0.0.5/social_gpt/ingestion/scraper/
--rw-r--r--   0 dineshsingh   (501) staff       (20)        0 2023-06-12 18:55:48.000000 social_gpt-0.0.5/social_gpt/ingestion/scraper/__init__.py
--rw-r--r--   0 dineshsingh   (501) staff       (20)      306 2023-06-13 14:23:25.000000 social_gpt-0.0.5/social_gpt/ingestion/scraper/scraper_factory.py
--rw-r--r--   0 dineshsingh   (501) staff       (20)      258 2023-06-13 07:48:49.000000 social_gpt-0.0.5/social_gpt/ingestion/scraper/social_scraper.py
--rw-r--r--   0 dineshsingh   (501) staff       (20)     1708 2023-06-13 14:23:25.000000 social_gpt-0.0.5/social_gpt/ingestion/scraper/youtube_scraper.py
-drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-14 08:00:10.640003 social_gpt-0.0.5/social_gpt/query/
--rw-r--r--   0 dineshsingh   (501) staff       (20)        0 2023-06-13 09:26:30.000000 social_gpt-0.0.5/social_gpt/query/__init__.py
--rw-r--r--   0 dineshsingh   (501) staff       (20)      586 2023-06-13 10:15:48.000000 social_gpt-0.0.5/social_gpt/query/query_helper.py
-drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-14 08:00:10.639112 social_gpt-0.0.5/social_gpt.egg-info/
--rw-r--r--   0 dineshsingh   (501) staff       (20)      400 2023-06-14 08:00:10.000000 social_gpt-0.0.5/social_gpt.egg-info/PKG-INFO
--rw-r--r--   0 dineshsingh   (501) staff       (20)      578 2023-06-14 08:00:10.000000 social_gpt-0.0.5/social_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 dineshsingh   (501) staff       (20)        1 2023-06-14 08:00:10.000000 social_gpt-0.0.5/social_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 dineshsingh   (501) staff       (20)     2071 2023-06-14 08:00:10.000000 social_gpt-0.0.5/social_gpt.egg-info/requires.txt
--rw-r--r--   0 dineshsingh   (501) staff       (20)       11 2023-06-14 08:00:10.000000 social_gpt-0.0.5/social_gpt.egg-info/top_level.txt
+drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-14 08:03:02.088663 social_gpt-0.0.6/
+-rw-r--r--   0 dineshsingh   (501) staff       (20)     1072 2023-06-13 14:09:04.000000 social_gpt-0.0.6/LICENSE
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      400 2023-06-14 08:03:02.088524 social_gpt-0.0.6/PKG-INFO
+-rw-r--r--   0 dineshsingh   (501) staff       (20)       12 2023-06-13 14:08:39.000000 social_gpt-0.0.6/README.md
+-rw-r--r--   0 dineshsingh   (501) staff       (20)       99 2023-06-13 14:09:35.000000 social_gpt-0.0.6/pyproject.toml
+-rw-r--r--   0 dineshsingh   (501) staff       (20)       38 2023-06-14 08:03:02.088699 social_gpt-0.0.6/setup.cfg
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      716 2023-06-14 08:02:14.000000 social_gpt-0.0.6/setup.py
+drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-14 08:03:02.085639 social_gpt-0.0.6/social_gpt/
+-rw-r--r--   0 dineshsingh   (501) staff       (20)       21 2023-06-13 14:49:17.000000 social_gpt-0.0.6/social_gpt/__init__.py
+drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-14 08:03:02.086812 social_gpt-0.0.6/social_gpt/ingestion/
+-rw-r--r--   0 dineshsingh   (501) staff       (20)        0 2023-06-07 11:16:57.000000 social_gpt-0.0.6/social_gpt/ingestion/__init__.py
+-rw-r--r--   0 dineshsingh   (501) staff       (20)     1650 2023-06-13 10:34:27.000000 social_gpt-0.0.6/social_gpt/ingestion/indexer.py
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      515 2023-06-13 14:23:25.000000 social_gpt-0.0.6/social_gpt/ingestion/ingestion.py
+drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-14 08:03:02.087837 social_gpt-0.0.6/social_gpt/ingestion/scraper/
+-rw-r--r--   0 dineshsingh   (501) staff       (20)        0 2023-06-12 18:55:48.000000 social_gpt-0.0.6/social_gpt/ingestion/scraper/__init__.py
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      306 2023-06-13 14:23:25.000000 social_gpt-0.0.6/social_gpt/ingestion/scraper/scraper_factory.py
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      258 2023-06-13 07:48:49.000000 social_gpt-0.0.6/social_gpt/ingestion/scraper/social_scraper.py
+-rw-r--r--   0 dineshsingh   (501) staff       (20)     1708 2023-06-13 14:23:25.000000 social_gpt-0.0.6/social_gpt/ingestion/scraper/youtube_scraper.py
+drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-14 08:03:02.088240 social_gpt-0.0.6/social_gpt/query/
+-rw-r--r--   0 dineshsingh   (501) staff       (20)        0 2023-06-13 09:26:30.000000 social_gpt-0.0.6/social_gpt/query/__init__.py
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      586 2023-06-13 10:15:48.000000 social_gpt-0.0.6/social_gpt/query/query_helper.py
+drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-14 08:03:02.086291 social_gpt-0.0.6/social_gpt.egg-info/
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      400 2023-06-14 08:03:02.000000 social_gpt-0.0.6/social_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      578 2023-06-14 08:03:02.000000 social_gpt-0.0.6/social_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 dineshsingh   (501) staff       (20)        1 2023-06-14 08:03:02.000000 social_gpt-0.0.6/social_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 dineshsingh   (501) staff       (20)     2053 2023-06-14 08:03:02.000000 social_gpt-0.0.6/social_gpt.egg-info/requires.txt
+-rw-r--r--   0 dineshsingh   (501) staff       (20)       11 2023-06-14 08:03:02.000000 social_gpt-0.0.6/social_gpt.egg-info/top_level.txt
```

### Comparing `social_gpt-0.0.5/LICENSE` & `social_gpt-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `social_gpt-0.0.5/setup.py` & `social_gpt-0.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fh:
     requirements = fh.read().splitlines()
 
 setuptools.setup(
     name="social_gpt",
-    version="0.0.5",
+    version="0.0.6",
     author="dinesh1301",
     author_email="dinesh@topmate.io",
     description="Social gpt",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dinesh1301/social-gpt2",
     packages=setuptools.find_packages(),
```

### Comparing `social_gpt-0.0.5/social_gpt/ingestion/indexer.py` & `social_gpt-0.0.6/social_gpt/ingestion/indexer.py`

 * *Files identical despite different names*

### Comparing `social_gpt-0.0.5/social_gpt/ingestion/ingestion.py` & `social_gpt-0.0.6/social_gpt/ingestion/ingestion.py`

 * *Files identical despite different names*

### Comparing `social_gpt-0.0.5/social_gpt/ingestion/scraper/youtube_scraper.py` & `social_gpt-0.0.6/social_gpt/ingestion/scraper/youtube_scraper.py`

 * *Files identical despite different names*

### Comparing `social_gpt-0.0.5/social_gpt/query/query_helper.py` & `social_gpt-0.0.6/social_gpt/query/query_helper.py`

 * *Files identical despite different names*

### Comparing `social_gpt-0.0.5/social_gpt.egg-info/SOURCES.txt` & `social_gpt-0.0.6/social_gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `social_gpt-0.0.5/social_gpt.egg-info/requires.txt` & `social_gpt-0.0.6/social_gpt.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,14 @@
 requests-toolbelt==1.0.0
 requirementslib==1.6.9
 rfc3986==2.0.0
 rich==13.4.2
 rsa==4.9
 s3fs==2023.6.0
 six==1.16.0
-social-gpt==0.0.2
 SQLAlchemy==2.0.16
 stack-data==0.6.2
 tenacity==8.2.2
 tiktoken==0.4.0
 toml==0.10.2
 tomlkit==0.11.8
 tqdm==4.65.0
```

