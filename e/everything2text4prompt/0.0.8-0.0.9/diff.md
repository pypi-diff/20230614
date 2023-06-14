# Comparing `tmp/everything2text4prompt-0.0.8.tar.gz` & `tmp/everything2text4prompt-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "everything2text4prompt-0.0.8.tar", last modified: Tue May 30 15:40:19 2023, max compression
+gzip compressed data, was "everything2text4prompt-0.0.9.tar", last modified: Sun Jun 11 13:27:57 2023, max compression
```

## Comparing `everything2text4prompt-0.0.8.tar` & `everything2text4prompt-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 15:40:19.774934 everything2text4prompt-0.0.8/
--rw-rw-rw-   0        0        0     1089 2023-05-18 13:27:55.000000 everything2text4prompt-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1052 2023-05-30 15:40:19.774934 everything2text4prompt-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      658 2023-05-18 13:34:54.000000 everything2text4prompt-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 15:40:19.755960 everything2text4prompt-0.0.8/everything2text4prompt/
--rw-rw-rw-   0        0        0      234 2023-05-26 16:18:10.000000 everything2text4prompt-0.0.8/everything2text4prompt/__init__.py
--rw-rw-rw-   0        0        0     2423 2023-05-30 15:39:08.000000 everything2text4prompt-0.0.8/everything2text4prompt/everything2text4prompt.py
--rw-rw-rw-   0        0        0      452 2023-05-26 16:14:35.000000 everything2text4prompt-0.0.8/everything2text4prompt/pdf_util.py
-drwxrwxrwx   0        0        0        0 2023-05-30 15:40:19.770919 everything2text4prompt-0.0.8/everything2text4prompt/playground/
--rw-rw-rw-   0        0        0      754 2023-05-19 14:34:30.000000 everything2text4prompt-0.0.8/everything2text4prompt/playground/test_split_mp3.py
--rw-rw-rw-   0        0        0      340 2023-05-19 15:00:50.000000 everything2text4prompt-0.0.8/everything2text4prompt/playground/test_whisper.py
--rw-rw-rw-   0        0        0     1183 2023-05-26 16:14:59.000000 everything2text4prompt-0.0.8/everything2text4prompt/podcast_util.py
--rw-rw-rw-   0        0        0     2223 2023-05-30 15:31:27.000000 everything2text4prompt-0.0.8/everything2text4prompt/util.py
--rw-rw-rw-   0        0        0     3682 2023-05-30 15:39:12.000000 everything2text4prompt-0.0.8/everything2text4prompt/youtube_util.py
-drwxrwxrwx   0        0        0        0 2023-05-30 15:40:19.765933 everything2text4prompt-0.0.8/everything2text4prompt.egg-info/
--rw-rw-rw-   0        0        0     1052 2023-05-30 15:40:19.000000 everything2text4prompt-0.0.8/everything2text4prompt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      585 2023-05-30 15:40:19.000000 everything2text4prompt-0.0.8/everything2text4prompt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 15:40:19.000000 everything2text4prompt-0.0.8/everything2text4prompt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-30 15:40:19.000000 everything2text4prompt-0.0.8/everything2text4prompt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-05-30 15:40:19.000000 everything2text4prompt-0.0.8/everything2text4prompt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 15:40:19.775948 everything2text4prompt-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      785 2023-05-30 15:40:04.000000 everything2text4prompt-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 13:27:57.030394 everything2text4prompt-0.0.9/
+-rw-rw-rw-   0        0        0     1089 2023-05-18 13:27:55.000000 everything2text4prompt-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1052 2023-06-11 13:27:57.028400 everything2text4prompt-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      658 2023-05-18 13:34:54.000000 everything2text4prompt-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 13:27:56.993492 everything2text4prompt-0.0.9/everything2text4prompt/
+-rw-rw-rw-   0        0        0      234 2023-05-26 16:18:10.000000 everything2text4prompt-0.0.9/everything2text4prompt/__init__.py
+-rw-rw-rw-   0        0        0     2423 2023-06-11 13:26:08.000000 everything2text4prompt-0.0.9/everything2text4prompt/everything2text4prompt.py
+-rw-rw-rw-   0        0        0      452 2023-05-26 16:14:35.000000 everything2text4prompt-0.0.9/everything2text4prompt/pdf_util.py
+drwxrwxrwx   0        0        0        0 2023-06-11 13:27:57.026404 everything2text4prompt-0.0.9/everything2text4prompt/playground/
+-rw-rw-rw-   0        0        0      754 2023-05-19 14:34:30.000000 everything2text4prompt-0.0.9/everything2text4prompt/playground/test_split_mp3.py
+-rw-rw-rw-   0        0        0      340 2023-05-19 15:00:50.000000 everything2text4prompt-0.0.9/everything2text4prompt/playground/test_whisper.py
+-rw-rw-rw-   0        0        0     1183 2023-05-26 16:14:59.000000 everything2text4prompt-0.0.9/everything2text4prompt/podcast_util.py
+-rw-rw-rw-   0        0        0     2223 2023-05-30 15:31:27.000000 everything2text4prompt-0.0.9/everything2text4prompt/util.py
+-rw-rw-rw-   0        0        0     4543 2023-06-11 13:26:21.000000 everything2text4prompt-0.0.9/everything2text4prompt/youtube_util.py
+drwxrwxrwx   0        0        0        0 2023-06-11 13:27:57.004462 everything2text4prompt-0.0.9/everything2text4prompt.egg-info/
+-rw-rw-rw-   0        0        0     1052 2023-06-11 13:27:56.000000 everything2text4prompt-0.0.9/everything2text4prompt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      585 2023-06-11 13:27:56.000000 everything2text4prompt-0.0.9/everything2text4prompt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 13:27:56.000000 everything2text4prompt-0.0.9/everything2text4prompt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-06-11 13:27:56.000000 everything2text4prompt-0.0.9/everything2text4prompt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-11 13:27:56.000000 everything2text4prompt-0.0.9/everything2text4prompt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 13:27:57.030394 everything2text4prompt-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      785 2023-06-11 13:21:19.000000 everything2text4prompt-0.0.9/setup.py
```

### Comparing `everything2text4prompt-0.0.8/LICENSE` & `everything2text4prompt-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `everything2text4prompt-0.0.8/PKG-INFO` & `everything2text4prompt-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: everything2text4prompt
-Version: 0.0.8
+Version: 0.0.9
 Summary: Convert many medium into text, and the text format is specialized for prompt input
 Home-page: https://github.com/michaelthwan/everything2text4prompt
 Author: michaethwan
 Author-email: michaelthwan@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `everything2text4prompt-0.0.8/README.md` & `everything2text4prompt-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `everything2text4prompt-0.0.8/everything2text4prompt/everything2text4prompt.py` & `everything2text4prompt-0.0.9/everything2text4prompt/everything2text4prompt.py`

 * *Files identical despite different names*

### Comparing `everything2text4prompt-0.0.8/everything2text4prompt/playground/test_split_mp3.py` & `everything2text4prompt-0.0.9/everything2text4prompt/playground/test_split_mp3.py`

 * *Files identical despite different names*

### Comparing `everything2text4prompt-0.0.8/everything2text4prompt/podcast_util.py` & `everything2text4prompt-0.0.9/everything2text4prompt/podcast_util.py`

 * *Files identical despite different names*

### Comparing `everything2text4prompt-0.0.8/everything2text4prompt/util.py` & `everything2text4prompt-0.0.9/everything2text4prompt/util.py`

 * *Files identical despite different names*

### Comparing `everything2text4prompt-0.0.8/everything2text4prompt/youtube_util.py` & `everything2text4prompt-0.0.9/everything2text4prompt/youtube_util.py`

 * *Files 16% similar despite different names*

```diff
@@ -56,15 +56,20 @@
             return ts_transcript_list
 
         if is_url(target_source):
             video_id = extract_video_id_from_url(target_source)
         else:
             video_id = target_source
 
-        preferred_lang = ['en', 'zh', 'zh-Hans', 'zh-Hant', 'ja', 'it', 'de', 'fr']
+        preferred_lang = ['en', 'zh', 'zh-HK', 'zh-Hans', 'zh-Hant', 'ja', 'ko', 'it', 'de', 'fr',
+                          'tr', 'tk', 'lg', 'da', 'eu', 'mi', 'jv', 'eo', 'gl', 'ca', 'nso', 'gu', 'sw', 'ne', 'ny', 'gn', 'be', 'lt', 'ig', 'is', 'hu', 'id', 'hi', 'ky', 'lo', 'ay', 'fy', 'es',
+                          'kri', 'hr', 'kn', 'iw', 'el', 'hy', 'bn', 'la', 'lv', 'ln', 'fa', 'bs', 'pl', 'fi', 'ak', 'am', 'ar', 'az', 'sq', 'as', 'ru', 'bg', 'sd', 'af', 'kk', 'cy', 'co', 'xh', 'yo',
+                          'hmn', 'dv', 'sn', 'ee', 'haw', 'ku', 'no', 'pa', 'ka', 'th', 'ta', 'te', 'ht', 'uk', 'uz', 'ur', 'ts', 'zu', 'so', 'mt', 'ms', 'mk', 'mg', 'mr', 'ml', 'km', 'ceb', 'cs',
+                          'sa', 'nl', 'bho', 'su', 'ti', 'sl', 'sk', 'ps', 'fil', 'vi', 'tg', 'st', 'sr', 'or', 'om', 'yi', 'et', 'ga', 'sv', 'pt', 'si', 'ug', 'mn', 'qu', 'ha', 'my', 'rw', 'lb',
+                          'sm', 'ro', 'gd', 'tt', ]
         try:
             transcript = YouTubeTranscriptApi.get_transcript(video_id, preferred_lang)
         except Exception as e:
             import youtube_transcript_api
             if isinstance(e, youtube_transcript_api._errors.TranscriptsDisabled):
                 raise Exception(e)
             transcript_list = YouTubeTranscriptApi.list_transcripts(video_id)
```

### Comparing `everything2text4prompt-0.0.8/everything2text4prompt.egg-info/PKG-INFO` & `everything2text4prompt-0.0.9/everything2text4prompt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: everything2text4prompt
-Version: 0.0.8
+Version: 0.0.9
 Summary: Convert many medium into text, and the text format is specialized for prompt input
 Home-page: https://github.com/michaelthwan/everything2text4prompt
 Author: michaethwan
 Author-email: michaelthwan@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `everything2text4prompt-0.0.8/everything2text4prompt.egg-info/SOURCES.txt` & `everything2text4prompt-0.0.9/everything2text4prompt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `everything2text4prompt-0.0.8/setup.py` & `everything2text4prompt-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="everything2text4prompt",
-    version="0.0.8",
+    version="0.0.9",
     description="Convert many medium into text, and the text format is specialized for prompt input",
     # package_dir={'': 'everything2text4prompt'},
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/michaelthwan/everything2text4prompt",
     author="michaethwan",
```

