# Comparing `tmp/recognize-0.1.8.tar.gz` & `tmp/recognize-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recognize-0.1.8.tar", max compression
+gzip compressed data, was "recognize-0.1.9.tar", max compression
```

## Comparing `recognize-0.1.8.tar` & `recognize-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-06-05 10:54:25.494041 recognize-0.1.8/README.md
--rw-r--r--   0        0        0      436 2023-06-07 22:21:03.584083 recognize-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 10:51:05.501277 recognize-0.1.8/recognize/__init__.py
--rw-r--r--   0        0        0        0 2023-06-03 22:10:35.106880 recognize-0.1.8/recognize/commands/__init__.py
--rw-r--r--   0        0        0        0 2023-06-03 22:21:58.098646 recognize-0.1.8/recognize/commands/lib/__init__.py
--rw-r--r--   0        0        0     4471 2023-06-07 22:20:45.932619 recognize-0.1.8/recognize/commands/lib/client.py
--rw-r--r--   0        0        0      175 2023-06-05 10:43:58.870449 recognize-0.1.8/recognize/commands/lib/entries.py
--rw-r--r--   0        0        0     1574 2023-06-07 17:10:59.829887 recognize-0.1.8/recognize/commands/lib/helpers.py
--rw-r--r--   0        0        0     3288 2023-06-07 17:10:59.830868 recognize-0.1.8/recognize/commands/search.py
--rw-r--r--   0        0        0     1723 2023-06-07 17:10:59.831782 recognize-0.1.8/recognize/commands/upload.py
--rw-r--r--   0        0        0      713 2023-06-07 17:10:59.832702 recognize-0.1.8/recognize/main.py
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 recognize-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1759 2023-06-08 09:57:25.053257 recognize-0.1.9/README.md
+-rw-r--r--   0        0        0      436 2023-06-08 10:18:37.607604 recognize-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 10:51:05.501277 recognize-0.1.9/recognize/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-03 22:10:35.106880 recognize-0.1.9/recognize/commands/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-03 22:21:58.098646 recognize-0.1.9/recognize/commands/lib/__init__.py
+-rw-r--r--   0        0        0     4506 2023-06-08 08:59:41.212224 recognize-0.1.9/recognize/commands/lib/client.py
+-rw-r--r--   0        0        0      175 2023-06-05 10:43:58.870449 recognize-0.1.9/recognize/commands/lib/entries.py
+-rw-r--r--   0        0        0     1574 2023-06-07 17:10:59.829887 recognize-0.1.9/recognize/commands/lib/helpers.py
+-rw-r--r--   0        0        0     5224 2023-06-08 09:26:55.545387 recognize-0.1.9/recognize/commands/search.py
+-rw-r--r--   0        0        0     2674 2023-06-08 09:07:30.779601 recognize-0.1.9/recognize/commands/upload.py
+-rw-r--r--   0        0        0      713 2023-06-08 10:18:04.611309 recognize-0.1.9/recognize/main.py
+-rw-r--r--   0        0        0     2297 1970-01-01 00:00:00.000000 recognize-0.1.9/PKG-INFO
```

### Comparing `recognize-0.1.8/recognize/commands/lib/client.py` & `recognize-0.1.9/recognize/commands/lib/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,27 +65,28 @@
 
         try:
             st = speedtest.Speedtest()
             upload_speed_mbps = st.upload() / 1e6  # Convert bits per second to Mbps
         except:
             upload_speed_mbps = 10
 
-        semaphore = asyncio.Semaphore(min(10, max(1, int(upload_speed_mbps / 2))))
+        max_concurrent_uploads = min(15, max(1, int(upload_speed_mbps / 2)))
+        semaphore = asyncio.Semaphore(max_concurrent_uploads)
 
         tasks = [upload_file(semaphore, file_path, url, self.dev) for file_path in file_paths]
 
         with rich.progress.Progress(
                 "[progress.percentage]{task.percentage:>3.0f}%",
                 rich.progress.BarColumn(bar_width=None),
                 rich.progress.MofNCompleteColumn(),
         ) as progress:
             download_task = progress.add_task(description="Uploading files...", total=len(tasks))
             progress.console.print(
                 f'[bold green]Current upload speed: {int(upload_speed_mbps)} Mbps. '
-                f'Number of concurrent uploads limited to {min(10, max(1, int(upload_speed_mbps / 2)))}.'
+                f'Number of concurrent uploads limited to {max_concurrent_uploads}.'
             )
             for task in asyncio.as_completed(tasks):
                 path, success, message = await task
                 progress.console.print(
                     f"{'[bold blue]Uploaded' if success else '[bold red]Failed'}: {path}. {message if not success else ''}")
                 progress.update(download_task, advance=1)
```

### Comparing `recognize-0.1.8/recognize/commands/lib/helpers.py` & `recognize-0.1.9/recognize/commands/lib/helpers.py`

 * *Files identical despite different names*

### Comparing `recognize-0.1.8/recognize/main.py` & `recognize-0.1.9/recognize/main.py`

 * *Files identical despite different names*

