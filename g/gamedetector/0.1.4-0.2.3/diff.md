# Comparing `tmp/gamedetector-0.1.4.tar.gz` & `tmp/gamedetector-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamedetector-0.1.4.tar", max compression
+gzip compressed data, was "gamedetector-0.2.3.tar", max compression
```

## Comparing `gamedetector-0.1.4.tar` & `gamedetector-0.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-08 17:01:09.805215 gamedetector-0.1.4/gamedetector/__init__.py
--rw-r--r--   0        0        0     3735 2023-06-09 18:22:23.018869 gamedetector-0.1.4/gamedetector/app_exes.json
--rw-r--r--   0        0        0    16146 2023-06-10 19:57:53.452187 gamedetector-0.1.4/gamedetector/game_detect.py
--rw-r--r--   0        0        0     1093 2023-06-08 17:00:52.471193 gamedetector-0.1.4/LICENSE
--rw-r--r--   0        0        0      805 2023-06-10 19:57:49.201527 gamedetector-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2288 2023-06-09 18:24:36.455517 gamedetector-0.1.4/README.md
--rw-r--r--   0        0        0     3044 1970-01-01 00:00:00.000000 gamedetector-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-08 17:01:09.805215 gamedetector-0.2.3/gamedetector/__init__.py
+-rw-r--r--   0        0        0     6617 2023-06-13 07:00:31.535362 gamedetector-0.2.3/gamedetector/app_exes.json
+-rw-r--r--   0        0        0    31602 2023-06-13 21:41:18.856944 gamedetector-0.2.3/gamedetector/game_detect.py
+-rw-r--r--   0        0        0     1093 2023-06-08 17:00:52.471193 gamedetector-0.2.3/LICENSE
+-rw-r--r--   0        0        0      824 2023-06-13 22:19:27.566898 gamedetector-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3155 2023-06-13 06:59:04.881783 gamedetector-0.2.3/README.md
+-rw-r--r--   0        0        0     3930 1970-01-01 00:00:00.000000 gamedetector-0.2.3/PKG-INFO
```

### Comparing `gamedetector-0.1.4/gamedetector/app_exes.json` & `gamedetector-0.2.3/gamedetector/app_exes.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8328392621870883%*

 * *Differences: {"'exes'": "{insert: [(25, OrderedDict([('filename', 'scriptinterpreter.exe'), ('description', "*

 * *           "'Interpreter for KSP scripts.')])), (26, OrderedDict([('filename', 'binpatch.exe'), "*

 * *           "('description', 'Patcher for Dwarf Fortress')])), (27, OrderedDict([('filename', "*

 * *           "'AnnouncementsWindow.exe'), ('description', 'Announcements for Dwarf Fortress')])), "*

 * *           "(28, OrderedDict([('filename', 'optipng.exe'), ('description', 'PNG optimizer used by "*

 * *           "Dwarf Fortre […]*

```diff
@@ -95,18 +95,103 @@
         {
             "description": "Utility for The Sims 4",
             "filename": "Cleanup.exe"
         },
         {
             "description": "Activation utility for Origin games (i.e. The Sims 4)",
             "filename": "ActivationUI.exe"
+        },
+        {
+            "description": "Interpreter for KSP scripts.",
+            "filename": "scriptinterpreter.exe"
+        },
+        {
+            "description": "Patcher for Dwarf Fortress",
+            "filename": "binpatch.exe"
+        },
+        {
+            "description": "Announcements for Dwarf Fortress",
+            "filename": "AnnouncementsWindow.exe"
+        },
+        {
+            "description": "PNG optimizer used by Dwarf Fortress",
+            "filename": "optipng.exe"
+        },
+        {
+            "description": "Sound engine used by Dwarf Fortress",
+            "filename": "SoundCenSeGTK.exe"
+        },
+        {
+            "description": "MO2",
+            "filename": "ModOrganizer.exe"
+        },
+        {
+            "description": "NexusMods link handler, used by MO2",
+            "filename": "nxmhandler.exe"
+        },
+        {
+            "description": "Utility for MO2",
+            "filename": "QtWebEngineProcess.exe"
+        },
+        {
+            "description": "Explorer utility for MO2",
+            "filename": "Explorer++.exe"
+        },
+        {
+            "description": "Load Order Organizer Tool, used with MO2",
+            "filename": "lootcli.exe"
+        },
+        {
+            "description": "CLI client for NexusMods",
+            "filename": "NexusClientCLI.exe"
+        },
+        {
+            "description": "Bash patch creator, tool for MO2",
+            "filename": "Wrye Bash.exe"
+        },
+        {
+            "description": "7z File Compression CLI",
+            "filename": "7z.exe"
+        },
+        {
+            "description": "File compression CLI",
+            "filename": "lzma.exe"
+        },
+        {
+            "description": "PNG optimizer used for Bash patches",
+            "filename": "pngcrush.exe"
+        },
+        {
+            "description": "Distribution of 7z",
+            "filename": "7za.exe"
+        },
+        {
+            "description": "Viewer for NIF files, typically for Bethesda games",
+            "filename": "NifViewer.exe"
+        },
+        {
+            "description": "4GB Patch for Elder Scrolls: Oblivion. Allows more than 4GB of memory to be used.",
+            "filename": "4gb patch.exe"
+        },
+        {
+            "description": "Mod Manager for Elder Scrolls: Oblivion.",
+            "filename": "OblivionModManager.exe"
+        },
+        {
+            "description": "Similar to SKSE for Skyrim; script loader for Oblivion",
+            "filename": "obse_loader.exe"
+        },
+        {
+            "description": "Utility for Dwarf Fortress",
+            "filename": "Armok Vision.exe"
         }
     ],
     "fuzz": [
         "vcredist",
+        "install",
         "uninstall",
         "setup",
         "crashreport",
         "crashpad_handler",
         "klist",
         "ktab",
         "rmiregistry",
@@ -123,10 +208,16 @@
         "switcher",
         "server",
         "jjs",
         "language-changer",
         "dlc-toggler",
         "Baapp",
         "essimporter",
-        "iniimporter"
+        "iniimporter",
+        "unins000",
+        "scriptinterpreter",
+        "soundsense",
+        "usvfs_proxy_",
+        "helper",
+        "SKIDROW"
     ]
 }
```

### Comparing `gamedetector-0.1.4/LICENSE` & `gamedetector-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gamedetector-0.1.4/pyproject.toml` & `gamedetector-0.2.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "gamedetector"
-version = "0.1.4"
+version = "0.2.3"
 description = "The GameDetector library allows you to detect a game within a folder, returning information like Steam AppId, game name, and version."
 authors = ["Aareon Sullivan <askully13@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 fuzzysearch = "^0.7.3"
 requests = "^2.31.0"
 detect-delimiter = "^0.1.1"
 ujson = "^5.7.0"
 beautifulsoup4 = "^4.12.2"
 ratelimit = "^2.2.1"
+py7zr = "^0.20.5"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pipenv = "^2023.6.2"
 poetry = "^1.5.1"
 flake8 = "^6.0.0"
```

### Comparing `gamedetector-0.1.4/README.md` & `gamedetector-0.2.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 # GameDetector
 
 Detect games, get Steam info, profit. This program allows you to select a folder on your system (probably in your game library), that contains a game. It looks in the game folder for files that can identify what game it is, get a Steam `AppId` for said game, and find a reasonable list of `EXE` files that could possibly be the game executable.
 
 The purpose of this application is so that it can be used in a much larger application, an automatic game manager for data hoarders. I'll let you know more about this as I develop it, but believe me, it'll be super rad.
 
-## What this program can and won't do
+## Disclaimer
 
 - Does not circumvent DRM
 - Does not encourage the use of pirated software
 - Uses publicly available APIs provided by Steam or others
 - Makes a reasonable attempt to respect ratelimits
 - Caches responses to save bandwidth and API load
 - Does not download or upload game data to any server
 
+## Features
+- Very fast (reading from compressed archives is limited by 7-zip)
+- Folder support
+- 7-zip archive support
+- GOG game support
+- Steam game support
+- DRM-free games support
+
 ## Compatibility
 
 Currently, only Windows 10/11 are officially supported, but Debian/Linux support is planned in the future.
+The project uses `pathlib` so handling different paths should be trivial, its just not tested.
+The only known dependency issue is `pywin32`, and there's already a stub for the single function using it for Linux systems to continue using the library.
 
 ## Installing
 
 Install [Python 3.10+](https://python.org/downloads)
 
 Clone the repository and install dependency manager (`pipenv`)
 ```sh
@@ -27,23 +37,34 @@
 cd GameDetector
 py -m pip install pipenv
 pipenv install
 ```
 
 After installing dependencies, and given that their were no errors in doing so, run the application.
 ```sh
-py ./src/game_detect.py
+cd GameDetector
+py ./gamedetector/game_detect.py
 ```
 
-## What to expect after running
+## What to expect after running directly
 
 After executing the program, you will be prompted to select a folder (game folder). The program will then attempt to detect what game it is based on things like folder name, as well as checking known files that are commonly available in many distributions of games. It will tell you the name of the game detected, the version, the Steam AppId (if available on Steam), as well as a game description.
 
 This program isn't super useful to regular users, but it will be extremely handy to have as a library for other applications.
 
+## Usage as a library
+```py
+from pathlib import Path
+
+from gamedetector.game_detect import detect_folder, detect_7z, NonSteamGame, SteamGame, NoGameException, SteamApiException
+
+game_path = detect_folder(Path("some path to a game"))  # will return either NonSteamGame, or SteamGame if AppId is found
+game_7z_path = detect_7z(Path("path to 7z file containing game"))  # will return same as above
+```
+
 ## Reporting bugs
 
 Please see [the Issues page](https://github.com/Aareon/GameDetector/issues). Please include the full output from the program.
 
 ## License
 
 MIT (free as in free beer, free to redistribute with credit, free to use commercially with credit)
```

### Comparing `gamedetector-0.1.4/PKG-INFO` & `gamedetector-0.2.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,56 @@
 Metadata-Version: 2.1
 Name: gamedetector
-Version: 0.1.4
+Version: 0.2.3
 Summary: The GameDetector library allows you to detect a game within a folder, returning information like Steam AppId, game name, and version.
 License: MIT
 Author: Aareon Sullivan
 Author-email: askully13@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: detect-delimiter (>=0.1.1,<0.2.0)
 Requires-Dist: fuzzysearch (>=0.7.3,<0.8.0)
+Requires-Dist: py7zr (>=0.20.5,<0.21.0)
 Requires-Dist: ratelimit (>=2.2.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: ujson (>=5.7.0,<6.0.0)
 Description-Content-Type: text/markdown
 
 # GameDetector
 
 Detect games, get Steam info, profit. This program allows you to select a folder on your system (probably in your game library), that contains a game. It looks in the game folder for files that can identify what game it is, get a Steam `AppId` for said game, and find a reasonable list of `EXE` files that could possibly be the game executable.
 
 The purpose of this application is so that it can be used in a much larger application, an automatic game manager for data hoarders. I'll let you know more about this as I develop it, but believe me, it'll be super rad.
 
-## What this program can and won't do
+## Disclaimer
 
 - Does not circumvent DRM
 - Does not encourage the use of pirated software
 - Uses publicly available APIs provided by Steam or others
 - Makes a reasonable attempt to respect ratelimits
 - Caches responses to save bandwidth and API load
 - Does not download or upload game data to any server
 
+## Features
+- Very fast (reading from compressed archives is limited by 7-zip)
+- Folder support
+- 7-zip archive support
+- GOG game support
+- Steam game support
+- DRM-free games support
+
 ## Compatibility
 
 Currently, only Windows 10/11 are officially supported, but Debian/Linux support is planned in the future.
+The project uses `pathlib` so handling different paths should be trivial, its just not tested.
+The only known dependency issue is `pywin32`, and there's already a stub for the single function using it for Linux systems to continue using the library.
 
 ## Installing
 
 Install [Python 3.10+](https://python.org/downloads)
 
 Clone the repository and install dependency manager (`pipenv`)
 ```sh
@@ -47,23 +58,34 @@
 cd GameDetector
 py -m pip install pipenv
 pipenv install
 ```
 
 After installing dependencies, and given that their were no errors in doing so, run the application.
 ```sh
-py ./src/game_detect.py
+cd GameDetector
+py ./gamedetector/game_detect.py
 ```
 
-## What to expect after running
+## What to expect after running directly
 
 After executing the program, you will be prompted to select a folder (game folder). The program will then attempt to detect what game it is based on things like folder name, as well as checking known files that are commonly available in many distributions of games. It will tell you the name of the game detected, the version, the Steam AppId (if available on Steam), as well as a game description.
 
 This program isn't super useful to regular users, but it will be extremely handy to have as a library for other applications.
 
+## Usage as a library
+```py
+from pathlib import Path
+
+from gamedetector.game_detect import detect_folder, detect_7z, NonSteamGame, SteamGame, NoGameException, SteamApiException
+
+game_path = detect_folder(Path("some path to a game"))  # will return either NonSteamGame, or SteamGame if AppId is found
+game_7z_path = detect_7z(Path("path to 7z file containing game"))  # will return same as above
+```
+
 ## Reporting bugs
 
 Please see [the Issues page](https://github.com/Aareon/GameDetector/issues). Please include the full output from the program.
 
 ## License
 
 MIT (free as in free beer, free to redistribute with credit, free to use commercially with credit)
```

