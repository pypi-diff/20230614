# Comparing `tmp/xklb-1.31.2.tar.gz` & `tmp/xklb-1.31.3.tar.gz`

## Comparing `xklb-1.31.2.tar` & `xklb-1.31.3.tar`

### file list

```diff
@@ -1,66 +1,67 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.31.2/.gitattributes
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 xklb-1.31.2/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.31.2/Windows.md
--rw-r--r--   0        0        0   490396 2020-02-02 00:00:00.000000 xklb-1.31.2/pdm.lock
--rw-r--r--   0        0        0    19137 2020-02-02 00:00:00.000000 xklb-1.31.2/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.31.2/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.31.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.31.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-1.31.2/.github/workflows/push.yaml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/__init__.py
--rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/books.py
--rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/consts.py
--rw-r--r--   0        0        0     8216 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/db.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/dl_config.py
--rw-r--r--   0        0        0    12453 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/dl_extract.py
--rw-r--r--   0        0        0    14103 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/fs_extract.py
--rw-r--r--   0        0        0     7515 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/gdl_backend.py
--rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/gdl_extract.py
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/gui.py
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/hn_extract.py
--rw-r--r--   0        0        0    11564 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/lb.py
--rw-r--r--   0        0        0     7288 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/media.py
--rw-r--r--   0        0        0    25135 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/play_actions.py
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/playback.py
--rw-r--r--   0        0        0    35233 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/player.py
--rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/playlists.py
--rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/praw_extract.py
--rw-r--r--   0        0        0     7949 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/search.py
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/subtitle.py
--rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/tabs_actions.py
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/tabs_extract.py
--rw-r--r--   0        0        0    15396 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/tube_backend.py
--rw-r--r--   0        0        0     5433 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/tube_extract.py
--rw-r--r--   0        0        0    75374 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/usage.py
--rw-r--r--   0        0        0    36702 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/block.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/christen.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/history.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     6044 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/relmv.py
--rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.31.2/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.31.2/LICENSE
--rw-r--r--   0        0        0    97830 2020-02-02 00:00:00.000000 xklb-1.31.2/README.md
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 xklb-1.31.2/pyproject.toml
--rw-r--r--   0        0        0   101457 2020-02-02 00:00:00.000000 xklb-1.31.2/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.31.3/.gitattributes
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 xklb-1.31.3/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.31.3/Windows.md
+-rw-r--r--   0        0        0   490396 2020-02-02 00:00:00.000000 xklb-1.31.3/pdm.lock
+-rw-r--r--   0        0        0    19137 2020-02-02 00:00:00.000000 xklb-1.31.3/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.31.3/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.31.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.31.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-1.31.3/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/__init__.py
+-rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/books.py
+-rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/consts.py
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/db.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/dl_config.py
+-rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/dl_extract.py
+-rw-r--r--   0        0        0    14103 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/fs_extract.py
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/gdl_backend.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/gdl_extract.py
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/gui.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/hn_extract.py
+-rw-r--r--   0        0        0    11781 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/lb.py
+-rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/media.py
+-rw-r--r--   0        0        0    25135 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/play_actions.py
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/playback.py
+-rw-r--r--   0        0        0    35233 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/player.py
+-rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/playlists.py
+-rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7949 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/search.py
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/subtitle.py
+-rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    15396 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/tube_extract.py
+-rw-r--r--   0        0        0    75973 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/usage.py
+-rw-r--r--   0        0        0    36702 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/scripts/dedupe_db.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/scripts/history.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     6044 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.31.3/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.31.3/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.31.3/LICENSE
+-rw-r--r--   0        0        0    97830 2020-02-02 00:00:00.000000 xklb-1.31.3/README.md
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 xklb-1.31.3/pyproject.toml
+-rw-r--r--   0        0        0   101457 2020-02-02 00:00:00.000000 xklb-1.31.3/PKG-INFO
```

### Comparing `xklb-1.31.2/TODO` & `xklb-1.31.3/TODO`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,18 @@
-- dedupe-db
-
-dedupe-db script
-
---bk path --pk id --upsert-columns play_count,time_played,playhead,time_downloaded,time_deleted,time_uploaded,webpath,language,title,tube_id,view_count,uploader,playlist_path,live_status
-
-SELECT MIN(id) AS min_id, path
-FROM your_table
-GROUP BY path;
-
-for col in args.upsert_columns:
-    SELECT play_count
-    FROM media
-    WHERE play_count IS NOT NULL
-
-    UPDATE media set play_count = ? WHERE path = ?
-
-
-DELETE FROM your_table
-WHERE id NOT IN (
-  SELECT min_id
-  FROM temp_table
-);
 
 lb bigdirs ~/lb/video.db
 
 /mnt/d/75_MovieQueue/unsorted/NRMwalkthroughHD/ should be 200GB
 
+- if limit is less than 120, check up to 120 files to see if they exist
+
 - scatter -- flatten to new directories
 
+default 16000 files, flat subdirectory
+
 - dlstatus print errors also:
 
 sqlite lb/fs/blogspot.db 'select error, count(*) from media group by 1 order by 2'
 [{"error": "NoExtractorError", "count(*)": 21},
  {"error": null, "count(*)": 46},
  {"error": "HTTPError", "count(*)": 112},
  {"error": "HTTPNotFoundError", "count(*)": 118}]
```

### Comparing `xklb-1.31.2/Windows.md` & `xklb-1.31.3/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/pdm.lock` & `xklb-1.31.3/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/readme.py` & `xklb-1.31.3/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.31.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.31.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/.github/workflows/push.yaml` & `xklb-1.31.3/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/av.py` & `xklb-1.31.3/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/books.py` & `xklb-1.31.3/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/consts.py` & `xklb-1.31.3/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/db.py` & `xklb-1.31.3/xklb/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
                 if index.unique == 1:
                     db.execute(f"REINDEX {index.name}")
                 else:
                     db.execute(f"DROP index {index.name}")
 
         for column in int_columns + str_columns:
             log.info("Creating index: %s", column)
-            db[table].create_index([column], if_not_exists=True, analyze=True)  # type: ignore
+            db[table].create_index([column], unique=column == "path", if_not_exists=True, analyze=True)  # type: ignore
 
         if any(fts_columns) and (db[table].detect_fts() is None or was_transformed):  # type: ignore
             log.info("Creating fts index: %s", fts_columns)
             db[table].enable_fts(
                 fts_columns,
                 create_triggers=True,
                 replace=True,
```

### Comparing `xklb-1.31.2/xklb/dl_config.py` & `xklb-1.31.3/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/dl_extract.py` & `xklb-1.31.3/xklb/dl_extract.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse, os, random, sys
 from pathlib import Path
 from typing import List, Tuple
 
 from xklb import db, gdl_backend, play_actions, player, tube_backend, usage, utils
 from xklb.consts import SC, DBType
+from xklb.media import get_paths
 from xklb.utils import log
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
         prog="library download",
         usage=usage.download,
@@ -199,34 +200,17 @@
         """
 
     return query, args.filter_bindings
 
 
 def process_downloadqueue(args) -> List[dict]:
     if args.playlist_files:
-        tables = args.db.table_names()
         known_playlists = set()
-        if "media" in tables and not args.force:
-            m_columns = db.columns(args, "media")
-            known_playlists = set(
-                d["path"]
-                for d in args.db.query(
-                    (
-                        "SELECT path from media"
-                        + " WHERE path in ("
-                        + ",".join(["?"] * len(args.playlists))
-                        + f") or {'web' if 'webpath' in m_columns else ''}path in ("
-                        + ",".join(["?"] * len(args.playlists))
-                        + ")"
-                        + " UNION ALL"
-                        + " SELECT path from playlists"
-                    ),
-                    [*args.playlists, *args.playlists],
-                )
-            )
+        if not args.force:
+            known_playlists = get_paths(args)
 
         Path(args.database).touch()
         playlist_files_data = set(utils.flatten(Path(p).read_text().splitlines() for p in args.playlists))
         playlists = list(playlist_files_data - known_playlists)
         log.warning(
             "%s new - %s known = %s to download",
             len(playlist_files_data),
```

### Comparing `xklb-1.31.2/xklb/fs_extract.py` & `xklb-1.31.3/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/gdl_backend.py` & `xklb-1.31.3/xklb/gdl_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 
 def parse_gdl_job_status(job_status, path):
     errors = []
 
     if job_status & 1:
         errors.append("UnspecifiedError")
         log.error("[%s]: gallery_dl gave an UnspecifiedError.", path)
-        raise NotImplementedError
 
     if job_status & 64:  # no extractor
         errors.append("NoExtractorError")
         log.info("[%s]: NoExtractorError", path)
 
     if job_status & 16 or job_status & 32:
         if job_status & 16:
```

### Comparing `xklb-1.31.2/xklb/gdl_extract.py` & `xklb-1.31.3/xklb/tube_extract.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse, sys
 from pathlib import Path
 
-from xklb import consts, db, gdl_backend, playlists, usage, utils
+from xklb import consts, db, media, playlists, tube_backend, usage, utils
 from xklb.consts import SC
 from xklb.utils import log
 
 
 def parse_args(action, usage) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library " + action,
@@ -18,107 +18,107 @@
         "-extractor-config",
         nargs=1,
         action=utils.ArgparseDict,
         default={},
         metavar="KEY=VALUE",
         help="Add key/value pairs to override or extend default downloader configuration",
     )
-    parser.add_argument("--download-archive", default="~/.local/share/gallerydl.sqlite3")
+    parser.add_argument("--download-archive", default="~/.local/share/yt_archive.txt")
     parser.add_argument("--safe", "-safe", action="store_true", help="Skip generic URLs")
     parser.add_argument("--no-sanitize", "-s", action="store_true", help="Don't sanitize some common URL parameters")
+    parser.add_argument("--extra", "-extra", action="store_true", help="Get full metadata (takes a lot longer)")
     parser.add_argument("--playlist-files", action="store_true", help="Read playlists from text files")
     parser.add_argument(
         "--force",
         "-f",
         action="store_true",
         help="Fetch metadata for paths even if they are already in the media table",
     )
+    parser.add_argument("--subs", action="store_true")
+    parser.add_argument("--auto-subs", "--autosubs", action="store_true")
+    parser.add_argument("--subtitle-languages", "--subtitle-language", "--sl", action=utils.ArgparseList)
     parser.add_argument("--extra-media-data", default={}, nargs=1, action=utils.ArgparseDict, metavar="KEY=VALUE")
     parser.add_argument("--extra-playlist-data", default={}, nargs=1, action=utils.ArgparseDict, metavar="KEY=VALUE")
     parser.add_argument("--ignore-errors", "--ignoreerrors", "-i", action="store_true", help=argparse.SUPPRESS)
 
     parser.add_argument("--timeout", "-T", help="Quit after x minutes")
     parser.add_argument("--verbose", "-v", action="count", default=0)
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
 
     parser.add_argument("database")
-    if action == SC.galleryadd:
+    if action == SC.tubeadd:
         parser.add_argument("playlists", nargs="+", help=argparse.SUPPRESS)
 
     args = parser.parse_args()
     args.action = action
 
     if args.db:
         args.database = args.db
-    if action == SC.galleryadd:
+    if action == SC.tubeadd:
         Path(args.database).touch()
     args.db = db.connect(args)
 
     if hasattr(args, "playlists"):
         args.playlists = list(set(s.strip() for s in args.playlists))
         if not args.no_sanitize:
             args.playlists = [utils.sanitize_url(args, p) for p in args.playlists]
         args.playlists = utils.conform(args.playlists)
 
     utils.timeout(args.timeout)
 
-    args.profile = consts.DBType.image
+    args.profile = consts.DBType.video
     log.info(utils.dict_filter_bool(args.__dict__))
     return args
 
 
-def gallery_add(args=None) -> None:
+def tube_add(args=None) -> None:
     if args:
-        sys.argv = ["galleryadd", *args]
+        sys.argv = ["tubeadd", *args]
 
-    args = parse_args(SC.galleryadd, usage=usage.galleryadd)
+    args = parse_args(SC.tubeadd, usage=usage.tubeadd)
     if args.playlist_files:
         args.playlists = list(utils.flatten([Path(p).read_text().splitlines() for p in args.playlists]))
 
-    tables = args.db.table_names()
-    known_playlists = []
-    if "media" in tables and not args.force:
-        m_columns = db.columns(args, "media")
-        known_playlists = list(
-            set(
-                d["path"]
-                for d in args.db.query(
-                    (
-                        "SELECT path from media"
-                        + " WHERE path in ("
-                        + ",".join(["?"] * len(args.playlists))
-                        + f") or {'web' if 'webpath' in m_columns else ''}path in ("
-                        + ",".join(["?"] * len(args.playlists))
-                        + ")"
-                        + " UNION ALL"
-                        + " SELECT path from playlists"
-                    ),
-                    [*args.playlists, *args.playlists],
-                )
-            ),
-        )
+    known_playlists = set()
+    if not args.force:
+        known_playlists = media.get_paths(args)
 
-    added_media_count = 0
     for path in args.playlists:
+        if args.safe and not tube_backend.is_supported(path):
+            log.info("[%s]: Skipping unsupported playlist (safe_mode)", path)
+            continue
+
         if path in known_playlists:
             log.info("[%s]: Already added. Skipping!", path)
             continue
 
-        if args.safe and not gdl_backend.is_supported(args, path):
-            log.info("[%s]: Skipping unsupported playlist (safe_mode)", path)
-            continue
+        tube_backend.get_playlist_metadata(args, path, tube_backend.tube_opts(args))
 
-        added_media_count += gdl_backend.get_playlist_metadata(args, path)
+        if args.extra:
+            log.warning("[%s]: Getting extra metadata", path)
+            tube_backend.get_extra_metadata(args, path)
 
     LARGE_NUMBER = 100_000
-    if not args.db["media"].detect_fts() or added_media_count > LARGE_NUMBER:
+    if not args.db["media"].detect_fts() or tube_backend.added_media_count > LARGE_NUMBER:
         db.optimize(args)
 
 
-def gallery_update(args=None) -> None:
+def tube_update(args=None) -> None:
     if args:
-        sys.argv = ["galleryupdate", *args]
+        sys.argv = ["tubeupdate", *args]
 
-    args = parse_args(SC.galleryupdate, usage=usage.galleryupdate)
+    args = parse_args(SC.tubeupdate, usage=usage.tubeupdate)
+    tube_playlists = playlists.get_all(args)
+    for d in tube_playlists:
+        tube_backend.get_playlist_metadata(
+            args,
+            d["path"],
+            tube_backend.tube_opts(
+                args,
+                playlist_opts=d.get("extractor_config", "{}"),
+                func_opts={"ignoreerrors": "only_download"},
+            ),
+        )
 
-    for d in playlists.get_all(args):
-        gdl_backend.get_playlist_metadata(args, d["path"])
+        if args.extra:
+            log.warning("[%s]: Getting extra metadata", d["path"])
+            tube_backend.get_extra_metadata(args, d["path"], playlist_dl_opts=d.get("extractor_config", "{}"))
```

### Comparing `xklb-1.31.2/xklb/gui.py` & `xklb-1.31.3/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/hn_extract.py` & `xklb-1.31.3/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/lb.py` & `xklb-1.31.3/xklb/lb.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from xklb.praw_extract import reddit_add, reddit_update
 from xklb.scripts.bigdirs import bigdirs
 from xklb.scripts.block import block
 from xklb.scripts.christen import christen
 from xklb.scripts.cluster_sort import cluster_sort
 from xklb.scripts.copy_play_counts import copy_play_counts
 from xklb.scripts.dedupe import dedupe
+from xklb.scripts.dedupe_db import dedupe_db
 from xklb.scripts.download_status import download_status
 from xklb.scripts.history import history
 from xklb.scripts.merge_dbs import merge_dbs
 from xklb.scripts.merge_online_local import merge_online_local
 from xklb.scripts.mining.extract_links import extract_links
 from xklb.scripts.mining.nouns import nouns
 from xklb.scripts.mining.pushshift import pushshift_extract
@@ -108,15 +109,15 @@
 
 
 def print_help(parser) -> None:
     print(usage())
     print(parser.epilog)
 
 
-subcommands = ["fs", "du"]
+subcommands = ["fs", "du", "dedupe"]
 
 
 def consecutive_prefixes(s):
     prefixes = [s[:j] for j in range(5, len(s)) if s[:j] and s[:j] not in subcommands]
     subcommands.extend(prefixes)
     return prefixes
 
@@ -168,16 +169,18 @@
     subp_scatter = add_parser(subparsers, "scatter")
     subp_scatter.set_defaults(func=scatter)
     subp_christen = add_parser(subparsers, "christen")
     subp_christen.set_defaults(func=christen)
 
     subp_merge_db = add_parser(subparsers, "merge-dbs", ["merge-db", "mergedb", "mergedbs", "merge_db", "merge_dbs"])
     subp_merge_db.set_defaults(func=merge_dbs)
-    subp_merge_db = add_parser(subparsers, "copy-play-counts")
-    subp_merge_db.set_defaults(func=copy_play_counts)
+    subp_dedupe_db = add_parser(subparsers, "dedupe-dbs", ["dedupe-db", "dedupedb", "dedupe_db"])
+    subp_dedupe_db.set_defaults(func=dedupe_db)
+    subp_copy_play_counts = add_parser(subparsers, "copy-play-counts")
+    subp_copy_play_counts.set_defaults(func=copy_play_counts)
 
     subp_dedupe = add_parser(subparsers, "dedupe")
     subp_dedupe.set_defaults(func=dedupe)
     subp_dedupe_local = add_parser(subparsers, "merge-online-local")
     subp_dedupe_local.set_defaults(func=merge_online_local)
     subp_optimize = add_parser(subparsers, "optimize", ["optimize-db"])
     subp_optimize.set_defaults(func=optimize_db)
```

### Comparing `xklb-1.31.2/xklb/media.py` & `xklb-1.31.3/xklb/media.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,24 @@
     return True
 
 
 def get(args, path):
     return args.db.pop_dict("select * from media where path = ?", path)
 
 
+def get_paths(args):
+    tables = args.db.table_names()
+    known_playlists = set()
+    if "media" in tables:
+        known_playlists.update(d["path"] for d in args.db.query("SELECT path from media"))
+    if "playlists" in tables:
+        known_playlists.update(d["path"] for d in args.db.query("SELECT path from playlists"))
+    return known_playlists
+
+
 def consolidate(v: dict) -> Optional[dict]:
     v = {
         **(v.pop("photo", None) or {}),
         **(v.pop("blog", None) or {}),
         **(v.pop("location", None) or {}),
         **(v.pop("post", None) or {}),
         **v,
```

### Comparing `xklb-1.31.2/xklb/play_actions.py` & `xklb-1.31.3/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/playback.py` & `xklb-1.31.3/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/player.py` & `xklb-1.31.3/xklb/player.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/playlists.py` & `xklb-1.31.3/xklb/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/praw_extract.py` & `xklb-1.31.3/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/search.py` & `xklb-1.31.3/xklb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/subtitle.py` & `xklb-1.31.3/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/tabs_actions.py` & `xklb-1.31.3/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/tabs_extract.py` & `xklb-1.31.3/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/tube_backend.py` & `xklb-1.31.3/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/tube_extract.py` & `xklb-1.31.3/xklb/gdl_extract.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse, sys
 from pathlib import Path
 
-from xklb import consts, db, playlists, tube_backend, usage, utils
+from xklb import consts, db, gdl_backend, media, playlists, usage, utils
 from xklb.consts import SC
 from xklb.utils import log
 
 
 def parse_args(action, usage) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library " + action,
@@ -18,126 +18,88 @@
         "-extractor-config",
         nargs=1,
         action=utils.ArgparseDict,
         default={},
         metavar="KEY=VALUE",
         help="Add key/value pairs to override or extend default downloader configuration",
     )
-    parser.add_argument("--download-archive", default="~/.local/share/yt_archive.txt")
+    parser.add_argument("--download-archive", default="~/.local/share/gallerydl.sqlite3")
     parser.add_argument("--safe", "-safe", action="store_true", help="Skip generic URLs")
     parser.add_argument("--no-sanitize", "-s", action="store_true", help="Don't sanitize some common URL parameters")
-    parser.add_argument("--extra", "-extra", action="store_true", help="Get full metadata (takes a lot longer)")
     parser.add_argument("--playlist-files", action="store_true", help="Read playlists from text files")
     parser.add_argument(
         "--force",
         "-f",
         action="store_true",
         help="Fetch metadata for paths even if they are already in the media table",
     )
-    parser.add_argument("--subs", action="store_true")
-    parser.add_argument("--auto-subs", "--autosubs", action="store_true")
-    parser.add_argument("--subtitle-languages", "--subtitle-language", "--sl", action=utils.ArgparseList)
     parser.add_argument("--extra-media-data", default={}, nargs=1, action=utils.ArgparseDict, metavar="KEY=VALUE")
     parser.add_argument("--extra-playlist-data", default={}, nargs=1, action=utils.ArgparseDict, metavar="KEY=VALUE")
     parser.add_argument("--ignore-errors", "--ignoreerrors", "-i", action="store_true", help=argparse.SUPPRESS)
 
     parser.add_argument("--timeout", "-T", help="Quit after x minutes")
     parser.add_argument("--verbose", "-v", action="count", default=0)
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
 
     parser.add_argument("database")
-    if action == SC.tubeadd:
+    if action == SC.galleryadd:
         parser.add_argument("playlists", nargs="+", help=argparse.SUPPRESS)
 
     args = parser.parse_args()
     args.action = action
 
     if args.db:
         args.database = args.db
-    if action == SC.tubeadd:
+    if action == SC.galleryadd:
         Path(args.database).touch()
     args.db = db.connect(args)
 
     if hasattr(args, "playlists"):
         args.playlists = list(set(s.strip() for s in args.playlists))
         if not args.no_sanitize:
             args.playlists = [utils.sanitize_url(args, p) for p in args.playlists]
         args.playlists = utils.conform(args.playlists)
 
     utils.timeout(args.timeout)
 
-    args.profile = consts.DBType.video
+    args.profile = consts.DBType.image
     log.info(utils.dict_filter_bool(args.__dict__))
     return args
 
 
-def tube_add(args=None) -> None:
+def gallery_add(args=None) -> None:
     if args:
-        sys.argv = ["tubeadd", *args]
+        sys.argv = ["galleryadd", *args]
 
-    args = parse_args(SC.tubeadd, usage=usage.tubeadd)
+    args = parse_args(SC.galleryadd, usage=usage.galleryadd)
     if args.playlist_files:
         args.playlists = list(utils.flatten([Path(p).read_text().splitlines() for p in args.playlists]))
 
-    tables = args.db.table_names()
-    known_playlists = []
-    if "media" in tables and not args.force:
-        m_columns = db.columns(args, "media")
-        known_playlists = list(
-            set(
-                d["path"]
-                for d in args.db.query(
-                    (
-                        "SELECT path from media"
-                        + " WHERE path in ("
-                        + ",".join(["?"] * len(args.playlists))
-                        + f") or {'web' if 'webpath' in m_columns else ''}path in ("
-                        + ",".join(["?"] * len(args.playlists))
-                        + ")"
-                        + " UNION ALL"
-                        + " SELECT path from playlists"
-                    ),
-                    [*args.playlists, *args.playlists],
-                )
-            ),
-        )
+    known_playlists = set()
+    if not args.force:
+        known_playlists = media.get_paths(args)
 
+    added_media_count = 0
     for path in args.playlists:
-        if args.safe and not tube_backend.is_supported(path):
-            log.info("[%s]: Skipping unsupported playlist (safe_mode)", path)
-            continue
-
         if path in known_playlists:
             log.info("[%s]: Already added. Skipping!", path)
             continue
 
-        tube_backend.get_playlist_metadata(args, path, tube_backend.tube_opts(args))
+        if args.safe and not gdl_backend.is_supported(args, path):
+            log.info("[%s]: Skipping unsupported playlist (safe_mode)", path)
+            continue
 
-        if args.extra:
-            log.warning("[%s]: Getting extra metadata", path)
-            tube_backend.get_extra_metadata(args, path)
+        added_media_count += gdl_backend.get_playlist_metadata(args, path)
 
     LARGE_NUMBER = 100_000
-    if not args.db["media"].detect_fts() or tube_backend.added_media_count > LARGE_NUMBER:
+    if not args.db["media"].detect_fts() or added_media_count > LARGE_NUMBER:
         db.optimize(args)
 
 
-def tube_update(args=None) -> None:
+def gallery_update(args=None) -> None:
     if args:
-        sys.argv = ["tubeupdate", *args]
+        sys.argv = ["galleryupdate", *args]
+
+    args = parse_args(SC.galleryupdate, usage=usage.galleryupdate)
 
-    args = parse_args(SC.tubeupdate, usage=usage.tubeupdate)
-    tube_playlists = playlists.get_all(args)
-    for d in tube_playlists:
-        tube_backend.get_playlist_metadata(
-            args,
-            d["path"],
-            tube_backend.tube_opts(
-                args,
-                playlist_opts=d.get("extractor_config", "{}"),
-                func_opts={"ignoreerrors": "only_download"},
-            ),
-        )
-
-        if args.extra:
-            log.warning("[%s]: Getting extra metadata", d["path"])
-            tube_backend.get_extra_metadata(args, d["path"], playlist_dl_opts=d.get("extractor_config", "{}"))
+    for d in playlists.get_all(args):
+        gdl_backend.get_playlist_metadata(args, d["path"])
```

### Comparing `xklb-1.31.2/xklb/usage.py` & `xklb-1.31.3/xklb/usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -786,14 +786,28 @@
         library copy-play-counts audio.db phone.db --source-prefix /storage/6E7B-7DCE/d --target-prefix /mnt/d
 """
 dedupe = """library [--audio | --id | --title | --filesystem] [--only-soft-delete] [--limit LIMIT] DATABASE
 
     Dedupe your files
 """
 
+dedupe_db = """library dedupe-dbs DATABASE TABLE --bk BUSINESS_KEYS [--pk PRIMARY_KEYS] [--only-columns COLUMNS]
+
+    Dedupe your database (not to be confused with the dedupe subcommand)
+
+    It should not need to be said but *backup* your database before trying this tool!
+
+    Dedupe-DB will help remove duplicate rows based on non-primary-key business keys
+
+        library dedupe-db ./video.db media --bk path
+
+    If --primary-keys is not provided table metadata primary keys will be used
+    If --only-columns is not provided all non-primary and non-business key columns will be upserted
+"""
+
 merge_dbs = """library merge-dbs DEST_DB SOURCE_DB ... [--only-target-columns] [--only-new-rows] [--upsert] [--pk PK ...] [--table TABLE ...]
 
     Merge-DBs will insert new rows from source dbs to target db, table by table. If primary key(s) are provided,
     and there is an existing row with the same PK, the default action is to delete the existing row and insert the new row
     replacing all existing fields.
 
     Upsert mode will update matching PK rows such that if a source row has a NULL field and
```

### Comparing `xklb-1.31.2/xklb/utils.py` & `xklb-1.31.3/xklb/utils.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/scripts/bigdirs.py` & `xklb-1.31.3/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/scripts/block.py` & `xklb-1.31.3/xklb/scripts/block.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/scripts/christen.py` & `xklb-1.31.3/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/scripts/cluster_sort.py` & `xklb-1.31.3/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/scripts/copy_play_counts.py` & `xklb-1.31.3/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/scripts/dedupe.py` & `xklb-1.31.3/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/scripts/download_status.py` & `xklb-1.31.3/xklb/scripts/download_status.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/scripts/history.py` & `xklb-1.31.3/xklb/scripts/history.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/scripts/merge_dbs.py` & `xklb-1.31.3/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/scripts/merge_online_local.py` & `xklb-1.31.3/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/scripts/move_list.py` & `xklb-1.31.3/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/scripts/optimize_db.py` & `xklb-1.31.3/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/scripts/playlists.py` & `xklb-1.31.3/xklb/scripts/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/scripts/redownload.py` & `xklb-1.31.3/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/scripts/relmv.py` & `xklb-1.31.3/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/scripts/scatter.py` & `xklb-1.31.3/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/scripts/streaming_tab_loader.py` & `xklb-1.31.3/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/scripts/mining/data.py` & `xklb-1.31.3/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/scripts/mining/extract_links.py` & `xklb-1.31.3/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/scripts/mining/nouns.py` & `xklb-1.31.3/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/scripts/mining/pushshift.py` & `xklb-1.31.3/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.31.3/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/xklb/assets/kotobago.png` & `xklb-1.31.3/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/.gitignore` & `xklb-1.31.3/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/LICENSE` & `xklb-1.31.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/README.md` & `xklb-1.31.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.31.002)
+    xk media library subcommands (v1.31.003)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-1.31.2/pyproject.toml` & `xklb-1.31.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.31.2/PKG-INFO` & `xklb-1.31.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.31.2
+Version: 1.31.3
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -224,15 +224,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.31.002)
+    xk media library subcommands (v1.31.003)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

