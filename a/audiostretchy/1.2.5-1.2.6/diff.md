# Comparing `tmp/audiostretchy-1.2.5.tar.gz` & `tmp/audiostretchy-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiostretchy-1.2.5.tar", last modified: Sat May  6 15:38:40 2023, max compression
+gzip compressed data, was "audiostretchy-1.2.6.tar", last modified: Wed Jun 14 18:51:59 2023, max compression
```

## Comparing `audiostretchy-1.2.5.tar` & `audiostretchy-1.2.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:38:40.176991 audiostretchy-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:38:40.168991 audiostretchy-1.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:38:40.172991 audiostretchy-1.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-05-06 15:38:40.176991 audiostretchy-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:38:40.172991 audiostretchy-1.2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:38:40.172991 audiostretchy-1.2.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-06 15:38:40.180991 audiostretchy-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:38:40.168991 audiostretchy-1.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:38:40.172991 audiostretchy-1.2.5/src/audiostretchy/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/src/audiostretchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/src/audiostretchy/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:38:40.176991 audiostretchy-1.2.5/src/audiostretchy/interface/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:38:40.176991 audiostretchy-1.2.5/src/audiostretchy/interface/linux/
--rwxr-xr-x   0 runner    (1001) docker     (123)    22664 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/src/audiostretchy/interface/linux/_stretch.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:38:40.176991 audiostretchy-1.2.5/src/audiostretchy/interface/mac/
--rwxr-xr-x   0 runner    (1001) docker     (123)    99483 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/src/audiostretchy/interface/mac/_stretch.dylib
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/src/audiostretchy/interface/tdhs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:38:40.176991 audiostretchy-1.2.5/src/audiostretchy/interface/win/
--rw-r--r--   0 runner    (1001) docker     (123)   104960 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/src/audiostretchy/interface/win/_stretch.dll
--rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/src/audiostretchy/stretch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:38:40.176991 audiostretchy-1.2.5/src/audiostretchy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-05-06 15:38:40.000000 audiostretchy-1.2.5/src/audiostretchy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-06 15:38:40.000000 audiostretchy-1.2.5/src/audiostretchy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:38:40.000000 audiostretchy-1.2.5/src/audiostretchy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-06 15:38:40.000000 audiostretchy-1.2.5/src/audiostretchy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:38:39.000000 audiostretchy-1.2.5/src/audiostretchy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-06 15:38:40.000000 audiostretchy-1.2.5/src/audiostretchy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 15:38:40.000000 audiostretchy-1.2.5/src/audiostretchy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:38:40.176991 audiostretchy-1.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   198991 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/tests/audio-1.2.mp3
--rw-r--r--   0 runner    (1001) docker     (123)  1091644 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/tests/audio-1.2.wav
--rw-r--r--   0 runner    (1001) docker     (123)   132118 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/tests/audio.mp3
--rw-r--r--   0 runner    (1001) docker     (123)   723534 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/tests/audio.wav
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-06 15:38:28.000000 audiostretchy-1.2.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:51:59.763776 audiostretchy-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:51:59.755775 audiostretchy-1.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:51:59.759775 audiostretchy-1.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-06-14 18:51:59.763776 audiostretchy-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:51:59.759775 audiostretchy-1.2.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:51:59.759775 audiostretchy-1.2.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-14 18:51:59.767776 audiostretchy-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:51:59.755775 audiostretchy-1.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:51:59.759775 audiostretchy-1.2.6/src/audiostretchy/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/src/audiostretchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/src/audiostretchy/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:51:59.763776 audiostretchy-1.2.6/src/audiostretchy/interface/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:51:59.763776 audiostretchy-1.2.6/src/audiostretchy/interface/linux/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22664 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/src/audiostretchy/interface/linux/_stretch.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:51:59.763776 audiostretchy-1.2.6/src/audiostretchy/interface/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    99483 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/src/audiostretchy/interface/mac/_stretch.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/src/audiostretchy/interface/tdhs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:51:59.763776 audiostretchy-1.2.6/src/audiostretchy/interface/win/
+-rw-r--r--   0 runner    (1001) docker     (123)   104960 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/src/audiostretchy/interface/win/_stretch.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/src/audiostretchy/stretch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:51:59.763776 audiostretchy-1.2.6/src/audiostretchy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-06-14 18:51:59.000000 audiostretchy-1.2.6/src/audiostretchy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-14 18:51:59.000000 audiostretchy-1.2.6/src/audiostretchy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 18:51:59.000000 audiostretchy-1.2.6/src/audiostretchy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-14 18:51:59.000000 audiostretchy-1.2.6/src/audiostretchy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 18:51:59.000000 audiostretchy-1.2.6/src/audiostretchy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-14 18:51:59.000000 audiostretchy-1.2.6/src/audiostretchy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-14 18:51:59.000000 audiostretchy-1.2.6/src/audiostretchy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:51:59.763776 audiostretchy-1.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   198991 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/tests/audio-1.2.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)  1091644 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/tests/audio-1.2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   132118 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/tests/audio.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)   723534 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/tests/audio.wav
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-14 18:51:47.000000 audiostretchy-1.2.6/tests/conftest.py
```

### Comparing `audiostretchy-1.2.5/.coveragerc` & `audiostretchy-1.2.6/.coveragerc`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.5/.github/workflows/ci.yaml` & `audiostretchy-1.2.6/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.5/.gitignore` & `audiostretchy-1.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.5/.pre-commit-config.yaml` & `audiostretchy-1.2.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.5/.readthedocs.yml` & `audiostretchy-1.2.6/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.5/LICENSE.txt` & `audiostretchy-1.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.5/PKG-INFO` & `audiostretchy-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostretchy
-Version: 1.2.5
+Version: 1.2.6
 Summary: AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. AudioStretchy is a wrapper around the audio-stretch C library by David Bryant.
 Home-page: https://github.com/twardoch/audiostretchy
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -26,15 +26,15 @@
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 # AudioStretchy
 
 AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. The library is a wrapper around David Bryant’s [audio-stretch](https://github.com/dbry/audio-stretch) C library. 
 
-_Version: **1.2.5**_
+_Version: **1.2.6**_
 
 ## Features
 
 - Fast, high-quality time stretching of audio files without changing their pitch
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
 - Supports WAV files and file-like objects. With `[all]` installation, also supports MP3 files and file-like objects
```

### Comparing `audiostretchy-1.2.5/README.md` & `audiostretchy-1.2.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # AudioStretchy
 
 AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. The library is a wrapper around David Bryant’s [audio-stretch](https://github.com/dbry/audio-stretch) C library. 
 
-_Version: **1.2.5**_
+_Version: **1.2.6**_
 
 ## Features
 
 - Fast, high-quality time stretching of audio files without changing their pitch
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
 - Supports WAV files and file-like objects. With `[all]` installation, also supports MP3 files and file-like objects
```

### Comparing `audiostretchy-1.2.5/docs/Makefile` & `audiostretchy-1.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.5/docs/conf.py` & `audiostretchy-1.2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.5/docs/index.md` & `audiostretchy-1.2.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.5/setup.cfg` & `audiostretchy-1.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.5/setup.py` & `audiostretchy-1.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.5/src/audiostretchy/__init__.py` & `audiostretchy-1.2.6/src/audiostretchy/__init__.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.5/src/audiostretchy/interface/linux/_stretch.so` & `audiostretchy-1.2.6/src/audiostretchy/interface/linux/_stretch.so`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.5/src/audiostretchy/interface/mac/_stretch.dylib` & `audiostretchy-1.2.6/src/audiostretchy/interface/mac/_stretch.dylib`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.5/src/audiostretchy/interface/tdhs.py` & `audiostretchy-1.2.6/src/audiostretchy/interface/tdhs.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.5/src/audiostretchy/interface/win/_stretch.dll` & `audiostretchy-1.2.6/src/audiostretchy/interface/win/_stretch.dll`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.5/src/audiostretchy/stretch.py` & `audiostretchy-1.2.6/src/audiostretchy/stretch.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.5/src/audiostretchy.egg-info/PKG-INFO` & `audiostretchy-1.2.6/src/audiostretchy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostretchy
-Version: 1.2.5
+Version: 1.2.6
 Summary: AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. AudioStretchy is a wrapper around the audio-stretch C library by David Bryant.
 Home-page: https://github.com/twardoch/audiostretchy
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -26,15 +26,15 @@
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 # AudioStretchy
 
 AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. The library is a wrapper around David Bryant’s [audio-stretch](https://github.com/dbry/audio-stretch) C library. 
 
-_Version: **1.2.5**_
+_Version: **1.2.6**_
 
 ## Features
 
 - Fast, high-quality time stretching of audio files without changing their pitch
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
 - Supports WAV files and file-like objects. With `[all]` installation, also supports MP3 files and file-like objects
```

### Comparing `audiostretchy-1.2.5/src/audiostretchy.egg-info/SOURCES.txt` & `audiostretchy-1.2.6/src/audiostretchy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.5/tests/audio-1.2.mp3` & `audiostretchy-1.2.6/tests/audio-1.2.mp3`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.5/tests/audio-1.2.wav` & `audiostretchy-1.2.6/tests/audio-1.2.wav`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.5/tests/audio.mp3` & `audiostretchy-1.2.6/tests/audio.mp3`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.5/tests/audio.wav` & `audiostretchy-1.2.6/tests/audio.wav`

 * *Files identical despite different names*

