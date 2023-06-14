# Comparing `tmp/cq23-1.7.0.tar.gz` & `tmp/cq23-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cq23-1.7.0.tar", last modified: Wed Jun 14 10:12:39 2023, max compression
+gzip compressed data, was "cq23-1.8.0.tar", last modified: Wed Jun 14 13:53:09 2023, max compression
```

## Comparing `cq23-1.7.0.tar` & `cq23-1.8.0.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:39.447709 cq23-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-14 10:12:39.447709 cq23-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-14 10:12:31.000000 cq23-1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-14 10:12:31.000000 cq23-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-14 10:12:39.447709 cq23-1.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:39.443709 cq23-1.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:39.443709 cq23-1.7.0/src/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:31.000000 cq23-1.7.0/src/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-14 10:12:31.000000 cq23-1.7.0/src/admin/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-14 10:12:31.000000 cq23-1.7.0/src/admin/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-14 10:12:31.000000 cq23-1.7.0/src/admin/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:39.443709 cq23-1.7.0/src/check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:31.000000 cq23-1.7.0/src/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-14 10:12:31.000000 cq23-1.7.0/src/check/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:39.443709 cq23-1.7.0/src/cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:31.000000 cq23-1.7.0/src/cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-14 10:12:31.000000 cq23-1.7.0/src/cleanup/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:39.443709 cq23-1.7.0/src/cq23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-14 10:12:39.000000 cq23-1.7.0/src/cq23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-14 10:12:39.000000 cq23-1.7.0/src/cq23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 10:12:39.000000 cq23-1.7.0/src/cq23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-14 10:12:39.000000 cq23-1.7.0/src/cq23.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-14 10:12:39.000000 cq23-1.7.0/src/cq23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-14 10:12:39.000000 cq23-1.7.0/src/cq23.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:39.447709 cq23-1.7.0/src/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:31.000000 cq23-1.7.0/src/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-14 10:12:31.000000 cq23-1.7.0/src/main/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-14 10:12:31.000000 cq23-1.7.0/src/main/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:39.447709 cq23-1.7.0/src/new_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:31.000000 cq23-1.7.0/src/new_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-14 10:12:31.000000 cq23-1.7.0/src/new_client/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:39.447709 cq23-1.7.0/src/run_game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:31.000000 cq23-1.7.0/src/run_game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-14 10:12:31.000000 cq23-1.7.0/src/run_game/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-14 10:12:31.000000 cq23-1.7.0/src/run_game/docker_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-14 10:12:31.000000 cq23-1.7.0/src/run_game/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:39.447709 cq23-1.7.0/src/web_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:31.000000 cq23-1.7.0/src/web_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-14 10:12:31.000000 cq23-1.7.0/src/web_server/flask_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:39.447709 cq23-1.7.0/src/zip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:31.000000 cq23-1.7.0/src/zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-14 10:12:31.000000 cq23-1.7.0/src/zip/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:09.150584 cq23-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-14 13:53:09.150584 cq23-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-14 13:53:00.000000 cq23-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-14 13:53:00.000000 cq23-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-14 13:53:09.150584 cq23-1.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:09.146584 cq23-1.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:09.146584 cq23-1.8.0/src/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:00.000000 cq23-1.8.0/src/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-14 13:53:00.000000 cq23-1.8.0/src/admin/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-14 13:53:00.000000 cq23-1.8.0/src/admin/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-14 13:53:00.000000 cq23-1.8.0/src/admin/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:09.146584 cq23-1.8.0/src/check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:00.000000 cq23-1.8.0/src/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-14 13:53:00.000000 cq23-1.8.0/src/check/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:09.146584 cq23-1.8.0/src/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:00.000000 cq23-1.8.0/src/cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-14 13:53:00.000000 cq23-1.8.0/src/cleanup/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:09.146584 cq23-1.8.0/src/cq23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-14 13:53:09.000000 cq23-1.8.0/src/cq23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-14 13:53:09.000000 cq23-1.8.0/src/cq23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 13:53:09.000000 cq23-1.8.0/src/cq23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-14 13:53:09.000000 cq23-1.8.0/src/cq23.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-14 13:53:09.000000 cq23-1.8.0/src/cq23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-14 13:53:09.000000 cq23-1.8.0/src/cq23.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:09.146584 cq23-1.8.0/src/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:00.000000 cq23-1.8.0/src/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-14 13:53:00.000000 cq23-1.8.0/src/main/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-14 13:53:00.000000 cq23-1.8.0/src/main/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:09.146584 cq23-1.8.0/src/new_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:00.000000 cq23-1.8.0/src/new_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-14 13:53:00.000000 cq23-1.8.0/src/new_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:09.146584 cq23-1.8.0/src/replay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:00.000000 cq23-1.8.0/src/replay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-14 13:53:00.000000 cq23-1.8.0/src/replay/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:09.150584 cq23-1.8.0/src/run_game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:00.000000 cq23-1.8.0/src/run_game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-14 13:53:00.000000 cq23-1.8.0/src/run_game/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-14 13:53:00.000000 cq23-1.8.0/src/run_game/docker_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-14 13:53:00.000000 cq23-1.8.0/src/run_game/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:09.150584 cq23-1.8.0/src/web_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:00.000000 cq23-1.8.0/src/web_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-14 13:53:00.000000 cq23-1.8.0/src/web_server/flask_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:09.150584 cq23-1.8.0/src/zip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:00.000000 cq23-1.8.0/src/zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-14 13:53:00.000000 cq23-1.8.0/src/zip/command.py
```

### Comparing `cq23-1.7.0/PKG-INFO` & `cq23-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 1.7.0
+Version: 1.8.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-1.7.0/setup.cfg` & `cq23-1.8.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cq23
-version = 1.7.0
+version = 1.8.0
 author = CodeQuest
 author_email = info@codequest.club
 description = CLI Tools for CodeQuest 23
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CALED-Team/cq23-cli-utilities
 project_urls =
```

### Comparing `cq23-1.7.0/src/admin/aws.py` & `cq23-1.8.0/src/admin/aws.py`

 * *Files identical despite different names*

### Comparing `cq23-1.7.0/src/admin/builder.py` & `cq23-1.8.0/src/admin/builder.py`

 * *Files identical despite different names*

### Comparing `cq23-1.7.0/src/admin/worker.py` & `cq23-1.8.0/src/admin/worker.py`

 * *Files identical despite different names*

### Comparing `cq23-1.7.0/src/check/command.py` & `cq23-1.8.0/src/check/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.7.0/src/cleanup/command.py` & `cq23-1.8.0/src/cleanup/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.7.0/src/cq23.egg-info/PKG-INFO` & `cq23-1.8.0/src/cq23.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 1.7.0
+Version: 1.8.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-1.7.0/src/cq23.egg-info/SOURCES.txt` & `cq23-1.8.0/src/cq23.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 src/cq23.egg-info/requires.txt
 src/cq23.egg-info/top_level.txt
 src/main/__init__.py
 src/main/command.py
 src/main/utils.py
 src/new_client/__init__.py
 src/new_client/command.py
+src/replay/__init__.py
+src/replay/command.py
 src/run_game/__init__.py
 src/run_game/command.py
 src/run_game/docker_tools.py
 src/run_game/gcs.py
 src/web_server/__init__.py
 src/web_server/flask_api.py
 src/zip/__init__.py
```

### Comparing `cq23-1.7.0/src/main/command.py` & `cq23-1.8.0/src/main/command.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import sys
 
 from admin.builder import command as builder
 from admin.worker import command as worker
 from check.command import check
 from cleanup.command import cleanup
 from new_client.command import new_client
+from replay.command import replay
 from run_game.command import run_game
 from zip.command import zip
 
 from .utils import restore_cwd
 
 
 def help_message():
     message = (
         "Available commands:\n\n"
         + "> cq23 new python my_bot\n"
         + "> cq23 run\n"
         + "> cq23 run map=<map name>\n"
+        + "> cq23 replay\n"
         + "> cq23 zip\n"
         + "> cq23 check\n"
         + "> cq23 cleanup\n\n"
         + "If you need help with the competition, post a message in Discord or email us at info@codequest.club."
     )
     print(message)
 
@@ -28,14 +30,15 @@
 @restore_cwd
 def route_command():
     command_args = sys.argv[1:]
 
     first_arg_mapping = {
         "new": new_client,
         "run": run_game,
+        "replay": replay,
         "cleanup": cleanup,
         "zip": zip,
         "check": check,
         "worker": worker,
         "builder": builder,
     }
```

### Comparing `cq23-1.7.0/src/main/utils.py` & `cq23-1.8.0/src/main/utils.py`

 * *Files identical despite different names*

### Comparing `cq23-1.7.0/src/new_client/command.py` & `cq23-1.8.0/src/new_client/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.7.0/src/run_game/command.py` & `cq23-1.8.0/src/run_game/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,28 +41,28 @@
         shutil.copy2(src_file, dst_file)
 
 
 def run_game(*args):
     docker_tools.ensure_docker_client_exists()
     game_files_dir = ".game_files"
     gcs_folder_name = "gcs"
-    gui_folder_name = "gui"
+    # gui_folder_name = "gui"
     gcs_repo = "https://github.com/CALED-Team/game-communication-system.git"
-    gui_repo = "https://github.com/CALED-Team/game-gui-23.git"
+    # gui_repo = "https://github.com/CALED-Team/game-gui-23.git"
 
     docker_tools.check_dockerfile_exists()
     docker_tools.build_and_tag_image(docker_tools.get_client_image_tag())
 
     if not os.path.exists(game_files_dir):
         os.makedirs(game_files_dir)
     os.chdir(game_files_dir)
     game_files_abs_path = os.getcwd()
 
     clone_or_pull_repository(gcs_repo, gcs_folder_name)
-    clone_or_pull_repository(gui_repo, gui_folder_name)
+    # clone_or_pull_repository(gui_repo, gui_folder_name)
     docker_tools.pull_latest_game_server()
     run_gcs(gcs_folder_name, extract_map_from_command_args(args))
     docker_tools.copy_replay_files(game_files_abs_path)
     copy_container_logs(game_files_abs_path, gcs_folder_name)
 
     # Go back to the same directory as we were (one up)
     os.chdir(os.path.dirname(os.getcwd()))
```

### Comparing `cq23-1.7.0/src/run_game/docker_tools.py` & `cq23-1.8.0/src/run_game/docker_tools.py`

 * *Files identical despite different names*

### Comparing `cq23-1.7.0/src/run_game/gcs.py` & `cq23-1.8.0/src/run_game/gcs.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 from . import docker_tools
 
 MATCH_TIMEOUT_SECONDS = 12 * 60  # This should ideally match the one in game worker
 
 
 def run_gui():
     replay_files_directory = os.path.join(os.getcwd(), "replay_files")
-    gui_directory = os.path.join(os.getcwd(), "gui")
+    # gui_directory = os.path.join(os.getcwd(), "gui")
     gui_process = Process(target=flask_api.start, args=(replay_files_directory,))
     gui_process.start()
-    webbrowser.open("file://" + os.path.join(gui_directory, "index.html"))
+    # webbrowser.open("file://" + os.path.join(gui_directory, "index.html"))
+    webbrowser.open("https://watch.codequest.club/?base_url=localhost:2023/")
     return gui_process
 
 
 def stop_gui(gui_process):
     func = os.environ.get("werkzeug.server.shutdown")
     if func is None:
         print("Can't stop gracefully, killing the server process.")
```

### Comparing `cq23-1.7.0/src/web_server/flask_api.py` & `cq23-1.8.0/src/web_server/flask_api.py`

 * *Files identical despite different names*

### Comparing `cq23-1.7.0/src/zip/command.py` & `cq23-1.8.0/src/zip/command.py`

 * *Files identical despite different names*

