# Comparing `tmp/cq23-1.6.2.tar.gz` & `tmp/cq23-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cq23-1.6.2.tar", last modified: Sat Jun  3 10:14:50 2023, max compression
+gzip compressed data, was "cq23-1.7.0.tar", last modified: Wed Jun 14 10:12:39 2023, max compression
```

## Comparing `cq23-1.6.2.tar` & `cq23-1.7.0.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:50.440699 cq23-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-03 10:14:50.440699 cq23-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-03 10:14:42.000000 cq23-1.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-03 10:14:42.000000 cq23-1.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-03 10:14:50.440699 cq23-1.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:50.436699 cq23-1.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:50.440699 cq23-1.6.2/src/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:42.000000 cq23-1.6.2/src/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-03 10:14:42.000000 cq23-1.6.2/src/admin/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-03 10:14:42.000000 cq23-1.6.2/src/admin/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-03 10:14:42.000000 cq23-1.6.2/src/admin/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:50.440699 cq23-1.6.2/src/check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:42.000000 cq23-1.6.2/src/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-03 10:14:42.000000 cq23-1.6.2/src/check/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:50.440699 cq23-1.6.2/src/cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:42.000000 cq23-1.6.2/src/cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-03 10:14:42.000000 cq23-1.6.2/src/cleanup/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:50.440699 cq23-1.6.2/src/cq23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-03 10:14:50.000000 cq23-1.6.2/src/cq23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-03 10:14:50.000000 cq23-1.6.2/src/cq23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 10:14:50.000000 cq23-1.6.2/src/cq23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-03 10:14:50.000000 cq23-1.6.2/src/cq23.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-03 10:14:50.000000 cq23-1.6.2/src/cq23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-03 10:14:50.000000 cq23-1.6.2/src/cq23.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:50.440699 cq23-1.6.2/src/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:42.000000 cq23-1.6.2/src/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-03 10:14:42.000000 cq23-1.6.2/src/main/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-03 10:14:42.000000 cq23-1.6.2/src/main/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:50.440699 cq23-1.6.2/src/new_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:42.000000 cq23-1.6.2/src/new_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-03 10:14:42.000000 cq23-1.6.2/src/new_client/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:50.440699 cq23-1.6.2/src/run_game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:42.000000 cq23-1.6.2/src/run_game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-03 10:14:42.000000 cq23-1.6.2/src/run_game/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-03 10:14:42.000000 cq23-1.6.2/src/run_game/docker_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-03 10:14:42.000000 cq23-1.6.2/src/run_game/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:50.440699 cq23-1.6.2/src/zip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:42.000000 cq23-1.6.2/src/zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-03 10:14:42.000000 cq23-1.6.2/src/zip/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:39.447709 cq23-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-14 10:12:39.447709 cq23-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-14 10:12:31.000000 cq23-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-14 10:12:31.000000 cq23-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-14 10:12:39.447709 cq23-1.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:39.443709 cq23-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:39.443709 cq23-1.7.0/src/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:31.000000 cq23-1.7.0/src/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-14 10:12:31.000000 cq23-1.7.0/src/admin/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-14 10:12:31.000000 cq23-1.7.0/src/admin/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-14 10:12:31.000000 cq23-1.7.0/src/admin/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:39.443709 cq23-1.7.0/src/check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:31.000000 cq23-1.7.0/src/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-14 10:12:31.000000 cq23-1.7.0/src/check/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:39.443709 cq23-1.7.0/src/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:31.000000 cq23-1.7.0/src/cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-14 10:12:31.000000 cq23-1.7.0/src/cleanup/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:39.443709 cq23-1.7.0/src/cq23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-14 10:12:39.000000 cq23-1.7.0/src/cq23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-14 10:12:39.000000 cq23-1.7.0/src/cq23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 10:12:39.000000 cq23-1.7.0/src/cq23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-14 10:12:39.000000 cq23-1.7.0/src/cq23.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-14 10:12:39.000000 cq23-1.7.0/src/cq23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-14 10:12:39.000000 cq23-1.7.0/src/cq23.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:39.447709 cq23-1.7.0/src/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:31.000000 cq23-1.7.0/src/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-14 10:12:31.000000 cq23-1.7.0/src/main/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-14 10:12:31.000000 cq23-1.7.0/src/main/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:39.447709 cq23-1.7.0/src/new_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:31.000000 cq23-1.7.0/src/new_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-14 10:12:31.000000 cq23-1.7.0/src/new_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:39.447709 cq23-1.7.0/src/run_game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:31.000000 cq23-1.7.0/src/run_game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-14 10:12:31.000000 cq23-1.7.0/src/run_game/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-14 10:12:31.000000 cq23-1.7.0/src/run_game/docker_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-14 10:12:31.000000 cq23-1.7.0/src/run_game/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:39.447709 cq23-1.7.0/src/web_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:31.000000 cq23-1.7.0/src/web_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-14 10:12:31.000000 cq23-1.7.0/src/web_server/flask_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:39.447709 cq23-1.7.0/src/zip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:12:31.000000 cq23-1.7.0/src/zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-14 10:12:31.000000 cq23-1.7.0/src/zip/command.py
```

### Comparing `cq23-1.6.2/PKG-INFO` & `cq23-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 1.6.2
+Version: 1.7.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-1.6.2/setup.cfg` & `cq23-1.7.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cq23
-version = 1.6.2
+version = 1.7.0
 author = CodeQuest
 author_email = info@codequest.club
 description = CLI Tools for CodeQuest 23
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CALED-Team/cq23-cli-utilities
 project_urls = 
@@ -20,14 +20,15 @@
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	docker>=6.0.1
 	boto3>=1.26.143
 	colorama>=0.4.6
+	flask>=2.2.5
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	cq23 = main.command:route_command
```

### Comparing `cq23-1.6.2/src/admin/aws.py` & `cq23-1.7.0/src/admin/aws.py`

 * *Files identical despite different names*

### Comparing `cq23-1.6.2/src/admin/builder.py` & `cq23-1.7.0/src/admin/builder.py`

 * *Files identical despite different names*

### Comparing `cq23-1.6.2/src/admin/worker.py` & `cq23-1.7.0/src/admin/worker.py`

 * *Files identical despite different names*

### Comparing `cq23-1.6.2/src/check/command.py` & `cq23-1.7.0/src/check/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.6.2/src/cleanup/command.py` & `cq23-1.7.0/src/cleanup/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.6.2/src/cq23.egg-info/PKG-INFO` & `cq23-1.7.0/src/cq23.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 1.6.2
+Version: 1.7.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-1.6.2/src/cq23.egg-info/SOURCES.txt` & `cq23-1.7.0/src/cq23.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -20,9 +20,11 @@
 src/main/utils.py
 src/new_client/__init__.py
 src/new_client/command.py
 src/run_game/__init__.py
 src/run_game/command.py
 src/run_game/docker_tools.py
 src/run_game/gcs.py
+src/web_server/__init__.py
+src/web_server/flask_api.py
 src/zip/__init__.py
 src/zip/command.py
```

### Comparing `cq23-1.6.2/src/main/command.py` & `cq23-1.7.0/src/main/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.6.2/src/main/utils.py` & `cq23-1.7.0/src/main/utils.py`

 * *Files identical despite different names*

### Comparing `cq23-1.6.2/src/new_client/command.py` & `cq23-1.7.0/src/new_client/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.6.2/src/run_game/command.py` & `cq23-1.7.0/src/run_game/command.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         subprocess.run(["git", "clone", repository_url, folder_path])
     else:
         # Pull the latest changes if the folder already exists
         current_dir = os.getcwd()
         os.chdir(folder_path)
         subprocess.run(["git", "pull"])
         os.chdir(current_dir)
-    print("GCS cloned successfully.")
+    print(folder_path + " cloned successfully.")
 
 
 def extract_map_from_command_args(args):
     map_arg = list(filter(lambda x: str(x).startswith("map="), args))
     if not map_arg:
         return None
     if len(map_arg) > 1:
@@ -41,25 +41,28 @@
         shutil.copy2(src_file, dst_file)
 
 
 def run_game(*args):
     docker_tools.ensure_docker_client_exists()
     game_files_dir = ".game_files"
     gcs_folder_name = "gcs"
+    gui_folder_name = "gui"
     gcs_repo = "https://github.com/CALED-Team/game-communication-system.git"
+    gui_repo = "https://github.com/CALED-Team/game-gui-23.git"
 
     docker_tools.check_dockerfile_exists()
     docker_tools.build_and_tag_image(docker_tools.get_client_image_tag())
 
     if not os.path.exists(game_files_dir):
         os.makedirs(game_files_dir)
     os.chdir(game_files_dir)
     game_files_abs_path = os.getcwd()
 
     clone_or_pull_repository(gcs_repo, gcs_folder_name)
+    clone_or_pull_repository(gui_repo, gui_folder_name)
     docker_tools.pull_latest_game_server()
     run_gcs(gcs_folder_name, extract_map_from_command_args(args))
     docker_tools.copy_replay_files(game_files_abs_path)
     copy_container_logs(game_files_abs_path, gcs_folder_name)
 
     # Go back to the same directory as we were (one up)
     os.chdir(os.path.dirname(os.getcwd()))
```

### Comparing `cq23-1.6.2/src/run_game/docker_tools.py` & `cq23-1.7.0/src/run_game/docker_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     dockerfile_path = os.path.join(current_dir, "Dockerfile")
 
     if os.path.isfile(dockerfile_path):
         print("Dockerfile found.")
     else:
         raise Exception(
             "Dockerfile not found! Make sure you run `cq23_run` from the directory that contains your bot's"
-            "Dockerfile."
+            " Dockerfile."
         )
 
 
 def build_and_tag_image(image_tag):
     print("Building the image...")
     current_dir = os.getcwd()
     dockerfile_path = os.path.join(current_dir, "Dockerfile")
```

### Comparing `cq23-1.6.2/src/zip/command.py` & `cq23-1.7.0/src/zip/command.py`

 * *Files identical despite different names*

