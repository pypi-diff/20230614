# Comparing `tmp/pyautosrt-0.1.7.tar.gz` & `tmp/pyautosrt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyautosrt-0.1.7.tar", last modified: Sat Apr 15 02:11:55 2023, max compression
+gzip compressed data, was "pyautosrt-0.2.1.tar", last modified: Mon Jun 12 04:42:11 2023, max compression
```

## Comparing `pyautosrt-0.1.7.tar` & `pyautosrt-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 02:11:55.658001 pyautosrt-0.1.7/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 pyautosrt-0.1.7/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 pyautosrt-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2055 2023-04-15 02:11:55.658750 pyautosrt-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     3061 2023-02-10 19:35:06.000000 pyautosrt-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 02:11:55.635524 pyautosrt-0.1.7/pyautosrt/
--rw-rw-rw-   0        0        0    40142 2023-04-15 02:08:42.000000 pyautosrt-0.1.7/pyautosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 02:11:55.655753 pyautosrt-0.1.7/pyautosrt.egg-info/
--rw-rw-rw-   0        0        0     2055 2023-04-15 02:11:54.000000 pyautosrt-0.1.7/pyautosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-04-15 02:11:55.000000 pyautosrt-0.1.7/pyautosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 02:11:54.000000 pyautosrt-0.1.7/pyautosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-15 02:11:54.000000 pyautosrt-0.1.7/pyautosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-04-15 02:11:54.000000 pyautosrt-0.1.7/pyautosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-15 02:11:54.000000 pyautosrt-0.1.7/pyautosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-04-15 02:11:55.663245 pyautosrt-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1512 2023-04-15 02:08:56.000000 pyautosrt-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 04:42:11.062891 pyautosrt-0.2.1/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 pyautosrt-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 pyautosrt-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2055 2023-06-12 04:42:11.063642 pyautosrt-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3452 2023-04-24 17:27:22.000000 pyautosrt-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 04:42:11.011197 pyautosrt-0.2.1/pyautosrt/
+-rw-rw-rw-   0        0        0   213024 2023-06-12 04:41:04.000000 pyautosrt-0.2.1/pyautosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 04:42:11.046412 pyautosrt-0.2.1/pyautosrt.egg-info/
+-rw-rw-rw-   0        0        0     2055 2023-06-12 04:42:10.000000 pyautosrt-0.2.1/pyautosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-06-12 04:42:10.000000 pyautosrt-0.2.1/pyautosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 04:42:10.000000 pyautosrt-0.2.1/pyautosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-12 04:42:10.000000 pyautosrt-0.2.1/pyautosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2023-06-12 04:42:10.000000 pyautosrt-0.2.1/pyautosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-12 04:42:10.000000 pyautosrt-0.2.1/pyautosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-12 04:42:11.066639 pyautosrt-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1850 2023-06-11 02:57:09.000000 pyautosrt-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 04:42:11.061396 pyautosrt-0.2.1/test/
+-rw-rw-rw-   0        0        0    40142 2023-04-15 02:08:42.000000 pyautosrt-0.2.1/test/__init__.py
```

### Comparing `pyautosrt-0.1.7/LICENSE` & `pyautosrt-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyautosrt-0.1.7/PKG-INFO` & `pyautosrt-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautosrt
-Version: 0.1.7
+Version: 0.2.1
 Summary: pyautosrt is a python based desktop app to generate subtitle and translated subtitle file
 Home-page: https://github.com/botbahlul/pyautosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `pyautosrt-0.1.7/README.md` & `pyautosrt-0.2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,83 +1,84 @@
 # pyautosrt <a href="https://pypi.python.org/pypi/pyautosrt"><img src="https://img.shields.io/pypi/v/pyautosrt.svg"></img></a>
-  
-### Auto-generated subtitles for any video
+
+
+
+https://user-images.githubusercontent.com/88623122/218178963-fb77891c-1845-4514-8806-069dc342dca3.mp4
+
+
+
+### Auto generate subtitles files for any video/audio files
 
 PyAutoSRT is a PySimpleGUI based desktop app to auto generate subtitle and translated subtitle file for any video or audio file
 
+The core script is a modified version of original autosub made by Anastasis Germanidis
+https://github.com/agermanidis/autosub
+
 ### Installation
 
-if you don't have python on your Windows system you can get compiled version from https://github.com/botbahlul/pyautosrt/releases/
+If you don't have python on your Windows system you can get compiled version from https://github.com/botbahlul/pyautosrt/releases/
 
-just extract those ffmpeg.exe and pyautosrt.exe into a folder that has been added to PATH ENVIRONTMET for example in C:\Windows\system32
+Just extract those ffmpeg.exe and pyautosrt.exe into a folder that has been added to PATH ENVIRONTMET for example in C:\Windows\system32
 
-you can get latest version of ffmpeg from https://www.ffmpeg.org/
+You can get latest version of ffmpeg from https://www.ffmpeg.org/
 
-in Linux you have to install this script with python (version minimal 3.8 ) and install ffmpeg with your linux package manager for example in debian based linux distribution you can type :
+In Linux you have to install this script with python (version minimal 3.8 ) and install ffmpeg with your linux package manager for example in debian based linux distribution you can type :
 
 ```
 apt update
 apt install -y ffmpeg
 ```
 
-to install this pyautosrt, just type :
+To install this pyautosrt, just type :
 ```
 pip install pyautosrt
 ```
 
-you can compile this script into a single executable file with pyinstaller by downloading __init__.py file, rename it to pyautosrt.py and type :
+You can compile this script into a single executable file with pyinstaller by downloading "\__init\__.py" file, rename it to pyautosrt.py and type :
 ```
 pip install pyinstaller
 pyinstaller --onefile pyautosrt.py
 ```
 
-the executable compiled file will be placed by pyinstaller into dist subfolder of your current working folder, so you can just rename and put that compiled file into a folder that has been added to your PATH ENVIRONTMENT so you can execute it from anywhere
+The executable compiled file will be placed by pyinstaller into dist subfolder of your current working folder, so you can just rename and put that compiled file into a folder that has been added to your PATH ENVIRONTMENT so you can execute it from anywhere
 
 I was succesfuly compiled it in Windows 10 with pyinstaller-5.1 and Pyhton-3.10.4, and python-3.8.12 in Debian 9
 
-another alternative way to install this script with python is by cloning this git (or downloading this git as zip then extract it into a folder), and then just type :
+NOTES : SINCE VERSION 0.1.9 YOU SHOULD USE THAT \"mypyinstaller.bat\" (FOR WINDOWS) OR \"mypyinstaller.sh\" (FOR LINUX) TO COMPILE THAT \"pyautosrt.pyw\"
+
+Another alternative way to install this script with python is by cloning this git (or downloading this git as zip then extract it into a folder), and then just type :
 
 ```
 python setup.py build
 python setup.py install
 ```
 
-### Simple usage example 
-
-```
-pyautosrt --list-languages
-pyautosrt -S zh-CN -D en "Episode 1.mp4"
-```
-
-### usage 
+### Usage 
 
 ```
-pyautosrt [-h] [-C CONCURRENCY] [-o OUTPUT] [-F FORMAT]
-             [-S SRC_LANGUAGE] [-D DST_LANGUAGE]
-             [-n RENAME] [-p PATIENCE] [-v]
-             [--list-formats] [--list-languages]
-             [source_path]
+usage: pyautosrt.py [-h] [-S SRC_LANGUAGE] [-D DST_LANGUAGE] [-ll] [-F FORMAT] [-lf] [-v] [source_path ...]
 
 positional arguments:
-  source_path           Path to the video or audio file
+  source_path           Path to the video or audio files to generate subtitle (use wildcard for multiple files or separate them with
+                        space eg. "file 1.mp4" "file 2.mp4")
 
 options:
   -h, --help            show this help message and exit
-  -C CONCURRENCY, --concurrency CONCURRENCY
-                        Number of concurrent API requests to make
-  -o OUTPUT, --output OUTPUT
-                        Output path for subtitles (by default, subtitles are saved in the same directory and name as the source path)
-  -F FORMAT, --format FORMAT
-                        Destination subtitle format
   -S SRC_LANGUAGE, --src-language SRC_LANGUAGE
-                        Language spoken in source file
+                        Spoken language
   -D DST_LANGUAGE, --dst-language DST_LANGUAGE
-                        Desired language for the subtitles
-  -v, --version         show program's version number and exit
-  -lf, --list-formats   List all available subtitle formats
+                        Desired language for translation
   -ll, --list-languages
-                        List all available source/destination languages
+                        List all available source/translation languages
+  -F FORMAT, --format FORMAT
+                        Desired subtitle format
+  -lf, --list-formats   List all available subtitle formats
+  -v, --version         show program's version number and exit
 ```
 
+Those command switch '-S' and '-D' are not mandatory. It's just to make combobox directly select your desired language if you prefer to type it rather that click on combobox.
+
+UPDATE NOTES : SINCE VERSION 0.1.1 YOU CAN SELECT MULTIPLE VIDEO/AUDIO FILES, BUT REMEMBER THAT ALL FILES YOU SELECT SHOULD HAVE SAME AUDIO LANGUAGE AND DESIRED TRANSLATION LANGUAGE.
+
 ### License
 
 MIT
```

#### html2text {}

```diff
@@ -1,35 +1,42 @@
-# pyautosrt [https://img.shields.io/pypi/v/pyautosrt.svg] ### Auto-generated
-subtitles for any video PyAutoSRT is a PySimpleGUI based desktop app to auto
-generate subtitle and translated subtitle file for any video or audio file ###
-Installation if you don't have python on your Windows system you can get
-compiled version from https://github.com/botbahlul/pyautosrt/releases/ just
-extract those ffmpeg.exe and pyautosrt.exe into a folder that has been added to
-PATH ENVIRONTMET for example in C:\Windows\system32 you can get latest version
-of ffmpeg from https://www.ffmpeg.org/ in Linux you have to install this script
-with python (version minimal 3.8 ) and install ffmpeg with your linux package
-manager for example in debian based linux distribution you can type : ``` apt
-update apt install -y ffmpeg ``` to install this pyautosrt, just type : ``` pip
-install pyautosrt ``` you can compile this script into a single executable file
-with pyinstaller by downloading __init__.py file, rename it to pyautosrt.py and
-type : ``` pip install pyinstaller pyinstaller --onefile pyautosrt.py ``` the
-executable compiled file will be placed by pyinstaller into dist subfolder of
-your current working folder, so you can just rename and put that compiled file
-into a folder that has been added to your PATH ENVIRONTMENT so you can execute
-it from anywhere I was succesfuly compiled it in Windows 10 with pyinstaller-
-5.1 and Pyhton-3.10.4, and python-3.8.12 in Debian 9 another alternative way to
+# pyautosrt [https://img.shields.io/pypi/v/pyautosrt.svg] https://user-
+images.githubusercontent.com/88623122/218178963-fb77891c-1845-4514-8806-
+069dc342dca3.mp4 ### Auto generate subtitles files for any video/audio files
+PyAutoSRT is a PySimpleGUI based desktop app to auto generate subtitle and
+translated subtitle file for any video or audio file The core script is a
+modified version of original autosub made by Anastasis Germanidis https://
+github.com/agermanidis/autosub ### Installation If you don't have python on
+your Windows system you can get compiled version from https://github.com/
+botbahlul/pyautosrt/releases/ Just extract those ffmpeg.exe and pyautosrt.exe
+into a folder that has been added to PATH ENVIRONTMET for example in C:
+\Windows\system32 You can get latest version of ffmpeg from https://
+www.ffmpeg.org/ In Linux you have to install this script with python (version
+minimal 3.8 ) and install ffmpeg with your linux package manager for example in
+debian based linux distribution you can type : ``` apt update apt install -
+y ffmpeg ``` To install this pyautosrt, just type : ``` pip install pyautosrt
+``` You can compile this script into a single executable file with pyinstaller
+by downloading "\__init\__.py" file, rename it to pyautosrt.py and type : ```
+pip install pyinstaller pyinstaller --onefile pyautosrt.py ``` The executable
+compiled file will be placed by pyinstaller into dist subfolder of your current
+working folder, so you can just rename and put that compiled file into a folder
+that has been added to your PATH ENVIRONTMENT so you can execute it from
+anywhere I was succesfuly compiled it in Windows 10 with pyinstaller-5.1 and
+Pyhton-3.10.4, and python-3.8.12 in Debian 9 NOTES : SINCE VERSION 0.1.9 YOU
+SHOULD USE THAT \"mypyinstaller.bat\" (FOR WINDOWS) OR \"mypyinstaller.sh\"
+(FOR LINUX) TO COMPILE THAT \"pyautosrt.pyw\" Another alternative way to
 install this script with python is by cloning this git (or downloading this git
 as zip then extract it into a folder), and then just type : ``` python setup.py
-build python setup.py install ``` ### Simple usage example ``` pyautosrt --
-list-languages pyautosrt -S zh-CN -D en "Episode 1.mp4" ``` ### usage ```
-pyautosrt [-h] [-C CONCURRENCY] [-o OUTPUT] [-F FORMAT] [-S SRC_LANGUAGE] [-
-D DST_LANGUAGE] [-n RENAME] [-p PATIENCE] [-v] [--list-formats] [--list-
-languages] [source_path] positional arguments: source_path Path to the video or
-audio file options: -h, --help show this help message and exit -C CONCURRENCY,
---concurrency CONCURRENCY Number of concurrent API requests to make -o OUTPUT,
---output OUTPUT Output path for subtitles (by default, subtitles are saved in
-the same directory and name as the source path) -F FORMAT, --format FORMAT
-Destination subtitle format -S SRC_LANGUAGE, --src-language SRC_LANGUAGE
-Language spoken in source file -D DST_LANGUAGE, --dst-language DST_LANGUAGE
-Desired language for the subtitles -v, --version show program's version number
-and exit -lf, --list-formats List all available subtitle formats -ll, --list-
-languages List all available source/destination languages ``` ### License MIT
+build python setup.py install ``` ### Usage ``` usage: pyautosrt.py [-h] [-
+S SRC_LANGUAGE] [-D DST_LANGUAGE] [-ll] [-F FORMAT] [-lf] [-v] [source_path
+...] positional arguments: source_path Path to the video or audio files to
+generate subtitle (use wildcard for multiple files or separate them with space
+eg. "file 1.mp4" "file 2.mp4") options: -h, --help show this help message and
+exit -S SRC_LANGUAGE, --src-language SRC_LANGUAGE Spoken language -
+D DST_LANGUAGE, --dst-language DST_LANGUAGE Desired language for translation -
+ll, --list-languages List all available source/translation languages -F FORMAT,
+--format FORMAT Desired subtitle format -lf, --list-formats List all available
+subtitle formats -v, --version show program's version number and exit ``` Those
+command switch '-S' and '-D' are not mandatory. It's just to make combobox
+directly select your desired language if you prefer to type it rather that
+click on combobox. UPDATE NOTES : SINCE VERSION 0.1.1 YOU CAN SELECT MULTIPLE
+VIDEO/AUDIO FILES, BUT REMEMBER THAT ALL FILES YOU SELECT SHOULD HAVE SAME
+AUDIO LANGUAGE AND DESIRED TRANSLATION LANGUAGE. ### License MIT
```

### Comparing `pyautosrt-0.1.7/pyautosrt/__init__.py` & `pyautosrt-0.2.1/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pyautosrt-0.1.7/pyautosrt.egg-info/PKG-INFO` & `pyautosrt-0.2.1/pyautosrt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautosrt
-Version: 0.1.7
+Version: 0.2.1
 Summary: pyautosrt is a python based desktop app to generate subtitle and translated subtitle file
 Home-page: https://github.com/botbahlul/pyautosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

