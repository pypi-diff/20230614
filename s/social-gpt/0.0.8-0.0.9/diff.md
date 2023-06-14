# Comparing `tmp/social_gpt-0.0.8.tar.gz` & `tmp/social_gpt-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "social_gpt-0.0.8.tar", last modified: Wed Jun 14 08:53:23 2023, max compression
+gzip compressed data, was "social_gpt-0.0.9.tar", last modified: Wed Jun 14 11:31:57 2023, max compression
```

## Comparing `social_gpt-0.0.8.tar` & `social_gpt-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-14 08:53:23.040770 social_gpt-0.0.8/
--rw-r--r--   0 dineshsingh   (501) staff       (20)     1072 2023-06-13 14:09:04.000000 social_gpt-0.0.8/LICENSE
--rw-r--r--   0 dineshsingh   (501) staff       (20)     1111 2023-06-14 08:53:23.040622 social_gpt-0.0.8/PKG-INFO
--rw-r--r--   0 dineshsingh   (501) staff       (20)      723 2023-06-14 08:48:33.000000 social_gpt-0.0.8/README.md
--rw-r--r--   0 dineshsingh   (501) staff       (20)       99 2023-06-13 14:09:35.000000 social_gpt-0.0.8/pyproject.toml
--rw-r--r--   0 dineshsingh   (501) staff       (20)       38 2023-06-14 08:53:23.040819 social_gpt-0.0.8/setup.cfg
--rw-r--r--   0 dineshsingh   (501) staff       (20)      750 2023-06-14 08:52:25.000000 social_gpt-0.0.8/setup.py
-drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-14 08:53:23.035432 social_gpt-0.0.8/social_gpt/
--rw-r--r--   0 dineshsingh   (501) staff       (20)       21 2023-06-13 14:49:17.000000 social_gpt-0.0.8/social_gpt/__init__.py
-drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-14 08:53:23.038590 social_gpt-0.0.8/social_gpt/ingestion/
--rw-r--r--   0 dineshsingh   (501) staff       (20)       19 2023-06-14 08:51:18.000000 social_gpt-0.0.8/social_gpt/ingestion/__init__.py
--rw-r--r--   0 dineshsingh   (501) staff       (20)     1650 2023-06-13 10:34:27.000000 social_gpt-0.0.8/social_gpt/ingestion/indexer.py
--rw-r--r--   0 dineshsingh   (501) staff       (20)      495 2023-06-14 08:44:12.000000 social_gpt-0.0.8/social_gpt/ingestion/ingestion.py
-drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-14 08:53:23.039820 social_gpt-0.0.8/social_gpt/ingestion/scraper/
--rw-r--r--   0 dineshsingh   (501) staff       (20)       17 2023-06-14 08:52:07.000000 social_gpt-0.0.8/social_gpt/ingestion/scraper/__init__.py
--rw-r--r--   0 dineshsingh   (501) staff       (20)      270 2023-06-14 08:44:25.000000 social_gpt-0.0.8/social_gpt/ingestion/scraper/scraper_factory.py
--rw-r--r--   0 dineshsingh   (501) staff       (20)      258 2023-06-13 07:48:49.000000 social_gpt-0.0.8/social_gpt/ingestion/scraper/social_scraper.py
--rw-r--r--   0 dineshsingh   (501) staff       (20)     1690 2023-06-14 08:44:35.000000 social_gpt-0.0.8/social_gpt/ingestion/scraper/youtube_scraper.py
-drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-14 08:53:23.040323 social_gpt-0.0.8/social_gpt/query/
--rw-r--r--   0 dineshsingh   (501) staff       (20)       15 2023-06-14 08:51:46.000000 social_gpt-0.0.8/social_gpt/query/__init__.py
--rw-r--r--   0 dineshsingh   (501) staff       (20)      586 2023-06-13 10:15:48.000000 social_gpt-0.0.8/social_gpt/query/query_helper.py
-drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-14 08:53:23.037015 social_gpt-0.0.8/social_gpt.egg-info/
--rw-r--r--   0 dineshsingh   (501) staff       (20)     1111 2023-06-14 08:53:23.000000 social_gpt-0.0.8/social_gpt.egg-info/PKG-INFO
--rw-r--r--   0 dineshsingh   (501) staff       (20)      578 2023-06-14 08:53:23.000000 social_gpt-0.0.8/social_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 dineshsingh   (501) staff       (20)        1 2023-06-14 08:53:23.000000 social_gpt-0.0.8/social_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 dineshsingh   (501) staff       (20)     1215 2023-06-14 08:53:23.000000 social_gpt-0.0.8/social_gpt.egg-info/requires.txt
--rw-r--r--   0 dineshsingh   (501) staff       (20)       11 2023-06-14 08:53:23.000000 social_gpt-0.0.8/social_gpt.egg-info/top_level.txt
+drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-14 11:31:57.014809 social_gpt-0.0.9/
+-rw-r--r--   0 dineshsingh   (501) staff       (20)     1072 2023-06-13 14:09:04.000000 social_gpt-0.0.9/LICENSE
+-rw-r--r--   0 dineshsingh   (501) staff       (20)     1111 2023-06-14 11:31:57.014602 social_gpt-0.0.9/PKG-INFO
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      723 2023-06-14 08:48:33.000000 social_gpt-0.0.9/README.md
+-rw-r--r--   0 dineshsingh   (501) staff       (20)       99 2023-06-13 14:09:35.000000 social_gpt-0.0.9/pyproject.toml
+-rw-r--r--   0 dineshsingh   (501) staff       (20)       38 2023-06-14 11:31:57.014856 social_gpt-0.0.9/setup.cfg
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      750 2023-06-14 11:31:16.000000 social_gpt-0.0.9/setup.py
+drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-14 11:31:57.011843 social_gpt-0.0.9/social_gpt/
+-rw-r--r--   0 dineshsingh   (501) staff       (20)       21 2023-06-13 14:49:17.000000 social_gpt-0.0.9/social_gpt/__init__.py
+drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-14 11:31:57.013055 social_gpt-0.0.9/social_gpt/ingestion/
+-rw-r--r--   0 dineshsingh   (501) staff       (20)       19 2023-06-14 08:51:18.000000 social_gpt-0.0.9/social_gpt/ingestion/__init__.py
+-rw-r--r--   0 dineshsingh   (501) staff       (20)     1650 2023-06-13 10:34:27.000000 social_gpt-0.0.9/social_gpt/ingestion/indexer.py
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      539 2023-06-14 11:29:36.000000 social_gpt-0.0.9/social_gpt/ingestion/ingestion.py
+drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-14 11:31:57.013962 social_gpt-0.0.9/social_gpt/ingestion/scraper/
+-rw-r--r--   0 dineshsingh   (501) staff       (20)       17 2023-06-14 08:52:07.000000 social_gpt-0.0.9/social_gpt/ingestion/scraper/__init__.py
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      328 2023-06-14 11:30:01.000000 social_gpt-0.0.9/social_gpt/ingestion/scraper/scraper_factory.py
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      258 2023-06-13 07:48:49.000000 social_gpt-0.0.9/social_gpt/ingestion/scraper/social_scraper.py
+-rw-r--r--   0 dineshsingh   (501) staff       (20)     1675 2023-06-14 11:30:39.000000 social_gpt-0.0.9/social_gpt/ingestion/scraper/youtube_scraper.py
+drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-14 11:31:57.014225 social_gpt-0.0.9/social_gpt/query/
+-rw-r--r--   0 dineshsingh   (501) staff       (20)       15 2023-06-14 08:51:46.000000 social_gpt-0.0.9/social_gpt/query/__init__.py
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      586 2023-06-13 10:15:48.000000 social_gpt-0.0.9/social_gpt/query/query_helper.py
+drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-14 11:31:57.012563 social_gpt-0.0.9/social_gpt.egg-info/
+-rw-r--r--   0 dineshsingh   (501) staff       (20)     1111 2023-06-14 11:31:56.000000 social_gpt-0.0.9/social_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      578 2023-06-14 11:31:56.000000 social_gpt-0.0.9/social_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 dineshsingh   (501) staff       (20)        1 2023-06-14 11:31:56.000000 social_gpt-0.0.9/social_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 dineshsingh   (501) staff       (20)     1215 2023-06-14 11:31:56.000000 social_gpt-0.0.9/social_gpt.egg-info/requires.txt
+-rw-r--r--   0 dineshsingh   (501) staff       (20)       11 2023-06-14 11:31:56.000000 social_gpt-0.0.9/social_gpt.egg-info/top_level.txt
```

### Comparing `social_gpt-0.0.8/LICENSE` & `social_gpt-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `social_gpt-0.0.8/PKG-INFO` & `social_gpt-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: social_gpt
-Version: 0.0.8
+Version: 0.0.9
 Summary: Social gpt
 Home-page: https://github.com/dinesh1301/social-gpt2
 Author: dinesh1301
 Author-email: dinesh@topmate.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `social_gpt-0.0.8/README.md` & `social_gpt-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `social_gpt-0.0.8/setup.py` & `social_gpt-0.0.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fh:
     requirements = [line.split('==')[0] for line in fh.read().splitlines()]
 
 setuptools.setup(
     name="social_gpt",
-    version="0.0.8",
+    version="0.0.9",
     author="dinesh1301",
     author_email="dinesh@topmate.io",
     description="Social gpt",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dinesh1301/social-gpt2",
     packages=setuptools.find_packages(),
```

### Comparing `social_gpt-0.0.8/social_gpt/ingestion/indexer.py` & `social_gpt-0.0.9/social_gpt/ingestion/indexer.py`

 * *Files identical despite different names*

### Comparing `social_gpt-0.0.8/social_gpt/ingestion/scraper/youtube_scraper.py` & `social_gpt-0.0.9/social_gpt/ingestion/scraper/youtube_scraper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import os
 from typing import List
 
-from llama_index import Document
-
-from social_scraper import SocialScraper
 import googleapiclient
-from googleapiclient.discovery import build
-from youtube_transcript_api import YouTubeTranscriptApi
 from dotenv import load_dotenv
+from llama_index import Document
+from youtube_transcript_api import YouTubeTranscriptApi
+
+from social_gpt.ingestion.scraper.social_scraper import SocialScraper
 
 load_dotenv()
 
 YOUTUBE_API_SERVICE_NAME = 'youtube'
 YOUTUBE_API_VERSION = 'v3'
```

### Comparing `social_gpt-0.0.8/social_gpt/query/query_helper.py` & `social_gpt-0.0.9/social_gpt/query/query_helper.py`

 * *Files identical despite different names*

### Comparing `social_gpt-0.0.8/social_gpt.egg-info/PKG-INFO` & `social_gpt-0.0.9/social_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: social-gpt
-Version: 0.0.8
+Version: 0.0.9
 Summary: Social gpt
 Home-page: https://github.com/dinesh1301/social-gpt2
 Author: dinesh1301
 Author-email: dinesh@topmate.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `social_gpt-0.0.8/social_gpt.egg-info/SOURCES.txt` & `social_gpt-0.0.9/social_gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `social_gpt-0.0.8/social_gpt.egg-info/requires.txt` & `social_gpt-0.0.9/social_gpt.egg-info/requires.txt`

 * *Files identical despite different names*

