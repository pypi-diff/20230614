# Comparing `tmp/newscleaner-0.0.2.tar.gz` & `tmp/newscleaner-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newscleaner-0.0.2.tar", last modified: Wed Jun 14 05:36:37 2023, max compression
+gzip compressed data, was "newscleaner-0.1.3.tar", last modified: Mon May 22 05:38:55 2023, max compression
```

## Comparing `newscleaner-0.0.2.tar` & `newscleaner-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 05:36:37.709744 newscleaner-0.0.2/
--rw-rw-rw-   0        0        0     1073 2023-05-10 10:09:49.000000 newscleaner-0.0.2/LICENCE.txt
--rw-rw-rw-   0        0        0       34 2023-05-10 10:10:08.000000 newscleaner-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      559 2023-06-14 05:36:37.709744 newscleaner-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       17 2023-05-29 11:40:52.000000 newscleaner-0.0.2/README.md
--rw-rw-rw-   0        0        0       84 2023-05-10 10:10:18.000000 newscleaner-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 05:36:37.709744 newscleaner-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      882 2023-06-14 05:35:26.000000 newscleaner-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 05:36:37.521087 newscleaner-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-14 05:36:37.694142 newscleaner-0.0.2/src/newscleaner/
--rw-rw-rw-   0        0        0        0 2023-05-15 10:03:44.000000 newscleaner-0.0.2/src/newscleaner/__init__.py
--rw-rw-rw-   0        0        0    24730 2023-06-14 05:28:33.000000 newscleaner-0.0.2/src/newscleaner/clean.py
--rw-rw-rw-   0        0        0     2415 2023-05-19 11:00:25.000000 newscleaner-0.0.2/src/newscleaner/cleaner.py
--rw-rw-rw-   0        0        0     8199 2023-05-22 10:30:16.000000 newscleaner-0.0.2/src/newscleaner/regex.json
--rw-rw-rw-   0        0        0      882 2023-05-19 12:27:21.000000 newscleaner-0.0.2/src/newscleaner/setup.py
--rw-rw-rw-   0        0        0      675 2023-05-19 11:00:53.000000 newscleaner-0.0.2/src/newscleaner/tags.json
-drwxrwxrwx   0        0        0        0 2023-06-14 05:36:37.709744 newscleaner-0.0.2/src/newscleaner.egg-info/
--rw-rw-rw-   0        0        0      559 2023-06-14 05:36:37.000000 newscleaner-0.0.2/src/newscleaner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2023-05-10 10:01:43.000000 newscleaner-0.0.2/src/newscleaner.egg-info/PKG-INFO.txt
--rw-rw-rw-   0        0        0      409 2023-06-14 05:36:37.000000 newscleaner-0.0.2/src/newscleaner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 05:36:37.000000 newscleaner-0.0.2/src/newscleaner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-14 05:36:37.000000 newscleaner-0.0.2/src/newscleaner.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 05:38:55.258994 newscleaner-0.1.3/
+-rw-rw-rw-   0        0        0     1073 2023-05-10 10:09:49.000000 newscleaner-0.1.3/LICENCE.txt
+-rw-rw-rw-   0        0        0       34 2023-05-10 10:10:08.000000 newscleaner-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      567 2023-05-22 05:38:55.258994 newscleaner-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       25 2023-05-10 10:10:09.000000 newscleaner-0.1.3/README.md
+-rw-rw-rw-   0        0        0       84 2023-05-10 10:10:18.000000 newscleaner-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-22 05:38:55.258994 newscleaner-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      882 2023-05-22 05:36:37.000000 newscleaner-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 05:38:55.149659 newscleaner-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-22 05:38:55.258994 newscleaner-0.1.3/src/newscleaner/
+-rw-rw-rw-   0        0        0        0 2023-05-15 10:03:44.000000 newscleaner-0.1.3/src/newscleaner/__init__.py
+-rw-rw-rw-   0        0        0    16260 2023-05-22 05:35:40.000000 newscleaner-0.1.3/src/newscleaner/clean.py
+-rw-rw-rw-   0        0        0     2415 2023-05-19 11:00:25.000000 newscleaner-0.1.3/src/newscleaner/cleaner.py
+-rw-rw-rw-   0        0        0     8095 2023-05-19 09:38:44.000000 newscleaner-0.1.3/src/newscleaner/regex.json
+-rw-rw-rw-   0        0        0      882 2023-05-19 12:27:21.000000 newscleaner-0.1.3/src/newscleaner/setup.py
+-rw-rw-rw-   0        0        0      675 2023-05-19 11:00:53.000000 newscleaner-0.1.3/src/newscleaner/tags.json
+drwxrwxrwx   0        0        0        0 2023-05-22 05:38:55.258994 newscleaner-0.1.3/src/newscleaner.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-05-22 05:38:55.000000 newscleaner-0.1.3/src/newscleaner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-05-10 10:01:43.000000 newscleaner-0.1.3/src/newscleaner.egg-info/PKG-INFO.txt
+-rw-rw-rw-   0        0        0      409 2023-05-22 05:38:55.000000 newscleaner-0.1.3/src/newscleaner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 05:38:55.000000 newscleaner-0.1.3/src/newscleaner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-22 05:38:55.000000 newscleaner-0.1.3/src/newscleaner.egg-info/top_level.txt
```

### Comparing `newscleaner-0.0.2/LICENCE.txt` & `newscleaner-0.1.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `newscleaner-0.0.2/PKG-INFO` & `newscleaner-0.1.3/src/newscleaner.egg-info/PKG-INFO.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1
-Name: newscleaner
-Version: 0.0.2
-Summary: Package to clean up noise from news articles
-Home-page: https://github.com/pankajjha/newscleaner
-Author: Lakshita Kain
-Author-email: mail@pankajjha.me
-Project-URL: Bug Tracker, https://github.com/pankajjha/newscleaner/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENCE.txt
-
-# Article Cleaner
+Metadata-Version: 2.1
+Name: newscleaner
+Version: 0.0.5
+Summary: Package to clean up waste postfix from articles
+Home-page: https://github.com/pankajjha/newscleaner
+Author: Pankaj Jha
+Author-email: mail@pankajjha.me
+Project-URL: Bug Tracker, https://github.com/pankajjha/newscleaner/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
+# Article Postfix Cleaner
```

### Comparing `newscleaner-0.0.2/setup.py` & `newscleaner-0.1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="newscleaner",
-    version="0.0.2",
-    author="Lakshita Kain",
+    version="0.1.3",
+    author="Pankaj Jha",
     author_email="mail@pankajjha.me",
-    description="Package to clean up noise from news articles",
+    description="Package to clean up waste postfix from articles",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pankajjha/newscleaner",
     project_urls={
         "Bug Tracker": "https://github.com/pankajjha/newscleaner/issues",
     },
     classifiers=[
```

### Comparing `newscleaner-0.0.2/src/newscleaner/cleaner.py` & `newscleaner-0.1.3/src/newscleaner/cleaner.py`

 * *Files identical despite different names*

### Comparing `newscleaner-0.0.2/src/newscleaner/regex.json` & `newscleaner-0.1.3/src/newscleaner/regex.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981684981684982%*

 * *Differences: {"'perfect_match'": '{delete: [22]}'}*

```diff
@@ -18,15 +18,14 @@
         "UP NEXT",
         "Get today\u2019s headlines in minutes with",
         "Your Florida Daily",
         "FILE - ",
         "See video of the play here ",
         "*",
         "Get Boston local news, weather forecasts, lifestyle and entertainment stories to your inbox.",
-        "Get Southern California news, weather forecasts and entertainment stories to your inbox. . ",
         "\u2019s newsletters.",
         "Read the full story on NBCNews.com here.",
         "PHOTOS",
         "pic\\.twitter\\.com/\\w+",
         "Get Boston local news, weather forecasts, lifestyle and entertainment stories to your inbox. \u2019s newsletters.",
         "Get Chicago local news, weather forecasts, sports and entertainment stories to your inbox.",
         "Read the full story on NBCNews.com here.",
```

### Comparing `newscleaner-0.0.2/src/newscleaner/setup.py` & `newscleaner-0.1.3/src/newscleaner/setup.py`

 * *Files identical despite different names*

### Comparing `newscleaner-0.0.2/src/newscleaner/tags.json` & `newscleaner-0.1.3/src/newscleaner/tags.json`

 * *Files identical despite different names*

