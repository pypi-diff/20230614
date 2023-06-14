# Comparing `tmp/lecture_automator-1.0.0.tar.gz` & `tmp/lecture_automator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lecture_automator-1.0.0.tar", max compression
+gzip compressed data, was "lecture_automator-1.1.0.tar", max compression
```

## Comparing `lecture_automator-1.0.0.tar` & `lecture_automator-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0     2733 2023-05-11 20:11:42.478981 lecture_automator-1.0.0/README.md
--rw-r--r--   0        0        0     2208 2023-05-11 20:10:35.111655 lecture_automator-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-09 16:38:42.823945 lecture_automator-1.0.0/src/lecture_automator/__init__.py
--rw-r--r--   0        0        0     1142 2023-05-11 20:10:35.112014 lecture_automator-1.0.0/src/lecture_automator/cli.py
--rw-r--r--   0        0        0      792 2023-05-11 20:10:35.112300 lecture_automator-1.0.0/src/lecture_automator/compiler.py
--rw-r--r--   0        0        0        0 2023-05-01 10:48:09.376126 lecture_automator-1.0.0/src/lecture_automator/gen_speech/__init__.py
--rw-r--r--   0        0        0       43 2023-05-11 20:10:35.112561 lecture_automator-1.0.0/src/lecture_automator/gen_speech/exceptions.py
--rw-r--r--   0        0        0     3082 2023-05-11 20:10:35.113119 lecture_automator-1.0.0/src/lecture_automator/gen_speech/gen_speech.py
--rw-r--r--   0        0        0     1970 2023-05-11 20:10:35.113510 lecture_automator-1.0.0/src/lecture_automator/gen_speech/utils.py
--rw-r--r--   0        0        0        0 2023-05-11 20:10:35.113563 lecture_automator-1.0.0/src/lecture_automator/gen_video/__init__.py
--rw-r--r--   0        0        0       47 2023-05-11 20:10:35.113973 lecture_automator-1.0.0/src/lecture_automator/gen_video/exceptions.py
--rw-r--r--   0        0        0     1179 2023-05-11 20:10:35.114255 lecture_automator-1.0.0/src/lecture_automator/gen_video/gen_video.py
--rw-r--r--   0        0        0      469 2023-05-11 20:10:35.114460 lecture_automator-1.0.0/src/lecture_automator/gen_video/utils.py
--rw-r--r--   0        0        0     1090 2023-05-11 20:10:35.114753 lecture_automator-1.0.0/src/lecture_automator/marp_api.py
--rw-r--r--   0        0        0        0 2023-05-11 20:10:35.114804 lecture_automator-1.0.0/src/lecture_automator/parser/__init__.py
--rw-r--r--   0        0        0     1394 2023-05-11 20:10:35.119965 lecture_automator-1.0.0/src/lecture_automator/parser/command_handler.py
--rw-r--r--   0        0        0       84 2023-05-11 20:10:35.115338 lecture_automator-1.0.0/src/lecture_automator/parser/exceptions.py
--rw-r--r--   0        0        0     4364 2023-05-11 20:10:35.119793 lecture_automator-1.0.0/src/lecture_automator/parser/parser.py
--rw-r--r--   0        0        0      369 2023-05-11 20:10:35.115995 lecture_automator-1.0.0/src/lecture_automator/settings.py
--rw-r--r--   0        0        0      749 2023-05-11 20:10:35.116220 lecture_automator-1.0.0/src/lecture_automator/web.py
--rw-r--r--   0        0        0     3402 1970-01-01 00:00:00.000000 lecture_automator-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     5661 2023-05-14 15:34:36.841907 lecture_automator-1.1.0/README.md
+-rw-r--r--   0        0        0     2225 2023-05-14 15:34:36.843037 lecture_automator-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-09 16:38:42.823945 lecture_automator-1.1.0/src/lecture_automator/__init__.py
+-rw-r--r--   0        0        0     1503 2023-05-14 15:34:36.843184 lecture_automator-1.1.0/src/lecture_automator/cli.py
+-rw-r--r--   0        0        0     1151 2023-05-14 15:34:36.843364 lecture_automator-1.1.0/src/lecture_automator/compiler.py
+-rw-r--r--   0        0        0        0 2023-05-01 10:48:09.376126 lecture_automator-1.1.0/src/lecture_automator/gen_speech/__init__.py
+-rw-r--r--   0        0        0       43 2023-05-11 20:10:35.112561 lecture_automator-1.1.0/src/lecture_automator/gen_speech/exceptions.py
+-rw-r--r--   0        0        0     3228 2023-05-14 15:34:36.843546 lecture_automator-1.1.0/src/lecture_automator/gen_speech/gen_speech.py
+-rw-r--r--   0        0        0     1970 2023-05-11 20:10:35.113510 lecture_automator-1.1.0/src/lecture_automator/gen_speech/utils.py
+-rw-r--r--   0        0        0        0 2023-05-11 20:10:35.113563 lecture_automator-1.1.0/src/lecture_automator/gen_video/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-14 15:34:36.843879 lecture_automator-1.1.0/src/lecture_automator/gen_video/exceptions.py
+-rw-r--r--   0        0        0     1241 2023-05-14 15:34:36.844105 lecture_automator-1.1.0/src/lecture_automator/gen_video/gen_video.py
+-rw-r--r--   0        0        0      469 2023-05-11 20:10:35.114460 lecture_automator-1.1.0/src/lecture_automator/gen_video/utils.py
+-rw-r--r--   0        0        0        0 2023-05-14 15:34:36.844140 lecture_automator-1.1.0/src/lecture_automator/marp_api/__init__.py
+-rw-r--r--   0        0        0      181 2023-05-14 15:34:36.844545 lecture_automator-1.1.0/src/lecture_automator/marp_api/exceptions.py
+-rw-r--r--   0        0        0     1416 2023-05-14 15:34:36.844781 lecture_automator-1.1.0/src/lecture_automator/marp_api/marp_api.py
+-rw-r--r--   0        0        0        0 2023-05-11 20:10:35.114804 lecture_automator-1.1.0/src/lecture_automator/parser/__init__.py
+-rw-r--r--   0        0        0     1359 2023-05-14 15:34:36.845279 lecture_automator-1.1.0/src/lecture_automator/parser/command_handler.py
+-rw-r--r--   0        0        0       84 2023-05-11 20:10:35.115338 lecture_automator-1.1.0/src/lecture_automator/parser/exceptions.py
+-rw-r--r--   0        0        0     4364 2023-05-11 20:10:35.119793 lecture_automator-1.1.0/src/lecture_automator/parser/parser.py
+-rw-r--r--   0        0        0      369 2023-05-11 20:10:35.115995 lecture_automator-1.1.0/src/lecture_automator/settings.py
+-rw-r--r--   0        0        0      749 2023-05-14 15:32:24.947200 lecture_automator-1.1.0/src/lecture_automator/web.py
+-rw-r--r--   0        0        0     6368 1970-01-01 00:00:00.000000 lecture_automator-1.1.0/PKG-INFO
```

### Comparing `lecture_automator-1.0.0/pyproject.toml` & `lecture_automator-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "lecture-automator"
-version = "1.0.0"
+version = "1.1.0"
 description = ""
 authors = ["CapBlood <stalker.anonim@mail.ru>"]
 readme = "README.md"
 homepage = "https://github.com/CapBlood/lecture-automator.git"
 
 [tool.poetry.dependencies]
 python = "^3.8,<=3.9"
 ffmpeg-python = "^0.2.0"
 torch = "^2.0.0"
 numpy = "^1.24.2"
 click = "^8.1.3"
 sympy = "^1.11.1"
 streamlit = "^1.22.0"
+tqdm = "^4.65.0"
 
 [tool.poetry.extras]
 test = ["pytest"]
 
 [tool.poetry.group.dev.dependencies]
 pytest-cov = "^4.0.0"
 tox = "^4.4.11"
```

### Comparing `lecture_automator-1.0.0/src/lecture_automator/cli.py` & `lecture_automator-1.1.0/src/lecture_automator/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import click
+from ffmpeg._run import Error as FFmpegError
 
 from lecture_automator.compiler import compile_text_md
+from lecture_automator.marp_api.exceptions import MarpError
 from lecture_automator.web import run_web
 
 
 @click.group()
 def cli():
     pass
 
@@ -36,18 +38,26 @@
         'значение 1 соответствует разрешению 1280x720.'
     )
 )
 def convert(input_md, out_path, scale, vformat):
     with open(input_md) as file:
         md_text = file.read()
 
-    compile_text_md(
-        md_text, out_path=out_path,
-        vformat=vformat, scale=scale
-    )
+    try:
+        compile_text_md(
+            md_text, out_path=out_path,
+            vformat=vformat, scale=scale,
+            verbose_progress=True
+        )
+    except FFmpegError as e:
+        print('Ошибка ffmpeg:')
+        print(e.stderr.decode())
+    except MarpError as e:
+        print('Ошибка Marp:')
+        print(e.stderr.decode())
 
 
 @cli.command()
 def web():
     run_web()
```

### Comparing `lecture_automator-1.0.0/src/lecture_automator/gen_speech/gen_speech.py` & `lecture_automator-1.1.0/src/lecture_automator/gen_speech/gen_speech.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     Returns:
         str: путь к синтезированной речи.
     """
 
     model.to(device)
 
     model.save_wav(
-        text=text,
+        ssml_text=text,
         speaker=SPEAKER,
         audio_path=out_path,
         sample_rate=SAMPLE_RATE
     )
 
     return out_path
 
@@ -61,14 +61,18 @@
     model = torch.package.PackageImporter(model_path).load_pickle(
         "tts_models", "model"
     )
 
     return model
 
 
+def preprocess_ssml_text(text: str) -> str:
+    return '<speak>{}</speak>'.format(text)
+
+
 def text_to_speech(text: str, out_path: str, device: str = 'cpu') -> str:
     """Синтез речи.
 
     Args:
         text (str): текст для синтеза речи.
         out_path (str): путь для сохранения сгенерированной речи.
         device (str, optional): устройство для вычислений (cuda, cpu и т.д.).
@@ -80,14 +84,15 @@
 
     model = get_model(MODEL_FILENAME)
 
     if len(text) > MAX_SYMBOLS:
         texts = divide_text(text, max_length=MAX_SYMBOLS)
     else:
         texts = [text]
+    texts = list(map(preprocess_ssml_text, texts))
 
     with tempfile.TemporaryDirectory() as tmpdirname:
         temp_wavs = []
         for i, t in enumerate(texts):
             temp_out_path = os.path.join(tmpdirname, 'speech_{}'.format(str(i)))
             generate_speech(model, t, temp_out_path)
             temp_wavs.append(temp_out_path)
```

### Comparing `lecture_automator-1.0.0/src/lecture_automator/gen_speech/utils.py` & `lecture_automator-1.1.0/src/lecture_automator/gen_speech/utils.py`

 * *Files identical despite different names*

### Comparing `lecture_automator-1.0.0/src/lecture_automator/gen_video/gen_video.py` & `lecture_automator-1.1.0/src/lecture_automator/gen_video/gen_video.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,8 +22,10 @@
 
     vcodec, acodec = get_codecs(vformat)
 
     joined = ffmpeg.concat(*files, v=1, a=1).node
     ffmpeg.output(
         joined[0], joined[1], output_name,
         f=vformat, vcodec=vcodec, acodec=acodec
-    ).run(overwrite_output=True)
+    ).run(overwrite_output=True,
+          capture_stdout=True,
+          capture_stderr=True)
```

### Comparing `lecture_automator-1.0.0/src/lecture_automator/marp_api.py` & `lecture_automator-1.1.0/src/lecture_automator/marp_api/marp_api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import os
 import subprocess
 import tempfile
 
+from lecture_automator.marp_api.exceptions import MarpError
+
 
 def generate_marp_slides(outdir: str, md_text: str, type_images: str = 'png', scale: float = 2.0) -> None:
     """Генерация слайдов презентации Marp в виде набора изображений.
 
     Args:
         outdir (str): директория для сохранения изображений.
         md_text (str): текст файла Markdown презентации Marp.
@@ -13,18 +15,27 @@
     """
 
     with tempfile.TemporaryDirectory() as tmpdirname:
         path_to_md = os.path.join(tmpdirname, "input.md")
         with open(path_to_md, "w") as file:
             file.write(md_text)
 
-        subprocess.run(
-            ['marp', '--images', type_images, '--image-scale', str(scale), '-o', 'Slide.png', path_to_md],
+        process = subprocess.Popen(
+            ['marp', '--images', type_images, '--image-scale', str(scale),
+             '-o', 'Slide.png', path_to_md],
+            stdin=subprocess.PIPE,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
             cwd=outdir
         )
 
+        out, err = process.communicate()
+        retcode = process.poll()
+        if retcode:
+            raise MarpError(out, err)
+
 
 if __name__ == '__main__':
     with open('examples/Example.md') as file:
         text = file.read()
 
     generate_marp_slides('examples', text, scale=1.5)
```

### Comparing `lecture_automator-1.0.0/src/lecture_automator/parser/command_handler.py` & `lecture_automator-1.1.0/src/lecture_automator/parser/command_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,14 @@
         handler = SpeechHandler()
         return handler.handle(slide, name_command, arg, start_pos, end_pos, metadata)
 
 
 class SpeechHandler(CommandHandler):
     def handle(self, slide, name_command, arg, start_pos, end_pos, metadata) -> str:
         if name_command == 'speech':
-            print(slide[end_pos:])
             if re.sub(r'(?m)[ \n\t]+', '', slide[end_pos:]):
                 raise Exception(
                     'Управляющая конструкция /speech должна находиться в конце описания слайда!'
                 )
             metadata.update(
                 {
                     'speech': arg
```

### Comparing `lecture_automator-1.0.0/src/lecture_automator/parser/parser.py` & `lecture_automator-1.1.0/src/lecture_automator/parser/parser.py`

 * *Files identical despite different names*

### Comparing `lecture_automator-1.0.0/src/lecture_automator/web.py` & `lecture_automator-1.1.0/src/lecture_automator/web.py`

 * *Files identical despite different names*

