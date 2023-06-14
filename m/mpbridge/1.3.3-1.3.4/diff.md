# Comparing `tmp/mpbridge-1.3.3.tar.gz` & `tmp/mpbridge-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpbridge-1.3.3.tar", last modified: Thu Feb 16 13:16:30 2023, max compression
+gzip compressed data, was "mpbridge-1.3.4.tar", last modified: Fri Mar 24 09:11:26 2023, max compression
```

## Comparing `mpbridge-1.3.3.tar` & `mpbridge-1.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 13:16:30.936561 mpbridge-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-02-16 13:16:19.000000 mpbridge-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-02-16 13:16:30.936561 mpbridge-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-02-16 13:16:19.000000 mpbridge-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 13:16:30.936561 mpbridge-1.3.3/mpbridge/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-16 13:16:19.000000 mpbridge-1.3.3/mpbridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-02-16 13:16:19.000000 mpbridge-1.3.3/mpbridge/bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-02-16 13:16:19.000000 mpbridge-1.3.3/mpbridge/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-02-16 13:16:19.000000 mpbridge-1.3.3/mpbridge/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-02-16 13:16:19.000000 mpbridge-1.3.3/mpbridge/pyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-02-16 13:16:19.000000 mpbridge-1.3.3/mpbridge/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-02-16 13:16:19.000000 mpbridge-1.3.3/mpbridge/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 13:16:30.936561 mpbridge-1.3.3/mpbridge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-02-16 13:16:30.000000 mpbridge-1.3.3/mpbridge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-02-16 13:16:30.000000 mpbridge-1.3.3/mpbridge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 13:16:30.000000 mpbridge-1.3.3/mpbridge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-16 13:16:30.000000 mpbridge-1.3.3/mpbridge.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-16 13:16:30.000000 mpbridge-1.3.3/mpbridge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-16 13:16:30.000000 mpbridge-1.3.3/mpbridge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-02-16 13:16:19.000000 mpbridge-1.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-16 13:16:30.936561 mpbridge-1.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 09:11:26.934616 mpbridge-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-24 09:11:13.000000 mpbridge-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-03-24 09:11:26.930616 mpbridge-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-03-24 09:11:13.000000 mpbridge-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 09:11:26.930616 mpbridge-1.3.4/mpbridge/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-24 09:11:13.000000 mpbridge-1.3.4/mpbridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-03-24 09:11:13.000000 mpbridge-1.3.4/mpbridge/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-03-24 09:11:13.000000 mpbridge-1.3.4/mpbridge/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-03-24 09:11:13.000000 mpbridge-1.3.4/mpbridge/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-03-24 09:11:13.000000 mpbridge-1.3.4/mpbridge/pyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-03-24 09:11:13.000000 mpbridge-1.3.4/mpbridge/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-03-24 09:11:13.000000 mpbridge-1.3.4/mpbridge/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 09:11:26.930616 mpbridge-1.3.4/mpbridge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-03-24 09:11:26.000000 mpbridge-1.3.4/mpbridge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-24 09:11:26.000000 mpbridge-1.3.4/mpbridge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 09:11:26.000000 mpbridge-1.3.4/mpbridge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-24 09:11:26.000000 mpbridge-1.3.4/mpbridge.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-24 09:11:26.000000 mpbridge-1.3.4/mpbridge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-24 09:11:26.000000 mpbridge-1.3.4/mpbridge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-24 09:11:13.000000 mpbridge-1.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 09:11:26.934616 mpbridge-1.3.4/setup.cfg
```

### Comparing `mpbridge-1.3.3/LICENSE` & `mpbridge-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mpbridge-1.3.3/PKG-INFO` & `mpbridge-1.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpbridge
-Version: 1.3.3
+Version: 1.3.4
 Summary: File System Bridge to facilitate working with files on Micropython devices
 License: MIT License
         
         Copyright (c) 2022 Amirreza Hamzavi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -112,14 +112,15 @@
 tests/test_1.py
 tests/test_2.py
 ```
 
 * `mpbridge.ignore` syntax is not as same as `.gitignore` files.
 * At this time `mpbridge.ignore` only supports specifying file and directory paths directly.
 * You should add a **slash** at the end of directory names: `dir1/`.
+* Performing `sync` with `--dry-run` flag can be helpful for debugging your ignore files.
 
 ## ✅ Supported platforms
 
 - Windows
 - MacOS
 - Linux
 - FreeBSD/BSD
```

### Comparing `mpbridge-1.3.3/README.md` & `mpbridge-1.3.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 tests/test_1.py
 tests/test_2.py
 ```
 
 * `mpbridge.ignore` syntax is not as same as `.gitignore` files.
 * At this time `mpbridge.ignore` only supports specifying file and directory paths directly.
 * You should add a **slash** at the end of directory names: `dir1/`.
+* Performing `sync` with `--dry-run` flag can be helpful for debugging your ignore files.
 
 ## ✅ Supported platforms
 
 - Windows
 - MacOS
 - Linux
 - FreeBSD/BSD
```

### Comparing `mpbridge-1.3.3/mpbridge/bridge.py` & `mpbridge-1.3.4/mpbridge/bridge.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,24 +36,24 @@
                 time.sleep(1)
         except KeyboardInterrupt:
             observer.stop()
             pyb.exit_raw_repl_verbose()
         observer.join()
 
 
-def sync(port: str, path: str, clean: bool):
+def sync(port: str, path: str, clean: bool, dry_run: bool, push_only: bool):
     port = utils.port_abbreviation(port)
     print(Fore.YELLOW, f"- Syncing files on {port} with {path}")
     utils.reset_term_color()
     pyb = SweetPyboard(device=port)
     pyb.enter_raw_repl_verbose()
     if clean:
-        print(Fore.YELLOW, "Clean Sync files")
-        pyb.delete_absent_items(dir_path=path)
-    pyb.sync_with_dir(dir_path=path)
+        print(Fore.YELLOW, f"Removing absent files from {port}")
+        pyb.delete_absent_items(dir_path=path, dry=dry_run)
+    pyb.sync_with_dir(dir_path=path, dry=dry_run, push=push_only)
     pyb.exit_raw_repl_verbose()
 
 
 def start_dev_mode(port: str, path: str, auto_reset: str, no_prompt: bool):
     path = utils.replace_backslashes(path)
     port = utils.port_abbreviation(port)
     print(Fore.YELLOW, f"- Syncing files on {port} with {path}")
```

### Comparing `mpbridge-1.3.3/mpbridge/handler.py` & `mpbridge-1.3.4/mpbridge/handler.py`

 * *Files identical despite different names*

### Comparing `mpbridge-1.3.3/mpbridge/ignore.py` & `mpbridge-1.3.4/mpbridge/ignore.py`

 * *Files identical despite different names*

### Comparing `mpbridge-1.3.3/mpbridge/pyboard.py` & `mpbridge-1.3.4/mpbridge/pyboard.py`

 * *Files 14% similar despite different names*

```diff
@@ -57,56 +57,62 @@
         for item in eval(f'[{buf.decode("utf-8")}]'):
             if item[1]:
                 files[item[0]] = item[2]
             else:
                 dirs[item[0]] = item[2]
         return dirs, files
 
-    def fs_verbose_get(self, src, dest, chunk_size=1024):
+    def fs_verbose_get(self, src, dest, chunk_size=1024, dry: bool = False):
         def print_prog(written, total):
             utils.print_progress_bar(
                 iteration=written, total=total, decimals=0,
                 prefix=f"{Fore.LIGHTCYAN_EX} ↓ Getting {src}".ljust(60),
                 suffix="Complete", length=15)
 
-        self.fs_get(src, dest, chunk_size=chunk_size, progress_callback=print_prog)
+        if not dry:
+            self.fs_get(src, dest, chunk_size=chunk_size, progress_callback=print_prog)
         print_prog(1, 1)
         utils.reset_term_color(new_line=True)
 
-    def fs_verbose_put(self, src, dest, chunk_size=1024):
+    def fs_verbose_put(self, src, dest, chunk_size=1024, dry: bool = False):
         def print_prog(written, total):
             utils.print_progress_bar(
                 iteration=written, total=total, decimals=0,
                 prefix=f"{Fore.LIGHTYELLOW_EX} ↑ Putting {dest}".ljust(60),
                 suffix="Complete", length=15)
 
-        self.fs_put(src, dest, chunk_size=chunk_size, progress_callback=print_prog)
+        if not dry:
+            self.fs_put(src, dest, chunk_size=chunk_size, progress_callback=print_prog)
         print_prog(1, 1)
         utils.reset_term_color(new_line=True)
 
-    def fs_verbose_rename(self, src, dest):
-        buf, consumer = generate_buffer()
-        self.exec_(f'from os import rename; rename("{src}", "{dest}")',
-                   data_consumer=consumer)
+    def fs_verbose_rename(self, src, dest, dry: bool = False):
+        if not dry:
+            buf, consumer = generate_buffer()
+            self.exec_(f'from os import rename; rename("{src}", "{dest}")',
+                       data_consumer=consumer)
         print(Fore.LIGHTBLUE_EX, "O Rename", src, "→", dest)
         utils.reset_term_color()
 
-    def fs_verbose_mkdir(self, dir_path):
-        self.fs_mkdir(dir_path)
+    def fs_verbose_mkdir(self, dir_path, dry: bool = False):
+        if not dry:
+            self.fs_mkdir(dir_path)
         print(Fore.LIGHTGREEN_EX, "* Created", dir_path)
         utils.reset_term_color()
 
-    def fs_verbose_rm(self, src):
-        self.fs_rm(src)
+    def fs_verbose_rm(self, src, dry: bool = False):
+        if not dry:
+            self.fs_rm(src)
         print(Fore.LIGHTRED_EX, "✕ Removed", src)
         utils.reset_term_color()
 
-    def fs_verbose_rmdir(self, dir_path):
+    def fs_verbose_rmdir(self, dir_path, dry: bool = False):
         try:
-            self.fs_rmdir(dir_path)
+            if not dry:
+                self.fs_rmdir(dir_path)
         except PyboardError:
             print(Fore.RED, "E Cannot remove directory", dir_path, "as it might be mounted")
         else:
             print(Fore.LIGHTRED_EX, "✕ Removed", dir_path)
         utils.reset_term_color()
 
     def copy_all(self, dest_dir_path):
@@ -114,54 +120,56 @@
         for rdir in rdirs:
             os.makedirs(dest_dir_path + rdir, exist_ok=True)
         for rfile in rfiles:
             self.fs_verbose_get(rfile, dest_dir_path + rfile, chunk_size=256)
         print(Fore.LIGHTGREEN_EX, "✓ Copied all files successfully")
         utils.reset_term_color()
 
-    def sync_with_dir(self, dir_path):
+    def sync_with_dir(self, dir_path, dry: bool = False, push: bool = False):
         print(Fore.YELLOW, "- Syncing")
         self.exec_raw_no_follow(SHA1_FUNC)
         dir_path = utils.replace_backslashes(dir_path)
         rdirs, rfiles = self.fs_recursive_listdir()
         ldirs, lfiles = utils.recursive_list_dir(dir_path)
         ignore = IgnoreStorage(dir_path=dir_path)
-        for rdir in rdirs.keys():
-            if rdir not in ldirs and not ignore.match_dir(rdir):
-                os.makedirs(dir_path + rdir, exist_ok=True)
+        if (not dry) and (not push):
+            for rdir in rdirs.keys():
+                if rdir not in ldirs and not ignore.match_dir(rdir):
+                    os.makedirs(dir_path + rdir, exist_ok=True)
         for ldir in ldirs.keys():
             if ldir not in rdirs and not ignore.match_dir(ldir):
-                self.fs_verbose_mkdir(ldir)
+                self.fs_verbose_mkdir(ldir, dry=dry)
         for lfile_rel, lfiles_abs in lfiles.items():
             if ignore.match_file(lfile_rel):
                 continue
             if rfiles.get(lfile_rel, None) == os.path.getsize(lfiles_abs):
                 if self.get_sha1(lfile_rel) == utils.get_file_sha1(lfiles_abs):
                     continue
-            self.fs_verbose_put(lfiles_abs, lfile_rel, chunk_size=256)
-        for rfile, rsize in rfiles.items():
-            if ignore.match_file(rfile):
-                continue
-            if rfile not in lfiles:
-                self.fs_verbose_get(rfile, dir_path + rfile, chunk_size=256)
+            self.fs_verbose_put(lfiles_abs, lfile_rel, chunk_size=256, dry=dry)
+        if not push:
+            for rfile, rsize in rfiles.items():
+                if ignore.match_file(rfile):
+                    continue
+                if rfile not in lfiles:
+                    self.fs_verbose_get(rfile, dir_path + rfile, chunk_size=256, dry=dry)
         print(Fore.LIGHTGREEN_EX, "✓ Files synced successfully")
 
-    def delete_absent_items(self, dir_path):
+    def delete_absent_items(self, dir_path, dry: bool = False):
         dir_path = utils.replace_backslashes(dir_path)
         rdirs, rfiles = self.fs_recursive_listdir()
         ldirs, lfiles = utils.recursive_list_dir(dir_path)
         ignore = IgnoreStorage(dir_path=dir_path)
         for rfile, rsize in rfiles.items():
             if not ignore.match_file(rfile) and rfile not in lfiles:
-                self.fs_verbose_rm(rfile)
+                self.fs_verbose_rm(rfile, dry=dry)
         for rdir in rdirs.keys():
             if not ignore.match_dir(rdir) and rdir not in ldirs:
                 # There might be ignored files in folders
                 with suppress(Exception):
-                    self.fs_verbose_rmdir(rdir)
+                    self.fs_verbose_rmdir(rdir, dry=dry)
 
     def clear_all(self):
         print(Fore.YELLOW, "- Deleting all files from MicroPython board")
         rdirs, rfiles = self.fs_recursive_listdir()
         for rfile in rfiles.keys():
             self.fs_verbose_rm(rfile)
         for rdir in rdirs.keys():
```

### Comparing `mpbridge-1.3.3/mpbridge/shell.py` & `mpbridge-1.3.4/mpbridge/shell.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,16 +28,21 @@
     bridge.start_bridge_mode(port)
 
 
 @main.command("sync", short_help='Sync files with a directory')
 @click.argument('port')
 @click.argument('dir_path', type=click.Path(
     exists=True, file_okay=False, dir_okay=True, resolve_path=True), default="")
-@click.option('--clean', "-c", is_flag=True, help="Execute Clean Sync")
-def sync(port, dir_path, clean):
+@click.option('--clean', "-c", is_flag=True,
+              help="Execute Clean Sync")
+@click.option('--push-only', "-p", is_flag=True,
+              help="Only push changes without pulling anything from remote device")
+@click.option('--dry-run', "-d", is_flag=True,
+              help="Test Sync command without performing any actions")
+def sync(port, dir_path, clean, dry_run, push_only):
     """Sync files of on [PORT] in specified directory [DIR_PATH]
 
     If [DIR_PATH] is not set, it defaults to the current path
 
     [PORT] can be full path or :
 
             a[n]  connect to serial port "/dev/ttyACM[n]"
@@ -62,15 +67,15 @@
 
             Push files that are not in the device but exist locally to the device.
 
             Check the hash of the files both in the local and the device,
 
             and then push the different files from the local to the device.
     """
-    bridge.sync(port, dir_path, clean)
+    bridge.sync(port, dir_path, clean, dry_run, push_only)
 
 
 @main.command("dev", short_help='Start development mode')
 @click.argument('port')
 @click.argument('dir_path', type=click.Path(
     exists=True, file_okay=False, dir_okay=True, resolve_path=True), default="")
 @click.option('--auto-reset', help="Enables auto reset before entering REPL",
```

### Comparing `mpbridge-1.3.3/mpbridge/utils.py` & `mpbridge-1.3.4/mpbridge/utils.py`

 * *Files identical despite different names*

### Comparing `mpbridge-1.3.3/mpbridge.egg-info/PKG-INFO` & `mpbridge-1.3.4/mpbridge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpbridge
-Version: 1.3.3
+Version: 1.3.4
 Summary: File System Bridge to facilitate working with files on Micropython devices
 License: MIT License
         
         Copyright (c) 2022 Amirreza Hamzavi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -112,14 +112,15 @@
 tests/test_1.py
 tests/test_2.py
 ```
 
 * `mpbridge.ignore` syntax is not as same as `.gitignore` files.
 * At this time `mpbridge.ignore` only supports specifying file and directory paths directly.
 * You should add a **slash** at the end of directory names: `dir1/`.
+* Performing `sync` with `--dry-run` flag can be helpful for debugging your ignore files.
 
 ## ✅ Supported platforms
 
 - Windows
 - MacOS
 - Linux
 - FreeBSD/BSD
```

### Comparing `mpbridge-1.3.3/pyproject.toml` & `mpbridge-1.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mpbridge"
-version = "1.3.3"
+version = "1.3.4"
 description = "File System Bridge to facilitate working with files on Micropython devices"
 license = { file = "LICENSE" }
 keywords = [
     "micropython",
     "filemanager",
     "file-manager",
     "filesystem",
```

