# Comparing `tmp/whisper_autosrt-0.1.2.tar.gz` & `tmp/whisper_autosrt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_autosrt-0.1.2.tar", last modified: Fri Jun  9 01:38:23 2023, max compression
+gzip compressed data, was "whisper_autosrt-0.1.3.tar", last modified: Wed Jun 14 19:38:15 2023, max compression
```

## Comparing `whisper_autosrt-0.1.2.tar` & `whisper_autosrt-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 01:38:23.281040 whisper_autosrt-0.1.2/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1956 2023-06-09 01:38:23.281789 whisper_autosrt-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4700 2023-05-27 16:57:41.000000 whisper_autosrt-0.1.2/README.md
--rw-rw-rw-   0        0        0      147 2023-06-09 01:38:23.284787 whisper_autosrt-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1642 2023-06-02 17:36:46.000000 whisper_autosrt-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 01:38:23.251074 whisper_autosrt-0.1.2/whisper_autosrt/
--rw-rw-rw-   0        0        0   136062 2023-06-09 01:37:23.000000 whisper_autosrt-0.1.2/whisper_autosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 01:38:23.279541 whisper_autosrt-0.1.2/whisper_autosrt.egg-info/
--rw-rw-rw-   0        0        0     1956 2023-06-09 01:38:23.000000 whisper_autosrt-0.1.2/whisper_autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-06-09 01:38:23.000000 whisper_autosrt-0.1.2/whisper_autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 01:38:23.000000 whisper_autosrt-0.1.2/whisper_autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-06-09 01:38:23.000000 whisper_autosrt-0.1.2/whisper_autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      119 2023-06-09 01:38:23.000000 whisper_autosrt-0.1.2/whisper_autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-09 01:38:23.000000 whisper_autosrt-0.1.2/whisper_autosrt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 19:38:15.569800 whisper_autosrt-0.1.3/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1956 2023-06-14 19:38:15.569800 whisper_autosrt-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4700 2023-05-27 16:57:41.000000 whisper_autosrt-0.1.3/README.md
+-rw-rw-rw-   0        0        0      147 2023-06-14 19:38:15.572797 whisper_autosrt-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1642 2023-06-02 17:36:46.000000 whisper_autosrt-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 19:38:15.531588 whisper_autosrt-0.1.3/whisper_autosrt/
+-rw-rw-rw-   0        0        0   142065 2023-06-14 19:37:26.000000 whisper_autosrt-0.1.3/whisper_autosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 19:38:15.567551 whisper_autosrt-0.1.3/whisper_autosrt.egg-info/
+-rw-rw-rw-   0        0        0     1956 2023-06-14 19:38:15.000000 whisper_autosrt-0.1.3/whisper_autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-06-14 19:38:15.000000 whisper_autosrt-0.1.3/whisper_autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 19:38:15.000000 whisper_autosrt-0.1.3/whisper_autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-14 19:38:15.000000 whisper_autosrt-0.1.3/whisper_autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      119 2023-06-14 19:38:15.000000 whisper_autosrt-0.1.3/whisper_autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-14 19:38:15.000000 whisper_autosrt-0.1.3/whisper_autosrt.egg-info/top_level.txt
```

### Comparing `whisper_autosrt-0.1.2/LICENSE` & `whisper_autosrt-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.1.2/PKG-INFO` & `whisper_autosrt-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper_autosrt
-Version: 0.1.2
+Version: 0.1.3
 Summary: a command line utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/whisper_autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `whisper_autosrt-0.1.2/README.md` & `whisper_autosrt-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.1.2/setup.py` & `whisper_autosrt-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.1.2/whisper_autosrt/__init__.py` & `whisper_autosrt-0.1.3/whisper_autosrt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import warnings
 warnings.filterwarnings("ignore", message=".*The 'nopython' keyword.*")
 from faster_whisper import WhisperModel
 import ctypes
 import shutil
 
 
-VERSION = "0.1.2"
+VERSION = "0.1.3"
 #marker='█'
 
 
 class WhisperLanguage:
     def __init__(self):
         self.list_codes = []
         self.list_codes.append("auto")
@@ -2287,15 +2287,16 @@
     parser.add_argument('-S', '--src-language', help="Language code of the audio language spoken in video/audio source_path", default="auto")
     parser.add_argument('-D', '--dst-language', help="Desired translation language code for the subtitles", default=None)
     parser.add_argument('-lS', '--list-src-languages', help="List all available src_languages (whisper supported languages)", action='store_true')
     parser.add_argument('-lD', '--list-dst-languages', help="List all available dst_languages (google translate supported languages)", action='store_true')
     parser.add_argument('-F', '--format', help="Desired subtitle format", default="srt")
     parser.add_argument('-lF', '--list-formats', help="List all supported subtitle formats", action='store_true')
     parser.add_argument('-c', '--concurrency', help="Number of concurrent calls for Google Translate API", type=int, default=10)
-    parser.add_argument('-e', '--embed', help="Boolean value (True or False) for embedding subtitle file into video file", type=bool, default=False)
+    parser.add_argument('-es', '--embed-src', help="Boolean value (True or False) for embedding original language subtitle file into video file", type=bool, default=False)
+    parser.add_argument('-ed', '--embed-dst', help="Boolean value (True or False) for embedding translated subtitle file into video file", type=bool, default=False)
     parser.add_argument('-fr', '--force-recognize', help="Boolean value (True or False) for re-recognize media file event if it's already has subtitles stream", type=bool, default=False)
     parser.add_argument('-v', '--version', action='version', version=VERSION)
 
     args = parser.parse_args()
 
     src_language = args.src_language
     dst_language = args.dst_language
@@ -2444,18 +2445,23 @@
     task = "transcribe"
     total_duration = 0
 
     if args.src_language in google_unsupported_languages and do_translate:
         task = "translate"
         src_language = "en"
 
-    if str(args.embed) == "true":
-        args.embed = True
-    if str(args.embed) == "false":
-        args.embed = False
+    if str(args.embed_src) == "true":
+        args.embed_src = True
+    if str(args.embed_src) == "false":
+        args.embed_src = False
+
+    if str(args.embed_dst) == "true":
+        args.embed_dst = True
+    if str(args.embed_dst) == "false":
+        args.embed_dst = False
 
     removed_media_filepaths = []
     dst_language = args.dst_language
 
     print("CHECKING EXISTING SUBTITLES STREAMS")
     print("===================================")
 
@@ -2490,15 +2496,15 @@
                     else:
                         stop_ffmpeg_linux(error_messages_callback=show_error_messages)
 
                     remove_temp_files("wav")
                     sys.exit(1)
 
                 except Exception as e:
-                    if not KeyboardInterrupt in e:
+                    if not KeyboardInterrupt in str(e):
                         pbar.finish()
                         pool.terminate()
                         pool.close()
                         pool.join()
                         print(e)
 
                         if sys.platform == "win32":
@@ -2509,41 +2515,53 @@
                         remove_temp_files("wav")
                         sys.exit(1)
 
             else:
                 src_language = args.src_language
 
             if src_language in google_unsupported_languages and args.force_recognize==False:
+                print("Language is not supported by Google Translate API")
                 removed_media_filepaths.append(media_filepath)
 
             else:
                 ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
 
                 subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
                 subtitle_streams_data = subtitle_stream_parser(media_filepath)
 
                 if subtitle_streams_data and subtitle_streams_data != []:
 
                     src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
 
                     if ffmpeg_src_language_code in subtitle_stream_parser.languages():
                         print("Is '%s' subtitle stream exist        : Yes" %(ffmpeg_src_language_code.center(3)))
+
                         subtitle_stream_regions = []
                         subtitle_stream_transcripts = []
                         for entry in src_subtitle_stream_timed_subtitles:
                             subtitle_stream_regions.append(entry[0])
                             subtitle_stream_transcripts.append(entry[1])
+
                         base, ext = os.path.splitext(media_filepath)
                         src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src_language, format=subtitle_format)
-                        writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
+
                         print(f"Extracting '{ffmpeg_src_language_code}' subtitle stream as   : '{src_subtitle_filepath}'")
+
+                        writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                         writer.write(src_subtitle_filepath)
+
                         if args.force_recognize == False:
                             removed_media_filepaths.append(media_filepath)
 
+                        # no translate process as instructed in command arguments
+
+                        # if args.embed_src is True we can't embed it because dst subtitle stream already exist
+                        if args.embed_src == True and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
+                            print(f"No need to embed '{ffmpeg_src_language_code}' subtitle stream because it's already existed")
+
                     else:
                         print("Is '%s' subtitle stream exist        : No" %(ffmpeg_src_language_code.center(3)))
 
             print("")
 
         if removed_media_filepaths:
             for removed_media_filepath in removed_media_filepaths:
@@ -2589,15 +2607,15 @@
                     else:
                         stop_ffmpeg_linux(error_messages_callback=show_error_messages)
 
                     remove_temp_files("wav")
                     sys.exit(1)
 
                 except Exception as e:
-                    if not KeyboardInterrupt in e:
+                    if not KeyboardInterrupt in str(e):
                         pbar.finish()
                         pool.terminate()
                         pool.close()
                         pool.join()
                         print(e)
 
                         if sys.platform == "win32":
@@ -2608,14 +2626,15 @@
                         remove_temp_files("wav")
                         sys.exit(1)
 
             else:
                 src_language = args.src_language
 
             if src_language in google_unsupported_languages and args.force_recognize==False:
+                print(f"Language '{src_language}' is not supported by Google Translate API")
                 removed_media_filepaths.append(media_filepath)
 
             else:
                 ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
                 ffmpeg_dst_language_code = google_language.ffmpeg_code_of_code[dst_language]
 
                 subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
@@ -2625,23 +2644,27 @@
 
                     src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
                     dst_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_dst_language_code)
 
                     # ffmpeg_src_language_code subtitle stream exist, we print it and extract it
                     if ffmpeg_src_language_code in subtitle_stream_parser.languages():
                         print("Is '%s' subtitle stream exist        : Yes" %(ffmpeg_src_language_code.center(3)))
+
                         subtitle_stream_regions = []
                         subtitle_stream_transcripts = []
                         for entry in src_subtitle_stream_timed_subtitles:
                             subtitle_stream_regions.append(entry[0])
                             subtitle_stream_transcripts.append(entry[1])
+
                         base, ext = os.path.splitext(media_filepath)
                         src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src_language, format=subtitle_format)
-                        writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
+
                         print(f"Extracting '{ffmpeg_src_language_code}' subtitle stream as   : '{src_subtitle_filepath}'")
+
+                        writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                         writer.write(src_subtitle_filepath)
 
                     # ffmpeg_src_language_code subtitle stream not exist, just print it
                     else:
                         print("Is '%s' subtitle stream exist        : No" %(ffmpeg_src_language_code.center(3)))
 
                     # ffmpeg_src_language_code subtitle stream exist, we print it and extract it
@@ -2658,16 +2681,16 @@
                         print(f"Extracting '{ffmpeg_dst_language_code}' subtitle stream as   : '{dst_subtitle_filepath}'")
                         writer.write(dst_subtitle_filepath)
 
                     # ffmpeg_dst_language_code subtitle stream not exist, just print it
                     else:
                         print("Is '%s' subtitle stream exist        : No" %(ffmpeg_dst_language_code.center(3)))
 
-                    # ffmpeg_dst_language_code subtitle stream = exist,
                     # ffmpeg_src_language_code subtitle stream = not exist,
+                    # ffmpeg_dst_language_code subtitle stream = exist,
                     # so we translate it from 'dst_language' to 'src_language'
                     if ffmpeg_dst_language_code in subtitle_stream_parser.languages() and ffmpeg_src_language_code not in subtitle_stream_parser.languages():
 
                         if dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
                             prompt = "Translating from %s to %s : " %(dst_language.center(8), src_language.center(8))
                             widgets = [prompt, Percentage(), ' ', Bar(), ' ', ETA()]
                             pbar = ProgressBar(widgets=widgets, maxval=len(dst_subtitle_stream_timed_subtitles)).start()
@@ -2677,41 +2700,50 @@
                             translated_subtitle_stream_transcripts = []
                             for i, translated_subtitle_stream_transcript in enumerate(pool.imap(transcript_translator, subtitle_stream_transcripts)):
                                 translated_subtitle_stream_transcripts.append(translated_subtitle_stream_transcript)
                                 pbar.update(i)
                             pbar.finish()
 
                             base, ext = os.path.splitext(media_filepath)
-                            dst_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src_language, format=subtitle_format)
+                            src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src_language, format=subtitle_format)
+
                             translation_writer = SubtitleWriter(subtitle_stream_regions, translated_subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
-                            translation_writer.write(dst_subtitle_filepath)
-                            print(f"Translated subtitles file saved as    : '{dst_subtitle_filepath}'")
+                            translation_writer.write(src_subtitle_filepath)
+
+                            print(f"Translated subtitles file saved as    : '{src_subtitle_filepath}'")
+
                             if args.force_recognize == False:
                                 removed_media_filepaths.append(media_filepath)
 
-                            if args.embed and dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
-                                base, ext = os.path.splitext(media_filepath)
-                                tmp_embedded_media_filepath_1 = "{base}.embedded1.{format}".format(base=base, format=ext[1:])
+                            if args.embed_src and dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
                                 ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
+
+                                base, ext = os.path.splitext(media_filepath)
+                                src_tmp_embedded_media_filepath = "{base}.{src}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
                                 embedded_media_filepath = "{base}.{src}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
 
                                 widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                                 pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                                subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_src_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                                result = subtitle_embedder(media_filepath)
+                                subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                                src_tmp_output = subtitle_embedder(media_filepath)
                                 pbar.finish()
 
-                                if os.path.isfile(tmp_embedded_media_filepath_1):
-                                    shutil.copy(tmp_embedded_media_filepath_1, embedded_media_filepath)
-                                    os.remove(tmp_embedded_media_filepath_1)
+                                if os.path.isfile(src_tmp_output):
+                                    shutil.copy(src_tmp_output, embedded_media_filepath)
+                                    os.remove(src_tmp_output)
+
                                 if os.path.isfile(embedded_media_filepath):
                                     print(f"Subtitle embedded {media_type} file saved as : '{embedded_media_filepath}'")
 
-                    # ffmpeg_dst_language_code subtitle stream = not exist,
+                            # if args.embed_dst is True we can't embed it because dst subtitle stream already exist
+                            if args.embed_dst == True and dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
+                                print(f"No need to embed '{ffmpeg_dst_language_code}' subtitle stream because it's already existed")
+
                     # ffmpeg_src_language_code subtitle stream = exist,
+                    # ffmpeg_dst_language_code subtitle stream = not exist,
                     # so we translate it from 'src_language' to 'dst_language'
                     if ffmpeg_dst_language_code not in subtitle_stream_parser.languages() and ffmpeg_src_language_code in subtitle_stream_parser.languages():
 
                         if src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
                             prompt = "Translating from %s to %s : " %(src_language.center(8), dst_language.center(8))
                             widgets = [prompt, Percentage(), ' ', Bar(), ' ', ETA()]
                             pbar = ProgressBar(widgets=widgets, maxval=len(src_subtitle_stream_timed_subtitles)).start()
@@ -2722,45 +2754,64 @@
                             for i, translated_subtitle_stream_transcript in enumerate(pool.imap(transcript_translator, subtitle_stream_transcripts)):
                                 translated_subtitle_stream_transcripts.append(translated_subtitle_stream_transcript)
                                 pbar.update(i)
                             pbar.finish()
 
                             base, ext = os.path.splitext(media_filepath)
                             dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=dst_language, format=subtitle_format)
+
                             translation_writer = SubtitleWriter(subtitle_stream_regions, translated_subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                             translation_writer.write(dst_subtitle_filepath)
+
                             print(f"Translated subtitles file saved as    : '{dst_subtitle_filepath}'")
+
                             if args.force_recognize == False:
                                 removed_media_filepaths.append(media_filepath)
 
-                        if args.embed and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
-                            ffmpeg_dst_language_code = google_language.ffmpeg_code_of_code[dst_language]
-                            base, ext = os.path.splitext(media_filepath)
-                            tmp_embedded_media_filepath_1 = "{base}.embedded1.{format}".format(base=base, format=ext[1:])
-                            embedded_media_filepath = "{base}.{dst}.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
+                            if args.embed_dst == True and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
+                                ffmpeg_dst_language_code = google_language.ffmpeg_code_of_code[dst_language]
 
-                            widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type}  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
-                            pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                            subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                            result = subtitle_embedder(media_filepath)
-                            pbar.finish()
+                                base, ext = os.path.splitext(media_filepath)
+                                dst_tmp_embedded_media_filepath = "{base}.{dst}.tmp.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
+                                embedded_media_filepath = "{base}.{dst}.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
+
+                                widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type}  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                                pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                                subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                                dst_tmp_output = subtitle_embedder(media_filepath)
+                                pbar.finish()
+
+                                if os.path.isfile(dst_tmp_output):
+                                    shutil.copy(dst_tmp_output, embedded_media_filepath)
+                                    os.remove(dst_tmp_output)
+
+                                if os.path.isfile(embedded_media_filepath):
+                                    print(f"Subtitle embedded {media_type} file saved as : '{embedded_media_filepath}'")
 
-                            if os.path.isfile(tmp_embedded_media_filepath_1):
-                                shutil.copy(tmp_embedded_media_filepath_1, embedded_media_filepath)
-                                os.remove(tmp_embedded_media_filepath_1)
-                            if os.path.isfile(embedded_media_filepath):
-                                print(f"Subtitle embedded {media_type} file saved as : '{embedded_media_filepath}'")
+                            # if args.embed_src is True then no need to embed it because src subtitle stream already exist
+                            if args.embed_src == True and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
+                                print(f"No need to embed '{ffmpeg_src_language_code}' subtitle stream because it's already existed")
 
                     # ffmpeg_dst_language_code subtitle stream = exist,
                     # ffmpeg_src_language_code subtitle stream = exist,
                     # so we remove media_filepath from the list of files to be proceed
                     elif ffmpeg_dst_language_code in subtitle_stream_parser.languages() and ffmpeg_src_language_code in subtitle_stream_parser.languages():
                         if args.force_recognize == False:
                             removed_media_filepaths.append(media_filepath)
 
+                        # no need to translate becouse both languages subtitle files already saved
+
+                        # if args.embed_src is True we can't embed it because dst subtitle stream already exist
+                        if args.embed_src == True and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
+                            print(f"No need to embed '{ffmpeg_src_language_code}' subtitle stream because it's already existed")
+
+                        # if args.embed_dst is True we can't embed it because dst subtitle stream already exist
+                        if args.embed_dst == True and dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
+                            print(f"No need to embed '{ffmpeg_dst_language_code}' subtitle stream because it's already existed")
+
                 print("")
 
         if removed_media_filepaths:
             for removed_media_filepath in removed_media_filepaths:
                 if removed_media_filepath in media_filepaths:
                     media_filepaths.remove(removed_media_filepath)
 
@@ -2815,14 +2866,15 @@
                 transcripts.append(segment.text)
                 pbar.update(progress)
             pbar.finish()
             timed_subtitles = [(r, t) for r, t in zip(regions, transcripts) if t]
 
             base, ext = os.path.splitext(media_filepath)
             src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src_language, format=subtitle_format)
+
             writer = SubtitleWriter(regions, transcripts, subtitle_format, error_messages_callback=show_error_messages)
             writer.write(src_subtitle_filepath)
 
             if do_translate:
                 timed_subtitles = writer.timed_subtitles
                 created_regions = []
                 created_subtitles = []
@@ -2840,82 +2892,141 @@
                 for i, translated_subtitle in enumerate(pool.imap(transcript_translator, created_subtitles)):
                     translated_subtitles.append(translated_subtitle)
                     pbar.update(i)
                 pbar.finish()
 
                 base, ext = os.path.splitext(media_filepath)
                 dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=args.dst_language, format=subtitle_format)
+
                 translation_writer = SubtitleWriter(created_regions, translated_subtitles, subtitle_format, error_messages_callback=show_error_messages)
                 translation_writer.write(dst_subtitle_filepath)
 
             if do_translate:
                 print(f"Original subtitles file saved as      : '{src_subtitle_filepath}'")
                 print(f"Translated subtitles file saved as    : '{dst_subtitle_filepath}'")
             else:
                 print(f"Subtitles file saved as               : '{src_subtitle_filepath}'")
 
-            if args.embed:
-                base, ext = os.path.splitext(media_filepath)
-                tmp_embedded_media_filepath_1 = "{base}.embedded1.{format}".format(base=base, format=ext[1:])
-                tmp_embedded_media_filepath_2 = "{base}.embedded2.{format}".format(base=base, format=ext[1:])
-                tmp_embedded_media_filepath_3 = "{base}.embedded3.{format}".format(base=base, format=ext[1:])
-                embedded_media_filepath = None
 
-                if do_translate:
+            # EMBEDDING SUBTITLE FILE
+
+            embedded_media_filepath = None
+
+            if do_translate == False:
+
+                if args.embed_src == True:
+
+                    ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
+
+                    base, ext = os.path.splitext(media_filepath)
+                    src_tmp_embedded_media_filepath = "{base}.{src}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
+                    embedded_media_filepath = "{base}.{src}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
+
+                    widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                    pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                    subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                    src_tmp_output = subtitle_embedder(media_filepath)
+                    pbar.finish()
+
+                    if os.path.isfile(src_tmp_output):
+                        shutil.copy(src_tmp_output, embedded_media_filepath)
+                        os.remove(src_tmp_output)
+                        print("Subtitle embedded {} file saved as   : {}".format(media_type, embedded_media_filepath))
+
+            elif do_translate == True:
+
+                if args.embed_src == True and args.embed_dst == True:
+
                     ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
                     ffmpeg_dst_language_code = google_language.ffmpeg_code_of_code[dst_language]
+
+                    base, ext = os.path.splitext(media_filepath)
+                    src_tmp_embedded_media_filepath = "{base}.{src}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
+                    src_dst_tmp_embedded_media_filepath = "{base}.{src}.{dst}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, dst=ffmpeg_dst_language_code, format=ext[1:])
                     embedded_media_filepath = "{base}.{src}.{dst}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, dst=ffmpeg_dst_language_code, format=ext[1:])
 
                     widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                     pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                    subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                    result = subtitle_embedder(media_filepath)
+                    subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                    src_tmp_output = subtitle_embedder(media_filepath)
                     pbar.finish()
 
-                    if os.path.isfile(tmp_embedded_media_filepath_1) and os.path.isfile(dst_subtitle_filepath):
-                        widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type}  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
-                        pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=tmp_embedded_media_filepath_2, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                        result = subtitle_embedder(tmp_embedded_media_filepath_1)
-                        pbar.finish()
-                    elif (not os.path.isfile(tmp_embedded_media_filepath_1)) and os.path.isfile(dst_subtitle_filepath):
+                    if os.path.isfile(src_tmp_output) and os.path.isfile(dst_subtitle_filepath):
                         widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type}  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                         pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=tmp_embedded_media_filepath_2, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                        result = subtitle_embedder(media_filepath)
+                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=src_dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                        src_dst_tmp_output = subtitle_embedder(src_tmp_embedded_media_filepath)
                         pbar.finish()
+                    else:
+                        print("Unknown error!")
 
-                    if os.path.isfile(tmp_embedded_media_filepath_2):
-                        shutil.copy(tmp_embedded_media_filepath_2, embedded_media_filepath)
+                    if os.path.isfile(src_dst_tmp_output):
+                        shutil.copy(src_dst_tmp_output, embedded_media_filepath)
+                        print("Subtitle embedded {} file saved as   : {}".format(media_type, embedded_media_filepath))
 
-                    if os.path.isfile(tmp_embedded_media_filepath_1):
-                        os.remove(tmp_embedded_media_filepath_1)
-                    if os.path.isfile(tmp_embedded_media_filepath_2):
-                        os.remove(tmp_embedded_media_filepath_2)
+                    if os.path.isfile(src_dst_tmp_output):
+                        os.remove(src_dst_tmp_output)
+
+                    if os.path.isfile(src_tmp_output):
+                        os.remove(src_tmp_output)
+
+                elif args.embed_src == True and args.embed_dst == False:
 
-                else:
                     ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
+
+                    base, ext = os.path.splitext(media_filepath)
+                    src_tmp_embedded_media_filepath = "{base}.{src}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
                     embedded_media_filepath = "{base}.{src}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
 
-                    #result = embed_subtitle_to_media(media_filepath, media_type, src_subtitle_filepath, ffmpeg_src_language_code, tmp_embedded_media_filepath_1)
+                    widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                    pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                    subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                    src_tmp_output = subtitle_embedder(media_filepath)
+                    pbar.finish()
+
+                    if os.path.isfile(src_tmp_output):
+                        shutil.copy(src_tmp_output, embedded_media_filepath)
+                        os.remove(src_tmp_embedded_media_filepath)
+                        print("Subtitle embedded {} file saved as   : {}".format(media_type, embedded_media_filepath))
+                    else:
+                        print("Unknown error!")
 
-                    widgets = [f"Embedding \'{ffmpeg_src_language_code}\' subtitles into {media_type}  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                elif args.embed_src == False and args.embed_dst == True:
+
+                    ffmpeg_dst_language_code = google_language.ffmpeg_code_of_code[dst_language]
+
+                    base, ext = os.path.splitext(media_filepath)
+                    dst_tmp_embedded_media_filepath = "{base}.{dst}.tmp.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
+                    embedded_media_filepath = "{base}.{dst}.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
+
+                    widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                     pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                    subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                    result = subtitle_embedder(media_filepath)
+                    subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                    dst_tmp_output = subtitle_embedder(media_filepath)
                     pbar.finish()
 
-                    if tmp_embedded_media_filepath_1:
-                        shutil.copy(tmp_embedded_media_filepath_1, embedded_media_filepath)
-                        os.remove(tmp_embedded_media_filepath_1)
+                    if os.path.isfile(dst_tmp_output):
+                        shutil.copy(dst_tmp_output, embedded_media_filepath)
+                        os.remove(dst_tmp_output)
+                        print("Subtitle embedded {} file saved as : {}".format(media_type, embedded_media_filepath))
+                    else:
+                        print("Unknown error!")
+
+            if do_translate == False:
+                if args.embed_src == True:
+                    if embedded_media_filepath and os.path.isfile(embedded_media_filepath):
+                        completed_tasks += 1
+                else:
+                    completed_tasks += 1
 
-            if not args.embed:
-                completed_tasks += 1
-            else:
-                if embedded_media_filepath and os.path.isfile(embedded_media_filepath):
+            elif do_translate == True:
+                if args.embed_src == True or args.embed_dst == True:
+                    if embedded_media_filepath and os.path.isfile(embedded_media_filepath):
+                        completed_tasks += 1
+                else:
                     completed_tasks += 1
 
             print("")
             if len(media_filepaths)>0 and completed_tasks == len(media_filepaths):
                 transcribe_end_time = time.time()
                 transcribe_elapsed_time = transcribe_end_time - transcribe_start_time
                 transcribe_elapsed_time_seconds = timedelta(seconds=int(transcribe_elapsed_time))
@@ -2937,15 +3048,15 @@
             else:
                 stop_ffmpeg_linux(error_messages_callback=show_error_messages)
 
             remove_temp_files("wav")
             return 1
 
         except Exception as e:
-            if not KeyboardInterrupt in e:
+            if not KeyboardInterrupt in str(e):
                 pbar.finish()
                 pool.terminate()
                 pool.close()
                 pool.join()
                 print(e)
 
                 if sys.platform == "win32":
```

### Comparing `whisper_autosrt-0.1.2/whisper_autosrt.egg-info/PKG-INFO` & `whisper_autosrt-0.1.3/whisper_autosrt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-autosrt
-Version: 0.1.2
+Version: 0.1.3
 Summary: a command line utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/whisper_autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

