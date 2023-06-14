# Comparing `tmp/lecture_automator-1.1.0.tar.gz` & `tmp/lecture_automator-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lecture_automator-1.1.0.tar", max compression
+gzip compressed data, was "lecture_automator-1.1.1.tar", max compression
```

## Comparing `lecture_automator-1.1.0.tar` & `lecture_automator-1.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     5661 2023-05-14 15:34:36.841907 lecture_automator-1.1.0/README.md
--rw-r--r--   0        0        0     2225 2023-05-14 15:34:36.843037 lecture_automator-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-09 16:38:42.823945 lecture_automator-1.1.0/src/lecture_automator/__init__.py
--rw-r--r--   0        0        0     1503 2023-05-14 15:34:36.843184 lecture_automator-1.1.0/src/lecture_automator/cli.py
--rw-r--r--   0        0        0     1151 2023-05-14 15:34:36.843364 lecture_automator-1.1.0/src/lecture_automator/compiler.py
--rw-r--r--   0        0        0        0 2023-05-01 10:48:09.376126 lecture_automator-1.1.0/src/lecture_automator/gen_speech/__init__.py
--rw-r--r--   0        0        0       43 2023-05-11 20:10:35.112561 lecture_automator-1.1.0/src/lecture_automator/gen_speech/exceptions.py
--rw-r--r--   0        0        0     3228 2023-05-14 15:34:36.843546 lecture_automator-1.1.0/src/lecture_automator/gen_speech/gen_speech.py
--rw-r--r--   0        0        0     1970 2023-05-11 20:10:35.113510 lecture_automator-1.1.0/src/lecture_automator/gen_speech/utils.py
--rw-r--r--   0        0        0        0 2023-05-11 20:10:35.113563 lecture_automator-1.1.0/src/lecture_automator/gen_video/__init__.py
--rw-r--r--   0        0        0       48 2023-05-14 15:34:36.843879 lecture_automator-1.1.0/src/lecture_automator/gen_video/exceptions.py
--rw-r--r--   0        0        0     1241 2023-05-14 15:34:36.844105 lecture_automator-1.1.0/src/lecture_automator/gen_video/gen_video.py
--rw-r--r--   0        0        0      469 2023-05-11 20:10:35.114460 lecture_automator-1.1.0/src/lecture_automator/gen_video/utils.py
--rw-r--r--   0        0        0        0 2023-05-14 15:34:36.844140 lecture_automator-1.1.0/src/lecture_automator/marp_api/__init__.py
--rw-r--r--   0        0        0      181 2023-05-14 15:34:36.844545 lecture_automator-1.1.0/src/lecture_automator/marp_api/exceptions.py
--rw-r--r--   0        0        0     1416 2023-05-14 15:34:36.844781 lecture_automator-1.1.0/src/lecture_automator/marp_api/marp_api.py
--rw-r--r--   0        0        0        0 2023-05-11 20:10:35.114804 lecture_automator-1.1.0/src/lecture_automator/parser/__init__.py
--rw-r--r--   0        0        0     1359 2023-05-14 15:34:36.845279 lecture_automator-1.1.0/src/lecture_automator/parser/command_handler.py
--rw-r--r--   0        0        0       84 2023-05-11 20:10:35.115338 lecture_automator-1.1.0/src/lecture_automator/parser/exceptions.py
--rw-r--r--   0        0        0     4364 2023-05-11 20:10:35.119793 lecture_automator-1.1.0/src/lecture_automator/parser/parser.py
--rw-r--r--   0        0        0      369 2023-05-11 20:10:35.115995 lecture_automator-1.1.0/src/lecture_automator/settings.py
--rw-r--r--   0        0        0      749 2023-05-14 15:32:24.947200 lecture_automator-1.1.0/src/lecture_automator/web.py
--rw-r--r--   0        0        0     6368 1970-01-01 00:00:00.000000 lecture_automator-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5773 2023-06-14 12:39:50.154495 lecture_automator-1.1.1/README.md
+-rw-r--r--   0        0        0     2225 2023-06-14 12:41:53.755829 lecture_automator-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-09 16:38:42.823945 lecture_automator-1.1.1/src/lecture_automator/__init__.py
+-rw-r--r--   0        0        0     1503 2023-05-14 15:34:36.843184 lecture_automator-1.1.1/src/lecture_automator/cli.py
+-rw-r--r--   0        0        0     1109 2023-06-14 12:39:52.314266 lecture_automator-1.1.1/src/lecture_automator/compiler.py
+-rw-r--r--   0        0        0        0 2023-05-01 10:48:09.376126 lecture_automator-1.1.1/src/lecture_automator/gen_speech/__init__.py
+-rw-r--r--   0        0        0       43 2023-05-11 20:10:35.112561 lecture_automator-1.1.1/src/lecture_automator/gen_speech/exceptions.py
+-rw-r--r--   0        0        0     3228 2023-05-14 15:34:36.843546 lecture_automator-1.1.1/src/lecture_automator/gen_speech/gen_speech.py
+-rw-r--r--   0        0        0     1970 2023-05-11 20:10:35.113510 lecture_automator-1.1.1/src/lecture_automator/gen_speech/utils.py
+-rw-r--r--   0        0        0        0 2023-05-11 20:10:35.113563 lecture_automator-1.1.1/src/lecture_automator/gen_video/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-14 15:34:36.843879 lecture_automator-1.1.1/src/lecture_automator/gen_video/exceptions.py
+-rw-r--r--   0        0        0     1241 2023-06-14 12:36:40.228661 lecture_automator-1.1.1/src/lecture_automator/gen_video/gen_video.py
+-rw-r--r--   0        0        0      469 2023-05-11 20:10:35.114460 lecture_automator-1.1.1/src/lecture_automator/gen_video/utils.py
+-rw-r--r--   0        0        0        0 2023-05-14 15:34:36.844140 lecture_automator-1.1.1/src/lecture_automator/marp_api/__init__.py
+-rw-r--r--   0        0        0      181 2023-05-14 15:34:36.844545 lecture_automator-1.1.1/src/lecture_automator/marp_api/exceptions.py
+-rw-r--r--   0        0        0     1605 2023-06-14 12:39:52.314495 lecture_automator-1.1.1/src/lecture_automator/marp_api/marp_api.py
+-rw-r--r--   0        0        0        0 2023-05-11 20:10:35.114804 lecture_automator-1.1.1/src/lecture_automator/parser/__init__.py
+-rw-r--r--   0        0        0     1359 2023-05-14 15:34:36.845279 lecture_automator-1.1.1/src/lecture_automator/parser/command_handler.py
+-rw-r--r--   0        0        0       84 2023-05-11 20:10:35.115338 lecture_automator-1.1.1/src/lecture_automator/parser/exceptions.py
+-rw-r--r--   0        0        0     4364 2023-06-14 12:31:21.937968 lecture_automator-1.1.1/src/lecture_automator/parser/parser.py
+-rw-r--r--   0        0        0      369 2023-05-11 20:10:35.115995 lecture_automator-1.1.1/src/lecture_automator/settings.py
+-rw-r--r--   0        0        0      749 2023-05-14 15:32:24.947200 lecture_automator-1.1.1/src/lecture_automator/web.py
+-rw-r--r--   0        0        0     6480 1970-01-01 00:00:00.000000 lecture_automator-1.1.1/PKG-INFO
```

### Comparing `lecture_automator-1.1.0/README.md` & `lecture_automator-1.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+<div style="text-align:center"><img width="200" 
+        height="200" src="assets/book-with-gear.png" /></div>
+
 # Lecture Automator
 
 Lecture Automator позволяет автоматически генерировать презентации с озвучкой для каждого из слайдов. Всё, что вам нужно сделать - написать текстовый файл Markdown со специальной разметкой, а остальное за вас сделает Lecture Automator.
 
 ## Установка
 
 С помощью pip (также необходимо установить ffmpeg и [Marp](https://github.com/marp-team/marp-cli)):
```

### Comparing `lecture_automator-1.1.0/pyproject.toml` & `lecture_automator-1.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lecture-automator"
-version = "1.1.0"
+version = "1.1.1"
 description = ""
 authors = ["CapBlood <stalker.anonim@mail.ru>"]
 readme = "README.md"
 homepage = "https://github.com/CapBlood/lecture-automator.git"
 
 [tool.poetry.dependencies]
 python = "^3.8,<=3.9"
```

### Comparing `lecture_automator-1.1.0/src/lecture_automator/cli.py` & `lecture_automator-1.1.1/src/lecture_automator/cli.py`

 * *Files identical despite different names*

### Comparing `lecture_automator-1.1.0/src/lecture_automator/compiler.py` & `lecture_automator-1.1.1/src/lecture_automator/compiler.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,16 +15,16 @@
                     verbose_progress: bool=False) -> None:
     md_data = parse_md(input_text_md)
 
     with tqdm(total=3, desc='Генерируем видео',
               bar_format='{l_bar}{bar}| {n_fmt}/{total_fmt}',
               disable=not verbose_progress) as bar:
         with tempfile.TemporaryDirectory() as tmpdirname:
-            generate_marp_slides(tmpdirname, md_data['md_text'], scale=scale)
-            slide_images = glob.glob(os.path.join(tmpdirname, 'Slide.*'))
+            slide_images = generate_marp_slides(
+                tmpdirname, md_data['md_text'], scale=scale)
             bar.update(1)
 
             audio_paths = texts_to_speeches(md_data['speech'], tmpdirname)
             bar.update(1)
 
             generate_video(slide_images, audio_paths, out_path, vformat=vformat)
             bar.update(1)
```

### Comparing `lecture_automator-1.1.0/src/lecture_automator/gen_speech/gen_speech.py` & `lecture_automator-1.1.1/src/lecture_automator/gen_speech/gen_speech.py`

 * *Files identical despite different names*

### Comparing `lecture_automator-1.1.0/src/lecture_automator/gen_speech/utils.py` & `lecture_automator-1.1.1/src/lecture_automator/gen_speech/utils.py`

 * *Files identical despite different names*

### Comparing `lecture_automator-1.1.0/src/lecture_automator/gen_video/gen_video.py` & `lecture_automator-1.1.1/src/lecture_automator/gen_video/gen_video.py`

 * *Files identical despite different names*

### Comparing `lecture_automator-1.1.0/src/lecture_automator/marp_api/marp_api.py` & `lecture_automator-1.1.1/src/lecture_automator/marp_api/marp_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import glob
 import os
 import subprocess
 import tempfile
 
 from lecture_automator.marp_api.exceptions import MarpError
 
 
@@ -29,13 +30,18 @@
         )
 
         out, err = process.communicate()
         retcode = process.poll()
         if retcode:
             raise MarpError(out, err)
 
+    slide_images = glob.glob(os.path.join(outdir, 'Slide.*'))
+    sorted_slide_images = sorted(slide_images, key=lambda p: os.path.basename(p))
+
+    return sorted_slide_images
+
 
 if __name__ == '__main__':
     with open('examples/Example.md') as file:
         text = file.read()
 
     generate_marp_slides('examples', text, scale=1.5)
```

### Comparing `lecture_automator-1.1.0/src/lecture_automator/parser/command_handler.py` & `lecture_automator-1.1.1/src/lecture_automator/parser/command_handler.py`

 * *Files identical despite different names*

### Comparing `lecture_automator-1.1.0/src/lecture_automator/parser/parser.py` & `lecture_automator-1.1.1/src/lecture_automator/parser/parser.py`

 * *Files identical despite different names*

### Comparing `lecture_automator-1.1.0/src/lecture_automator/web.py` & `lecture_automator-1.1.1/src/lecture_automator/web.py`

 * *Files identical despite different names*

### Comparing `lecture_automator-1.1.0/PKG-INFO` & `lecture_automator-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lecture-automator
-Version: 1.1.0
+Version: 1.1.1
 Summary: 
 Home-page: https://github.com/CapBlood/lecture-automator.git
 Author: CapBlood
 Author-email: stalker.anonim@mail.ru
 Requires-Python: >=3.8,<=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -15,14 +15,17 @@
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: streamlit (>=1.22.0,<2.0.0)
 Requires-Dist: sympy (>=1.11.1,<2.0.0)
 Requires-Dist: torch (>=2.0.0,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
+<div style="text-align:center"><img width="200" 
+        height="200" src="assets/book-with-gear.png" /></div>
+
 # Lecture Automator
 
 Lecture Automator позволяет автоматически генерировать презентации с озвучкой для каждого из слайдов. Всё, что вам нужно сделать - написать текстовый файл Markdown со специальной разметкой, а остальное за вас сделает Lecture Automator.
 
 ## Установка
 
 С помощью pip (также необходимо установить ffmpeg и [Marp](https://github.com/marp-team/marp-cli)):
```

