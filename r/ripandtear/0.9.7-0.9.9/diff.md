# Comparing `tmp/ripandtear-0.9.7.tar.gz` & `tmp/ripandtear-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ripandtear-0.9.7.tar", last modified: Fri Apr 28 18:06:58 2023, max compression
+gzip compressed data, was "ripandtear-0.9.9.tar", last modified: Tue May  9 13:23:04 2023, max compression
```

## Comparing `ripandtear-0.9.7.tar` & `ripandtear-0.9.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-28 18:06:58.711943 ripandtear-0.9.7/
--rw-rw-r--   0 beard     (1000) beard     (1000)    35064 2023-02-18 23:42:30.000000 ripandtear-0.9.7/LICENSE
--rw-rw-r--   0 beard     (1000) beard     (1000)    17411 2023-04-28 18:06:58.711943 ripandtear-0.9.7/PKG-INFO
--rw-rw-r--   0 beard     (1000) beard     (1000)    17021 2023-04-22 18:41:05.000000 ripandtear-0.9.7/README.md
--rw-rw-r--   0 beard     (1000) beard     (1000)       90 2023-02-20 00:52:42.000000 ripandtear-0.9.7/pyproject.toml
-drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-28 18:06:58.679944 ripandtear-0.9.7/ripandtear/
--rw-rw-r--   0 beard     (1000) beard     (1000)       22 2023-04-28 18:05:18.000000 ripandtear-0.9.7/ripandtear/__init__.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     8025 2023-04-28 17:48:44.000000 ripandtear-0.9.7/ripandtear/__main__.py
-drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-28 18:06:58.691944 ripandtear-0.9.7/ripandtear/extractors/
--rw-rw-r--   0 beard     (1000) beard     (1000)        0 2023-02-19 22:50:13.000000 ripandtear-0.9.7/ripandtear/extractors/__init__.py
--rw-rw-r--   0 beard     (1000) beard     (1000)    13598 2023-04-28 18:05:18.000000 ripandtear-0.9.7/ripandtear/extractors/bunkr.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     8646 2023-02-28 02:57:32.000000 ripandtear-0.9.7/ripandtear/extractors/common.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     6740 2023-04-11 15:19:35.000000 ripandtear-0.9.7/ripandtear/extractors/coomer.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     5143 2023-04-11 15:19:35.000000 ripandtear-0.9.7/ripandtear/extractors/cyberdrop.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     2451 2023-04-11 15:19:35.000000 ripandtear-0.9.7/ripandtear/extractors/gfycat.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     5370 2023-04-11 15:19:35.000000 ripandtear-0.9.7/ripandtear/extractors/gofile.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     7926 2023-04-11 15:19:35.000000 ripandtear-0.9.7/ripandtear/extractors/imgur.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     8128 2023-04-11 15:19:35.000000 ripandtear-0.9.7/ripandtear/extractors/jpg.py
--rw-rw-r--   0 beard     (1000) beard     (1000)    18471 2023-04-11 15:19:35.000000 ripandtear-0.9.7/ripandtear/extractors/reddit.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     9382 2023-04-22 18:41:05.000000 ripandtear-0.9.7/ripandtear/extractors/redgifs.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     6065 2023-04-11 15:19:35.000000 ripandtear-0.9.7/ripandtear/extractors/tiktits.py
-drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-28 18:06:58.707943 ripandtear-0.9.7/ripandtear/utils/
--rw-rw-r--   0 beard     (1000) beard     (1000)        0 2023-02-19 04:04:14.000000 ripandtear-0.9.7/ripandtear/utils/__init__.py
--rw-rw-r--   0 beard     (1000) beard     (1000)    10060 2023-02-28 02:57:32.000000 ripandtear-0.9.7/ripandtear/utils/cli_arguments.py
--rw-rw-r--   0 beard     (1000) beard     (1000)      708 2023-02-27 19:25:42.000000 ripandtear-0.9.7/ripandtear/utils/color.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     6767 2023-04-11 15:19:35.000000 ripandtear-0.9.7/ripandtear/utils/conductor.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     7198 2023-04-22 18:41:05.000000 ripandtear-0.9.7/ripandtear/utils/content_finder.py
--rw-rw-r--   0 beard     (1000) beard     (1000)      870 2023-02-27 19:25:42.000000 ripandtear-0.9.7/ripandtear/utils/custom_types.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     8474 2023-04-11 15:19:35.000000 ripandtear-0.9.7/ripandtear/utils/downloader.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     2847 2023-02-20 00:52:42.000000 ripandtear-0.9.7/ripandtear/utils/file_hasher.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     2369 2023-04-11 15:19:35.000000 ripandtear-0.9.7/ripandtear/utils/file_sorter.py
--rw-rw-r--   0 beard     (1000) beard     (1000)      467 2023-02-27 19:25:42.000000 ripandtear-0.9.7/ripandtear/utils/logger.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     2196 2023-02-27 19:25:42.000000 ripandtear-0.9.7/ripandtear/utils/progress.py
--rw-rw-r--   0 beard     (1000) beard     (1000)    11036 2023-02-28 02:58:35.000000 ripandtear-0.9.7/ripandtear/utils/rat_info.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     4775 2023-02-27 19:25:42.000000 ripandtear-0.9.7/ripandtear/utils/rat_interaction.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     4961 2023-04-11 15:19:35.000000 ripandtear-0.9.7/ripandtear/utils/tracker.py
-drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-28 18:06:58.683944 ripandtear-0.9.7/ripandtear.egg-info/
--rw-rw-r--   0 beard     (1000) beard     (1000)    17411 2023-04-28 18:06:58.000000 ripandtear-0.9.7/ripandtear.egg-info/PKG-INFO
--rw-rw-r--   0 beard     (1000) beard     (1000)     1111 2023-04-28 18:06:58.000000 ripandtear-0.9.7/ripandtear.egg-info/SOURCES.txt
--rw-rw-r--   0 beard     (1000) beard     (1000)        1 2023-04-28 18:06:58.000000 ripandtear-0.9.7/ripandtear.egg-info/dependency_links.txt
--rw-rw-r--   0 beard     (1000) beard     (1000)       58 2023-04-28 18:06:58.000000 ripandtear-0.9.7/ripandtear.egg-info/entry_points.txt
--rw-rw-r--   0 beard     (1000) beard     (1000)      405 2023-04-28 18:06:58.000000 ripandtear-0.9.7/ripandtear.egg-info/requires.txt
--rw-rw-r--   0 beard     (1000) beard     (1000)       11 2023-04-28 18:06:58.000000 ripandtear-0.9.7/ripandtear.egg-info/top_level.txt
--rw-rw-r--   0 beard     (1000) beard     (1000)     1058 2023-04-28 18:06:58.711943 ripandtear-0.9.7/setup.cfg
+drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-05-09 13:23:04.921460 ripandtear-0.9.9/
+-rw-rw-r--   0 beard     (1000) beard     (1000)    35064 2023-02-18 23:42:30.000000 ripandtear-0.9.9/LICENSE
+-rw-rw-r--   0 beard     (1000) beard     (1000)    17411 2023-05-09 13:23:04.921460 ripandtear-0.9.9/PKG-INFO
+-rw-rw-r--   0 beard     (1000) beard     (1000)    17021 2023-04-22 18:41:05.000000 ripandtear-0.9.9/README.md
+-rw-rw-r--   0 beard     (1000) beard     (1000)       90 2023-02-20 00:52:42.000000 ripandtear-0.9.9/pyproject.toml
+drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-05-09 13:23:04.913460 ripandtear-0.9.9/ripandtear/
+-rw-rw-r--   0 beard     (1000) beard     (1000)       22 2023-05-09 13:22:13.000000 ripandtear-0.9.9/ripandtear/__init__.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     8025 2023-04-28 17:48:44.000000 ripandtear-0.9.9/ripandtear/__main__.py
+drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-05-09 13:23:04.917460 ripandtear-0.9.9/ripandtear/extractors/
+-rw-rw-r--   0 beard     (1000) beard     (1000)        0 2023-02-19 22:50:13.000000 ripandtear-0.9.9/ripandtear/extractors/__init__.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)    13598 2023-04-28 18:05:18.000000 ripandtear-0.9.9/ripandtear/extractors/bunkr.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     8646 2023-02-28 02:57:32.000000 ripandtear-0.9.9/ripandtear/extractors/common.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     6742 2023-05-06 01:48:26.000000 ripandtear-0.9.9/ripandtear/extractors/coomer.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     5143 2023-04-11 15:19:35.000000 ripandtear-0.9.9/ripandtear/extractors/cyberdrop.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     2451 2023-04-11 15:19:35.000000 ripandtear-0.9.9/ripandtear/extractors/gfycat.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     5370 2023-04-11 15:19:35.000000 ripandtear-0.9.9/ripandtear/extractors/gofile.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     8015 2023-05-09 13:21:50.000000 ripandtear-0.9.9/ripandtear/extractors/imgur.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     8128 2023-04-11 15:19:35.000000 ripandtear-0.9.9/ripandtear/extractors/jpg.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)    18471 2023-04-11 15:19:35.000000 ripandtear-0.9.9/ripandtear/extractors/reddit.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     9382 2023-04-22 18:41:05.000000 ripandtear-0.9.9/ripandtear/extractors/redgifs.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     6065 2023-04-11 15:19:35.000000 ripandtear-0.9.9/ripandtear/extractors/tiktits.py
+drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-05-09 13:23:04.921460 ripandtear-0.9.9/ripandtear/utils/
+-rw-rw-r--   0 beard     (1000) beard     (1000)        0 2023-02-19 04:04:14.000000 ripandtear-0.9.9/ripandtear/utils/__init__.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)    10060 2023-02-28 02:57:32.000000 ripandtear-0.9.9/ripandtear/utils/cli_arguments.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)      708 2023-02-27 19:25:42.000000 ripandtear-0.9.9/ripandtear/utils/color.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     6767 2023-04-11 15:19:35.000000 ripandtear-0.9.9/ripandtear/utils/conductor.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     7197 2023-05-03 05:13:41.000000 ripandtear-0.9.9/ripandtear/utils/content_finder.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)      870 2023-02-27 19:25:42.000000 ripandtear-0.9.9/ripandtear/utils/custom_types.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     8474 2023-04-11 15:19:35.000000 ripandtear-0.9.9/ripandtear/utils/downloader.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     2847 2023-02-20 00:52:42.000000 ripandtear-0.9.9/ripandtear/utils/file_hasher.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     2369 2023-04-11 15:19:35.000000 ripandtear-0.9.9/ripandtear/utils/file_sorter.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)      467 2023-02-27 19:25:42.000000 ripandtear-0.9.9/ripandtear/utils/logger.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     2196 2023-02-27 19:25:42.000000 ripandtear-0.9.9/ripandtear/utils/progress.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)    11036 2023-02-28 02:58:35.000000 ripandtear-0.9.9/ripandtear/utils/rat_info.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     4775 2023-02-27 19:25:42.000000 ripandtear-0.9.9/ripandtear/utils/rat_interaction.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     4961 2023-04-11 15:19:35.000000 ripandtear-0.9.9/ripandtear/utils/tracker.py
+drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-05-09 13:23:04.913460 ripandtear-0.9.9/ripandtear.egg-info/
+-rw-rw-r--   0 beard     (1000) beard     (1000)    17411 2023-05-09 13:23:04.000000 ripandtear-0.9.9/ripandtear.egg-info/PKG-INFO
+-rw-rw-r--   0 beard     (1000) beard     (1000)     1111 2023-05-09 13:23:04.000000 ripandtear-0.9.9/ripandtear.egg-info/SOURCES.txt
+-rw-rw-r--   0 beard     (1000) beard     (1000)        1 2023-05-09 13:23:04.000000 ripandtear-0.9.9/ripandtear.egg-info/dependency_links.txt
+-rw-rw-r--   0 beard     (1000) beard     (1000)       58 2023-05-09 13:23:04.000000 ripandtear-0.9.9/ripandtear.egg-info/entry_points.txt
+-rw-rw-r--   0 beard     (1000) beard     (1000)      405 2023-05-09 13:23:04.000000 ripandtear-0.9.9/ripandtear.egg-info/requires.txt
+-rw-rw-r--   0 beard     (1000) beard     (1000)       11 2023-05-09 13:23:04.000000 ripandtear-0.9.9/ripandtear.egg-info/top_level.txt
+-rw-rw-r--   0 beard     (1000) beard     (1000)     1058 2023-05-09 13:23:04.921460 ripandtear-0.9.9/setup.cfg
```

### Comparing `ripandtear-0.9.7/LICENSE` & `ripandtear-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.7/PKG-INFO` & `ripandtear-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ripandtear
-Version: 0.9.7
+Version: 0.9.9
 Summary: An asynchronous file archival program
 Home-page: https://gitlab.com/johnny_barracuda/ripandtear/
 Author: Johnny-Barracuda
 Author-email: johnny_barracuda@protonmail.ch
 Project-URL: Bug Tracker, https://gitlab.com/johnny_barracuda/ripandtear/
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ripandtear-0.9.7/README.md` & `ripandtear-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.7/ripandtear/__main__.py` & `ripandtear-0.9.9/ripandtear/__main__.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.7/ripandtear/extractors/bunkr.py` & `ripandtear-0.9.9/ripandtear/extractors/bunkr.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.7/ripandtear/extractors/common.py` & `ripandtear-0.9.9/ripandtear/extractors/common.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.7/ripandtear/extractors/coomer.py` & `ripandtear-0.9.9/ripandtear/extractors/coomer.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                 response = await client.get(url, timeout=None, follow_redirects=True)
 
         except httpx.ReadError:
             await self.common_failed_attempt(url_dictionary.copy())
             return
 
         if response.status_code >= 300:
-            print(f"{response.status_code} - {url_dictionary}")
+            # print(f"{response.status_code} - {url_dictionary}")
             url_dictionary['status_code'] = response.status_code
             await self.common_bad_status_code(url_dictionary.copy())
             return
 
         return response
 
     async def single_content_download(self, url_dictionary: UrlDictionary) -> None:
```

### Comparing `ripandtear-0.9.7/ripandtear/extractors/cyberdrop.py` & `ripandtear-0.9.9/ripandtear/extractors/cyberdrop.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.7/ripandtear/extractors/gfycat.py` & `ripandtear-0.9.9/ripandtear/extractors/gfycat.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.7/ripandtear/extractors/gofile.py` & `ripandtear-0.9.9/ripandtear/extractors/gofile.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.7/ripandtear/extractors/imgur.py` & `ripandtear-0.9.9/ripandtear/extractors/imgur.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,19 @@
 
             log.debug("Multiple images found. Sending them to single download")
             tasks = []
             count = 0
             for entry in data['data']:
 
                 count += 1
-                image_hash = self.imgur_direct_image_hash(entry['link'])
+                try:
+                    image_hash = self.imgur_direct_image_hash(entry['link'])
+
+                except TypeError:
+                    continue
 
                 url_dictionary['album_name'] = album_hash
                 url_dictionary['count'] = count
 
                 tasks.append(asyncio.create_task(
                     self.imgur_single_download(image_hash, url_dictionary.copy())))
```

### Comparing `ripandtear-0.9.7/ripandtear/extractors/jpg.py` & `ripandtear-0.9.9/ripandtear/extractors/jpg.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.7/ripandtear/extractors/reddit.py` & `ripandtear-0.9.9/ripandtear/extractors/reddit.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.7/ripandtear/extractors/redgifs.py` & `ripandtear-0.9.9/ripandtear/extractors/redgifs.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.7/ripandtear/extractors/tiktits.py` & `ripandtear-0.9.9/ripandtear/extractors/tiktits.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.7/ripandtear/utils/cli_arguments.py` & `ripandtear-0.9.9/ripandtear/utils/cli_arguments.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.7/ripandtear/utils/color.py` & `ripandtear-0.9.9/ripandtear/utils/color.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.7/ripandtear/utils/conductor.py` & `ripandtear-0.9.9/ripandtear/utils/conductor.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.7/ripandtear/utils/content_finder.py` & `ripandtear-0.9.9/ripandtear/utils/content_finder.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 async def download_urls(args, url_dictionary: UrlDictionary) -> None:
 
     tasks = []
     for entry in args.download:
         for url in entry.split('|'):
 
             url_dictionary: UrlDictionary = url_dictionary_constructor(
-                url.strip(), url_dictionary.copy(), download=True,)
+                url.strip(), url_dictionary.copy(), download=True)
 
             tasks.append(asyncio.create_task(
                 conductor.validate_url(url_dictionary.copy())))
 
     await asyncio.gather(*tasks)
```

### Comparing `ripandtear-0.9.7/ripandtear/utils/custom_types.py` & `ripandtear-0.9.9/ripandtear/utils/custom_types.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.7/ripandtear/utils/downloader.py` & `ripandtear-0.9.9/ripandtear/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.7/ripandtear/utils/file_hasher.py` & `ripandtear-0.9.9/ripandtear/utils/file_hasher.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.7/ripandtear/utils/file_sorter.py` & `ripandtear-0.9.9/ripandtear/utils/file_sorter.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.7/ripandtear/utils/progress.py` & `ripandtear-0.9.9/ripandtear/utils/progress.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.7/ripandtear/utils/rat_info.py` & `ripandtear-0.9.9/ripandtear/utils/rat_info.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.7/ripandtear/utils/rat_interaction.py` & `ripandtear-0.9.9/ripandtear/utils/rat_interaction.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.7/ripandtear/utils/tracker.py` & `ripandtear-0.9.9/ripandtear/utils/tracker.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.7/ripandtear.egg-info/PKG-INFO` & `ripandtear-0.9.9/ripandtear.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ripandtear
-Version: 0.9.7
+Version: 0.9.9
 Summary: An asynchronous file archival program
 Home-page: https://gitlab.com/johnny_barracuda/ripandtear/
 Author: Johnny-Barracuda
 Author-email: johnny_barracuda@protonmail.ch
 Project-URL: Bug Tracker, https://gitlab.com/johnny_barracuda/ripandtear/
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ripandtear-0.9.7/ripandtear.egg-info/SOURCES.txt` & `ripandtear-0.9.9/ripandtear.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.7/setup.cfg` & `ripandtear-0.9.9/setup.cfg`

 * *Files identical despite different names*

