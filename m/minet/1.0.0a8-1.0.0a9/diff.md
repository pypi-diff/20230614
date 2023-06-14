# Comparing `tmp/minet-1.0.0a8.tar.gz` & `tmp/minet-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/minet-1.0.0a8.tar", last modified: Fri Mar 10 12:42:06 2023, max compression
+gzip compressed data, was "dist/minet-1.0.0a9.tar", last modified: Mon Mar 13 15:09:19 2023, max compression
```

## Comparing `minet-1.0.0a8.tar` & `minet-1.0.0a9.tar`

### file list

```diff
@@ -1,256 +1,256 @@
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     7589 2023-03-10 12:42:06.000000 minet-1.0.0a8/PKG-INFO
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     6059 2023-03-03 12:40:23.000000 minet-1.0.0a8/README.md
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      116 2023-03-10 11:00:15.000000 minet-1.0.0a8/minet/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       54 2023-03-10 12:41:47.000000 minet-1.0.0a8/minet/__version__.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/buzzsumo/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       52 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/buzzsumo/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     5418 2023-02-28 09:08:39.000000 minet-1.0.0a8/minet/buzzsumo/client.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1070 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/buzzsumo/constants.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      626 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/buzzsumo/exceptions.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      600 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/buzzsumo/formatters.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/cli/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-02-08 10:38:38.000000 minet-1.0.0a8/minet/cli/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      505 2023-02-28 10:46:18.000000 minet-1.0.0a8/minet/cli/__main__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    24537 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/argparse.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/cli/buzzsumo/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     4600 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/buzzsumo/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1083 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/buzzsumo/domain.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1021 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/buzzsumo/domain_summary.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      728 2023-02-21 13:49:04.000000 minet-1.0.0a8/minet/cli/buzzsumo/limit.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      514 2023-02-08 10:38:52.000000 minet-1.0.0a8/minet/cli/buzzsumo/utils.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1443 2023-03-03 12:39:02.000000 minet-1.0.0a8/minet/cli/commands.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2210 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/console.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      306 2023-03-03 16:38:14.000000 minet-1.0.0a8/minet/cli/constants.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/cli/cookies/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1360 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/cookies/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3295 2023-02-10 09:33:16.000000 minet-1.0.0a8/minet/cli/cookies/cookies.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/cli/crawl/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1381 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/crawl/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     8905 2023-03-01 15:58:50.000000 minet-1.0.0a8/minet/cli/crawl/crawl.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/cli/crowdtangle/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    12258 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/crowdtangle/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      747 2023-02-08 10:38:52.000000 minet-1.0.0a8/minet/cli/crowdtangle/leaderboard.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      612 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/crowdtangle/lists.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      486 2023-02-08 10:38:52.000000 minet-1.0.0a8/minet/cli/crowdtangle/posts.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1879 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/crowdtangle/posts_by_id.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      616 2023-02-08 10:38:52.000000 minet-1.0.0a8/minet/cli/crowdtangle/search.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1591 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/crowdtangle/summary.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3556 2023-02-28 09:08:39.000000 minet-1.0.0a8/minet/cli/crowdtangle/utils.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      616 2023-01-24 13:51:52.000000 minet-1.0.0a8/minet/cli/exceptions.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/cli/extract/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     5759 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/extract/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     6598 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/extract/extract.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/cli/facebook/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     8956 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/facebook/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1881 2023-02-22 10:29:26.000000 minet-1.0.0a8/minet/cli/facebook/comments.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1650 2023-02-21 15:26:01.000000 minet-1.0.0a8/minet/cli/facebook/post.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1362 2023-02-22 10:30:43.000000 minet-1.0.0a8/minet/cli/facebook/post_authors.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     7354 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/facebook/post_stats.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1593 2023-02-22 10:31:09.000000 minet-1.0.0a8/minet/cli/facebook/posts.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2498 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/facebook/url_likes.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1456 2023-02-21 15:17:07.000000 minet-1.0.0a8/minet/cli/facebook/utils.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/cli/fetch/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    11216 2023-03-10 11:19:34.000000 minet-1.0.0a8/minet/cli/fetch/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    12288 2023-03-10 12:30:45.000000 minet-1.0.0a8/minet/cli/fetch/fetch.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/cli/google/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2094 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/google/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1799 2023-02-08 10:38:52.000000 minet-1.0.0a8/minet/cli/google/sheets.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/cli/hyphe/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     4830 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/hyphe/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3765 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/hyphe/declare.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      618 2023-02-08 10:38:52.000000 minet-1.0.0a8/minet/cli/hyphe/destroy.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3542 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/hyphe/dump.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      600 2023-02-08 10:38:52.000000 minet-1.0.0a8/minet/cli/hyphe/reset.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3063 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/hyphe/tag.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      375 2023-02-08 10:38:52.000000 minet-1.0.0a8/minet/cli/hyphe/utils.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/cli/instagram/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    11024 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/instagram/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1568 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/instagram/comments.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1589 2023-02-22 10:31:32.000000 minet-1.0.0a8/minet/cli/instagram/hashtag.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1280 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/instagram/post_infos.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2097 2023-02-22 10:31:51.000000 minet-1.0.0a8/minet/cli/instagram/user_followers.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2134 2023-02-22 10:32:08.000000 minet-1.0.0a8/minet/cli/instagram/user_following.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1290 2023-02-22 10:32:26.000000 minet-1.0.0a8/minet/cli/instagram/user_infos.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2098 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/instagram/user_posts.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      762 2023-02-08 10:38:52.000000 minet-1.0.0a8/minet/cli/instagram/utils.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    14036 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/loading_bar.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/cli/mediacloud/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     4310 2023-03-03 12:18:44.000000 minet-1.0.0a8/minet/cli/mediacloud/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1499 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/mediacloud/medias.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1347 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/mediacloud/search.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      972 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/mediacloud/topic.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      351 2023-02-08 10:38:52.000000 minet-1.0.0a8/minet/cli/mediacloud/utils.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     7707 2023-03-10 12:08:44.000000 minet-1.0.0a8/minet/cli/reporters.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     4346 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/run.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/cli/scrape/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     5645 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/scrape/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     9595 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/scrape/scrape.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/cli/telegram/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2039 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/telegram/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1202 2023-02-22 10:33:12.000000 minet-1.0.0a8/minet/cli/telegram/channel_infos.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1385 2023-02-22 10:33:34.000000 minet-1.0.0a8/minet/cli/telegram/channel_messages.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/cli/tiktok/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2299 2023-03-03 12:19:55.000000 minet-1.0.0a8/minet/cli/tiktok/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1100 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/tiktok/search_videos.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/cli/twitter/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    20470 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/twitter/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    10877 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/twitter/attrition.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      410 2023-02-08 10:38:52.000000 minet-1.0.0a8/minet/cli/twitter/followers.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      404 2023-02-08 10:38:52.000000 minet-1.0.0a8/minet/cli/twitter/friends.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2702 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/twitter/list_followers.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2692 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/twitter/list_members.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2593 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/twitter/retweeters.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2805 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/twitter/scrape.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2794 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/twitter/tweet_count.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1439 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/twitter/tweet_date.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2973 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/twitter/tweet_search.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2443 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/twitter/tweets.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2467 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/twitter/user_search.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     6220 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/twitter/user_tweets.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3193 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/twitter/users.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     7171 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/twitter/utils.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/cli/url_extract/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1051 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/url_extract/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1065 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/url_extract/url_extract.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/cli/url_join/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1960 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/url_join/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2170 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/url_join/url_join.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/cli/url_parse/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     9354 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/url_parse/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     5667 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/url_parse/url_parse.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    12019 2023-03-10 12:26:55.000000 minet-1.0.0a8/minet/cli/utils.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/cli/wikipedia/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2589 2023-03-03 13:33:56.000000 minet-1.0.0a8/minet/cli/wikipedia/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1445 2023-03-03 16:17:34.000000 minet-1.0.0a8/minet/cli/wikipedia/pageviews.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/cli/youtube/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     6497 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/cli/youtube/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1023 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/youtube/captions.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1077 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/youtube/channel_videos.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      993 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/youtube/channels.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1804 2023-02-21 13:06:32.000000 minet-1.0.0a8/minet/cli/youtube/comments.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1116 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/youtube/search.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      961 2023-02-21 11:29:32.000000 minet-1.0.0a8/minet/cli/youtube/videos.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1203 2023-03-10 11:19:07.000000 minet-1.0.0a8/minet/constants.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/crawl/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      306 2023-03-03 15:52:20.000000 minet-1.0.0a8/minet/crawl/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    12642 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/crawl/crawler.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3526 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/crawl/queue.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     7353 2023-02-28 10:12:07.000000 minet-1.0.0a8/minet/crawl/spiders.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2669 2023-03-01 10:13:09.000000 minet-1.0.0a8/minet/crawl/state.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3245 2023-02-28 10:24:12.000000 minet-1.0.0a8/minet/crawl/types.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/crowdtangle/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      249 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/crowdtangle/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     4310 2023-02-28 09:08:39.000000 minet-1.0.0a8/minet/crowdtangle/client.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     4129 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/crowdtangle/constants.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1635 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/crowdtangle/exceptions.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     4443 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/crowdtangle/formatters.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      883 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/crowdtangle/leaderboard.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      744 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/crowdtangle/lists.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      821 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/crowdtangle/post.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1053 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/crowdtangle/posts.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1816 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/crowdtangle/search.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2227 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/crowdtangle/summary.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     6300 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/crowdtangle/utils.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     4904 2023-03-03 15:21:18.000000 minet-1.0.0a8/minet/encodings.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2733 2023-03-10 10:12:58.000000 minet-1.0.0a8/minet/exceptions.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/facebook/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      372 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/facebook/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1846 2023-02-13 08:59:23.000000 minet-1.0.0a8/minet/facebook/constants.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      597 2023-02-08 10:38:52.000000 minet-1.0.0a8/minet/facebook/exceptions.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      761 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/facebook/formatters.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    23828 2023-02-28 09:08:39.000000 minet-1.0.0a8/minet/facebook/mobile_scraper.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3377 2023-02-28 09:08:39.000000 minet-1.0.0a8/minet/facebook/post_id_from_url.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1158 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/facebook/utils.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    13519 2023-03-10 12:17:59.000000 minet-1.0.0a8/minet/fetch.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     6321 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/fs.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/google/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      245 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/google/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      727 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/google/exceptions.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2469 2023-02-28 09:08:39.000000 minet-1.0.0a8/minet/google/sheets.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      347 2023-02-28 09:08:39.000000 minet-1.0.0a8/minet/heuristics.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/hyphe/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      230 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/hyphe/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     4653 2023-02-28 09:08:39.000000 minet-1.0.0a8/minet/hyphe/client.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      728 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/hyphe/constants.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      750 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/hyphe/exceptions.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1356 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/hyphe/formatters.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/instagram/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       60 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/instagram/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    15896 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/instagram/api_scraper.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3157 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/instagram/constants.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1234 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/instagram/exceptions.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     9793 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/instagram/formatters.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      736 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/instagram/utils.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      179 2023-02-10 09:33:16.000000 minet-1.0.0a8/minet/loggers.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/mediacloud/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      246 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/mediacloud/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1831 2023-02-22 13:41:54.000000 minet-1.0.0a8/minet/mediacloud/client.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1602 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/mediacloud/constants.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      521 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/mediacloud/exceptions.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2983 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/mediacloud/formatters.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     4102 2023-02-28 09:08:39.000000 minet-1.0.0a8/minet/mediacloud/search.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1798 2023-02-28 09:08:39.000000 minet-1.0.0a8/minet/mediacloud/topic.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1828 2023-02-28 09:08:39.000000 minet-1.0.0a8/minet/mediacloud/utils.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2176 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/multiprocessing.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/scrape/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2349 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/scrape/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     8069 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/scrape/analysis.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     5103 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/scrape/compiler.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1442 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/scrape/constants.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2419 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/scrape/exceptions.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    10995 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/scrape/interpreter.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3084 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/scrape/mixin.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     4287 2023-02-13 08:50:52.000000 minet-1.0.0a8/minet/scrape/std.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2307 2023-02-28 09:08:39.000000 minet-1.0.0a8/minet/scrape/straining.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2485 2023-03-10 12:33:36.000000 minet-1.0.0a8/minet/scrape/typical.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1432 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/scrape/utils.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/telegram/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      238 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/telegram/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      970 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/telegram/constants.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      334 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/telegram/exceptions.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      564 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/telegram/formatters.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    12467 2023-02-28 09:08:39.000000 minet-1.0.0a8/minet/telegram/scraper.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/tiktok/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       54 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/tiktok/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2760 2023-02-28 09:08:39.000000 minet-1.0.0a8/minet/tiktok/api_scraper.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1701 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/tiktok/constants.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      708 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/tiktok/exceptions.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     4319 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/tiktok/formatters.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/twitter/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      110 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/twitter/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1469 2023-02-10 09:33:16.000000 minet-1.0.0a8/minet/twitter/api_client.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    15524 2023-02-28 09:08:39.000000 minet-1.0.0a8/minet/twitter/api_scraper.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      622 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/twitter/constants.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      771 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/twitter/exceptions.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      341 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/types.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     8482 2023-03-03 15:07:59.000000 minet-1.0.0a8/minet/utils.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    37349 2023-03-10 12:30:14.000000 minet-1.0.0a8/minet/web.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/wikipedia/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       77 2023-03-03 11:32:28.000000 minet-1.0.0a8/minet/wikipedia/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      282 2023-03-03 13:31:21.000000 minet-1.0.0a8/minet/wikipedia/exceptions.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      433 2023-03-03 11:44:20.000000 minet-1.0.0a8/minet/wikipedia/types.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3933 2023-03-10 08:58:32.000000 minet-1.0.0a8/minet/wikipedia/wikimedia_rest_api_client.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet/youtube/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      291 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/youtube/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    12872 2023-02-28 09:08:39.000000 minet-1.0.0a8/minet/youtube/client.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2050 2023-01-13 09:08:06.000000 minet-1.0.0a8/minet/youtube/constants.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1281 2023-01-24 09:13:03.000000 minet-1.0.0a8/minet/youtube/exceptions.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     5034 2023-01-18 09:40:29.000000 minet-1.0.0a8/minet/youtube/formatters.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2994 2023-02-22 13:43:18.000000 minet-1.0.0a8/minet/youtube/scrapers.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1295 2022-12-20 13:43:25.000000 minet-1.0.0a8/minet/youtube/utils.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet.egg-info/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     7589 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet.egg-info/PKG-INFO
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     5939 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet.egg-info/SOURCES.txt
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)        1 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet.egg-info/dependency_links.txt
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       51 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet.egg-info/entry_points.txt
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      414 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet.egg-info/requires.txt
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       11 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet.egg-info/top_level.txt
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)        1 2023-03-10 12:42:06.000000 minet-1.0.0a8/minet.egg-info/zip-safe
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       38 2023-03-10 12:42:06.000000 minet-1.0.0a8/setup.cfg
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1735 2023-03-10 09:37:11.000000 minet-1.0.0a8/setup.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/test/
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-03-10 12:42:06.000000 minet-1.0.0a8/test/crowdtangle/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)        0 2022-12-20 13:43:25.000000 minet-1.0.0a8/test/crowdtangle/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1154 2022-12-20 13:43:25.000000 minet-1.0.0a8/test/crowdtangle/utils_test.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/
+-rw-r--r--   0 Yomgui     (501) staff       (20)     7589 2023-03-13 15:09:19.000000 minet-1.0.0a9/PKG-INFO
+-rw-r--r--   0 Yomgui     (501) staff       (20)     6059 2023-03-08 12:24:54.000000 minet-1.0.0a9/README.md
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/
+-rw-r--r--   0 Yomgui     (501) staff       (20)      116 2023-03-11 12:07:39.000000 minet-1.0.0a9/minet/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)       54 2023-03-13 15:08:59.000000 minet-1.0.0a9/minet/__version__.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/buzzsumo/
+-rw-r--r--   0 Yomgui     (501) staff       (20)       52 2021-11-03 18:27:02.000000 minet-1.0.0a9/minet/buzzsumo/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     5418 2023-02-27 16:00:53.000000 minet-1.0.0a9/minet/buzzsumo/client.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1070 2022-05-23 15:01:42.000000 minet-1.0.0a9/minet/buzzsumo/constants.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      626 2021-11-04 16:02:36.000000 minet-1.0.0a9/minet/buzzsumo/exceptions.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      600 2022-05-23 15:01:42.000000 minet-1.0.0a9/minet/buzzsumo/formatters.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/cli/
+-rw-r--r--   0 Yomgui     (501) staff       (20)        0 2023-02-07 15:58:41.000000 minet-1.0.0a9/minet/cli/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      505 2023-03-01 19:11:18.000000 minet-1.0.0a9/minet/cli/__main__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)    24789 2023-03-13 11:50:34.000000 minet-1.0.0a9/minet/cli/argparse.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/cli/buzzsumo/
+-rw-r--r--   0 Yomgui     (501) staff       (20)     4600 2023-03-08 12:24:54.000000 minet-1.0.0a9/minet/cli/buzzsumo/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1083 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/buzzsumo/domain.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1021 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/buzzsumo/domain_summary.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      728 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/buzzsumo/limit.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      514 2023-02-07 16:07:27.000000 minet-1.0.0a9/minet/cli/buzzsumo/utils.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1443 2023-03-08 12:24:54.000000 minet-1.0.0a9/minet/cli/commands.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2210 2023-03-08 12:24:54.000000 minet-1.0.0a9/minet/cli/console.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      306 2022-05-23 15:01:42.000000 minet-1.0.0a9/minet/cli/constants.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/cli/cookies/
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1360 2023-03-08 12:24:54.000000 minet-1.0.0a9/minet/cli/cookies/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     3295 2023-02-20 13:29:59.000000 minet-1.0.0a9/minet/cli/cookies/cookies.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/cli/crawl/
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1381 2023-03-08 12:24:54.000000 minet-1.0.0a9/minet/cli/crawl/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     8923 2023-03-13 12:46:55.000000 minet-1.0.0a9/minet/cli/crawl/crawl.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/cli/crowdtangle/
+-rw-r--r--   0 Yomgui     (501) staff       (20)    12258 2023-03-08 12:24:54.000000 minet-1.0.0a9/minet/cli/crowdtangle/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      747 2023-02-20 16:03:46.000000 minet-1.0.0a9/minet/cli/crowdtangle/leaderboard.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      612 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/crowdtangle/lists.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      486 2023-02-07 16:07:27.000000 minet-1.0.0a9/minet/cli/crowdtangle/posts.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1879 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/crowdtangle/posts_by_id.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      616 2023-02-07 16:07:27.000000 minet-1.0.0a9/minet/cli/crowdtangle/search.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1591 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/crowdtangle/summary.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     3556 2023-02-27 16:00:53.000000 minet-1.0.0a9/minet/cli/crowdtangle/utils.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      616 2023-01-25 09:05:12.000000 minet-1.0.0a9/minet/cli/exceptions.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/cli/extract/
+-rw-r--r--   0 Yomgui     (501) staff       (20)     5759 2023-03-09 10:21:59.000000 minet-1.0.0a9/minet/cli/extract/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     6598 2023-03-09 10:09:15.000000 minet-1.0.0a9/minet/cli/extract/extract.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/cli/facebook/
+-rw-r--r--   0 Yomgui     (501) staff       (20)     8956 2023-03-08 12:24:54.000000 minet-1.0.0a9/minet/cli/facebook/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1881 2023-02-22 19:26:36.000000 minet-1.0.0a9/minet/cli/facebook/comments.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1650 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/facebook/post.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1362 2023-02-22 19:26:36.000000 minet-1.0.0a9/minet/cli/facebook/post_authors.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     7354 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/facebook/post_stats.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1593 2023-02-22 19:26:36.000000 minet-1.0.0a9/minet/cli/facebook/posts.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2498 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/facebook/url_likes.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1456 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/facebook/utils.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/cli/fetch/
+-rw-r--r--   0 Yomgui     (501) staff       (20)    11216 2023-03-11 12:07:39.000000 minet-1.0.0a9/minet/cli/fetch/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)    12737 2023-03-13 14:48:00.000000 minet-1.0.0a9/minet/cli/fetch/fetch.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/cli/google/
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2094 2023-03-08 12:24:54.000000 minet-1.0.0a9/minet/cli/google/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1799 2023-02-07 16:07:27.000000 minet-1.0.0a9/minet/cli/google/sheets.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/cli/hyphe/
+-rw-r--r--   0 Yomgui     (501) staff       (20)     4830 2023-03-08 12:24:54.000000 minet-1.0.0a9/minet/cli/hyphe/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     3765 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/hyphe/declare.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      618 2023-02-07 16:07:27.000000 minet-1.0.0a9/minet/cli/hyphe/destroy.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     3542 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/hyphe/dump.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      600 2023-02-07 16:07:27.000000 minet-1.0.0a9/minet/cli/hyphe/reset.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     3063 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/hyphe/tag.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      375 2023-02-20 20:39:41.000000 minet-1.0.0a9/minet/cli/hyphe/utils.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/cli/instagram/
+-rw-r--r--   0 Yomgui     (501) staff       (20)    11024 2023-03-08 13:01:08.000000 minet-1.0.0a9/minet/cli/instagram/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1568 2023-03-08 13:01:08.000000 minet-1.0.0a9/minet/cli/instagram/comments.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1589 2023-02-22 19:26:36.000000 minet-1.0.0a9/minet/cli/instagram/hashtag.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1280 2023-03-08 13:01:08.000000 minet-1.0.0a9/minet/cli/instagram/post_infos.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2097 2023-02-22 19:26:36.000000 minet-1.0.0a9/minet/cli/instagram/user_followers.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2134 2023-02-22 19:26:36.000000 minet-1.0.0a9/minet/cli/instagram/user_following.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1290 2023-02-22 19:26:36.000000 minet-1.0.0a9/minet/cli/instagram/user_infos.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2098 2023-03-08 13:01:08.000000 minet-1.0.0a9/minet/cli/instagram/user_posts.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      762 2023-02-07 16:07:27.000000 minet-1.0.0a9/minet/cli/instagram/utils.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)    14034 2023-03-13 12:00:27.000000 minet-1.0.0a9/minet/cli/loading_bar.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/cli/mediacloud/
+-rw-r--r--   0 Yomgui     (501) staff       (20)     4310 2023-03-08 12:24:54.000000 minet-1.0.0a9/minet/cli/mediacloud/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1499 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/mediacloud/medias.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1347 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/mediacloud/search.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      972 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/mediacloud/topic.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      351 2023-02-07 16:07:27.000000 minet-1.0.0a9/minet/cli/mediacloud/utils.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     7707 2023-03-11 12:07:39.000000 minet-1.0.0a9/minet/cli/reporters.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     4346 2023-03-08 12:24:54.000000 minet-1.0.0a9/minet/cli/run.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/cli/scrape/
+-rw-r--r--   0 Yomgui     (501) staff       (20)     5645 2023-03-09 15:54:33.000000 minet-1.0.0a9/minet/cli/scrape/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     9595 2023-03-09 15:46:48.000000 minet-1.0.0a9/minet/cli/scrape/scrape.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/cli/telegram/
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2039 2023-03-08 12:24:54.000000 minet-1.0.0a9/minet/cli/telegram/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1202 2023-02-22 19:26:36.000000 minet-1.0.0a9/minet/cli/telegram/channel_infos.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1385 2023-02-22 19:26:36.000000 minet-1.0.0a9/minet/cli/telegram/channel_messages.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/cli/tiktok/
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2299 2023-03-08 12:24:54.000000 minet-1.0.0a9/minet/cli/tiktok/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1100 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/tiktok/search_videos.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/cli/twitter/
+-rw-r--r--   0 Yomgui     (501) staff       (20)    20470 2023-03-09 15:01:34.000000 minet-1.0.0a9/minet/cli/twitter/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)    10877 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/twitter/attrition.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      410 2023-02-07 16:07:27.000000 minet-1.0.0a9/minet/cli/twitter/followers.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      404 2023-02-07 16:07:27.000000 minet-1.0.0a9/minet/cli/twitter/friends.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2702 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/twitter/list_followers.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2692 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/twitter/list_members.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2593 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/twitter/retweeters.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2805 2023-03-09 12:58:34.000000 minet-1.0.0a9/minet/cli/twitter/scrape.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2794 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/twitter/tweet_count.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1439 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/twitter/tweet_date.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2973 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/twitter/tweet_search.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2443 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/twitter/tweets.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2467 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/twitter/user_search.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     6220 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/twitter/user_tweets.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     3193 2023-03-09 12:10:57.000000 minet-1.0.0a9/minet/cli/twitter/users.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     7171 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/twitter/utils.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/cli/url_extract/
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1051 2023-03-08 12:24:54.000000 minet-1.0.0a9/minet/cli/url_extract/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1065 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/url_extract/url_extract.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/cli/url_join/
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1960 2023-03-08 12:24:54.000000 minet-1.0.0a9/minet/cli/url_join/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2170 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/url_join/url_join.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/cli/url_parse/
+-rw-r--r--   0 Yomgui     (501) staff       (20)     9354 2023-03-09 12:52:16.000000 minet-1.0.0a9/minet/cli/url_parse/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     5667 2023-03-09 11:59:46.000000 minet-1.0.0a9/minet/cli/url_parse/url_parse.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)    12086 2023-03-13 11:42:50.000000 minet-1.0.0a9/minet/cli/utils.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/cli/wikipedia/
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2589 2023-03-08 12:24:54.000000 minet-1.0.0a9/minet/cli/wikipedia/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1445 2023-03-08 12:24:54.000000 minet-1.0.0a9/minet/cli/wikipedia/pageviews.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/cli/youtube/
+-rw-r--r--   0 Yomgui     (501) staff       (20)     6497 2023-03-08 12:24:54.000000 minet-1.0.0a9/minet/cli/youtube/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1023 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/youtube/captions.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1077 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/youtube/channel_videos.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      993 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/youtube/channels.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1804 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/youtube/comments.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1116 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/youtube/search.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      961 2023-02-21 19:42:21.000000 minet-1.0.0a9/minet/cli/youtube/videos.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1203 2023-03-11 12:07:39.000000 minet-1.0.0a9/minet/constants.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/crawl/
+-rw-r--r--   0 Yomgui     (501) staff       (20)      306 2023-03-08 12:24:54.000000 minet-1.0.0a9/minet/crawl/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)    12873 2023-03-13 15:04:49.000000 minet-1.0.0a9/minet/crawl/crawler.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     3526 2023-03-08 14:28:22.000000 minet-1.0.0a9/minet/crawl/queue.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     7347 2023-03-13 11:36:56.000000 minet-1.0.0a9/minet/crawl/spiders.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2669 2023-03-01 19:11:18.000000 minet-1.0.0a9/minet/crawl/state.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     3245 2023-03-01 19:11:18.000000 minet-1.0.0a9/minet/crawl/types.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/crowdtangle/
+-rw-r--r--   0 Yomgui     (501) staff       (20)      249 2021-03-08 16:44:20.000000 minet-1.0.0a9/minet/crowdtangle/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     4310 2023-02-27 16:00:53.000000 minet-1.0.0a9/minet/crowdtangle/client.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     4129 2022-09-26 08:39:38.000000 minet-1.0.0a9/minet/crowdtangle/constants.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1635 2022-09-26 09:04:18.000000 minet-1.0.0a9/minet/crowdtangle/exceptions.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     4443 2022-05-23 15:01:42.000000 minet-1.0.0a9/minet/crowdtangle/formatters.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      883 2022-05-23 15:01:42.000000 minet-1.0.0a9/minet/crowdtangle/leaderboard.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      744 2022-05-23 15:01:42.000000 minet-1.0.0a9/minet/crowdtangle/lists.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      821 2022-05-23 15:01:42.000000 minet-1.0.0a9/minet/crowdtangle/post.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1053 2022-05-23 15:01:42.000000 minet-1.0.0a9/minet/crowdtangle/posts.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1816 2022-05-23 15:01:42.000000 minet-1.0.0a9/minet/crowdtangle/search.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2227 2022-05-23 15:01:42.000000 minet-1.0.0a9/minet/crowdtangle/summary.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     6300 2022-09-26 08:39:38.000000 minet-1.0.0a9/minet/crowdtangle/utils.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     4904 2023-03-08 12:24:54.000000 minet-1.0.0a9/minet/encodings.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     3054 2023-03-13 13:37:26.000000 minet-1.0.0a9/minet/exceptions.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)    12644 2023-03-13 13:27:44.000000 minet-1.0.0a9/minet/executors.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/facebook/
+-rw-r--r--   0 Yomgui     (501) staff       (20)      372 2022-05-23 15:01:42.000000 minet-1.0.0a9/minet/facebook/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1846 2023-02-13 19:33:34.000000 minet-1.0.0a9/minet/facebook/constants.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      597 2023-02-07 16:07:27.000000 minet-1.0.0a9/minet/facebook/exceptions.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      761 2022-11-09 09:40:33.000000 minet-1.0.0a9/minet/facebook/formatters.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)    23828 2023-02-27 16:00:53.000000 minet-1.0.0a9/minet/facebook/mobile_scraper.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     3377 2023-02-27 16:00:53.000000 minet-1.0.0a9/minet/facebook/post_id_from_url.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1158 2022-11-09 09:40:33.000000 minet-1.0.0a9/minet/facebook/utils.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     6321 2023-03-09 14:31:08.000000 minet-1.0.0a9/minet/fs.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/google/
+-rw-r--r--   0 Yomgui     (501) staff       (20)      245 2021-03-25 10:02:16.000000 minet-1.0.0a9/minet/google/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      727 2021-03-25 11:55:04.000000 minet-1.0.0a9/minet/google/exceptions.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2469 2023-02-27 16:00:53.000000 minet-1.0.0a9/minet/google/sheets.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      426 2023-03-13 13:10:18.000000 minet-1.0.0a9/minet/heuristics.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/hyphe/
+-rw-r--r--   0 Yomgui     (501) staff       (20)      230 2021-03-06 16:17:01.000000 minet-1.0.0a9/minet/hyphe/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     4653 2023-02-27 16:00:53.000000 minet-1.0.0a9/minet/hyphe/client.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      728 2022-05-23 15:01:42.000000 minet-1.0.0a9/minet/hyphe/constants.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      750 2023-02-06 13:48:20.000000 minet-1.0.0a9/minet/hyphe/exceptions.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1356 2022-05-23 15:01:42.000000 minet-1.0.0a9/minet/hyphe/formatters.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/instagram/
+-rw-r--r--   0 Yomgui     (501) staff       (20)       60 2021-02-27 15:50:34.000000 minet-1.0.0a9/minet/instagram/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)    15896 2023-03-08 13:01:08.000000 minet-1.0.0a9/minet/instagram/api_scraper.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     3157 2023-03-08 13:01:08.000000 minet-1.0.0a9/minet/instagram/constants.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1234 2023-01-12 10:08:18.000000 minet-1.0.0a9/minet/instagram/exceptions.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     9793 2023-03-08 13:01:08.000000 minet-1.0.0a9/minet/instagram/formatters.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      736 2023-03-08 13:01:08.000000 minet-1.0.0a9/minet/instagram/utils.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      179 2023-02-09 15:07:48.000000 minet-1.0.0a9/minet/loggers.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/mediacloud/
+-rw-r--r--   0 Yomgui     (501) staff       (20)      246 2021-03-15 20:07:35.000000 minet-1.0.0a9/minet/mediacloud/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1831 2023-02-22 19:26:36.000000 minet-1.0.0a9/minet/mediacloud/client.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1602 2022-05-23 15:01:42.000000 minet-1.0.0a9/minet/mediacloud/constants.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      521 2020-05-07 13:29:37.000000 minet-1.0.0a9/minet/mediacloud/exceptions.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2983 2022-05-23 15:01:42.000000 minet-1.0.0a9/minet/mediacloud/formatters.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     4102 2023-02-27 16:29:38.000000 minet-1.0.0a9/minet/mediacloud/search.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1798 2023-02-27 16:29:10.000000 minet-1.0.0a9/minet/mediacloud/topic.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1828 2023-02-27 16:00:53.000000 minet-1.0.0a9/minet/mediacloud/utils.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2176 2023-03-08 12:24:54.000000 minet-1.0.0a9/minet/multiprocessing.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/scrape/
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2349 2023-03-09 15:30:00.000000 minet-1.0.0a9/minet/scrape/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     8069 2023-03-09 13:25:48.000000 minet-1.0.0a9/minet/scrape/analysis.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     5103 2022-05-23 15:01:42.000000 minet-1.0.0a9/minet/scrape/compiler.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1442 2022-05-23 15:01:42.000000 minet-1.0.0a9/minet/scrape/constants.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2419 2021-10-20 19:53:49.000000 minet-1.0.0a9/minet/scrape/exceptions.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)    10995 2023-03-09 13:28:12.000000 minet-1.0.0a9/minet/scrape/interpreter.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     3084 2023-03-09 15:29:50.000000 minet-1.0.0a9/minet/scrape/mixin.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     4287 2023-02-13 19:33:34.000000 minet-1.0.0a9/minet/scrape/std.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2307 2023-02-27 16:00:53.000000 minet-1.0.0a9/minet/scrape/straining.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2485 2023-03-11 12:07:39.000000 minet-1.0.0a9/minet/scrape/typical.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1432 2023-03-09 15:29:39.000000 minet-1.0.0a9/minet/scrape/utils.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/telegram/
+-rw-r--r--   0 Yomgui     (501) staff       (20)      238 2022-11-21 14:34:18.000000 minet-1.0.0a9/minet/telegram/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      970 2022-11-21 14:34:18.000000 minet-1.0.0a9/minet/telegram/constants.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      334 2022-11-21 14:34:18.000000 minet-1.0.0a9/minet/telegram/exceptions.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      564 2022-11-21 14:34:18.000000 minet-1.0.0a9/minet/telegram/formatters.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)    12467 2023-02-27 16:00:53.000000 minet-1.0.0a9/minet/telegram/scraper.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/tiktok/
+-rw-r--r--   0 Yomgui     (501) staff       (20)       54 2022-11-24 08:52:04.000000 minet-1.0.0a9/minet/tiktok/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2760 2023-02-27 16:00:53.000000 minet-1.0.0a9/minet/tiktok/api_scraper.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1701 2023-01-12 10:08:18.000000 minet-1.0.0a9/minet/tiktok/constants.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      708 2022-11-24 08:52:04.000000 minet-1.0.0a9/minet/tiktok/exceptions.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     4319 2023-01-12 10:08:18.000000 minet-1.0.0a9/minet/tiktok/formatters.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/twitter/
+-rw-r--r--   0 Yomgui     (501) staff       (20)      110 2021-06-28 17:15:19.000000 minet-1.0.0a9/minet/twitter/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1469 2023-02-09 16:00:21.000000 minet-1.0.0a9/minet/twitter/api_client.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)    15524 2023-03-08 15:34:07.000000 minet-1.0.0a9/minet/twitter/api_scraper.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      622 2022-05-23 15:01:42.000000 minet-1.0.0a9/minet/twitter/constants.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      771 2021-08-26 08:16:15.000000 minet-1.0.0a9/minet/twitter/exceptions.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      503 2023-03-13 11:37:21.000000 minet-1.0.0a9/minet/types.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     8482 2023-03-08 12:24:54.000000 minet-1.0.0a9/minet/utils.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)    38050 2023-03-13 14:46:33.000000 minet-1.0.0a9/minet/web.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/wikipedia/
+-rw-r--r--   0 Yomgui     (501) staff       (20)       77 2023-03-08 12:24:54.000000 minet-1.0.0a9/minet/wikipedia/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      282 2023-03-08 12:24:54.000000 minet-1.0.0a9/minet/wikipedia/exceptions.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      433 2023-03-08 12:24:54.000000 minet-1.0.0a9/minet/wikipedia/types.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     3928 2023-03-13 12:42:43.000000 minet-1.0.0a9/minet/wikipedia/wikimedia_rest_api_client.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet/youtube/
+-rw-r--r--   0 Yomgui     (501) staff       (20)      291 2021-03-15 19:51:40.000000 minet-1.0.0a9/minet/youtube/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)    12872 2023-02-27 16:00:53.000000 minet-1.0.0a9/minet/youtube/client.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2050 2023-01-12 10:08:18.000000 minet-1.0.0a9/minet/youtube/constants.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1281 2023-01-23 16:01:01.000000 minet-1.0.0a9/minet/youtube/exceptions.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     5034 2023-01-23 13:21:38.000000 minet-1.0.0a9/minet/youtube/formatters.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2994 2023-02-22 19:26:36.000000 minet-1.0.0a9/minet/youtube/scrapers.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1295 2022-05-23 15:01:42.000000 minet-1.0.0a9/minet/youtube/utils.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet.egg-info/
+-rw-r--r--   0 Yomgui     (501) staff       (20)     7589 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet.egg-info/PKG-INFO
+-rw-r--r--   0 Yomgui     (501) staff       (20)     5943 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet.egg-info/SOURCES.txt
+-rw-r--r--   0 Yomgui     (501) staff       (20)        1 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet.egg-info/dependency_links.txt
+-rw-r--r--   0 Yomgui     (501) staff       (20)       51 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet.egg-info/entry_points.txt
+-rw-r--r--   0 Yomgui     (501) staff       (20)      414 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet.egg-info/requires.txt
+-rw-r--r--   0 Yomgui     (501) staff       (20)       11 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet.egg-info/top_level.txt
+-rw-r--r--   0 Yomgui     (501) staff       (20)        1 2023-03-13 15:09:19.000000 minet-1.0.0a9/minet.egg-info/zip-safe
+-rw-r--r--   0 Yomgui     (501) staff       (20)       38 2023-03-13 15:09:19.000000 minet-1.0.0a9/setup.cfg
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1735 2023-03-13 11:43:44.000000 minet-1.0.0a9/setup.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/test/
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-13 15:09:19.000000 minet-1.0.0a9/test/crowdtangle/
+-rw-r--r--   0 Yomgui     (501) staff       (20)        0 2020-10-27 19:52:31.000000 minet-1.0.0a9/test/crowdtangle/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1154 2022-05-23 15:01:42.000000 minet-1.0.0a9/test/crowdtangle/utils_test.py
```

### Comparing `minet-1.0.0a8/PKG-INFO` & `minet-1.0.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minet
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: A webmining CLI tool & library for python.
 Home-page: http://github.com/medialab/minet
 Author: Guillaume Plique, Pauline Breteau, Jules Farjas, Héloïse Théro, Jean Descamps, Amélie Pellé, Laura Miguel
 License: MIT
 Description: [![Build Status](https://github.com/medialab/minet/workflows/Tests/badge.svg)](https://github.com/medialab/minet/actions) [![DOI](https://zenodo.org/badge/169059797.svg)](https://zenodo.org/badge/latestdoi/169059797) [![download number](https://static.pepy.tech/badge/minet)](https://pepy.tech/project/minet)
         
         ![Minet](docs/img/minet.png)
```

### Comparing `minet-1.0.0a8/README.md` & `minet-1.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/buzzsumo/client.py` & `minet-1.0.0a9/minet/buzzsumo/client.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/buzzsumo/constants.py` & `minet-1.0.0a9/minet/buzzsumo/constants.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/buzzsumo/exceptions.py` & `minet-1.0.0a9/minet/buzzsumo/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/buzzsumo/formatters.py` & `minet-1.0.0a9/minet/buzzsumo/formatters.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/argparse.py` & `minet-1.0.0a9/minet/cli/argparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # =============================================================================
 # Minet Argparse Helpers
 # =============================================================================
 #
 # Miscellaneous helpers related to CLI argument parsing.
 #
 from typing import Optional
-from typing_extensions import TypedDict, NotRequired
+from minet.types import TypedDict, NotRequired
 
 import os
 import re
 import sys
 import shutil
 from os.path import isdir
 from io import TextIOBase
@@ -549,14 +549,15 @@
     input_help: NotRequired[str]
     no_help: NotRequired[bool]
     optional: NotRequired[bool]
     metavar: NotRequired[str]
 
 
 def resolve_typical_arguments(
+    package: str,
     args,
     no_output=False,
     resumer=None,
     resumer_kwargs=None,
     select: bool = False,
     total: bool = False,
     variadic_input: Optional[VariadicInputDefinition] = None,
@@ -622,37 +623,43 @@
             {
                 "flags": ["--explode"],
                 "help": "Use to indicate the character used to separate multiple values in a single CSV cell. Defaults to none, i.e. CSV cells having a single values, which is usually the case.",
             }
         )
 
         if not variadic_input.get("no_help", False):
+            split = package.split(".")
+            name = split[0]
+            cmd = split[-1].replace("_", "-")
+
             epilog_addendum = """
         how to use the command with a CSV file?
 
-        > A lot of minet commands, including this one, can both be
+        > A lot of {name} commands, including this one, can both be
         > given a single value to process or a bunch of them if
         > given the column of a CSV file passed to -i/--input instead.
 
         . Here is how to use a command with a single value:
-            $ minet cmd "value"
+            $ {name} {cmd} "value"
 
         . Here is how to use a command with a csv file:
-            $ minet cmd column_name -i file.csv
+            $ {name} {cmd} column_name -i file.csv
 
         . Here is how to read CSV file from stdin using `-`:
-            $ xsv search -s col . | minet cmd column_name -i -
+            $ xsv search -s col . | {name} {cmd} column_name -i -
 
         . Here is how to indicate that the CSV column may contain multiple
           values separated by a special character:
-            $ minet cmd column_name -i file.csv --explode "|"
+            $ {name} {cmd} column_name -i file.csv --explode "|"
 
         . This also works with single values:
-            $ minet cmd "value1,value2" --explode ","
-        """
+            $ {name} {cmd} "value1,value2" --explode ","
+        """.format(
+                name=name, cmd=cmd
+            )
 
     if select or variadic_input is not None:
 
         # TODO: actually one can use xsv mini dsl here
         args.append(
             {
                 "flags": ["-s", "--select"],
@@ -687,15 +694,15 @@
         args.append(output_argument)
 
     return args, epilog_addendum
 
 
 def command(
     name: str,
-    package=None,
+    package: str,
     title: Optional[str] = None,
     aliases=None,
     description=None,
     epilog=None,
     common_arguments=None,
     arguments=None,
     subcommands=None,
@@ -740,14 +747,15 @@
         }
 
         if common_arguments is not None:
             data["subparsers"]["common_arguments"] = common_arguments
 
     elif arguments is not None:
         data["arguments"], epilog_addendum = resolve_typical_arguments(
+            package,
             arguments,
             no_output=no_output,
             resumer=resumer,
             resumer_kwargs=resumer_kwargs,
             select=select,
             total=total,
             variadic_input=variadic_input,
@@ -764,17 +772,17 @@
 
     data.update(kwargs)
 
     return data
 
 
 def subcommand(
-    name,
-    package,
-    title,
+    name: str,
+    package: str,
+    title: str,
     description=None,
     epilog=None,
     arguments=[],
     resolve=None,
     resumer=None,
     resumer_kwargs=None,
     no_output=False,
@@ -788,14 +796,15 @@
     if description is not None:
         data["description"] = description
 
     if epilog is not None:
         data["epilog"] = epilog
 
     data["arguments"], epilog_addendum = resolve_typical_arguments(
+        package,
         arguments,
         no_output=no_output,
         resumer=resumer,
         resumer_kwargs=resumer_kwargs,
         select=select,
         total=total,
         variadic_input=variadic_input,
```

### Comparing `minet-1.0.0a8/minet/cli/buzzsumo/__init__.py` & `minet-1.0.0a9/minet/cli/buzzsumo/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/buzzsumo/domain.py` & `minet-1.0.0a9/minet/cli/buzzsumo/domain.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/buzzsumo/domain_summary.py` & `minet-1.0.0a9/minet/cli/buzzsumo/domain_summary.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/buzzsumo/limit.py` & `minet-1.0.0a9/minet/cli/buzzsumo/limit.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/buzzsumo/utils.py` & `minet-1.0.0a9/minet/cli/buzzsumo/utils.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/commands.py` & `minet-1.0.0a9/minet/cli/commands.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/console.py` & `minet-1.0.0a9/minet/cli/console.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/cookies/__init__.py` & `minet-1.0.0a9/minet/cli/cookies/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/cookies/cookies.py` & `minet-1.0.0a9/minet/cli/cookies/cookies.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/crawl/__init__.py` & `minet-1.0.0a9/minet/cli/crawl/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/crawl/crawl.py` & `minet-1.0.0a9/minet/cli/crawl/crawl.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,20 +88,20 @@
         writer.writerow(headers)
 
     return f, writer
 
 
 class ScraperReporter(object):
     def __init__(self, path: str, scraper: Scraper, resume=False):
-        if scraper.headers is None:
-            raise NotImplementedError("Scraper headers could not be inferred.")
+        if scraper.fieldnames is None:
+            raise NotImplementedError("Scraper fieldnames could not be inferred.")
 
-        f, writer = open_report(path, scraper.headers, resume)
+        f, writer = open_report(path, scraper.fieldnames, resume)
 
-        self.headers = scraper.headers
+        self.fieldnames = scraper.fieldnames
         self.file = f
         self.writer = writer
 
     def write(self, items) -> int:
         count = 0
 
         # TODO: maybe abstract this once step above
@@ -111,15 +111,15 @@
         for item in items:
             count += 1
 
             if not isinstance(item, dict):
                 self.writer.writerow([item])
                 continue
 
-            row = [item.get(k, "") for k in self.headers]
+            row = [item.get(k, "") for k in self.fieldnames]
             self.writer.writerow(row)
 
         return count
 
     def flush(self):
         self.file.flush()
```

### Comparing `minet-1.0.0a8/minet/cli/crowdtangle/__init__.py` & `minet-1.0.0a9/minet/cli/crowdtangle/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/crowdtangle/leaderboard.py` & `minet-1.0.0a9/minet/cli/crowdtangle/leaderboard.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/crowdtangle/lists.py` & `minet-1.0.0a9/minet/cli/crowdtangle/lists.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/crowdtangle/posts_by_id.py` & `minet-1.0.0a9/minet/cli/crowdtangle/posts_by_id.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/crowdtangle/search.py` & `minet-1.0.0a9/minet/cli/crowdtangle/search.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/crowdtangle/summary.py` & `minet-1.0.0a9/minet/cli/crowdtangle/summary.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/crowdtangle/utils.py` & `minet-1.0.0a9/minet/cli/crowdtangle/utils.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/exceptions.py` & `minet-1.0.0a9/minet/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/extract/__init__.py` & `minet-1.0.0a9/minet/cli/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/extract/extract.py` & `minet-1.0.0a9/minet/cli/extract/extract.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/facebook/__init__.py` & `minet-1.0.0a9/minet/cli/facebook/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/facebook/comments.py` & `minet-1.0.0a9/minet/cli/facebook/comments.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/facebook/post.py` & `minet-1.0.0a9/minet/cli/facebook/post.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/facebook/post_authors.py` & `minet-1.0.0a9/minet/cli/facebook/post_authors.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/facebook/post_stats.py` & `minet-1.0.0a9/minet/cli/facebook/post_stats.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/facebook/posts.py` & `minet-1.0.0a9/minet/cli/facebook/posts.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/facebook/url_likes.py` & `minet-1.0.0a9/minet/cli/facebook/url_likes.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/facebook/utils.py` & `minet-1.0.0a9/minet/cli/facebook/utils.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/fetch/__init__.py` & `minet-1.0.0a9/minet/cli/fetch/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/fetch/fetch.py` & `minet-1.0.0a9/minet/cli/fetch/fetch.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,62 +2,64 @@
 # Minet Fetch CLI Action
 # =============================================================================
 #
 # Action reading an input CSV file line by line and fetching the urls found
 # in the given column. This is done in a respectful multithreaded fashion to
 # optimize both running time & memory.
 #
-from typing import Optional, List, Union
+from typing import Optional, List, Union, Tuple
 
 import casanova
 from casanova import TabularRecord
 from dataclasses import dataclass
 from datetime import datetime
 from ural import is_shortened_url, could_be_html
 
-from minet.fetch import (
-    FetchResult,
-    FetchWorkerPayload,
-    FetchThreadPoolExecutor,
-    ResolveThreadPoolExecutor,
-)
+from minet.executors import RequestResult, HTTPWorkerPayload, HTTPThreadPoolExecutor
 from minet.fs import FilenameBuilder, ThreadSafeFilesWriter
 from minet.web import grab_cookies, parse_http_header, Response, RedirectionStack
-from minet.exceptions import InvalidURLError, FilenameFormattingError
+from minet.exceptions import InvalidURLError, FilenameFormattingError, HTTPCallbackError
+from minet.heuristics import should_spoof_ua_when_resolving
 from minet.cli.exceptions import InvalidArgumentsError, FatalError
 from minet.cli.reporters import report_error, report_filename_formatting_error
 from minet.cli.utils import with_enricher_and_loading_bar, with_ctrl_c_warning
 
 
 @dataclass
+class WorkerAddendum:
+    filename: Optional[str] = None
+    decoded_contents: Optional[str] = None
+
+
+@dataclass
 class FetchAddendum(TabularRecord):
     resolved_url: Optional[str] = None
     http_status: Optional[int] = None
     datetime_utc: Optional[datetime] = None
     fetch_error: Optional[str] = None
     filename: Optional[str] = None
     mimetype: Optional[str] = None
     encoding: Optional[str] = None
 
-    def infos_from_response(self, response: Response) -> None:
+    def infos_from_response(self, response: Response, addendum: WorkerAddendum) -> None:
         self.resolved_url = response.end_url
         self.http_status = response.status
         self.datetime_utc = response.end_datetime
-        self.filename = response.get("filename")
+        self.filename = addendum.filename
         self.encoding = response.encoding
         self.mimetype = response.mimetype
 
 
 @dataclass
 class FetchAddendumWithBody(FetchAddendum):
     body: Optional[str] = None
 
-    def infos_from_response(self, response: Response) -> None:
-        super().infos_from_response(response)
-        self.body = response.get("decoded_contents")
+    def infos_from_response(self, response: Response, addendum: WorkerAddendum) -> None:
+        super().infos_from_response(response, addendum)
+        self.body = addendum.decoded_contents
 
 
 @dataclass
 class ResolveAddendum(TabularRecord):
     resolved_url: Optional[str] = None
     http_status: Optional[int] = None
     resolution_error: Optional[str] = None
@@ -177,28 +179,33 @@
 
         # Url templating
         if cli_args.url_template:
             return cli_args.url_template.format(value=url)
 
         return url
 
-    def request_args(payload: FetchWorkerPayload):
+    def request_args(payload: HTTPWorkerPayload):
         cookie = None
 
         # Cookie
         if get_cookie:
             cookie = get_cookie(payload.url)
 
         # Headers
         headers = None
 
         if global_headers:
             headers = global_headers
 
-        return {"method": http_method, "cookie": cookie, "headers": headers}
+        return {
+            "method": http_method,
+            "cookie": cookie,
+            "headers": headers,
+            "spoof_ua": resolve and should_spoof_ua_when_resolving(payload.domain),
+        }
 
     # Worker callback internals
     filename_builder = None
     files_writer = None
 
     if not resolve:
         try:
@@ -213,15 +220,17 @@
                     "Check the list at the end of the command help:",
                     "  $ minet fetch -h",
                 ]
             )
 
         files_writer = ThreadSafeFilesWriter(cli_args.output_dir)
 
-    def worker_callback(result: FetchResult[List]) -> None:
+    def worker_callback(
+        result: RequestResult[Tuple[int, List[str]], None]
+    ) -> Optional[WorkerAddendum]:
         if cli_args.dont_save:
             return
 
         # NOTE: at this point the callback is only fired on success
         assert result.response
 
         row = result.item[1]
@@ -229,56 +238,56 @@
 
         if cli_args.keep_failed_contents and response.status != 200:
             return
 
         if cli_args.only_html and not response.is_html:
             return
 
+        addendum = WorkerAddendum()
+
         # First we need to build a filename
         filename_cell = row[filename_pos] if filename_pos is not None else None
 
         formatter_kwargs = {}
 
         if cli_args.filename_template and "row" in cli_args.filename_template:
             formatter_kwargs["row"] = enricher.wrap(row)
 
-        try:
-            assert filename_builder is not None
+        assert filename_builder is not None
 
-            filename = filename_builder(
-                response.end_url,
-                filename=filename_cell,
-                ext=response.ext,
-                formatter_kwargs=formatter_kwargs,
-                compressed=cli_args.compress,
-            )
-        except FilenameFormattingError as e:
-            result.error = e
-            return
+        filename = filename_builder(
+            response.end_url,
+            filename=filename_cell,
+            ext=response.ext,
+            formatter_kwargs=formatter_kwargs,
+            compressed=cli_args.compress,
+        )
 
-        response["filename"] = filename
+        addendum.filename = filename
 
         # Decoding the response data?
         data: Union[str, bytes] = response.body
 
         if response.is_text and (
             cli_args.standardize_encoding or cli_args.contents_in_report
         ):
             data = response.body.decode(response.likely_encoding, errors="replace")
 
             if cli_args.contents_in_report:
-                response["decoded_contents"] = data
+                addendum.decoded_contents = data
 
         # Writing the file?
         # TODO: specify what should happen when contents are empty (e.g. POST queries)
         if data and not cli_args.contents_in_report:
             assert files_writer is not None
 
             files_writer.write(filename, data, compress=cli_args.compress)
 
+        return addendum
+
     common_executor_kwargs = {
         "insecure": cli_args.insecure,
         "max_workers": cli_args.threads,
         "wait": False,
         "daemonic": False,
     }
     common_imap_kwargs = {
@@ -294,16 +303,16 @@
     # Normal fetch
     if not resolve:
 
         Addendum = (
             FetchAddendum if not cli_args.contents_in_report else FetchAddendumWithBody
         )
 
-        with FetchThreadPoolExecutor(**common_executor_kwargs) as executor:
-            for result in executor.imap_unordered(
+        with HTTPThreadPoolExecutor(**common_executor_kwargs) as executor:
+            for result in executor.request(
                 enricher,
                 request_args=request_args,
                 callback=worker_callback,
                 **common_imap_kwargs
             ):
                 with loading_bar.step():
                     index, row = result.item
@@ -314,49 +323,53 @@
                         continue
 
                     addendum = Addendum()
 
                     # No error
                     if result.error is None:
                         assert result.response is not None
+                        assert result.addendum is not None
 
                         response = result.response
                         status = response.status
 
                         loading_bar.inc_stat(status, style=get_style_for_status(status))
 
-                        addendum.infos_from_response(response)
+                        addendum.infos_from_response(response, result.addendum)
                         enricher.writerow(index, row, addendum)
 
                     # Handling potential errors
                     else:
-                        error_code = report_error(result.error)
+                        error = result.error
+
+                        if isinstance(error, HTTPCallbackError):
+                            error.unwrap(FilenameFormattingError)
+
+                        error_code = report_error(error)
 
                         loading_bar.inc_stat(error_code, style="error")
 
                         resolved_url = None
 
-                        if isinstance(result.error, InvalidURLError):
-                            resolved_url = result.error.url
+                        if isinstance(error, InvalidURLError):
+                            resolved_url = error.url
 
-                        if isinstance(result.error, FilenameFormattingError):
-                            loading_bar.print(
-                                report_filename_formatting_error(result.error)
-                            )
+                        if isinstance(error, FilenameFormattingError):
+                            loading_bar.print(report_filename_formatting_error(error))
 
                         addendum.fetch_error = error_code
                         addendum.resolved_url = resolved_url
 
                         enricher.writerow(index, row, addendum)
 
     # Resolve
     else:
 
-        with ResolveThreadPoolExecutor(**common_executor_kwargs) as executor:
-            for result in executor.imap_unordered(
+        with HTTPThreadPoolExecutor(**common_executor_kwargs) as executor:
+            for result in executor.resolve(
                 enricher,
                 resolve_args=request_args,
                 follow_meta_refresh=cli_args.follow_meta_refresh,
                 follow_js_relocation=cli_args.follow_js_relocation,
                 infer_redirection=cli_args.infer_redirection,
                 canonicalize=cli_args.canonicalize,
                 **common_imap_kwargs
```

### Comparing `minet-1.0.0a8/minet/cli/google/__init__.py` & `minet-1.0.0a9/minet/cli/google/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/google/sheets.py` & `minet-1.0.0a9/minet/cli/google/sheets.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/hyphe/__init__.py` & `minet-1.0.0a9/minet/cli/hyphe/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/hyphe/declare.py` & `minet-1.0.0a9/minet/cli/hyphe/declare.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/hyphe/destroy.py` & `minet-1.0.0a9/minet/cli/hyphe/destroy.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/hyphe/dump.py` & `minet-1.0.0a9/minet/cli/hyphe/dump.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/hyphe/reset.py` & `minet-1.0.0a9/minet/cli/hyphe/reset.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/hyphe/tag.py` & `minet-1.0.0a9/minet/cli/hyphe/tag.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/instagram/__init__.py` & `minet-1.0.0a9/minet/cli/instagram/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/instagram/comments.py` & `minet-1.0.0a9/minet/cli/instagram/comments.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/instagram/hashtag.py` & `minet-1.0.0a9/minet/cli/instagram/hashtag.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/instagram/post_infos.py` & `minet-1.0.0a9/minet/cli/instagram/post_infos.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/instagram/user_followers.py` & `minet-1.0.0a9/minet/cli/instagram/user_followers.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/instagram/user_following.py` & `minet-1.0.0a9/minet/cli/instagram/user_following.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/instagram/user_infos.py` & `minet-1.0.0a9/minet/cli/instagram/user_infos.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/instagram/user_posts.py` & `minet-1.0.0a9/minet/cli/instagram/user_posts.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/instagram/utils.py` & `minet-1.0.0a9/minet/cli/instagram/utils.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/loading_bar.py` & `minet-1.0.0a9/minet/cli/loading_bar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # =============================================================================
 # Minet Loading Bars
 # =============================================================================
 #
 # Various loading bar utilities used by minet CLI.
 #
 from typing import Optional, Iterable
-from typing_extensions import TypedDict, NotRequired
+from minet.types import TypedDict, NotRequired
 
 from contextlib import contextmanager
 from collections import OrderedDict, namedtuple
 from rich.live import Live
 from rich.text import Text
 from rich.table import Table, Column
 from rich.progress import (
@@ -400,15 +400,15 @@
             if not interrupted:
                 self.nested_advance(count)
 
     def advance(self, count=1):
         self.progress.update(self.task_id, advance=count)
 
     def nested_advance(self, count=1):
-        self.sub_total_sum += 1
+        self.sub_total_sum += count
         self.sub_progress.update(
             self.sub_task_id, advance=count, sub_total_sum=self.sub_total_sum
         )
 
     def nested_reset(self):
         self.sub_progress.reset(self.sub_task_id)
```

### Comparing `minet-1.0.0a8/minet/cli/mediacloud/__init__.py` & `minet-1.0.0a9/minet/cli/mediacloud/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/mediacloud/medias.py` & `minet-1.0.0a9/minet/cli/mediacloud/medias.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/mediacloud/search.py` & `minet-1.0.0a9/minet/cli/mediacloud/search.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/mediacloud/topic.py` & `minet-1.0.0a9/minet/cli/mediacloud/topic.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/reporters.py` & `minet-1.0.0a9/minet/cli/reporters.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/run.py` & `minet-1.0.0a9/minet/cli/run.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/scrape/__init__.py` & `minet-1.0.0a9/minet/cli/scrape/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/scrape/scrape.py` & `minet-1.0.0a9/minet/cli/scrape/scrape.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/telegram/__init__.py` & `minet-1.0.0a9/minet/cli/telegram/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/telegram/channel_infos.py` & `minet-1.0.0a9/minet/cli/telegram/channel_infos.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/telegram/channel_messages.py` & `minet-1.0.0a9/minet/cli/telegram/channel_messages.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/tiktok/__init__.py` & `minet-1.0.0a9/minet/cli/tiktok/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/tiktok/search_videos.py` & `minet-1.0.0a9/minet/cli/tiktok/search_videos.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/twitter/__init__.py` & `minet-1.0.0a9/minet/cli/twitter/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/twitter/attrition.py` & `minet-1.0.0a9/minet/cli/twitter/attrition.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/twitter/list_followers.py` & `minet-1.0.0a9/minet/cli/twitter/list_followers.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/twitter/list_members.py` & `minet-1.0.0a9/minet/cli/twitter/list_members.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/twitter/retweeters.py` & `minet-1.0.0a9/minet/cli/twitter/retweeters.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/twitter/scrape.py` & `minet-1.0.0a9/minet/cli/twitter/scrape.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/twitter/tweet_count.py` & `minet-1.0.0a9/minet/cli/twitter/tweet_count.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/twitter/tweet_date.py` & `minet-1.0.0a9/minet/cli/twitter/tweet_date.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/twitter/tweet_search.py` & `minet-1.0.0a9/minet/cli/twitter/tweet_search.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/twitter/tweets.py` & `minet-1.0.0a9/minet/cli/twitter/tweets.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/twitter/user_search.py` & `minet-1.0.0a9/minet/cli/twitter/user_search.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/twitter/user_tweets.py` & `minet-1.0.0a9/minet/cli/twitter/user_tweets.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/twitter/users.py` & `minet-1.0.0a9/minet/cli/twitter/users.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/twitter/utils.py` & `minet-1.0.0a9/minet/cli/twitter/utils.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/url_extract/__init__.py` & `minet-1.0.0a9/minet/cli/url_extract/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/url_extract/url_extract.py` & `minet-1.0.0a9/minet/cli/url_extract/url_extract.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/url_join/__init__.py` & `minet-1.0.0a9/minet/cli/url_join/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/url_join/url_join.py` & `minet-1.0.0a9/minet/cli/url_join/url_join.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/url_parse/__init__.py` & `minet-1.0.0a9/minet/cli/url_parse/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/url_parse/url_parse.py` & `minet-1.0.0a9/minet/cli/url_parse/url_parse.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/utils.py` & `minet-1.0.0a9/minet/cli/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,16 @@
             exc = record.exception
             pretty_time = format_seconds(record.sleep_time)
 
             exc_name = "%s.%s" % (exc.__class__.__module__, exc.__class__.__name__)
             exc_msg = str(exc)
 
             msg = [
-                "Will now wait for %s because of following exception:" % pretty_time,
+                "%s now wait for %s because of following exception:"
+                % ("A thread will" if record.from_thread else "Will", pretty_time),
                 exc_name,
             ]
 
             if exc_msg:
                 msg.append("Exception message: %s" % exc_msg)
 
             if record.epilog:
```

### Comparing `minet-1.0.0a8/minet/cli/wikipedia/__init__.py` & `minet-1.0.0a9/minet/cli/wikipedia/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/wikipedia/pageviews.py` & `minet-1.0.0a9/minet/cli/wikipedia/pageviews.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/youtube/__init__.py` & `minet-1.0.0a9/minet/cli/youtube/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/youtube/captions.py` & `minet-1.0.0a9/minet/cli/youtube/captions.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/youtube/channel_videos.py` & `minet-1.0.0a9/minet/cli/youtube/channel_videos.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/youtube/channels.py` & `minet-1.0.0a9/minet/cli/youtube/channels.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/youtube/comments.py` & `minet-1.0.0a9/minet/cli/youtube/comments.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/youtube/search.py` & `minet-1.0.0a9/minet/cli/youtube/search.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/cli/youtube/videos.py` & `minet-1.0.0a9/minet/cli/youtube/videos.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/constants.py` & `minet-1.0.0a9/minet/constants.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/crawl/crawler.py` & `minet-1.0.0a9/minet/crawl/crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     FunctionSpider,
     FunctionSpiderCallable,
     DefinitionSpider,
 )
 from minet.crawl.queue import CrawlerQueue, DumpType
 from minet.crawl.state import CrawlerState
 from minet.web import request, EXPECTED_WEB_ERRORS, AnyTimeout
-from minet.fetch import HTTPThreadPoolExecutor, CANCELLED
+from minet.executors import HTTPThreadPoolExecutor, CANCELLED
 from minet.exceptions import UnknownSpiderError, CancelledRequestError
 from minet.constants import (
     DEFAULT_DOMAIN_PARALLELISM,
     DEFAULT_IMAP_BUFFER_SIZE,
     DEFAULT_THROTTLE,
     DEFAULT_FETCH_MAX_REDIRECTS,
     DEFAULT_URLLIB3_TIMEOUT,
@@ -55,33 +55,39 @@
 ) -> CrawlJob[CrawlJobDataType]:
     if isinstance(url_or_job, CrawlJob):
         return url_or_job
 
     return CrawlJob(url=url_or_job)
 
 
+def coerce_spider(target):
+    if isinstance(target, Spider):
+        return target
+
+    if callable(target):
+        return FunctionSpider(target)
+
+    raise TypeError("expecting a spider or a callable")
+
+
 RequestArgsType = Callable[[CrawlJob[CrawlJobDataType]], Dict]
 
 
 class CrawlWorker(Generic[CrawlJobDataType, CrawlJobOutputDataType]):
     def __init__(
         self,
         crawler: "Crawler",
         *,
         request_args: Optional[RequestArgsType[CrawlJobDataType]] = None,
         max_redirects: int = DEFAULT_FETCH_MAX_REDIRECTS,
-        callback: Optional[
-            Callable[[CrawlResult[CrawlJobDataType, CrawlJobOutputDataType]], None]
-        ] = None,
     ):
         self.crawler = crawler
 
         self.request_args = request_args
         self.max_redirects = max_redirects
-        self.callback = callback
 
         self.cancel_event = self.crawler.executor.cancel_event
         self.local_context = self.crawler.executor.local_context
 
         self.default_request_kwargs = {
             "pool_manager": crawler.executor.pool_manager,
             "max_redirects": max_redirects,
@@ -160,14 +166,15 @@
 
             return result
 
 
 CrawlJobDataTypes = TypeVar("CrawlJobDataTypes", bound=Mapping)
 CrawlJobOutputDataTypes = TypeVar("CrawlJobOutputDataTypes")
 Spiders = Union[
+    FunctionSpiderCallable[CrawlJobDataTypes, CrawlJobOutputDataTypes],
     Spider[CrawlJobDataTypes, CrawlJobOutputDataTypes],
     Dict[str, Spider[CrawlJobDataTypes, CrawlJobOutputDataTypes]],
 ]
 
 # TODO: try creating a kwarg type for those
 # NOTE: crawling could work depth-first if we wanted
 class Crawler(Generic[CrawlJobDataTypes, CrawlJobOutputDataTypes]):
@@ -181,15 +188,15 @@
     finished: bool
     singular: bool
 
     __spiders: Dict[str, Spider[CrawlJobDataTypes, CrawlJobOutputDataTypes]]
 
     def __init__(
         self,
-        spiders: Spiders[CrawlJobDataTypes, CrawlJobOutputDataTypes],
+        spider_or_spiders: Spiders[CrawlJobDataTypes, CrawlJobOutputDataTypes],
         queue_path: Optional[str] = None,
         resume: bool = False,
         buffer_size: int = DEFAULT_IMAP_BUFFER_SIZE,
         domain_parallelism: int = DEFAULT_DOMAIN_PARALLELISM,
         throttle: float = DEFAULT_THROTTLE,
         max_workers: Optional[int] = None,
         wait: bool = True,
@@ -239,23 +246,23 @@
         if self.resuming and self.queue.qsize() == 0:
             self.finished = True
 
         # Initializing state
         self.state = CrawlerState(jobs_queued=self.queue.qsize())
 
         # Spiders
-        if isinstance(spiders, Spider):
-            self.__spiders = {DEFAULT_SPIDER_KEY: spiders}
-            self.singular = True
-        elif isinstance(spiders, Mapping):
+        if isinstance(spider_or_spiders, Mapping):
             self.__spiders = {}
             self.singular = False
 
-            for name, spider in spiders.items():
-                self.__spiders[name] = spider
+            for name, spider in spider_or_spiders.items():
+                self.__spiders[name] = coerce_spider(spider)
+        elif isinstance(spider_or_spiders, Spider) or callable(spider_or_spiders):
+            self.__spiders = {DEFAULT_SPIDER_KEY: coerce_spider(spider_or_spiders)}
+            self.singular = True
         else:
             raise TypeError("expecting a single spider or a mapping of spiders")
 
     def __repr__(self):
         class_name = self.__class__.__name__
 
         return "<{class_name} {number}>".format(
```

### Comparing `minet-1.0.0a8/minet/crawl/queue.py` & `minet-1.0.0a9/minet/crawl/queue.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/crawl/spiders.py` & `minet-1.0.0a9/minet/crawl/spiders.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Union,
     Callable,
     Dict,
     Iterator,
     Iterable,
     Generic,
 )
-from typing_extensions import TypedDict, NotRequired
+from minet.types import TypedDict, NotRequired
 
 from urllib.parse import urljoin
 from bs4 import BeautifulSoup
 
 from minet.crawl.types import (
     UrlOrCrawlJob,
     CrawlJob,
```

### Comparing `minet-1.0.0a8/minet/crawl/state.py` & `minet-1.0.0a9/minet/crawl/state.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/crawl/types.py` & `minet-1.0.0a9/minet/crawl/types.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/crowdtangle/client.py` & `minet-1.0.0a9/minet/crowdtangle/client.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/crowdtangle/constants.py` & `minet-1.0.0a9/minet/crowdtangle/constants.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/crowdtangle/exceptions.py` & `minet-1.0.0a9/minet/crowdtangle/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/crowdtangle/formatters.py` & `minet-1.0.0a9/minet/crowdtangle/formatters.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/crowdtangle/leaderboard.py` & `minet-1.0.0a9/minet/crowdtangle/leaderboard.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/crowdtangle/lists.py` & `minet-1.0.0a9/minet/crowdtangle/lists.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/crowdtangle/post.py` & `minet-1.0.0a9/minet/crowdtangle/post.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/crowdtangle/posts.py` & `minet-1.0.0a9/minet/crowdtangle/posts.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/crowdtangle/search.py` & `minet-1.0.0a9/minet/crowdtangle/search.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/crowdtangle/summary.py` & `minet-1.0.0a9/minet/crowdtangle/summary.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/crowdtangle/utils.py` & `minet-1.0.0a9/minet/crowdtangle/utils.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/encodings.py` & `minet-1.0.0a9/minet/encodings.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/exceptions.py` & `minet-1.0.0a9/minet/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,14 +64,26 @@
 
 class InvalidStatusError(MinetError):
     def __init__(self, status: int):
         super().__init__(str(status))
         self.status = status
 
 
+class HTTPCallbackError(MinetError):
+    def __init__(self, reason: Exception):
+        super().__init__("HTTPCallbackError: " + str(reason))
+        self.reason = reason
+
+    def unwrap(self, allow) -> Exception:
+        if not isinstance(self.reason, allow):
+            raise self.reason
+
+        return self.reason
+
+
 class CancelledRequestError(MinetError):
     pass
 
 
 class FinalTimeoutError(MinetError):
     pass
```

### Comparing `minet-1.0.0a8/minet/facebook/constants.py` & `minet-1.0.0a9/minet/facebook/constants.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/facebook/exceptions.py` & `minet-1.0.0a9/minet/facebook/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/facebook/formatters.py` & `minet-1.0.0a9/minet/facebook/formatters.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/facebook/mobile_scraper.py` & `minet-1.0.0a9/minet/facebook/mobile_scraper.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/facebook/post_id_from_url.py` & `minet-1.0.0a9/minet/facebook/post_id_from_url.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/facebook/utils.py` & `minet-1.0.0a9/minet/facebook/utils.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/fetch.py` & `minet-1.0.0a9/minet/executors.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # =============================================================================
-# Minet Multithreaded Fetch
+# Minet HTTP Multithreaded Executors
 # =============================================================================
 #
 # Exposing a specialized quenouille wrapper grabbing various urls from the
 # web in a multithreaded fashion.
 #
 from typing import (
     Optional,
@@ -20,42 +20,42 @@
 import urllib3
 import threading
 from threading import Event
 from quenouille import ThreadPoolExecutor
 from ural import get_domain_name, ensure_protocol
 from tenacity import RetryCallState
 
-from minet.exceptions import CancelledRequestError
+from minet.exceptions import CancelledRequestError, HTTPCallbackError
 from minet.web import (
     create_pool_manager,
     create_request_retryer,
     request,
     resolve,
     Response,
     RedirectionStack,
     AnyTimeout,
     EXPECTED_WEB_ERRORS,
 )
-from minet.heuristics import should_spoof_ua_when_resolving
 from minet.constants import (
     DEFAULT_DOMAIN_PARALLELISM,
     DEFAULT_IMAP_BUFFER_SIZE,
     DEFAULT_THROTTLE,
     DEFAULT_URLLIB3_TIMEOUT,
     DEFAULT_FETCH_MAX_REDIRECTS,
     DEFAULT_RESOLVE_MAX_REDIRECTS,
 )
 
 ItemType = TypeVar("ItemType")
 ResultType = TypeVar("ResultType")
+AddendumType = TypeVar("AddendumType")
 
 CANCELLED = object()
 
 
-class FetchWorkerPayload(Generic[ItemType]):
+class HTTPWorkerPayload(Generic[ItemType]):
     __slots__ = ("item", "url", "__has_cached_domain", "__domain")
 
     item: ItemType
     url: Optional[str]
 
     __has_cached_domain: bool
     __domain: Optional[str]
@@ -75,30 +75,32 @@
             self.__domain = get_domain_name(self.url)
 
         self.__has_cached_domain = True
 
         return self.__domain
 
 
-RequestArgsType = Callable[[FetchWorkerPayload[ItemType]], Dict]
+ArgsCallbackType = Callable[[HTTPWorkerPayload[ItemType]], Dict]
 
 
-class FetchResult(Generic[ItemType]):
-    __slots__ = ("item", "url", "error", "response")
+class RequestResult(Generic[ItemType, AddendumType]):
+    __slots__ = ("item", "url", "error", "response", "addendum")
 
     item: ItemType
     url: Optional[str]
     error: Optional[Exception]
     response: Optional[Response]
+    addendum: Optional[AddendumType]
 
     def __init__(self, item: ItemType, url: Optional[str]):
         self.item = item
         self.url = url
         self.error = None
         self.response = None
+        self.addendum = None
 
     def __repr__(self):
         name = self.__class__.__name__
 
         if not self.url:
             return "<{name} null!>".format(name=name)
 
@@ -113,27 +115,29 @@
         assert self.response is not None
 
         return "<{name} url={url!r} status={status!r}>".format(
             name=name, url=self.url, status=self.response.status
         )
 
 
-class ResolveResult(Generic[ItemType]):
-    __slots__ = ("item", "url", "error", "stack")
+class ResolveResult(Generic[ItemType, AddendumType]):
+    __slots__ = ("item", "url", "error", "stack", "addendum")
 
     item: ItemType
     url: Optional[str]
     error: Optional[Exception]
     stack: Optional[RedirectionStack]
+    addendum: Optional[AddendumType]
 
     def __init__(self, item: ItemType, url: Optional[str]):
         self.item = item
         self.url = url
         self.error = None
         self.stack = None
+        self.addendum = None
 
     def __repr__(self):
         name = self.__class__.__name__
 
         if not self.url:
             return "<{name} null!>".format(name=name)
 
@@ -148,179 +152,129 @@
             name=name,
             url=self.url,
             status=self.stack[-1].status,
             redirects=len(self.stack),
         )
 
 
-def key_by_domain_name(payload: FetchWorkerPayload) -> Optional[str]:
+def key_by_domain_name(payload: HTTPWorkerPayload) -> Optional[str]:
     return payload.domain
 
 
 def payloads_iter(
     iterable: Iterable[ItemType],
     key: Optional[Callable[[ItemType], Optional[str]]] = None,
-) -> Iterator[FetchWorkerPayload[ItemType]]:
+) -> Iterator[HTTPWorkerPayload[ItemType]]:
     for item in iterable:
         url = item if key is None else key(item)
 
         if not url:
-            yield FetchWorkerPayload(item=item, url=None)
+            yield HTTPWorkerPayload(item=item, url=None)
             continue
 
         # Url cleanup
         url = ensure_protocol(url.strip())  # type: ignore
 
-        yield FetchWorkerPayload(item=item, url=url)
+        yield HTTPWorkerPayload(item=item, url=url)
 
 
-class FetchWorker(Generic[ItemType]):
+class HTTPWorker(Generic[ItemType, AddendumType]):
     def __init__(
         self,
         pool_manager: urllib3.PoolManager,
         cancel_event: Event,
         local_context: threading.local,
         *,
-        request_args: Optional[RequestArgsType[ItemType]] = None,
+        resolving: bool = False,
+        get_args: Optional[ArgsCallbackType[ItemType]] = None,
         max_redirects: int = DEFAULT_FETCH_MAX_REDIRECTS,
-        callback: Optional[Callable[[FetchResult[ItemType]], None]] = None,
-    ):
-        self.cancel_event = cancel_event
-        self.local_context = local_context
-        self.request_args = request_args
-        self.callback = callback
-
-        self.default_request_kwargs = {
-            "pool_manager": pool_manager,
-            "max_redirects": max_redirects,
-            "cancel_event": cancel_event,
-        }
-
-    def __call__(
-        self, payload: FetchWorkerPayload[ItemType]
-    ) -> Union[object, FetchResult[ItemType]]:
-        item, url = payload.item, payload.url
-
-        result = FetchResult(item, url)
-
-        # Noop
-        if url is None:
-            return result
-
-        kwargs = {}
-
-        if self.cancel_event.is_set():
-            return CANCELLED
-
-        if self.request_args is not None:
-            # NOTE: request_args must be threadsafe
-            kwargs = self.request_args(payload)
-
-        if self.cancel_event.is_set():
-            return CANCELLED
-
-        try:
-            retryer = getattr(self.local_context, "retryer", None)
-            kwargs.update(self.default_request_kwargs)
-
-            if retryer is not None:
-                response = retryer(request, url, **kwargs)
-            else:
-                response = request(url, **kwargs)
-
-        except CancelledRequestError:
-            return CANCELLED
-
-        except EXPECTED_WEB_ERRORS as error:
-            result.error = error
-
-        else:
-            result.response = response
-
-            if self.callback is not None:
-                if self.cancel_event.is_set():
-                    return CANCELLED
-
-                self.callback(result)
-
-        return result
-
-
-class ResolveWorker(Generic[ItemType]):
-    def __init__(
-        self,
-        pool_manager: urllib3.PoolManager,
-        cancel_event: Event,
-        local_context: threading.local,
-        *,
-        resolve_args: Optional[RequestArgsType[ItemType]] = None,
-        max_redirects: int = DEFAULT_RESOLVE_MAX_REDIRECTS,
         follow_refresh_header: bool = True,
         follow_meta_refresh: bool = False,
         follow_js_relocation: bool = False,
         infer_redirection: bool = False,
         canonicalize: bool = False,
+        callback: Optional[
+            Callable[[RequestResult[ItemType, AddendumType]], AddendumType]
+        ] = None,
     ):
         self.cancel_event = cancel_event
         self.local_context = local_context
-        self.resolve_args = resolve_args
+        self.get_args = get_args
+        self.callback = callback
 
-        self.default_resolve_kwargs = {
+        self.resolving = resolving
+        self.fn = request if not resolving else resolve
+        self.Result = RequestResult if not resolving else ResolveResult
+
+        self.default_kwargs = {
             "pool_manager": pool_manager,
             "max_redirects": max_redirects,
             "cancel_event": cancel_event,
             "follow_refresh_header": follow_refresh_header,
             "follow_meta_refresh": follow_meta_refresh,
             "follow_js_relocation": follow_js_relocation,
             "infer_redirection": infer_redirection,
             "canonicalize": canonicalize,
         }
 
     def __call__(
-        self, payload: FetchWorkerPayload[ItemType]
-    ) -> Union[object, ResolveResult[ItemType]]:
+        self, payload: HTTPWorkerPayload[ItemType]
+    ) -> Union[object, RequestResult[ItemType, AddendumType]]:
         item, url = payload.item, payload.url
 
-        result = ResolveResult(item, url)
+        result = self.Result(item, url)
 
         # Noop
         if url is None:
             return result
 
         kwargs = {}
 
         if self.cancel_event.is_set():
             return CANCELLED
 
-        if self.resolve_args is not None:
-            # NOTE: resolve_args must be threadsafe
-            kwargs = self.resolve_args(payload)
+        if self.get_args is not None:
+            # NOTE: given callback must be threadsafe
+            kwargs = self.get_args(payload)
 
         if self.cancel_event.is_set():
             return CANCELLED
 
-        # NOTE: should it be just in the CLI?
-        if "spoof_ua" not in kwargs and payload.domain is not None:
-            kwargs["spoof_ua"] = should_spoof_ua_when_resolving(payload.domain)
-
         try:
             retryer = getattr(self.local_context, "retryer", None)
-            kwargs.update(self.default_resolve_kwargs)
+            kwargs.update(self.default_kwargs)
 
             if retryer is not None:
-                stack = retryer(resolve, url, **kwargs)
+                output = retryer(self.fn, url, **kwargs)
             else:
-                stack = resolve(url, **kwargs)
+                output = self.fn(url, **kwargs)
 
         except CancelledRequestError:
             return CANCELLED
+
         except EXPECTED_WEB_ERRORS as error:
             result.error = error
+
         else:
-            result.stack = stack
+            if self.resolving:
+                result.stack = output
+            else:
+                result.response = output
+
+            if self.callback is not None:
+                if self.cancel_event.is_set():
+                    return CANCELLED
+
+                try:
+                    if retryer is not None:
+                        result.addendum = retryer(self.callback, result)
+                    else:
+                        result.addendum = self.callback(result)
+                except Exception as reason:
+                    result.error = HTTPCallbackError(reason)
 
         return result
 
 
 class HTTPThreadPoolExecutor(ThreadPoolExecutor):
     def __init__(
         self,
@@ -377,89 +331,95 @@
         self.cancel_event.set()
 
     def shutdown(self, wait=True) -> None:
         self.cancel()
         self.pool_manager.clear()
         return super().shutdown(wait=wait)
 
-    def imap(self, *args, **kwargs):
-        raise NotImplementedError
-
-
-class FetchThreadPoolExecutor(HTTPThreadPoolExecutor):
-    def imap_unordered(
+    def request(
         self,
         iterator: Iterable[ItemType],
         *,
+        ordered: bool = False,
         key: Optional[Callable[[ItemType], Optional[str]]] = None,
         throttle: float = DEFAULT_THROTTLE,
-        request_args: Optional[RequestArgsType[ItemType]] = None,
+        request_args: Optional[ArgsCallbackType[ItemType]] = None,
         buffer_size: int = DEFAULT_IMAP_BUFFER_SIZE,
         domain_parallelism: int = DEFAULT_DOMAIN_PARALLELISM,
         max_redirects: int = DEFAULT_FETCH_MAX_REDIRECTS,
-        callback: Optional[Callable[[FetchResult[ItemType]], None]] = None,
-    ) -> Iterator[FetchResult[ItemType]]:
+        callback: Optional[
+            Callable[[RequestResult[ItemType, AddendumType]], None]
+        ] = None,
+    ) -> Iterator[RequestResult[ItemType, AddendumType]]:
 
         # TODO: validate
-        worker = FetchWorker(
+        worker = HTTPWorker(
             self.pool_manager,
             self.cancel_event,
             self.local_context,
-            request_args=request_args,
+            get_args=request_args,
             max_redirects=max_redirects,
             callback=callback,
         )
 
-        imap_unordered = super().imap_unordered(
+        method = super().imap if ordered else super().imap_unordered
+
+        imap_unordered = method(
             payloads_iter(iterator, key=key),
             worker,
             key=key_by_domain_name,
             parallelism=domain_parallelism,
             buffer_size=buffer_size,
             throttle=throttle,
         )
 
-        return (item for item in imap_unordered if item is not CANCELLED)
-
+        return (item for item in imap_unordered if item is not CANCELLED)  # type: ignore
 
-class ResolveThreadPoolExecutor(HTTPThreadPoolExecutor):
-    def imap_unordered(
+    def resolve(
         self,
         iterator: Iterable[ItemType],
         *,
+        ordered: bool = False,
         key: Optional[Callable[[ItemType], Optional[str]]] = None,
         throttle: float = DEFAULT_THROTTLE,
-        resolve_args: Optional[RequestArgsType[ItemType]] = None,
+        resolve_args: Optional[ArgsCallbackType[ItemType]] = None,
         buffer_size: int = DEFAULT_IMAP_BUFFER_SIZE,
         domain_parallelism: int = DEFAULT_DOMAIN_PARALLELISM,
-        max_redirects: int = DEFAULT_FETCH_MAX_REDIRECTS,
+        max_redirects: int = DEFAULT_RESOLVE_MAX_REDIRECTS,
         follow_refresh_header: bool = True,
         follow_meta_refresh: bool = False,
         follow_js_relocation: bool = False,
         infer_redirection: bool = False,
         canonicalize: bool = False,
-    ) -> Iterator[ResolveResult[ItemType]]:
+        callback: Optional[
+            Callable[[ResolveResult[ItemType, AddendumType]], None]
+        ] = None,
+    ) -> Iterator[ResolveResult[ItemType, AddendumType]]:
 
         # TODO: validate
-        worker = ResolveWorker(
+        worker = HTTPWorker(
             self.pool_manager,
             self.cancel_event,
             self.local_context,
-            resolve_args=resolve_args,
+            resolving=True,
+            get_args=resolve_args,
             max_redirects=max_redirects,
             follow_refresh_header=follow_refresh_header,
             follow_meta_refresh=follow_meta_refresh,
             follow_js_relocation=follow_js_relocation,
             infer_redirection=infer_redirection,
             canonicalize=canonicalize,
+            callback=callback,
         )
 
-        imap_unordered = super().imap_unordered(
+        method = super().imap if ordered else super().imap_unordered
+
+        imap_unordered = method(
             payloads_iter(iterator, key=key),
             worker,
             key=key_by_domain_name,
             parallelism=domain_parallelism,
             buffer_size=buffer_size,
             throttle=throttle,
         )
 
-        return (item for item in imap_unordered if item is not CANCELLED)
+        return (item for item in imap_unordered if item is not CANCELLED)  # type: ignore
```

### Comparing `minet-1.0.0a8/minet/fs.py` & `minet-1.0.0a9/minet/fs.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/google/exceptions.py` & `minet-1.0.0a9/minet/google/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/google/sheets.py` & `minet-1.0.0a9/minet/google/sheets.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/hyphe/client.py` & `minet-1.0.0a9/minet/hyphe/client.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/hyphe/constants.py` & `minet-1.0.0a9/minet/hyphe/constants.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/hyphe/exceptions.py` & `minet-1.0.0a9/minet/hyphe/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/hyphe/formatters.py` & `minet-1.0.0a9/minet/hyphe/formatters.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/instagram/api_scraper.py` & `minet-1.0.0a9/minet/instagram/api_scraper.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/instagram/constants.py` & `minet-1.0.0a9/minet/instagram/constants.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/instagram/exceptions.py` & `minet-1.0.0a9/minet/instagram/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/instagram/formatters.py` & `minet-1.0.0a9/minet/instagram/formatters.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/instagram/utils.py` & `minet-1.0.0a9/minet/instagram/utils.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/mediacloud/client.py` & `minet-1.0.0a9/minet/mediacloud/client.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/mediacloud/constants.py` & `minet-1.0.0a9/minet/mediacloud/constants.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/mediacloud/exceptions.py` & `minet-1.0.0a9/minet/mediacloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/mediacloud/formatters.py` & `minet-1.0.0a9/minet/mediacloud/formatters.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/mediacloud/search.py` & `minet-1.0.0a9/minet/mediacloud/search.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/mediacloud/topic.py` & `minet-1.0.0a9/minet/mediacloud/topic.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/mediacloud/utils.py` & `minet-1.0.0a9/minet/mediacloud/utils.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/multiprocessing.py` & `minet-1.0.0a9/minet/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/scrape/__init__.py` & `minet-1.0.0a9/minet/scrape/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/scrape/analysis.py` & `minet-1.0.0a9/minet/scrape/analysis.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/scrape/compiler.py` & `minet-1.0.0a9/minet/scrape/compiler.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/scrape/constants.py` & `minet-1.0.0a9/minet/scrape/constants.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/scrape/exceptions.py` & `minet-1.0.0a9/minet/scrape/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/scrape/interpreter.py` & `minet-1.0.0a9/minet/scrape/interpreter.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/scrape/mixin.py` & `minet-1.0.0a9/minet/scrape/mixin.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/scrape/std.py` & `minet-1.0.0a9/minet/scrape/std.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/scrape/straining.py` & `minet-1.0.0a9/minet/scrape/straining.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/scrape/typical.py` & `minet-1.0.0a9/minet/scrape/typical.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/scrape/utils.py` & `minet-1.0.0a9/minet/scrape/utils.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/telegram/constants.py` & `minet-1.0.0a9/minet/telegram/constants.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/telegram/formatters.py` & `minet-1.0.0a9/minet/telegram/formatters.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/telegram/scraper.py` & `minet-1.0.0a9/minet/telegram/scraper.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/tiktok/api_scraper.py` & `minet-1.0.0a9/minet/tiktok/api_scraper.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/tiktok/constants.py` & `minet-1.0.0a9/minet/tiktok/constants.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/tiktok/exceptions.py` & `minet-1.0.0a9/minet/tiktok/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/tiktok/formatters.py` & `minet-1.0.0a9/minet/tiktok/formatters.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/twitter/api_client.py` & `minet-1.0.0a9/minet/twitter/api_client.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/twitter/api_scraper.py` & `minet-1.0.0a9/minet/twitter/api_scraper.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/twitter/constants.py` & `minet-1.0.0a9/minet/twitter/constants.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/twitter/exceptions.py` & `minet-1.0.0a9/minet/twitter/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/utils.py` & `minet-1.0.0a9/minet/utils.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/web.py` & `minet-1.0.0a9/minet/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import urllib3
 import urllib3.exceptions as urllib3_exceptions
 import urllib.error
 import ural
 import json
 import mimetypes
 import functools
+import threading
 import warnings
 from bs4 import BeautifulSoup, XMLParsedAsHTMLWarning, SoupStrainer
 from datetime import datetime
 from timeit import default_timer as timer
 from io import BytesIO
 from threading import Event
 from itertools import chain
@@ -1041,14 +1042,15 @@
     cookie=None,
     spoof_ua: bool = True,
     follow_redirects: bool = True,
     max_redirects: int = 5,
     follow_refresh_header: bool = True,
     follow_meta_refresh: bool = False,
     follow_js_relocation: bool = False,
+    infer_redirection: bool = False,
     canonicalize: bool = False,
     known_encoding: Optional[str] = None,
     timeout: Optional[AnyTimeout] = None,
     body=None,
     json_body=None,
     cancel_event: Optional[Event] = None,
     raise_on_statuses: Optional[Container[int]] = None,
@@ -1092,14 +1094,15 @@
             method,
             headers=final_headers,
             body=final_body,
             max_redirects=max_redirects,
             follow_refresh_header=follow_refresh_header,
             follow_meta_refresh=follow_meta_refresh,
             follow_js_relocation=follow_js_relocation,
+            infer_redirection=infer_redirection,
             canonicalize=canonicalize,
             timeout=timeout,
             cancel_event=cancel_event,
         )
 
     if raise_on_statuses is not None:
         if buffered_response.status in raise_on_statuses:
@@ -1202,14 +1205,16 @@
 
         exception = retry_state.outcome.exception()
 
         sleepers_logger.warn(
             "request_retryer starts sleeping",
             extra={
                 "source": "request_retryer",
+                "from_thread": threading.current_thread()
+                is not threading.main_thread(),
                 "retry_state": retry_state,
                 "exception": exception,
                 "sleep_time": retry_state.next_action.sleep,
                 "epilog": self.epilog_builder(retry_state)
                 if self.epilog_builder is not None
                 else None,
             },
@@ -1239,19 +1244,19 @@
 class RequestRetrying(Retrying):
     def __init__(
         self, *args, invalid_statuses: Optional[Container[int]] = None, **kwargs
     ):
         self._invalid_statuses = invalid_statuses
         super().__init__(*args, **kwargs)
 
-    def __call__(self, *args, **kwargs):
-        if self._invalid_statuses is not None:
+    def __call__(self, fn, *args, **kwargs):
+        if self._invalid_statuses is not None and fn in (request, resolve):
             kwargs["raise_on_statuses"] = self._invalid_statuses
 
-        return super().__call__(*args, **kwargs)
+        return super().__call__(fn, *args, **kwargs)
 
 
 def create_request_retryer(
     min: float = 10,
     max: float = ONE_DAY,
     max_attempts: int = 9,
     before_sleep=noop,
@@ -1282,14 +1287,28 @@
         for exc in additional_exceptions:
             retryable_exception_types.append(exc)
 
     retry_condition = retry_if_exception_type(
         exception_types=tuple(retryable_exception_types)
     )
 
+    # By default we also retry subsets of new connection error
+    def temporary_failure_predicate(exc: BaseException) -> bool:
+        if not isinstance(exc, urllib3_exceptions.NewConnectionError):
+            return False
+
+        msg = str(exc).lower()
+
+        if "errno -3" in msg or "temporary failure in name resolution" in msg:
+            return True
+
+        return False
+
+    retry_condition |= retry_if_exception(temporary_failure_predicate)
+
     if retry_on_statuses is not None:
 
         def status_predicate(exc: BaseException) -> bool:
             if isinstance(exc, InvalidStatusError) and exc.status in retry_on_statuses:
                 return True
 
             return False
```

### Comparing `minet-1.0.0a8/minet/wikipedia/wikimedia_rest_api_client.py` & `minet-1.0.0a9/minet/wikipedia/wikimedia_rest_api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Iterator, TypeVar, Callable, Tuple, List, Optional
 
 from urllib.parse import quote, unquote
 
-from minet.fetch import FetchThreadPoolExecutor
+from minet.executors import HTTPThreadPoolExecutor
 
 from minet.wikipedia.exceptions import (
     WikimediaRESTAPIThrottledError,
     WikimediaRESTAPIServerError,
 )
 from minet.wikipedia.types import Granularity, Agent, Access, WikipediaPageViewsItem
 
@@ -85,16 +85,16 @@
                 access=access,
                 granularity=granularity,
                 agent=agent,
             )
 
             return url
 
-        with FetchThreadPoolExecutor(max_workers=threads, retry=True) as executor:
-            for result in executor.imap_unordered(
+        with HTTPThreadPoolExecutor(max_workers=threads, retry=True) as executor:
+            for result in executor.request(
                 pages,
                 key=api_url_from_item,
                 domain_parallelism=threads,
                 throttle=0,
             ):
                 if result.error:
                     raise result.error
```

### Comparing `minet-1.0.0a8/minet/youtube/client.py` & `minet-1.0.0a9/minet/youtube/client.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/youtube/constants.py` & `minet-1.0.0a9/minet/youtube/constants.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/youtube/exceptions.py` & `minet-1.0.0a9/minet/youtube/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/youtube/formatters.py` & `minet-1.0.0a9/minet/youtube/formatters.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/youtube/scrapers.py` & `minet-1.0.0a9/minet/youtube/scrapers.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet/youtube/utils.py` & `minet-1.0.0a9/minet/youtube/utils.py`

 * *Files identical despite different names*

### Comparing `minet-1.0.0a8/minet.egg-info/PKG-INFO` & `minet-1.0.0a9/minet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minet
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: A webmining CLI tool & library for python.
 Home-page: http://github.com/medialab/minet
 Author: Guillaume Plique, Pauline Breteau, Jules Farjas, Héloïse Théro, Jean Descamps, Amélie Pellé, Laura Miguel
 License: MIT
 Description: [![Build Status](https://github.com/medialab/minet/workflows/Tests/badge.svg)](https://github.com/medialab/minet/actions) [![DOI](https://zenodo.org/badge/169059797.svg)](https://zenodo.org/badge/latestdoi/169059797) [![download number](https://static.pepy.tech/badge/minet)](https://pepy.tech/project/minet)
         
         ![Minet](docs/img/minet.png)
```

### Comparing `minet-1.0.0a8/minet.egg-info/SOURCES.txt` & `minet-1.0.0a9/minet.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 README.md
 setup.py
 minet/__init__.py
 minet/__version__.py
 minet/constants.py
 minet/encodings.py
 minet/exceptions.py
-minet/fetch.py
+minet/executors.py
 minet/fs.py
 minet/heuristics.py
 minet/loggers.py
 minet/multiprocessing.py
 minet/types.py
 minet/utils.py
 minet/web.py
```

### Comparing `minet-1.0.0a8/setup.py` & `minet-1.0.0a9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,16 +37,16 @@
         "quenouille>=1.7.1,<2",
         "rich>=13,<14",
         "rich-argparse>=1,<2",
         "soupsieve>=2.1,<3",
         "tenacity>=8,<9",
         "trafilatura>=1.4.1,<1.5",
         "twitwi>=0.16.1,<0.17",
-        "ural>=0.39,<0.40",
+        "ural>=0.40,<0.41",
         "urllib3>=1.26.9,<2",
     ],
     extras_require={
-        ":python_version<'3.10'": ["typing_extensions"],
+        ":python_version<'3.11'": ["typing_extensions"],
     },
     entry_points={"console_scripts": ["minet=minet.cli.__main__:main"]},
     zip_safe=True,
 )
```

### Comparing `minet-1.0.0a8/test/crowdtangle/utils_test.py` & `minet-1.0.0a9/test/crowdtangle/utils_test.py`

 * *Files identical despite different names*

