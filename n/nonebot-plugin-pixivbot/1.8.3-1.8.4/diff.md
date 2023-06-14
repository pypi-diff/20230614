# Comparing `tmp/nonebot_plugin_pixivbot-1.8.3.tar.gz` & `tmp/nonebot_plugin_pixivbot-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pixivbot-1.8.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_pixivbot-1.8.4.tar", max compression
```

## Comparing `nonebot_plugin_pixivbot-1.8.3.tar` & `nonebot_plugin_pixivbot-1.8.4.tar`

### file list

```diff
@@ -1,171 +1,171 @@
--rw-r--r--   0        0        0     1085 2023-02-13 05:42:01.812872 nonebot_plugin_pixivbot-1.8.3/LICENSE
--rw-r--r--   0        0        0     1825 2023-04-27 09:46:24.103248 nonebot_plugin_pixivbot-1.8.3/pyproject.toml
--rw-r--r--   0        0        0    17274 2023-04-27 09:52:32.622538 nonebot_plugin_pixivbot-1.8.3/README.md
--rw-r--r--   0        0        0     1192 2023-04-26 10:41:42.734890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/__init__.py
--rw-r--r--   0        0        0     7793 2023-04-27 09:37:04.739003 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/config.py
--rw-r--r--   0        0        0     4322 2023-04-26 10:41:42.734890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/context.py
--rw-r--r--   0        0        0      443 2023-02-13 05:42:01.817870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/__init__.py
--rw-r--r--   0        0        0       56 2023-02-13 05:42:01.817870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/errors.py
--rw-r--r--   0        0        0     1515 2023-02-13 05:42:01.817870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/interval_task_repo.py
--rw-r--r--   0        0        0      488 2023-04-26 10:41:42.735891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/local_tag/__init__.py
--rw-r--r--   0        0        0      535 2023-04-26 10:41:42.735891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/local_tag/base.py
--rw-r--r--   0        0        0     2643 2023-04-26 10:41:42.736891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/local_tag/mongo.py
--rw-r--r--   0        0        0     2702 2023-04-26 10:41:42.736891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/local_tag/sql.py
--rw-r--r--   0        0        0      541 2023-04-26 10:41:42.737892 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_binding/__init__.py
--rw-r--r--   0        0        0      387 2023-04-26 10:41:42.737892 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_binding/base.py
--rw-r--r--   0        0        0     2087 2023-04-26 10:41:42.738890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_binding/mongo.py
--rw-r--r--   0        0        0     2715 2023-04-26 10:41:42.739891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_binding/sql.py
--rw-r--r--   0        0        0      262 2023-02-13 05:42:01.821870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/__init__.py
--rw-r--r--   0        0        0     1524 2023-02-13 05:42:01.822870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/base.py
--rw-r--r--   0        0        0     1829 2023-04-26 10:41:42.739891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/compressor.py
--rw-r--r--   0        0        0      355 2023-02-13 05:42:01.822870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/enums.py
--rw-r--r--   0        0        0      334 2023-02-13 05:42:01.823870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/errors.py
--rw-r--r--   0        0        0     1036 2023-02-13 05:42:01.823870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/lazy_illust.py
--rw-r--r--   0        0        0      826 2023-03-15 03:52:01.493698 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/__init__.py
--rw-r--r--   0        0        0     2823 2023-03-15 03:26:56.195873 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/base.py
--rw-r--r--   0        0        0     3419 2023-04-26 10:41:42.740890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/dummy.py
--rw-r--r--   0        0        0    31650 2023-04-26 10:41:42.820890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo.py
--rw-r--r--   0        0        0     4802 2023-04-26 08:33:36.389185 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo_models.py
--rw-r--r--   0        0        0    33317 2023-04-26 10:41:42.821890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql.py
--rw-r--r--   0        0        0     3536 2023-04-26 08:33:36.390185 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql_models.py
--rw-r--r--   0        0        0     9990 2023-04-26 10:41:42.822892 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator.py
--rw-r--r--   0        0        0    22139 2023-04-26 10:41:42.822892 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator_repo.py
--rw-r--r--   0        0        0      332 2023-04-26 10:41:42.823892 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/models.py
--rw-r--r--   0        0        0    18860 2023-04-27 09:37:04.734003 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/remote_repo.py
--rw-r--r--   0        0        0     1079 2023-02-13 05:42:01.829870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/__init__.py
--rw-r--r--   0        0        0     1820 2023-02-13 05:42:01.830870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/lifecycle_mixin.py
--rw-r--r--   0        0        0     3211 2023-02-13 05:42:01.830870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/migration_manager.py
--rw-r--r--   0        0        0     5774 2023-04-26 10:41:42.787891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/__init__.py
--rw-r--r--   0        0        0      290 2023-04-26 10:41:42.743890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/meta_info.py
--rw-r--r--   0        0        0      693 2023-02-13 05:42:01.833870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/__init__.py
--rw-r--r--   0        0        0     1424 2023-02-13 05:42:01.833870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v1_to_v2.py
--rw-r--r--   0        0        0      674 2023-02-13 05:42:01.833870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v2_to_v3.py
--rw-r--r--   0        0        0     2729 2023-02-13 05:42:01.834869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v3_to_v4.py
--rw-r--r--   0        0        0     1039 2023-02-13 05:42:01.834869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v4_to_v5.py
--rw-r--r--   0        0        0     3306 2023-02-13 05:42:01.834869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v5_to_v6.py
--rw-r--r--   0        0        0      416 2023-02-13 05:42:01.835870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v6_to_v7.py
--rw-r--r--   0        0        0     5781 2023-04-26 10:41:42.788890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/sql/__init__.py
--rw-r--r--   0        0        0      306 2023-03-13 13:51:04.755048 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/sql/meta_info.py
--rw-r--r--   0        0        0      457 2023-02-13 05:42:01.837870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/sql/migration/__init__.py
--rw-r--r--   0        0        0     3824 2023-02-13 05:42:01.838869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v1_to_v2.py
--rw-r--r--   0        0        0     1842 2023-02-13 05:42:01.839869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v2_to_v3.py
--rw-r--r--   0        0        0      360 2023-02-13 05:42:01.839869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v3_to_v4.py
--rw-r--r--   0        0        0      520 2023-04-26 10:41:42.744892 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/subscription/__init__.py
--rw-r--r--   0        0        0      177 2023-04-26 10:41:42.745891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/subscription/base.py
--rw-r--r--   0        0        0     4446 2023-04-26 10:41:42.745891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/subscription/mongo.py
--rw-r--r--   0        0        0     5698 2023-04-26 10:41:42.746890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/subscription/sql.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.842870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/utils/__init__.py
--rw-r--r--   0        0        0      164 2023-02-13 05:42:01.842870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/utils/shortuuid.py
--rw-r--r--   0        0        0      814 2023-02-13 05:42:01.843869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/utils/sql/__init__.py
--rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/utils/sql/utc_datetime.py
--rw-r--r--   0        0        0      720 2023-02-13 05:42:01.842870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/utils/sql.pyi
--rw-r--r--   0        0        0      517 2023-04-26 10:41:42.747890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/watch_task/__init__.py
--rw-r--r--   0        0        0      226 2023-04-26 10:41:42.747890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/watch_task/base.py
--rw-r--r--   0        0        0     5155 2023-04-26 10:41:42.748890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/watch_task/mongo.py
--rw-r--r--   0        0        0     6613 2023-04-26 10:41:42.748890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/watch_task/sql.py
--rw-r--r--   0        0        0      964 2023-03-15 03:24:39.857013 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/enums.py
--rw-r--r--   0        0        0      102 2023-02-14 03:27:31.463009 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/global_context.py
--rw-r--r--   0        0        0       92 2023-02-13 05:42:01.847870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/__init__.py
--rw-r--r--   0        0        0     9597 2023-04-26 11:20:41.866640 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/base.py
--rw-r--r--   0        0        0      308 2023-02-13 05:42:01.847870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/__init__.py
--rw-r--r--   0        0        0     2489 2023-04-26 11:20:41.835065 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/bind.py
--rw-r--r--   0        0        0     2481 2023-03-29 02:34:22.114209 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/command.py
--rw-r--r--   0        0        0     1207 2023-04-26 11:20:41.815065 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/help.py
--rw-r--r--   0        0        0      804 2023-04-26 11:20:41.870642 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/invalidate_cache.py
--rw-r--r--   0        0        0     4291 2023-04-26 11:28:38.961827 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/schedule.py
--rw-r--r--   0        0        0     1363 2023-03-29 02:34:22.116335 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/subcommand.py
--rw-r--r--   0        0        0     6050 2023-04-26 11:28:38.966828 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/watch.py
--rw-r--r--   0        0        0      633 2023-02-13 05:42:01.851870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/__init__.py
--rw-r--r--   0        0        0      688 2023-03-29 02:34:22.117934 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/base.py
--rw-r--r--   0        0        0     1629 2023-04-26 11:11:55.420381 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/illust.py
--rw-r--r--   0        0        0     1440 2023-04-26 11:20:41.831066 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/more.py
--rw-r--r--   0        0        0     2817 2023-04-26 11:20:41.858064 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/random_bookmark.py
--rw-r--r--   0        0        0     1752 2023-04-26 11:20:41.846065 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/random_illust.py
--rw-r--r--   0        0        0     1599 2023-04-26 11:20:41.862066 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/random_recommended_illust.py
--rw-r--r--   0        0        0     2006 2023-04-26 11:20:41.839065 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/random_related_illust.py
--rw-r--r--   0        0        0     2089 2023-04-26 11:20:41.819065 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/random_user_illust.py
--rw-r--r--   0        0        0     4204 2023-04-26 11:20:41.854065 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/ranking.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.857869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/__init__.py
--rw-r--r--   0        0        0      524 2023-03-29 02:34:22.124122 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/base.py
--rw-r--r--   0        0        0     2012 2023-03-29 02:34:22.125123 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/combined_interceptor.py
--rw-r--r--   0        0        0     1380 2023-03-29 02:34:22.125123 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/default_error_interceptor.py
--rw-r--r--   0        0        0     1134 2023-03-29 02:34:22.126120 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/loading_prompt_interceptor.py
--rw-r--r--   0        0        0     1947 2023-03-29 02:34:54.094101 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/permission_interceptor.py
--rw-r--r--   0        0        0      654 2023-03-29 02:34:22.127120 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/record_req_interceptor.py
--rw-r--r--   0        0        0      919 2023-03-29 02:34:22.128120 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/retry_interceptor.py
--rw-r--r--   0        0        0     1526 2023-03-29 02:34:22.128120 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/service_interceptor.py
--rw-r--r--   0        0        0      673 2023-03-29 02:34:22.129121 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/timeout_interceptor.py
--rw-r--r--   0        0        0      201 2023-02-13 05:42:01.861870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/pkg_context.py
--rw-r--r--   0        0        0     3378 2023-04-26 10:41:42.749891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/recorder.py
--rw-r--r--   0        0        0      325 2023-02-14 11:56:02.041347 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/schedule/__init__.py
--rw-r--r--   0        0        0      349 2023-04-26 11:20:41.850065 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/schedule/base.py
--rw-r--r--   0        0        0      461 2023-03-29 02:34:22.131121 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/schedule/random_bookmark.py
--rw-r--r--   0        0        0      453 2023-03-29 02:34:22.131121 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/schedule/random_illust.py
--rw-r--r--   0        0        0      498 2023-03-29 02:34:22.132122 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/schedule/random_recommended_illust.py
--rw-r--r--   0        0        0      470 2023-03-29 02:34:22.132122 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/schedule/random_user_illust.py
--rw-r--r--   0        0        0      432 2023-03-29 02:34:22.133120 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/schedule/ranking.py
--rw-r--r--   0        0        0       27 2023-02-13 05:42:01.862870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/sniffer/__init__.py
--rw-r--r--   0        0        0     1011 2023-04-26 11:20:41.843065 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/sniffer/illust_link.py
--rw-r--r--   0        0        0     1382 2023-02-13 05:42:01.863870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/utils.py
--rw-r--r--   0        0        0      112 2023-02-14 12:15:47.490983 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/watch/__init__.py
--rw-r--r--   0        0        0      865 2023-04-26 11:20:41.827066 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/watch/base.py
--rw-r--r--   0        0        0     2498 2023-04-26 10:41:42.749891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/watch/following_illusts.py
--rw-r--r--   0        0        0     1864 2023-04-26 10:41:42.750890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/watch/user_illusts.py
--rw-r--r--   0        0        0      530 2023-02-13 05:42:01.865869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/__init__.py
--rw-r--r--   0        0        0     1366 2023-02-13 05:42:01.865869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/identifier.py
--rw-r--r--   0        0        0     1858 2023-04-27 09:18:54.765186 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/illust.py
--rw-r--r--   0        0        0      352 2023-02-13 05:42:01.866870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/interval_task.py
--rw-r--r--   0        0        0      157 2023-02-13 05:42:01.867870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/message/__init__.py
--rw-r--r--   0        0        0     2623 2023-02-13 05:42:01.867870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/message/illust_message.py
--rw-r--r--   0        0        0     2443 2023-02-13 05:42:01.867870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/message/illust_messages.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.868870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/old/__init__.py
--rw-r--r--   0        0        0      120 2023-02-13 05:42:01.868870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/old/pixiv_binding.py
--rw-r--r--   0        0        0      950 2023-02-13 05:42:01.868870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/old/subscription.py
--rw-r--r--   0        0        0      242 2023-02-13 05:42:01.869870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/pixiv_binding.py
--rw-r--r--   0        0        0     1450 2023-04-26 10:52:37.464803 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/subscription.py
--rw-r--r--   0        0        0      203 2023-02-13 05:42:01.870869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/tag.py
--rw-r--r--   0        0        0      131 2023-02-13 05:42:01.870869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/user.py
--rw-r--r--   0        0        0      242 2023-02-13 05:42:01.871622 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/user_preview.py
--rw-r--r--   0        0        0     1004 2023-04-26 10:52:37.460801 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/watch_task.py
--rw-r--r--   0        0        0     1680 2023-02-14 03:39:10.628376 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/plugin_service.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.872870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/protocol_dep/__init__.py
--rw-r--r--   0        0        0      914 2023-03-14 09:12:27.158624 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/protocol_dep/authenticator.py
--rw-r--r--   0        0        0     2757 2023-03-29 02:34:22.136711 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/protocol_dep/post_dest.py
--rw-r--r--   0        0        0     1445 2023-02-14 03:32:29.851104 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/protocol_dep/postman.py
--rw-r--r--   0        0        0     1452 2023-02-14 03:32:29.852102 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/protocol_dep/protocol_dep.py
--rw-r--r--   0        0        0       49 2023-02-13 05:42:01.874870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/__init__.py
--rw-r--r--   0        0        0     5469 2023-04-26 11:26:09.322980 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/interval_task_worker.py
--rw-r--r--   0        0        0      958 2023-04-26 10:41:42.751891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/pixiv_account_binder.py
--rw-r--r--   0        0        0     6023 2023-04-26 10:41:42.751891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/pixiv_service.py
--rw-r--r--   0        0        0     2244 2023-02-13 05:42:01.877869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/roulette.py
--rw-r--r--   0        0        0     5640 2023-04-26 10:41:42.752891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/scheduler.py
--rw-r--r--   0        0        0     3821 2023-04-26 10:41:42.752891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/watchman.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.878870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/__init__.py
--rw-r--r--   0        0        0      230 2023-03-29 02:34:22.138709 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/algorithm.py
--rw-r--r--   0        0        0      265 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/coros.py
--rw-r--r--   0        0        0     1148 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/decode_integer.py
--rw-r--r--   0        0        0      515 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/errors.py
--rw-r--r--   0        0        0     3604 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/expires_lru_dict.py
--rw-r--r--   0        0        0       95 2023-04-26 10:41:42.825893 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/format.py
--rw-r--r--   0        0        0      494 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/lazy_delegation.py
--rw-r--r--   0        0        0     4188 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/lifecycler.py
--rw-r--r--   0        0        0      776 2023-03-01 13:53:49.845581 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/nonebot.py
--rw-r--r--   0        0        0     8753 2023-03-15 03:26:56.198873 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/shared_agen.py
--rw-r--r--   0        0        0      384 2023-02-13 05:42:01.882870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/__init__.py
--rw-r--r--   0        0        0      866 2023-03-14 09:12:27.159625 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/config.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.883870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/protocol_dep/__init__.py
--rw-r--r--   0        0        0     5195 2023-03-23 15:08:25.496164 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/protocol_dep/authenticator.py
--rw-r--r--   0        0        0     5346 2023-03-23 15:08:25.498161 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/protocol_dep/post_dest.py
--rw-r--r--   0        0        0     2046 2023-02-14 03:32:29.855103 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/protocol_dep/postman.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.885870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/utils/__init__.py
--rw-r--r--   0        0        0     1083 2023-02-13 05:42:01.885870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/utils/card_builder.py
--rw-r--r--   0        0        0     1008 2023-02-13 05:42:01.886870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/utils/illust_card.py
--rw-r--r--   0        0        0      479 2023-04-26 08:29:16.962322 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/__init__.py
--rw-r--r--   0        0        0      896 2023-02-13 05:42:01.887870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/config.py
--rw-r--r--   0        0        0       20 2023-03-29 02:34:22.139710 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/handler/__init__.py
--rw-r--r--   0        0        0     1468 2023-03-29 02:34:22.140709 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/handler/poke.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.888870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/__init__.py
--rw-r--r--   0        0        0     1512 2023-02-14 03:32:29.856103 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/authenticator.py
--rw-r--r--   0        0        0     4845 2023-04-27 09:44:58.747904 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/post_dest.py
--rw-r--r--   0        0        0     4048 2023-04-27 09:45:35.643691 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/postman.py
--rw-r--r--   0        0        0    18812 1970-01-01 00:00:00.000000 nonebot_plugin_pixivbot-1.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-02-13 05:42:01.812872 nonebot_plugin_pixivbot-1.8.4/LICENSE
+-rw-r--r--   0        0        0     1825 2023-04-27 15:02:42.913096 nonebot_plugin_pixivbot-1.8.4/pyproject.toml
+-rw-r--r--   0        0        0    17595 2023-04-27 10:16:31.843054 nonebot_plugin_pixivbot-1.8.4/README.md
+-rw-r--r--   0        0        0     1192 2023-04-26 10:41:42.734890 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/__init__.py
+-rw-r--r--   0        0        0     7793 2023-04-27 09:37:04.739003 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/config.py
+-rw-r--r--   0        0        0     4411 2023-04-27 10:16:31.872054 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/context.py
+-rw-r--r--   0        0        0      443 2023-02-13 05:42:01.817870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/__init__.py
+-rw-r--r--   0        0        0       56 2023-02-13 05:42:01.817870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/errors.py
+-rw-r--r--   0        0        0     1515 2023-02-13 05:42:01.817870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/interval_task_repo.py
+-rw-r--r--   0        0        0      488 2023-04-26 10:41:42.735891 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/local_tag/__init__.py
+-rw-r--r--   0        0        0      535 2023-04-26 10:41:42.735891 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/local_tag/base.py
+-rw-r--r--   0        0        0     2643 2023-04-26 10:41:42.736891 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/local_tag/mongo.py
+-rw-r--r--   0        0        0     2702 2023-04-26 10:41:42.736891 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/local_tag/sql.py
+-rw-r--r--   0        0        0      541 2023-04-26 10:41:42.737892 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_binding/__init__.py
+-rw-r--r--   0        0        0      387 2023-04-26 10:41:42.737892 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_binding/base.py
+-rw-r--r--   0        0        0     2087 2023-04-26 10:41:42.738890 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_binding/mongo.py
+-rw-r--r--   0        0        0     2715 2023-04-26 10:41:42.739891 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_binding/sql.py
+-rw-r--r--   0        0        0      262 2023-02-13 05:42:01.821870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/__init__.py
+-rw-r--r--   0        0        0     1524 2023-02-13 05:42:01.822870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/base.py
+-rw-r--r--   0        0        0     1829 2023-04-26 10:41:42.739891 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/compressor.py
+-rw-r--r--   0        0        0      355 2023-02-13 05:42:01.822870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/enums.py
+-rw-r--r--   0        0        0      334 2023-02-13 05:42:01.823870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/errors.py
+-rw-r--r--   0        0        0     1036 2023-02-13 05:42:01.823870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/lazy_illust.py
+-rw-r--r--   0        0        0      826 2023-03-15 03:52:01.493698 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/__init__.py
+-rw-r--r--   0        0        0     2823 2023-03-15 03:26:56.195873 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/base.py
+-rw-r--r--   0        0        0     3419 2023-04-26 10:41:42.740890 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/dummy.py
+-rw-r--r--   0        0        0    31650 2023-04-26 10:41:42.820890 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo.py
+-rw-r--r--   0        0        0     4802 2023-04-26 08:33:36.389185 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo_models.py
+-rw-r--r--   0        0        0    33317 2023-04-26 10:41:42.821890 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql.py
+-rw-r--r--   0        0        0     3536 2023-04-26 08:33:36.390185 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql_models.py
+-rw-r--r--   0        0        0     9990 2023-04-26 10:41:42.822892 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator.py
+-rw-r--r--   0        0        0    22139 2023-04-26 10:41:42.822892 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator_repo.py
+-rw-r--r--   0        0        0      332 2023-04-26 10:41:42.823892 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/models.py
+-rw-r--r--   0        0        0    18821 2023-04-27 13:33:43.566359 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/remote_repo.py
+-rw-r--r--   0        0        0     1079 2023-02-13 05:42:01.829870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/__init__.py
+-rw-r--r--   0        0        0     1820 2023-02-13 05:42:01.830870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/lifecycle_mixin.py
+-rw-r--r--   0        0        0     3211 2023-02-13 05:42:01.830870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/migration_manager.py
+-rw-r--r--   0        0        0     5774 2023-04-26 10:41:42.787891 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/mongo/__init__.py
+-rw-r--r--   0        0        0      290 2023-04-26 10:41:42.743890 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/mongo/meta_info.py
+-rw-r--r--   0        0        0      693 2023-02-13 05:42:01.833870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/mongo/migration/__init__.py
+-rw-r--r--   0        0        0     1424 2023-02-13 05:42:01.833870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v1_to_v2.py
+-rw-r--r--   0        0        0      674 2023-02-13 05:42:01.833870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v2_to_v3.py
+-rw-r--r--   0        0        0     2729 2023-02-13 05:42:01.834869 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v3_to_v4.py
+-rw-r--r--   0        0        0     1039 2023-02-13 05:42:01.834869 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v4_to_v5.py
+-rw-r--r--   0        0        0     3306 2023-02-13 05:42:01.834869 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v5_to_v6.py
+-rw-r--r--   0        0        0      416 2023-02-13 05:42:01.835870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v6_to_v7.py
+-rw-r--r--   0        0        0     5781 2023-04-26 10:41:42.788890 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/sql/__init__.py
+-rw-r--r--   0        0        0      306 2023-03-13 13:51:04.755048 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/sql/meta_info.py
+-rw-r--r--   0        0        0      457 2023-02-13 05:42:01.837870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/sql/migration/__init__.py
+-rw-r--r--   0        0        0     3824 2023-02-13 05:42:01.838869 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v1_to_v2.py
+-rw-r--r--   0        0        0     1842 2023-02-13 05:42:01.839869 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v2_to_v3.py
+-rw-r--r--   0        0        0      360 2023-02-13 05:42:01.839869 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v3_to_v4.py
+-rw-r--r--   0        0        0      520 2023-04-26 10:41:42.744892 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/subscription/__init__.py
+-rw-r--r--   0        0        0      177 2023-04-26 10:41:42.745891 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/subscription/base.py
+-rw-r--r--   0        0        0     4446 2023-04-26 10:41:42.745891 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/subscription/mongo.py
+-rw-r--r--   0        0        0     5698 2023-04-26 10:41:42.746890 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/subscription/sql.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.842870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/utils/__init__.py
+-rw-r--r--   0        0        0      164 2023-02-13 05:42:01.842870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/utils/shortuuid.py
+-rw-r--r--   0        0        0      814 2023-02-13 05:42:01.843869 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/utils/sql/__init__.py
+-rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843869 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/utils/sql/utc_datetime.py
+-rw-r--r--   0        0        0      720 2023-02-13 05:42:01.842870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/utils/sql.pyi
+-rw-r--r--   0        0        0      517 2023-04-26 10:41:42.747890 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/watch_task/__init__.py
+-rw-r--r--   0        0        0      226 2023-04-26 10:41:42.747890 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/watch_task/base.py
+-rw-r--r--   0        0        0     5155 2023-04-26 10:41:42.748890 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/watch_task/mongo.py
+-rw-r--r--   0        0        0     6613 2023-04-26 10:41:42.748890 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/watch_task/sql.py
+-rw-r--r--   0        0        0      964 2023-03-15 03:24:39.857013 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/enums.py
+-rw-r--r--   0        0        0      102 2023-02-14 03:27:31.463009 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/global_context.py
+-rw-r--r--   0        0        0       92 2023-02-13 05:42:01.847870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/__init__.py
+-rw-r--r--   0        0        0     9597 2023-04-26 11:20:41.866640 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/base.py
+-rw-r--r--   0        0        0      308 2023-02-13 05:42:01.847870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/command/__init__.py
+-rw-r--r--   0        0        0     2489 2023-04-26 11:20:41.835065 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/command/bind.py
+-rw-r--r--   0        0        0     2481 2023-03-29 02:34:22.114209 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/command/command.py
+-rw-r--r--   0        0        0     1207 2023-04-26 11:20:41.815065 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/command/help.py
+-rw-r--r--   0        0        0      804 2023-04-26 11:20:41.870642 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/command/invalidate_cache.py
+-rw-r--r--   0        0        0     4291 2023-04-26 11:28:38.961827 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/command/schedule.py
+-rw-r--r--   0        0        0     1363 2023-03-29 02:34:22.116335 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/command/subcommand.py
+-rw-r--r--   0        0        0     6050 2023-04-26 11:28:38.966828 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/command/watch.py
+-rw-r--r--   0        0        0      633 2023-02-13 05:42:01.851870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/common/__init__.py
+-rw-r--r--   0        0        0      688 2023-03-29 02:34:22.117934 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/common/base.py
+-rw-r--r--   0        0        0     1629 2023-04-26 11:11:55.420381 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/common/illust.py
+-rw-r--r--   0        0        0     1440 2023-04-26 11:20:41.831066 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/common/more.py
+-rw-r--r--   0        0        0     2817 2023-04-26 11:20:41.858064 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/common/random_bookmark.py
+-rw-r--r--   0        0        0     1752 2023-04-26 11:20:41.846065 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/common/random_illust.py
+-rw-r--r--   0        0        0     1599 2023-04-26 11:20:41.862066 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/common/random_recommended_illust.py
+-rw-r--r--   0        0        0     2006 2023-04-26 11:20:41.839065 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/common/random_related_illust.py
+-rw-r--r--   0        0        0     2089 2023-04-26 11:20:41.819065 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/common/random_user_illust.py
+-rw-r--r--   0        0        0     4204 2023-04-26 11:20:41.854065 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/common/ranking.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.857869 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/interceptor/__init__.py
+-rw-r--r--   0        0        0      524 2023-03-29 02:34:22.124122 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/interceptor/base.py
+-rw-r--r--   0        0        0     2012 2023-03-29 02:34:22.125123 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/interceptor/combined_interceptor.py
+-rw-r--r--   0        0        0     1601 2023-04-27 13:28:45.858775 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/interceptor/default_error_interceptor.py
+-rw-r--r--   0        0        0     1134 2023-03-29 02:34:22.126120 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/interceptor/loading_prompt_interceptor.py
+-rw-r--r--   0        0        0     1947 2023-03-29 02:34:54.094101 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/interceptor/permission_interceptor.py
+-rw-r--r--   0        0        0      654 2023-03-29 02:34:22.127120 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/interceptor/record_req_interceptor.py
+-rw-r--r--   0        0        0      938 2023-04-27 15:02:23.301078 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/interceptor/retry_interceptor.py
+-rw-r--r--   0        0        0     1526 2023-03-29 02:34:22.128120 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/interceptor/service_interceptor.py
+-rw-r--r--   0        0        0      673 2023-03-29 02:34:22.129121 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/interceptor/timeout_interceptor.py
+-rw-r--r--   0        0        0      201 2023-02-13 05:42:01.861870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/pkg_context.py
+-rw-r--r--   0        0        0     3378 2023-04-26 10:41:42.749891 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/recorder.py
+-rw-r--r--   0        0        0      325 2023-02-14 11:56:02.041347 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/schedule/__init__.py
+-rw-r--r--   0        0        0      349 2023-04-26 11:20:41.850065 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/schedule/base.py
+-rw-r--r--   0        0        0      461 2023-03-29 02:34:22.131121 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/schedule/random_bookmark.py
+-rw-r--r--   0        0        0      453 2023-03-29 02:34:22.131121 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/schedule/random_illust.py
+-rw-r--r--   0        0        0      498 2023-03-29 02:34:22.132122 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/schedule/random_recommended_illust.py
+-rw-r--r--   0        0        0      470 2023-03-29 02:34:22.132122 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/schedule/random_user_illust.py
+-rw-r--r--   0        0        0      432 2023-03-29 02:34:22.133120 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/schedule/ranking.py
+-rw-r--r--   0        0        0       27 2023-02-13 05:42:01.862870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/sniffer/__init__.py
+-rw-r--r--   0        0        0     1011 2023-04-26 11:20:41.843065 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/sniffer/illust_link.py
+-rw-r--r--   0        0        0     1382 2023-02-13 05:42:01.863870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/utils.py
+-rw-r--r--   0        0        0      112 2023-02-14 12:15:47.490983 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/watch/__init__.py
+-rw-r--r--   0        0        0      865 2023-04-26 11:20:41.827066 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/watch/base.py
+-rw-r--r--   0        0        0     2498 2023-04-26 10:41:42.749891 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/watch/following_illusts.py
+-rw-r--r--   0        0        0     1864 2023-04-26 10:41:42.750890 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/watch/user_illusts.py
+-rw-r--r--   0        0        0      530 2023-02-13 05:42:01.865869 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/model/__init__.py
+-rw-r--r--   0        0        0     1366 2023-02-13 05:42:01.865869 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/model/identifier.py
+-rw-r--r--   0        0        0     1858 2023-04-27 09:18:54.765186 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/model/illust.py
+-rw-r--r--   0        0        0      352 2023-02-13 05:42:01.866870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/model/interval_task.py
+-rw-r--r--   0        0        0      157 2023-02-13 05:42:01.867870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/model/message/__init__.py
+-rw-r--r--   0        0        0     2623 2023-02-13 05:42:01.867870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/model/message/illust_message.py
+-rw-r--r--   0        0        0     2443 2023-02-13 05:42:01.867870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/model/message/illust_messages.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.868870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/model/old/__init__.py
+-rw-r--r--   0        0        0      120 2023-02-13 05:42:01.868870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/model/old/pixiv_binding.py
+-rw-r--r--   0        0        0      950 2023-02-13 05:42:01.868870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/model/old/subscription.py
+-rw-r--r--   0        0        0      242 2023-02-13 05:42:01.869870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/model/pixiv_binding.py
+-rw-r--r--   0        0        0     1450 2023-04-26 10:52:37.464803 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/model/subscription.py
+-rw-r--r--   0        0        0      203 2023-02-13 05:42:01.870869 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/model/tag.py
+-rw-r--r--   0        0        0      131 2023-02-13 05:42:01.870869 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/model/user.py
+-rw-r--r--   0        0        0      242 2023-02-13 05:42:01.871622 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/model/user_preview.py
+-rw-r--r--   0        0        0     1004 2023-04-26 10:52:37.460801 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/model/watch_task.py
+-rw-r--r--   0        0        0     1680 2023-02-14 03:39:10.628376 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/plugin_service.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.872870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/protocol_dep/__init__.py
+-rw-r--r--   0        0        0      914 2023-03-14 09:12:27.158624 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/protocol_dep/authenticator.py
+-rw-r--r--   0        0        0     2757 2023-03-29 02:34:22.136711 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/protocol_dep/post_dest.py
+-rw-r--r--   0        0        0     1445 2023-02-14 03:32:29.851104 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/protocol_dep/postman.py
+-rw-r--r--   0        0        0     1452 2023-02-14 03:32:29.852102 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/protocol_dep/protocol_dep.py
+-rw-r--r--   0        0        0       49 2023-02-13 05:42:01.874870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/service/__init__.py
+-rw-r--r--   0        0        0     5470 2023-04-27 13:38:00.669631 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/service/interval_task_worker.py
+-rw-r--r--   0        0        0      958 2023-04-26 10:41:42.751891 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/service/pixiv_account_binder.py
+-rw-r--r--   0        0        0     6023 2023-04-26 10:41:42.751891 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/service/pixiv_service.py
+-rw-r--r--   0        0        0     2244 2023-02-13 05:42:01.877869 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/service/roulette.py
+-rw-r--r--   0        0        0     5640 2023-04-26 10:41:42.752891 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/service/scheduler.py
+-rw-r--r--   0        0        0     3821 2023-04-26 10:41:42.752891 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/service/watchman.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.878870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/utils/__init__.py
+-rw-r--r--   0        0        0      230 2023-03-29 02:34:22.138709 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/utils/algorithm.py
+-rw-r--r--   0        0        0      265 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/utils/coros.py
+-rw-r--r--   0        0        0     1148 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/utils/decode_integer.py
+-rw-r--r--   0        0        0      515 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/utils/errors.py
+-rw-r--r--   0        0        0     3604 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/utils/expires_lru_dict.py
+-rw-r--r--   0        0        0       95 2023-04-26 10:41:42.825893 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/utils/format.py
+-rw-r--r--   0        0        0      494 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/utils/lazy_delegation.py
+-rw-r--r--   0        0        0     4188 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/utils/lifecycler.py
+-rw-r--r--   0        0        0      776 2023-03-01 13:53:49.845581 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/utils/nonebot.py
+-rw-r--r--   0        0        0     8653 2023-04-27 14:59:21.481094 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/utils/shared_agen.py
+-rw-r--r--   0        0        0      384 2023-02-13 05:42:01.882870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_kook/__init__.py
+-rw-r--r--   0        0        0      866 2023-03-14 09:12:27.159625 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_kook/config.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.883870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_kook/protocol_dep/__init__.py
+-rw-r--r--   0        0        0     5195 2023-03-23 15:08:25.496164 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_kook/protocol_dep/authenticator.py
+-rw-r--r--   0        0        0     5346 2023-03-23 15:08:25.498161 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_kook/protocol_dep/post_dest.py
+-rw-r--r--   0        0        0     2046 2023-02-14 03:32:29.855103 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_kook/protocol_dep/postman.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.885870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_kook/utils/__init__.py
+-rw-r--r--   0        0        0     1083 2023-02-13 05:42:01.885870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_kook/utils/card_builder.py
+-rw-r--r--   0        0        0     1008 2023-02-13 05:42:01.886870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_kook/utils/illust_card.py
+-rw-r--r--   0        0        0      479 2023-04-26 08:29:16.962322 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_onebot_v11/__init__.py
+-rw-r--r--   0        0        0      896 2023-02-13 05:42:01.887870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_onebot_v11/config.py
+-rw-r--r--   0        0        0       20 2023-03-29 02:34:22.139710 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_onebot_v11/handler/__init__.py
+-rw-r--r--   0        0        0     1468 2023-03-29 02:34:22.140709 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_onebot_v11/handler/poke.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.888870 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/__init__.py
+-rw-r--r--   0        0        0     1512 2023-02-14 03:32:29.856103 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/authenticator.py
+-rw-r--r--   0        0        0     4845 2023-04-27 09:44:58.747904 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/post_dest.py
+-rw-r--r--   0        0        0     4028 2023-04-27 13:34:24.653172 nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/postman.py
+-rw-r--r--   0        0        0    19121 1970-01-01 00:00:00.000000 nonebot_plugin_pixivbot-1.8.4/PKG-INFO
```

### Comparing `nonebot_plugin_pixivbot-1.8.3/LICENSE` & `nonebot_plugin_pixivbot-1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/pyproject.toml` & `nonebot_plugin_pixivbot-1.8.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-pixivbot"
-version = "1.8.3"
+version = "1.8.4"
 description = "Nonebot Plugin PixivBot"
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/ssttkkl/nonebot-plugin-pixivbot"
 packages = [
     { include = "nonebot_plugin_pixivbot", from = "src" },
```

### Comparing `nonebot_plugin_pixivbot-1.8.3/README.md` & `nonebot_plugin_pixivbot-1.8.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -173,24 +173,36 @@
 
 **遇到问题时请先尝试执行`pip install nonebot-plugin-pixivbot -U`更新到最新版本**。
 
 Issue请尽可能带上详细的日志、配置文件与环境信息。功能请求请移步Discussion。
 
 ### 内部错误：<class 'pixivpy_async.error.NoTokenError'>No access_token Found!
 
-没登录成功，多半是网络问题
+没登录成功，多半是网络问题。在国内请配置代理。
 
 如果登录成功的话会在bot初始化后有这几句：
 
 ```
 03-13 11:19:36 [SUCCESS] nonebot_plugin_pixivbot | refresh access token successfully. new token expires in 3600 seconds.
 03-13 11:19:36 [DEBUG] nonebot_plugin_pixivbot | access_token: ***************
 03-13 11:19:36 [DEBUG] nonebot_plugin_pixivbot | refresh_token: *****************
 ```
 
+### 如何配置代理
+
+将`pixiv_proxy`配置项设为代理服务器地址（支持http、socks5协议）
+
+```
+pixiv_proxy=socks5://127.0.0.1:7890
+```
+
+### 发送合并转发消息惨遭风控
+
+将`pixiv_onebot_send_forward_message`配置项设为`never`可禁用合并转发
+
 ### 内部错误：<class 'sqlalchemy.exc.OperationalError'>(sqlite3.OperationalError) near "ON": syntax error
 
 多半是SQLite版本过低，不支持ON CONFLICT子句，如果是Linux系统请更新安装的SQLite版本
 
 ## 配置项一览
 
 最小配置：
```

#### html2text {}

```diff
@@ -113,20 +113,25 @@
 ``` å·ä½å¯ä»¥åè[nonebot-plugin-access-control](https://github.com/
 ssttkkl/nonebot-plugin-access-control)çææ¡£è¿è¡æéæ§å¶ã ##
 å¸¸è§é®é¢ **éå°é®é¢æ¶è¯·åå°è¯æ§è¡`pip install nonebot-plugin-
 pixivbot -U`æ´æ°å°ææ°çæ¬**ã
 Issueè¯·å°½å¯è½å¸¦ä¸è¯¦ç»çæ¥å¿ãéç½®æä»¶ä¸ç¯å¢ä¿¡æ¯ãåè½è¯·æ±è¯·ç§»æ­¥Discussionã
 ### åé¨éè¯¯ï¼
 pixivpy_async.error.NoTokenError'>No access_token Found!
-æ²¡ç»å½æåï¼å¤åæ¯ç½ç»é®é¢
+æ²¡ç»å½æåï¼å¤åæ¯ç½ç»é®é¢ãå¨å½åè¯·éç½®ä»£çã
 å¦æç»å½æåçè¯ä¼å¨botåå§ååæè¿å å¥ï¼ ``` 03-13 11:19:36
 [SUCCESS] nonebot_plugin_pixivbot | refresh access token successfully. new
 token expires in 3600 seconds. 03-13 11:19:36 [DEBUG] nonebot_plugin_pixivbot |
 access_token: *************** 03-13 11:19:36 [DEBUG] nonebot_plugin_pixivbot |
-refresh_token: ***************** ``` ### åé¨éè¯¯ï¼
+refresh_token: ***************** ``` ### å¦ä½éç½®ä»£ç
+å°`pixiv_proxy`éç½®é¡¹è®¾ä¸ºä»£çæå¡å¨å°åï¼æ¯æhttpãsocks5åè®®ï¼
+``` pixiv_proxy=socks5://127.0.0.1:7890 ``` ###
+åéåå¹¶è½¬åæ¶æ¯æ¨é­é£æ§
+å°`pixiv_onebot_send_forward_message`éç½®é¡¹è®¾ä¸º`never`å¯ç¦ç¨åå¹¶è½¬å
+### åé¨éè¯¯ï¼
 sqlalchemy.exc.OperationalError'>(sqlite3.OperationalError) near "ON": syntax
 error å¤åæ¯SQLiteçæ¬è¿ä½ï¼ä¸æ¯æON
 CONFLICTå­å¥ï¼å¦ææ¯Linuxç³»ç»è¯·æ´æ°å®è£çSQLiteçæ¬ ##
 éç½®é¡¹ä¸è§ æå°éç½®ï¼ ``` pixiv_refresh_token= #
 åé¢è·åçREFRESH_TOKEN ```
 é¤æå°éç½®åºç°çéç½®é¡¹ä»¥å¤é½æ¯å¯éé¡¹ï¼ç»åºçæ¯é»è®¤å¼ï¼å»ºè®®åªå°èªå·±éè¦çé¡¹å å¥.env.prodæä»¶
 å®æ´éç½®ï¼ ``` # æ°æ®åºéç½® pixiv_data_source= #
```

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/__init__.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/config.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/context.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from typing import TypeVar, Type, Callable, Union, Generic
+from typing import TypeVar, Type, Callable, Union, Generic, Dict
 
 from nonebot.log import logger
 
 T = TypeVar("T")
 T2 = TypeVar("T2")
 
 
@@ -38,15 +38,15 @@
             self._cached = True
         return self._cache
 
 
 class Context:
     def __init__(self, parent: "Context" = None):
         self._parent = parent
-        self._container = {}
+        self._container: Dict[T, Provider[T]] = {}
 
     @property
     def parent(self) -> "Context":
         return self._parent
 
     @property
     def root(self) -> "Context":
@@ -104,15 +104,15 @@
             return True
         return False
 
     def bind(self, key: Type[T], src_key: Type[T2]):
         """
         bind key (usually the implementation class) to src_key (usually the base class)
         """
-        self._container[key] = self._find_provider(src_key)
+        self._container[key] = DynamicProvider(lambda: self._find_provider(src_key).provide(), use_cache=False)
         logger.trace(f"bind bean {key} to {src_key}")
 
     def bind_singleton_to(self, key: Type[T], *args, **kwargs) -> Callable[[Type[T2]], Type[T2]]:
         """
         decorator for a class (usually the implementation class) to bind to another class (usually the base class)
         """
 
@@ -122,15 +122,15 @@
             return cls
 
         return decorator
 
     def require(self, key: Type[T]) -> T:
         return self._find_provider(key).provide()
 
-    def _find_provider(self, key: Type[T]) -> T:
+    def _find_provider(self, key: Type[T]) -> Provider[T]:
         if key in self._container:
             return self._container[key]
         elif self._parent is not None:
             return self._parent._find_provider(key)
         else:
             raise KeyError(key)
 
@@ -142,8 +142,8 @@
             return True
         elif self._parent is not None:
             return self._parent.__contains__(key)
         else:
             return False
 
 
-__all__ = ("Context", )
+__all__ = ("Context",)
```

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/interval_task_repo.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/interval_task_repo.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/local_tag/base.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/local_tag/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/local_tag/mongo.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/local_tag/mongo.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/local_tag/sql.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/local_tag/sql.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_binding/__init__.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_binding/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_binding/mongo.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_binding/mongo.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_binding/sql.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_binding/sql.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/base.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/compressor.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/compressor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/lazy_illust.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/lazy_illust.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/__init__.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/base.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/dummy.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/dummy.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo_models.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo_models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql_models.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql_models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator_repo.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator_repo.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/remote_repo.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/pixiv_repo/remote_repo.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,17 +87,15 @@
         while True:
             try:
                 result = await self._refresh()
                 await sleep(result.expires_in * 0.8)
             except CancelledError as e:
                 raise e
             except Exception as e:
-                logger.error(
-                    "failed to refresh access token, will retry in 60s.")
-                logger.exception(e)
+                logger.opt(exception=e).error("failed to refresh access token, will retry after 60s.")
                 await sleep(60)
 
     def start(self):
         self._pclient = PixivClient(proxy=_conf.pixiv_proxy, timeout=_conf.pixiv_query_timeout)
         self._papi = AppPixivAPI(client=self._pclient.start())
         self._papi.set_additional_headers({'Accept-Language': 'zh-CN'})
         self._refresh_daemon = create_task(self._refresh_daemon_worker())
```

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/__init__.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/lifecycle_mixin.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/lifecycle_mixin.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/migration_manager.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/migration_manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/__init__.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/__init__.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/mongo/migration/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v1_to_v2.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v1_to_v2.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v2_to_v3.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v2_to_v3.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v3_to_v4.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v3_to_v4.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v4_to_v5.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v4_to_v5.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v5_to_v6.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v5_to_v6.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/sql/__init__.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v1_to_v2.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v1_to_v2.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v2_to_v3.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v2_to_v3.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/subscription/__init__.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/subscription/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/subscription/mongo.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/subscription/mongo.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/subscription/sql.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/subscription/sql.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/utils/sql/__init__.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/utils/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/utils/sql/utc_datetime.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/utils/sql/utc_datetime.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/utils/sql.pyi` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/utils/sql.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/watch_task/__init__.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/watch_task/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/watch_task/mongo.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/watch_task/mongo.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/watch_task/sql.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/data/watch_task/sql.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/enums.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/enums.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/base.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/bind.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/command/bind.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/command.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/command/command.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/help.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/command/help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/invalidate_cache.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/command/invalidate_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/schedule.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/command/schedule.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/subcommand.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/command/subcommand.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/watch.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/command/watch.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/__init__.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/base.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/common/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/illust.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/common/illust.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/more.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/common/more.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/random_bookmark.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/common/random_bookmark.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/random_illust.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/common/random_illust.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/random_recommended_illust.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/common/random_recommended_illust.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/random_related_illust.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/common/random_related_illust.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/random_user_illust.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/common/random_user_illust.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/ranking.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/common/ranking.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/base.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/interceptor/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/combined_interceptor.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/interceptor/combined_interceptor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/default_error_interceptor.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/interceptor/default_error_interceptor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 import asyncio
 from typing import Callable, TYPE_CHECKING
 
 from aiohttp import ServerConnectionError
 from nonebot import logger
 from nonebot.exception import ActionFailed
+from pixivpy_async.error import NoTokenError
 
-from nonebot_plugin_pixivbot.utils.errors import BadRequestError, QueryError
+from nonebot_plugin_pixivbot.utils.errors import BadRequestError, QueryError, RateLimitError
 from .base import Interceptor
 from ..pkg_context import context
 
 if TYPE_CHECKING:
     from nonebot_plugin_pixivbot.handler.base import Handler
 
 
 @context.register_singleton()
 class DefaultErrorInterceptor(Interceptor):
     async def intercept(self, handler: "Handler", wrapped_func: Callable, *args, **kwargs):
         try:
             await wrapped_func(*args, **kwargs)
-        except (asyncio.TimeoutError, ServerConnectionError, ConnectionError) as e:
+        except (NoTokenError,
+                RateLimitError,
+                asyncio.TimeoutError,
+                ServerConnectionError,
+                ConnectionError) as e:
             logger.warning(e)
             if not handler.silently:
-                await handler.post_plain_text("网络错误")
+                await handler.post_plain_text(f"网络错误，请稍后再试（<{type(e).__name__}> {e}）")
         except (BadRequestError, QueryError) as e:
             if not handler.silently:
                 await handler.post_plain_text(str(e))
         except ActionFailed as e:
             # 避免当发送消息错误时再尝试发送
             raise e
         except Exception as e:
             if not handler.silently:
-                await handler.post_plain_text(f"内部错误：{type(e)}{e}")
+                await handler.post_plain_text(f"内部错误：<{type(e).__name__}> {e}")
             raise e  # 重新抛出，让上层可以处理（如scheduler中需要处理Handler的异常）
```

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/loading_prompt_interceptor.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/interceptor/loading_prompt_interceptor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/permission_interceptor.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/interceptor/permission_interceptor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/record_req_interceptor.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/interceptor/record_req_interceptor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/retry_interceptor.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/interceptor/retry_interceptor.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,13 @@
     async def intercept(self, handler: "Handler", wrapped_func: Callable, *args, **kwargs):
         err = None
 
         for i in range(10):
             try:
                 return await wrapped_func(*args, **kwargs)
             except exception as e:
-                logger.error(f"Retrying... {i + 1}/10")
-                logger.exception(e)
+                logger.opt(exception=e).error(f"Network error occurred while handling, retrying... {i + 1}/10")
                 err = e
             except Exception as e:
                 raise e
 
         raise err
```

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/service_interceptor.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/interceptor/service_interceptor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/timeout_interceptor.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/interceptor/timeout_interceptor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/recorder.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/recorder.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/sniffer/illust_link.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/sniffer/illust_link.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/utils.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/watch/base.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/watch/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/watch/following_illusts.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/watch/following_illusts.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/watch/user_illusts.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/handler/watch/user_illusts.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/__init__.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/model/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/identifier.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/model/identifier.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/illust.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/model/illust.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/message/illust_message.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/model/message/illust_message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/message/illust_messages.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/model/message/illust_messages.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/old/subscription.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/model/old/subscription.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/subscription.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/model/subscription.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/watch_task.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/model/watch_task.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/plugin_service.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/plugin_service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/protocol_dep/authenticator.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/protocol_dep/authenticator.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/protocol_dep/post_dest.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/protocol_dep/post_dest.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/protocol_dep/postman.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/protocol_dep/postman.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/protocol_dep/protocol_dep.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/protocol_dep/protocol_dep.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/interval_task_worker.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/service/interval_task_worker.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,25 +33,23 @@
     def __init__(self):
         @on_bot_connect(replay=True)
         async def _(bot: Bot):
             async for task in self.repo.get_by_bot(get_bot_user_identifier(bot)):
                 try:
                     self._add_job(task)
                 except Exception as e:
-                    logger.error(f"[{self.tag}] error occurred when adding job for task \"{task}\"")
-                    logger.exception(e)
+                    logger.opt(exception=e).error(f"[{self.tag}] error occurred when adding job for task \"{task}\"")
 
         @on_bot_disconnect()
         async def _(bot: Bot):
             async for task in self.repo.get_by_bot(get_bot_user_identifier(bot)):
                 try:
                     self._remove_job(task)
                 except Exception as e:
-                    logger.error(f"[{self.tag}] error occurred when removing job for task \"{task}\"")
-                    logger.exception(e)
+                    logger.opt(exception=e).error(f"[{self.tag}] error occurred when removing job for task \"{task}\"")
 
     @classmethod
     def _make_job_id(cls, item: T):
         return f'{cls.tag} {item.subscriber} {item.code}'
 
     @abstractmethod
     async def _handle_trigger(self, item: T, post_dest: PostDestination[T_UID, T_GID]):
@@ -62,15 +60,15 @@
 
         bot = get_bot(item.bot.user_id)
         post_dest = pd_factory_mgr.build(bot, item.subscriber.user_id, item.subscriber.group_id)
 
         try:
             await self._handle_trigger(item, post_dest)
         except ActionFailed as e:
-            logger.error(f"[{self.tag}] ActionFailed {e}")
+            logger.opt(exception=e).error(f"[{self.tag}] action failed when handling task \"{item.code}\"")
 
             available = auth_mgr.available(post_dest)
             if isawaitable(available):
                 available = await available
 
             if not available:
                 logger.info(f"[{self.tag}] {post_dest} is no longer available, removing all his tasks...")
```

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/pixiv_account_binder.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/service/pixiv_account_binder.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/pixiv_service.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/service/pixiv_service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/roulette.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/service/roulette.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/scheduler.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/service/scheduler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/watchman.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/service/watchman.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/decode_integer.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/utils/decode_integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/errors.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/utils/errors.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/expires_lru_dict.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/utils/expires_lru_dict.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/lifecycler.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/utils/lifecycler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/nonebot.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/utils/nonebot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/shared_agen.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot/utils/shared_agen.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,14 @@
                             try:
                                 new_data = await self._origin.__anext__()
                             except StopAsyncIteration:
                                 self._stopped = True
                                 await self._manager.on_agen_stop(self._identifier, self._got_items)
                                 break
                             except Exception as e:
-                                logger.error(f"error {type(e)} raised by agen {self._identifier}")
                                 await self._manager.on_agen_error(self._identifier, e)
                                 raise e
 
                             await self._manager.on_agen_next(self._identifier, new_data)
 
                             self._got_items.append(new_data)
                             self._got += 1
```

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/config.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_kook/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/protocol_dep/authenticator.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_kook/protocol_dep/authenticator.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/protocol_dep/post_dest.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_kook/protocol_dep/post_dest.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/protocol_dep/postman.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_kook/protocol_dep/postman.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/utils/card_builder.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_kook/utils/card_builder.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/utils/illust_card.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_kook/utils/illust_card.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/config.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_onebot_v11/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/handler/poke.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_onebot_v11/handler/poke.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/authenticator.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/authenticator.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/post_dest.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/post_dest.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/postman.py` & `nonebot_plugin_pixivbot-1.8.4/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/postman.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,17 @@
 
 
 @asynccontextmanager
 async def feedback_on_action_failed(post_dest: PostDestination):
     try:
         yield
     except ActionFailed as e:
-        logger.error("图片发送失败，可能是机器人被风控")
-        logger.error(e)
+        logger.opt(exception=e).error("发送失败，可能是机器人被风控")
 
-        await post_dest.post_single(Message([MessageSegment.text("图片发送失败，可能是机器人被风控")]))
+        await post_dest.post_single(Message([MessageSegment.text("发送失败，可能是机器人被风控")]))
 
 
 @context.register_singleton()
 class Postman(BasePostman[int, int], manager=PostmanManager):
     adapter = "onebot"
 
     def make_illust_msg(self, model: IllustMessageModel) -> Message:
```

### Comparing `nonebot_plugin_pixivbot-1.8.3/PKG-INFO` & `nonebot_plugin_pixivbot-1.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pixivbot
-Version: 1.8.3
+Version: 1.8.4
 Summary: Nonebot Plugin PixivBot
 Home-page: https://github.com/ssttkkl/nonebot-plugin-pixivbot
 License: MIT
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -217,24 +217,36 @@
 
 **遇到问题时请先尝试执行`pip install nonebot-plugin-pixivbot -U`更新到最新版本**。
 
 Issue请尽可能带上详细的日志、配置文件与环境信息。功能请求请移步Discussion。
 
 ### 内部错误：<class 'pixivpy_async.error.NoTokenError'>No access_token Found!
 
-没登录成功，多半是网络问题
+没登录成功，多半是网络问题。在国内请配置代理。
 
 如果登录成功的话会在bot初始化后有这几句：
 
 ```
 03-13 11:19:36 [SUCCESS] nonebot_plugin_pixivbot | refresh access token successfully. new token expires in 3600 seconds.
 03-13 11:19:36 [DEBUG] nonebot_plugin_pixivbot | access_token: ***************
 03-13 11:19:36 [DEBUG] nonebot_plugin_pixivbot | refresh_token: *****************
 ```
 
+### 如何配置代理
+
+将`pixiv_proxy`配置项设为代理服务器地址（支持http、socks5协议）
+
+```
+pixiv_proxy=socks5://127.0.0.1:7890
+```
+
+### 发送合并转发消息惨遭风控
+
+将`pixiv_onebot_send_forward_message`配置项设为`never`可禁用合并转发
+
 ### 内部错误：<class 'sqlalchemy.exc.OperationalError'>(sqlite3.OperationalError) near "ON": syntax error
 
 多半是SQLite版本过低，不支持ON CONFLICT子句，如果是Linux系统请更新安装的SQLite版本
 
 ## 配置项一览
 
 最小配置：
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-pixivbot Version: 1.8.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-pixivbot Version: 1.8.4 Summary:
 Nonebot Plugin PixivBot Home-page: https://github.com/ssttkkl/nonebot-plugin-
 pixivbot License: MIT Author: ssttkkl Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Provides-Extra: kook
 Provides-Extra: mongo Provides-Extra: onebot Provides-Extra: postgresql
@@ -139,20 +139,25 @@
 ``` å·ä½å¯ä»¥åè[nonebot-plugin-access-control](https://github.com/
 ssttkkl/nonebot-plugin-access-control)çææ¡£è¿è¡æéæ§å¶ã ##
 å¸¸è§é®é¢ **éå°é®é¢æ¶è¯·åå°è¯æ§è¡`pip install nonebot-plugin-
 pixivbot -U`æ´æ°å°ææ°çæ¬**ã
 Issueè¯·å°½å¯è½å¸¦ä¸è¯¦ç»çæ¥å¿ãéç½®æä»¶ä¸ç¯å¢ä¿¡æ¯ãåè½è¯·æ±è¯·ç§»æ­¥Discussionã
 ### åé¨éè¯¯ï¼
 pixivpy_async.error.NoTokenError'>No access_token Found!
-æ²¡ç»å½æåï¼å¤åæ¯ç½ç»é®é¢
+æ²¡ç»å½æåï¼å¤åæ¯ç½ç»é®é¢ãå¨å½åè¯·éç½®ä»£çã
 å¦æç»å½æåçè¯ä¼å¨botåå§ååæè¿å å¥ï¼ ``` 03-13 11:19:36
 [SUCCESS] nonebot_plugin_pixivbot | refresh access token successfully. new
 token expires in 3600 seconds. 03-13 11:19:36 [DEBUG] nonebot_plugin_pixivbot |
 access_token: *************** 03-13 11:19:36 [DEBUG] nonebot_plugin_pixivbot |
-refresh_token: ***************** ``` ### åé¨éè¯¯ï¼
+refresh_token: ***************** ``` ### å¦ä½éç½®ä»£ç
+å°`pixiv_proxy`éç½®é¡¹è®¾ä¸ºä»£çæå¡å¨å°åï¼æ¯æhttpãsocks5åè®®ï¼
+``` pixiv_proxy=socks5://127.0.0.1:7890 ``` ###
+åéåå¹¶è½¬åæ¶æ¯æ¨é­é£æ§
+å°`pixiv_onebot_send_forward_message`éç½®é¡¹è®¾ä¸º`never`å¯ç¦ç¨åå¹¶è½¬å
+### åé¨éè¯¯ï¼
 sqlalchemy.exc.OperationalError'>(sqlite3.OperationalError) near "ON": syntax
 error å¤åæ¯SQLiteçæ¬è¿ä½ï¼ä¸æ¯æON
 CONFLICTå­å¥ï¼å¦ææ¯Linuxç³»ç»è¯·æ´æ°å®è£çSQLiteçæ¬ ##
 éç½®é¡¹ä¸è§ æå°éç½®ï¼ ``` pixiv_refresh_token= #
 åé¢è·åçREFRESH_TOKEN ```
 é¤æå°éç½®åºç°çéç½®é¡¹ä»¥å¤é½æ¯å¯éé¡¹ï¼ç»åºçæ¯é»è®¤å¼ï¼å»ºè®®åªå°èªå·±éè¦çé¡¹å å¥.env.prodæä»¶
 å®æ´éç½®ï¼ ``` # æ°æ®åºéç½® pixiv_data_source= #
```

