# Comparing `tmp/autosrt-1.3.8.tar.gz` & `tmp/autosrt-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosrt-1.3.8.tar", last modified: Wed Jun  7 16:25:38 2023, max compression
+gzip compressed data, was "autosrt-1.3.9.tar", last modified: Wed Jun  7 20:06:20 2023, max compression
```

## Comparing `autosrt-1.3.8.tar` & `autosrt-1.3.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 16:25:38.080466 autosrt-1.3.8/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.3.8/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.3.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2018 2023-06-07 16:25:38.080466 autosrt-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 16:25:38.024275 autosrt-1.3.8/autosrt/
--rw-rw-rw-   0        0        0   117288 2023-06-07 16:25:01.000000 autosrt-1.3.8/autosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 16:25:38.059487 autosrt-1.3.8/autosrt.egg-info/
--rw-rw-rw-   0        0        0     2018 2023-06-07 16:25:37.000000 autosrt-1.3.8/autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-06-07 16:25:37.000000 autosrt-1.3.8/autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 16:25:37.000000 autosrt-1.3.8/autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-07 16:25:37.000000 autosrt-1.3.8/autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       97 2023-06-07 16:25:37.000000 autosrt-1.3.8/autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-07 16:25:37.000000 autosrt-1.3.8/autosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-07 16:25:38.084964 autosrt-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 16:25:38.075970 autosrt-1.3.8/test/
--rw-rw-rw-   0        0        0     7435 2023-06-06 20:34:53.000000 autosrt-1.3.8/test/test1.py
--rw-rw-rw-   0        0        0     4481 2023-06-06 20:37:56.000000 autosrt-1.3.8/test/test2.py
--rw-rw-rw-   0        0        0     9938 2023-06-06 20:52:44.000000 autosrt-1.3.8/test/test3.py
--rw-rw-rw-   0        0        0    68819 2023-05-09 15:49:36.000000 autosrt-1.3.8/test/test4.py
+drwxrwxrwx   0        0        0        0 2023-06-07 20:06:20.641807 autosrt-1.3.9/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.3.9/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2018 2023-06-07 20:06:20.641807 autosrt-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.3.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 20:06:20.603597 autosrt-1.3.9/autosrt/
+-rw-rw-rw-   0        0        0   115678 2023-06-07 20:05:48.000000 autosrt-1.3.9/autosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 20:06:20.626822 autosrt-1.3.9/autosrt.egg-info/
+-rw-rw-rw-   0        0        0     2018 2023-06-07 20:06:20.000000 autosrt-1.3.9/autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-06-07 20:06:20.000000 autosrt-1.3.9/autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 20:06:20.000000 autosrt-1.3.9/autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-07 20:06:20.000000 autosrt-1.3.9/autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       97 2023-06-07 20:06:20.000000 autosrt-1.3.9/autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-07 20:06:20.000000 autosrt-1.3.9/autosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-07 20:06:20.645555 autosrt-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 20:06:20.638810 autosrt-1.3.9/test/
+-rw-rw-rw-   0        0        0     7435 2023-06-06 20:34:53.000000 autosrt-1.3.9/test/test1.py
+-rw-rw-rw-   0        0        0     4481 2023-06-06 20:37:56.000000 autosrt-1.3.9/test/test2.py
+-rw-rw-rw-   0        0        0     9938 2023-06-06 20:52:44.000000 autosrt-1.3.9/test/test3.py
+-rw-rw-rw-   0        0        0    68819 2023-05-09 15:49:36.000000 autosrt-1.3.9/test/test4.py
```

### Comparing `autosrt-1.3.8/LICENSE` & `autosrt-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.8/PKG-INFO` & `autosrt-1.3.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.3.8
+Version: 1.3.9
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.3.8/README.md` & `autosrt-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.8/autosrt/__init__.py` & `autosrt-1.3.9/autosrt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from glob import glob, escape
 import time
 from datetime import datetime, timedelta
 from pathlib import Path
 import shlex
 import shutil
 
-VERSION = "1.3.8"
+VERSION = "1.3.9"
 
 def stop_ffmpeg_windows(error_messages_callback=None):
     try:
         tasklist_output = subprocess.check_output(['tasklist'], creationflags=subprocess.CREATE_NO_WINDOW).decode('utf-8')
         ffmpeg_pid = None
         for line in tasklist_output.split('\n'):
             if "ffmpeg" in line:
@@ -2194,116 +2194,106 @@
     print("CHECKING EXISTING SUBTITLES STREAMS")
     print("===================================")
 
     if do_translate == False:
 
         for media_filepath in media_filepaths:
             ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
-            #print("Checking existing '{}' subtites streams in {}".format(ffmpeg_src_language_code, media_filepath))
             print("Checking %s" %media_filepath)
 
             subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
             subtitle_streams_data = subtitle_stream_parser(media_filepath)
 
             if subtitle_streams_data and subtitle_streams_data != []:
 
                 src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
 
                 if ffmpeg_src_language_code in subtitle_stream_parser.languages():
-                    #print(f"'{ffmpeg_src_language_code}' subtitle stream already existed in {media_filepath}")
                     print("Is '%s' subtitle stream exist          : Yes" %(ffmpeg_src_language_code.center(3)))
                     subtitle_stream_regions = []
                     subtitle_stream_transcripts = []
                     for entry in src_subtitle_stream_timed_subtitles:
                         subtitle_stream_regions.append(entry[0])
                         subtitle_stream_transcripts.append(entry[1])
                     base, ext = os.path.splitext(media_filepath)
                     src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=args.src_language, format=subtitle_format)
                     writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                     print(f"Extracting '{ffmpeg_src_language_code}'subtitle stream as      : {src_subtitle_filepath}")
                     writer.write(src_subtitle_filepath)
                     removed_media_filepaths.append(media_filepath)
 
                 else:
-                    #print(f"No '{ffmpeg_src_language_code}' subtitle stream found in {media_filepath}")
                     print("Is '%s' subtitle stream exist          : No" %(ffmpeg_src_language_code.center(3)))
 
         print("")
 
         if removed_media_filepaths:
             for removed_media_filepath in removed_media_filepaths:
                 media_filepaths.remove(removed_media_filepath)
 
         if not media_filepaths:
             print("Nothing else to do, exiting")
             sys.exit(0)
 
-
     elif do_translate == True:
 
         for media_filepath in media_filepaths:
             ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
-            #print("Checking existing '{}' subtites streams in {}".format(ffmpeg_src_language_code, media_filepath))
             print("Checking %s" %media_filepath)
 
             subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
             subtitle_streams_data = subtitle_stream_parser(media_filepath)
 
             if subtitle_streams_data and subtitle_streams_data != []:
 
                 src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
 
                 if ffmpeg_src_language_code in subtitle_stream_parser.languages():
-                    #print(f"'{ffmpeg_src_language_code}' subtitle stream already existed in {media_filepath}")
                     print("Is '%s' subtitle stream exist          : Yes" %(ffmpeg_src_language_code.center(3)))
                     subtitle_stream_regions = []
                     subtitle_stream_transcripts = []
                     for entry in src_subtitle_stream_timed_subtitles:
                         subtitle_stream_regions.append(entry[0])
                         subtitle_stream_transcripts.append(entry[1])
                     base, ext = os.path.splitext(media_filepath)
                     src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=args.src_language, format=subtitle_format)
                     writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                     print(f"Extracting '{ffmpeg_src_language_code}'subtitle stream as      : {src_subtitle_filepath}")
                     writer.write(src_subtitle_filepath)
 
                 else:
-                    #print(f"No '{ffmpeg_src_language_code}' subtitle stream found in {media_filepath}")
                     print("Is '%s' subtitle stream exist          : No" %(ffmpeg_src_language_code.center(3)))
 
         for media_filepath in media_filepaths:
             ffmpeg_dst_language_code = language.ffmpeg_code_of_code[args.dst_language]
-            #print("Checking existing '{}' subtites streams in {}".format(ffmpeg_dst_language_code, media_filepath))
             print("Checking %s" %media_filepath)
 
             subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
             subtitle_streams_data = subtitle_stream_parser(media_filepath)
 
             if subtitle_streams_data and subtitle_streams_data != []:
 
                 src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
                 dst_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_dst_language_code)
 
                 if ffmpeg_dst_language_code in subtitle_stream_parser.languages():
-                    #print(f"'{ffmpeg_dst_language_code}' subtitle stream already existed in {media_filepath}")
                     print("Is '%s' subtitle stream exist          : Yes" %(ffmpeg_dst_language_code.center(3)))
                     subtitle_stream_regions = []
                     subtitle_stream_transcripts = []
                     for entry in dst_subtitle_stream_timed_subtitles:
                         subtitle_stream_regions.append(entry[0])
                         subtitle_stream_transcripts.append(entry[1])
                     base, ext = os.path.splitext(media_filepath)
                     dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=args.dst_language, format=subtitle_format)
                     writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                     print(f"Extracting '{ffmpeg_dst_language_code}'subtitle stream as      : {dst_subtitle_filepath}")
                     writer.write(dst_subtitle_filepath)
                     removed_media_filepaths.append(media_filepath)
 
                 else:
-                    #print(f"No '{ffmpeg_dst_language_code}' subtitle stream found in {media_filepath}")
                     print("Is '%s' subtitle stream exist          : No" %(ffmpeg_dst_language_code.center(3)))
 
                     if src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
                         prompt = "Translating from %s to %s   : " %(args.src_language.center(8), args.dst_language.center(8))
                         widgets = [prompt, Percentage(), ' ', Bar(), ' ', ETA()]
                         pbar = ProgressBar(widgets=widgets, maxval=len(src_subtitle_stream_timed_subtitles)).start()
 
@@ -2321,41 +2311,35 @@
                         translation_writer.write(dst_subtitle_filepath)
                         print("Translated subtitles file saved as      : {}" .format(dst_subtitle_filepath))
                         removed_media_filepaths.append(media_filepath)
 
                     if args.embed and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
                         base, ext = os.path.splitext(media_filepath)
                         tmp_embedded_media_filepath_1 = "{base}.embedded1.{format}".format(base=base, format=ext[1:])
-                        tmp_embedded_media_filepath_2 = "{base}.embedded2.{format}".format(base=base, format=ext[1:])
                         embedded_media_filepath = "{base}.embedded.{format}".format(base=base, format=ext[1:])
-                        ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
                         ffmpeg_dst_language_code = language.ffmpeg_code_of_code[args.dst_language]
-                        result = embed_subtitle_to_media(media_filepath, media_type, src_subtitle_filepath, ffmpeg_src_language_code, tmp_embedded_media_filepath_1)
-                        if os.path.isfile(tmp_embedded_media_filepath_1):
-                            result = embed_subtitle_to_media(tmp_embedded_media_filepath_1, media_type, dst_subtitle_filepath, ffmpeg_dst_language_code, tmp_embedded_media_filepath_2)
-                        else:
-                            result = embed_subtitle_to_media(media_filepath, media_type, dst_subtitle_filepath, ffmpeg_dst_language_code, tmp_embedded_media_filepath_2)
 
-                        if os.path.isfile(tmp_embedded_media_filepath_2):
-                            shutil.copy(tmp_embedded_media_filepath_2, embedded_media_filepath)
+                        widgets = [f"Embedding \'{ffmpeg_dst_language_code}\' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                        pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                        result = subtitle_embedder(media_filepath)
+                        pbar.finish()
+
                         if os.path.isfile(tmp_embedded_media_filepath_1):
-                            os.remove(tmp_embedded_media_filepath_1)
-                        if os.path.isfile(tmp_embedded_media_filepath_2):
-                            os.remove(tmp_embedded_media_filepath_2)
+                            shutil.copy(tmp_embedded_media_filepath_1, embedded_media_filepath)
                         if os.path.isfile(embedded_media_filepath):
                             print("Subtitle embedded {} file saved as   : {}".format(media_type, embedded_media_filepath))
 
         print("")
 
         if removed_media_filepaths:
             for removed_media_filepath in removed_media_filepaths:
                 if removed_media_filepath in media_filepaths:
                     media_filepaths.remove(removed_media_filepath)
 
-        #print("Left media_filepaths = {}".format(media_filepaths))
         if not media_filepaths:
             print("Nothing else to do, exiting")
             sys.exit(0)
 
 
     print("PERFORMING SPEECH RECOGNITION FOR MEDIA FILES THAT HAVE NO SUBTITLE STREAMS")
     print("===========================================================================")
@@ -2450,48 +2434,47 @@
                         if os.path.isfile(tmp_embedded_media_filepath_1) and os.path.isfile(dst_subtitle_filepath):
                             result = embed_subtitle_to_media(tmp_embedded_media_filepath_1, media_type, dst_subtitle_filepath, ffmpeg_dst_language_code, tmp_embedded_media_filepath_2)
                         else:
                             result = embed_subtitle_to_media(media_filepath, media_type, dst_subtitle_filepath, ffmpeg_dst_language_code, tmp_embedded_media_filepath_2)
                         '''
 
                         # USING CLASS
-                        widgets = [f"Embedding \'{ffmpeg_src_language_code}\' subtitles into {media_type}     : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                        widgets = [f"Embedding \'{ffmpeg_src_language_code}\' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                         pbar = ProgressBar(widgets=widgets, maxval=100).start()
                         subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
                         result = subtitle_embedder(media_filepath)
                         pbar.finish()
 
                         if os.path.isfile(tmp_embedded_media_filepath_1) and os.path.isfile(dst_subtitle_filepath):
-                            widgets = [f"Embedding \'{ffmpeg_dst_language_code}\' subtitles into {media_type}     : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                            widgets = [f"Embedding \'{ffmpeg_dst_language_code}\' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                             pbar = ProgressBar(widgets=widgets, maxval=100).start()
                             subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=tmp_embedded_media_filepath_2, progress_callback=show_progress, error_messages_callback=show_error_messages)
                             result = subtitle_embedder(tmp_embedded_media_filepath_1)
                             pbar.finish()
                         elif (not os.path.isfile(tmp_embedded_media_filepath_1)) and os.path.isfile(dst_subtitle_filepath):
                             widgets = [f"Embedding \'{ffmpeg_dst_language_code}\' subtitles into {media_type}     : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                             pbar = ProgressBar(widgets=widgets, maxval=100).start()
                             subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=tmp_embedded_media_filepath_2, progress_callback=show_progress, error_messages_callback=show_error_messages)
                             result = subtitle_embedder(media_filepath)
                             pbar.finish()
 
-
                         if os.path.isfile(tmp_embedded_media_filepath_2):
                             shutil.copy(tmp_embedded_media_filepath_2, embedded_media_filepath)
 
                         if os.path.isfile(tmp_embedded_media_filepath_1):
                             os.remove(tmp_embedded_media_filepath_1)
                         if os.path.isfile(tmp_embedded_media_filepath_2):
                             os.remove(tmp_embedded_media_filepath_2)
 
                     else:
                         ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
 
                         #result = embed_subtitle_to_media(media_filepath, media_type, src_subtitle_filepath, ffmpeg_src_language_code, tmp_embedded_media_filepath_1)
 
-                        widgets = [f"Embedding \'{ffmpeg_src_language_code}\' subtitles into {media_type}     : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                        widgets = [f"Embedding \'{ffmpeg_src_language_code}\' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                         pbar = ProgressBar(widgets=widgets, maxval=100).start()
                         subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
                         result = subtitle_embedder(media_filepath)
                         pbar.finish()
 
                         if tmp_embedded_media_filepath_1:
                             shutil.copy(tmp_embedded_media_filepath_1, embedded_media_filepath)
```

### Comparing `autosrt-1.3.8/autosrt.egg-info/PKG-INFO` & `autosrt-1.3.9/autosrt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.3.8
+Version: 1.3.9
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.3.8/setup.py` & `autosrt-1.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.8/test/test1.py` & `autosrt-1.3.9/test/test1.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.8/test/test2.py` & `autosrt-1.3.9/test/test2.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.8/test/test3.py` & `autosrt-1.3.9/test/test3.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.8/test/test4.py` & `autosrt-1.3.9/test/test4.py`

 * *Files identical despite different names*

