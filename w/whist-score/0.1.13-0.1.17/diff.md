# Comparing `tmp/whist_score-0.1.13.tar.gz` & `tmp/whist_score-0.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whist_score-0.1.13.tar", last modified: Mon Jun 12 19:39:36 2023, max compression
+gzip compressed data, was "whist_score-0.1.17.tar", last modified: Mon Jun 12 20:11:41 2023, max compression
```

## Comparing `whist_score-0.1.13.tar` & `whist_score-0.1.17.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-06-12 19:39:36.457894 whist_score-0.1.13/
--rw-rw-r--   0 erwin     (1000) erwin     (1000)    35149 2023-06-12 16:32:28.000000 whist_score-0.1.13/LICENSE
--rw-rw-r--   0 erwin     (1000) erwin     (1000)       14 2023-06-12 19:29:48.000000 whist_score-0.1.13/MANIFEST.in
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      424 2023-06-12 19:39:36.457894 whist_score-0.1.13/PKG-INFO
--rw-rw-r--   0 erwin     (1000) erwin     (1000)        0 2023-06-12 16:24:02.000000 whist_score-0.1.13/README.md
-drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-06-12 19:39:36.457894 whist_score-0.1.13/config/
--rw-rw-r--   0 erwin     (1000) erwin     (1000)     3269 2023-06-12 17:47:59.000000 whist_score-0.1.13/config/abondance_point_system.json
--rw-rw-r--   0 erwin     (1000) erwin     (1000)     1299 2023-06-12 17:44:14.000000 whist_score-0.1.13/config/game_types.json
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      671 2023-06-12 17:44:58.000000 whist_score-0.1.13/config/miserie_point_system.json
--rw-rw-r--   0 erwin     (1000) erwin     (1000)     1913 2023-06-12 17:46:13.000000 whist_score-0.1.13/config/solo_point_system.json
--rw-rw-r--   0 erwin     (1000) erwin     (1000)     1277 2023-06-12 17:45:32.000000 whist_score-0.1.13/config/troel_point_system.json
--rw-rw-r--   0 erwin     (1000) erwin     (1000)     3869 2023-06-12 17:47:06.000000 whist_score-0.1.13/config/vragen_en_meegaan_point_system.json
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      797 2023-06-12 18:53:38.000000 whist_score-0.1.13/main.py
--rw-rw-r--   0 erwin     (1000) erwin     (1000)       38 2023-06-12 19:39:36.457894 whist_score-0.1.13/setup.cfg
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      996 2023-06-12 19:31:35.000000 whist_score-0.1.13/setup.py
-drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-06-12 19:39:36.457894 whist_score-0.1.13/whist_score/
--rw-rw-r--   0 erwin     (1000) erwin     (1000)        0 2023-06-05 09:19:17.000000 whist_score-0.1.13/whist_score/__init__.py
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      827 2023-06-12 19:18:00.000000 whist_score-0.1.13/whist_score/constants.py
-drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-06-12 19:39:36.457894 whist_score-0.1.13/whist_score/models/
--rw-rw-r--   0 erwin     (1000) erwin     (1000)    17347 2023-06-12 19:12:55.000000 whist_score-0.1.13/whist_score/models/Game.py
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      505 2023-06-05 14:32:02.000000 whist_score-0.1.13/whist_score/models/Player.py
--rw-rw-r--   0 erwin     (1000) erwin     (1000)    10315 2023-06-12 19:19:38.000000 whist_score-0.1.13/whist_score/models/RoundTypes.py
--rw-rw-r--   0 erwin     (1000) erwin     (1000)        0 2023-06-05 09:22:20.000000 whist_score-0.1.13/whist_score/models/__init__.py
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      252 2023-06-12 18:46:17.000000 whist_score-0.1.13/whist_score/utils.py
-drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-06-12 19:39:36.457894 whist_score-0.1.13/whist_score/views/
--rw-rw-r--   0 erwin     (1000) erwin     (1000)        0 2023-06-05 10:00:47.000000 whist_score-0.1.13/whist_score/views/__init__.py
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      973 2023-06-12 18:53:29.000000 whist_score-0.1.13/whist_score/views/games.py
-drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-06-12 19:39:36.457894 whist_score-0.1.13/whist_score.egg-info/
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      424 2023-06-12 19:39:36.000000 whist_score-0.1.13/whist_score.egg-info/PKG-INFO
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      700 2023-06-12 19:39:36.000000 whist_score-0.1.13/whist_score.egg-info/SOURCES.txt
--rw-rw-r--   0 erwin     (1000) erwin     (1000)        1 2023-06-12 19:39:36.000000 whist_score-0.1.13/whist_score.egg-info/dependency_links.txt
--rw-rw-r--   0 erwin     (1000) erwin     (1000)       42 2023-06-12 19:39:36.000000 whist_score-0.1.13/whist_score.egg-info/entry_points.txt
--rw-rw-r--   0 erwin     (1000) erwin     (1000)       29 2023-06-12 19:39:36.000000 whist_score-0.1.13/whist_score.egg-info/requires.txt
--rw-rw-r--   0 erwin     (1000) erwin     (1000)       12 2023-06-12 19:39:36.000000 whist_score-0.1.13/whist_score.egg-info/top_level.txt
+drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-06-12 20:11:41.198916 whist_score-0.1.17/
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)    35149 2023-06-12 16:32:28.000000 whist_score-0.1.17/LICENSE
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       14 2023-06-12 19:29:48.000000 whist_score-0.1.17/MANIFEST.in
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      424 2023-06-12 20:11:41.198916 whist_score-0.1.17/PKG-INFO
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)        0 2023-06-12 16:24:02.000000 whist_score-0.1.17/README.md
+drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-06-12 20:11:41.198916 whist_score-0.1.17/config/
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)     3269 2023-06-12 17:47:59.000000 whist_score-0.1.17/config/abondance_point_system.json
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)     1299 2023-06-12 17:44:14.000000 whist_score-0.1.17/config/game_types.json
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      671 2023-06-12 17:44:58.000000 whist_score-0.1.17/config/miserie_point_system.json
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)     1913 2023-06-12 17:46:13.000000 whist_score-0.1.17/config/solo_point_system.json
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)     1277 2023-06-12 17:45:32.000000 whist_score-0.1.17/config/troel_point_system.json
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)     3869 2023-06-12 17:47:06.000000 whist_score-0.1.17/config/vragen_en_meegaan_point_system.json
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      797 2023-06-12 18:53:38.000000 whist_score-0.1.17/main.py
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       38 2023-06-12 20:11:41.198916 whist_score-0.1.17/setup.cfg
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      996 2023-06-12 20:11:37.000000 whist_score-0.1.17/setup.py
+drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-06-12 20:11:41.198916 whist_score-0.1.17/whist_score/
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)        0 2023-06-05 09:19:17.000000 whist_score-0.1.17/whist_score/__init__.py
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      967 2023-06-12 20:11:26.000000 whist_score-0.1.17/whist_score/constants.py
+drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-06-12 20:11:41.198916 whist_score-0.1.17/whist_score/models/
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)    17347 2023-06-12 19:12:55.000000 whist_score-0.1.17/whist_score/models/Game.py
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      505 2023-06-05 14:32:02.000000 whist_score-0.1.17/whist_score/models/Player.py
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)    10168 2023-06-12 20:02:52.000000 whist_score-0.1.17/whist_score/models/RoundTypes.py
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)        0 2023-06-05 09:22:20.000000 whist_score-0.1.17/whist_score/models/__init__.py
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      252 2023-06-12 18:46:17.000000 whist_score-0.1.17/whist_score/utils.py
+drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-06-12 20:11:41.198916 whist_score-0.1.17/whist_score/views/
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)        0 2023-06-05 10:00:47.000000 whist_score-0.1.17/whist_score/views/__init__.py
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      973 2023-06-12 18:53:29.000000 whist_score-0.1.17/whist_score/views/games.py
+drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-06-12 20:11:41.198916 whist_score-0.1.17/whist_score.egg-info/
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      424 2023-06-12 20:11:41.000000 whist_score-0.1.17/whist_score.egg-info/PKG-INFO
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      700 2023-06-12 20:11:41.000000 whist_score-0.1.17/whist_score.egg-info/SOURCES.txt
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)        1 2023-06-12 20:11:41.000000 whist_score-0.1.17/whist_score.egg-info/dependency_links.txt
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       42 2023-06-12 20:11:41.000000 whist_score-0.1.17/whist_score.egg-info/entry_points.txt
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       29 2023-06-12 20:11:41.000000 whist_score-0.1.17/whist_score.egg-info/requires.txt
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       12 2023-06-12 20:11:41.000000 whist_score-0.1.17/whist_score.egg-info/top_level.txt
```

### Comparing `whist_score-0.1.13/LICENSE` & `whist_score-0.1.17/LICENSE`

 * *Files identical despite different names*

### Comparing `whist_score-0.1.13/config/abondance_point_system.json` & `whist_score-0.1.17/config/abondance_point_system.json`

 * *Files identical despite different names*

### Comparing `whist_score-0.1.13/config/game_types.json` & `whist_score-0.1.17/config/game_types.json`

 * *Files identical despite different names*

### Comparing `whist_score-0.1.13/config/miserie_point_system.json` & `whist_score-0.1.17/config/miserie_point_system.json`

 * *Files identical despite different names*

### Comparing `whist_score-0.1.13/config/solo_point_system.json` & `whist_score-0.1.17/config/solo_point_system.json`

 * *Files identical despite different names*

### Comparing `whist_score-0.1.13/config/troel_point_system.json` & `whist_score-0.1.17/config/troel_point_system.json`

 * *Files identical despite different names*

### Comparing `whist_score-0.1.13/config/vragen_en_meegaan_point_system.json` & `whist_score-0.1.17/config/vragen_en_meegaan_point_system.json`

 * *Files identical despite different names*

### Comparing `whist_score-0.1.13/main.py` & `whist_score-0.1.17/main.py`

 * *Files identical despite different names*

### Comparing `whist_score-0.1.13/setup.py` & `whist_score-0.1.17/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 setup(
     name="whist_score",
-    version="0.1.13",
+    version="0.1.17",
     author="Erwin Mintiens",
     author_email="erwin.mintiens@protonmail.com",
     license_files=("LICENSE",),
     description="whist_score is a scorekeeper for the whist card game.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/erwinmintiens/whist-score",
```

### Comparing `whist_score-0.1.13/whist_score/constants.py` & `whist_score-0.1.17/whist_score/constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import os
+from pathlib import Path
 
 MISERIE = "Miserie"
 KLEINE_MISERIE = f"Kleine {MISERIE}"
 GROTE_MISERIE = f"Grote {MISERIE}"
 GROTE_MISERIE_OP_TAFEL = f"{GROTE_MISERIE} op tafel"
 SOLO_SLIM = "Solo Slim"
 KLEINE_SOLO_SLIM = f"Kleine {SOLO_SLIM}"
 GROTE_SOLO_SLIM = f"Grote {SOLO_SLIM}"
 VRAGEN_EN_MEEGAAN = "Vragen en Meegaan"
 SOLO = "Solo"
 TROEL = "Troel"
 PICCOLO = "Piccolo"
 ABONDANCE = "Abondance"
 SAVE_FOLDER = "./results/"
-CONFIG_FOLDER = os.path.join(os.path.dirname(__file__), "config")
+CONFIG_FOLDER = os.path.join(
+    Path(os.path.abspath(__file__)).parent.absolute(), "config"
+)
+# CONFIG_FOLDER = os.path.join(os.path.dirname(os.path.abspath(__file__)), "config")
 SOLO_POINT_SYSTEM_FILE_NAME = "solo_point_system.json"
 ABONDANCE_POINT_SYSTEM_FILE_NAME = "abondance_point_system.json"
 MISERIE_POINT_SYSTEM_FILE_NAME = "miserie_point_system.json"
 TROEL_POINT_SYSTEM_FILE_NAME = "troel_point_system.json"
 VRAGEN_EN_MEEGAAN_POINT_SYSTEM_FILE_NAME = "vragen_en_meegaan_point_system.json"
 GAME_TYPES_FILE_NAME = "game_types.json"
```

### Comparing `whist_score-0.1.13/whist_score/models/Game.py` & `whist_score-0.1.17/whist_score/models/Game.py`

 * *Files identical despite different names*

### Comparing `whist_score-0.1.13/whist_score/models/RoundTypes.py` & `whist_score-0.1.17/whist_score/models/RoundTypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,8 @@
 from whist_score.constants import (
-    # SOLO_POINT_SYSTEM,
-    # MISERIE_POINT_SYSTEM,
-    # ABONDANCE_POINT_SYSTEM,
-    # VRAGEN_EN_MEEGAAN_POINT_SYSTEM,
-    # TROEL_POINT_SYSTEM,
     CONFIG_FOLDER,
     SOLO_POINT_SYSTEM_FILE_NAME,
     ABONDANCE_POINT_SYSTEM_FILE_NAME,
     TROEL_POINT_SYSTEM_FILE_NAME,
     VRAGEN_EN_MEEGAAN_POINT_SYSTEM_FILE_NAME,
     MISERIE_POINT_SYSTEM_FILE_NAME,
 )
```

### Comparing `whist_score-0.1.13/whist_score/views/games.py` & `whist_score-0.1.17/whist_score/views/games.py`

 * *Files identical despite different names*

### Comparing `whist_score-0.1.13/whist_score.egg-info/SOURCES.txt` & `whist_score-0.1.17/whist_score.egg-info/SOURCES.txt`

 * *Files identical despite different names*

