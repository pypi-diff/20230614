# Comparing `tmp/aunly-bbot-1.4.1.tar.gz` & `tmp/aunly-bbot-1.5.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aunly-bbot-1.4.1.tar", last modified: Tue Jun 13 05:30:07 2023, max compression
+gzip compressed data, was "aunly-bbot-1.5.0b1.tar", last modified: Wed Jun 14 07:43:49 2023, max compression
```

## Comparing `aunly-bbot-1.4.1.tar` & `aunly-bbot-1.5.0b1.tar`

### file list

```diff
@@ -1,104 +1,105 @@
--rwxr-xr-x   0        0        0    34523 2023-06-13 05:29:56.165277 aunly-bbot-1.4.1/LICENSE
--rw-r--r--   0        0        0       61 2023-06-13 05:29:56.165277 aunly-bbot-1.4.1/aunly_bbot/__main__.py
--rw-r--r--   0        0        0     3361 2023-06-13 05:29:56.165277 aunly-bbot-1.4.1/aunly_bbot/bot.py
--rw-r--r--   0        0        0     1753 2023-06-13 05:29:56.165277 aunly-bbot-1.4.1/aunly_bbot/cli/__init__.py
--rw-r--r--   0        0        0     2197 2023-06-13 05:29:56.165277 aunly-bbot-1.4.1/aunly_bbot/cli/api.py
--rw-r--r--   0        0        0    22595 2023-06-13 05:29:56.165277 aunly-bbot-1.4.1/aunly_bbot/cli/config.py
--rw-r--r--   0        0        0      401 2023-06-13 05:29:56.165277 aunly-bbot-1.4.1/aunly_bbot/cli/run.py
--rw-r--r--   0        0        0     1981 2023-06-13 05:29:56.165277 aunly-bbot-1.4.1/aunly_bbot/core/__init__.py
--rw-r--r--   0        0        0     3054 2023-06-13 05:29:56.165277 aunly-bbot-1.4.1/aunly_bbot/core/announcement.py
--rw-r--r--   0        0        0      944 2023-06-13 05:29:56.165277 aunly-bbot-1.4.1/aunly_bbot/core/bot_config.py
--rw-r--r--   0        0        0      162 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/core/context.py
--rw-r--r--   0        0        0     5470 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/core/control.py
--rw-r--r--   0        0        0    10888 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/core/data.py
--rw-r--r--   0        0        0     1796 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/core/group_config.py
--rw-r--r--   0        0        0     2562 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/core/log.py
--rw-r--r--   0        0        0     2957 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/core/subgroup_config.py
--rw-r--r--   0        0        0     1996 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/__init__.py
--rw-r--r--   0        0        0      322 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/add_talk.py
--rw-r--r--   0        0        0     1526 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/admin/add.py
--rw-r--r--   0        0        0     1523 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/admin/remove.py
--rw-r--r--   0        0        0     1088 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/announcement.py
--rw-r--r--   0        0        0     2264 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/configure/atall.py
--rw-r--r--   0        0        0     2316 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/configure/nick.py
--rwxr-xr-x   0        0        0    13750 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/content_resolve.py
--rw-r--r--   0        0        0     1415 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/init.py
--rw-r--r--   0        0        0     2480 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/menu/__init__.py
--rw-r--r--   0        0        0     2491 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/quit_group.py
--rw-r--r--   0        0        0     1068 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/status.py
--rw-r--r--   0        0        0     1456 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/subgroup/add.py
--rw-r--r--   0        0        0     2455 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/subgroup/add_up.py
--rw-r--r--   0        0        0     1336 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/subgroup/get_subgroup.py
--rw-r--r--   0        0        0     1355 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/subgroup/remove.py
--rw-r--r--   0        0        0     2259 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/subgroup/remove_up.py
--rw-r--r--   0        0        0     1666 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/up/get_subscribe.py
--rw-r--r--   0        0        0     2547 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/up/subscribe.py
--rw-r--r--   0        0        0     2101 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/up/unsubscribe.py
--rw-r--r--   0        0        0     1447 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/vip/add.py
--rw-r--r--   0        0        0     1446 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/vip/remove.py
--rw-r--r--   0        0        0     3017 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/vive_dynamic.py
--rw-r--r--   0        0        0     1554 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/web_auth.py
--rw-r--r--   0        0        0     1454 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/whitelist/add.py
--rw-r--r--   0        0        0     1015 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/whitelist/close.py
--rw-r--r--   0        0        0     1014 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/whitelist/open.py
--rw-r--r--   0        0        0     1566 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/command/whitelist/remove.py
--rw-r--r--   0        0        0     4026 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/event/bot_launch.py
--rw-r--r--   0        0        0     1432 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/event/exception.py
--rw-r--r--   0        0        0     1940 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/event/invited_join_group.py
--rw-r--r--   0        0        0     1762 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/event/join_group.py
--rw-r--r--   0        0        0     1923 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/event/leave_group.py
--rw-r--r--   0        0        0     1291 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/event/mute.py
--rw-r--r--   0        0        0     1475 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/event/new_friend.py
--rw-r--r--   0        0        0      919 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/event/offline.py
--rw-r--r--   0        0        0     1183 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/event/prem_change.py
--rw-r--r--   0        0        0    16966 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/pusher/dynamic.py
--rw-r--r--   0        0        0    15163 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/pusher/init.py
--rw-r--r--   0        0        0    10666 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/pusher/live.py
--rw-r--r--   0        0        0     2102 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/scheduler/refresh_token.py
--rw-r--r--   0        0        0      946 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/function/scheduler/version_update.py
--rw-r--r--   0        0        0     2856 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/model/bcut_asr.py
--rw-r--r--   0        0        0     7654 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/model/config.py
--rw-r--r--   0        0        0       93 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/model/exception.py
--rw-r--r--   0        0        0     1742 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/model/fastapi.py
--rw-r--r--   0        0        0      322 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/model/openai.py
--rw-r--r--   0        0        0     3985 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/static/bot_config.exp.yaml
--rw-r--r--   0        0        0     9159 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/static/mobile_style.js
--rw-r--r--   0        0        0      684 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/static/mobile_style_bak.js
--rw-r--r--   0        0        0      850 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/test.py
--rw-r--r--   0        0        0      675 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/utils/b23_extract.py
--rw-r--r--   0        0        0     6184 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/utils/bcut_asr.py
--rw-r--r--   0        0        0      780 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/utils/bilibili_parse.py
--rw-r--r--   0        0        0     4760 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/utils/bilibili_request.py
--rw-r--r--   0        0        0     6398 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/utils/browser_shot.py
--rw-r--r--   0        0        0     1160 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/utils/column_resolve.py
--rw-r--r--   0        0        0      735 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/utils/content_summarise.py
--rw-r--r--   0        0        0     2165 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/utils/detect_package.py
--rw-r--r--   0        0        0     8979 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/utils/draw_bili_image.py
--rw-r--r--   0        0        0      551 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/utils/dynamic_shot.py
--rw-r--r--   0        0        0      310 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/utils/fastapi.py
--rw-r--r--   0        0        0     4384 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/utils/fonts_provider.py
--rw-r--r--   0        0        0     6164 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/utils/openai.py
--rw-r--r--   0        0        0     1103 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/utils/pil_shot.py
--rw-r--r--   0        0        0     5069 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/utils/send_action.py
--rw-r--r--   0        0        0     1867 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/utils/strings.py
--rw-r--r--   0        0        0     3030 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/utils/text2image.py
--rw-r--r--   0        0        0      516 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/utils/time_tools.py
--rw-r--r--   0        0        0     2474 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/utils/uid_extract.py
--rw-r--r--   0        0        0     5876 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/utils/up_operation.py
--rw-r--r--   0        0        0     1089 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/utils/update_version.py
--rw-r--r--   0        0        0     1666 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/utils/verify_mah.py
--rw-r--r--   0        0        0     3803 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/utils/video_subtitle.py
--rw-r--r--   0        0        0      713 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/utils/wordcloud.py
--rw-r--r--   0        0        0     1509 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/website/__init__.py
--rw-r--r--   0        0        0      415 2023-06-13 05:29:56.169277 aunly-bbot-1.4.1/aunly_bbot/website/api/router/__init__.py
--rw-r--r--   0        0        0     4953 2023-06-13 05:29:56.173277 aunly-bbot-1.4.1/aunly_bbot/website/api/router/auth.py
--rw-r--r--   0        0        0     1266 2023-06-13 05:29:56.173277 aunly-bbot-1.4.1/aunly_bbot/website/api/router/config.py
--rw-r--r--   0        0        0     2730 2023-06-13 05:29:56.173277 aunly-bbot-1.4.1/aunly_bbot/website/api/router/follow.py
--rw-r--r--   0        0        0     1664 2023-06-13 05:29:56.173277 aunly-bbot-1.4.1/aunly_bbot/website/api/router/home.py
--rw-r--r--   0        0        0     1459 2023-06-13 05:29:56.173277 aunly-bbot-1.4.1/aunly_bbot/website/api/router/user.py
--rw-r--r--   0        0        0     4009 2023-06-13 05:29:56.173277 aunly-bbot-1.4.1/aunly_bbot/website/api/router/ws.py
--rw-r--r--   0        0        0    87542 2023-06-13 05:29:56.173277 aunly-bbot-1.4.1/aunly_bbot/website/static/html/favicon.ico
--rw-r--r--   0        0        0      306 2023-06-13 05:29:56.173277 aunly-bbot-1.4.1/aunly_bbot/website/static/html/index.html
--rw-r--r--   0        0        0     1676 2023-06-13 05:29:56.177277 aunly-bbot-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     5120 2023-06-13 05:29:56.177277 aunly-bbot-1.4.1/readme.md
--rw-r--r--   0        0        0     5714 1970-01-01 00:00:00.000000 aunly-bbot-1.4.1/PKG-INFO
+-rwxr-xr-x   0        0        0    34523 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/LICENSE
+-rw-r--r--   0        0        0       61 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/__main__.py
+-rw-r--r--   0        0        0     3361 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/bot.py
+-rw-r--r--   0        0        0     1753 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/cli/__init__.py
+-rw-r--r--   0        0        0     2302 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/cli/api.py
+-rw-r--r--   0        0        0    22667 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/cli/config.py
+-rw-r--r--   0        0        0      401 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/cli/run.py
+-rw-r--r--   0        0        0     1981 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/core/__init__.py
+-rw-r--r--   0        0        0     3054 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/core/announcement.py
+-rw-r--r--   0        0        0      944 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/core/bot_config.py
+-rw-r--r--   0        0        0      162 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/core/context.py
+-rw-r--r--   0        0        0     5470 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/core/control.py
+-rw-r--r--   0        0        0    10888 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/core/data.py
+-rw-r--r--   0        0        0     1796 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/core/group_config.py
+-rw-r--r--   0        0        0     2620 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/core/log.py
+-rw-r--r--   0        0        0     2957 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/core/subgroup_config.py
+-rw-r--r--   0        0        0     1996 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/__init__.py
+-rw-r--r--   0        0        0      322 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/add_talk.py
+-rw-r--r--   0        0        0     1526 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/admin/add.py
+-rw-r--r--   0        0        0     1523 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/admin/remove.py
+-rw-r--r--   0        0        0     1088 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/announcement.py
+-rw-r--r--   0        0        0     2264 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/configure/atall.py
+-rw-r--r--   0        0        0     2316 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/configure/nick.py
+-rwxr-xr-x   0        0        0    13750 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/content_resolve.py
+-rw-r--r--   0        0        0     1415 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/init.py
+-rw-r--r--   0        0        0     2480 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/menu/__init__.py
+-rw-r--r--   0        0        0     2491 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/quit_group.py
+-rw-r--r--   0        0        0     1068 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/status.py
+-rw-r--r--   0        0        0     1456 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/subgroup/add.py
+-rw-r--r--   0        0        0     2455 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/subgroup/add_up.py
+-rw-r--r--   0        0        0     1336 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/subgroup/get_subgroup.py
+-rw-r--r--   0        0        0     1355 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/subgroup/remove.py
+-rw-r--r--   0        0        0     2259 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/subgroup/remove_up.py
+-rw-r--r--   0        0        0     1666 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/up/get_subscribe.py
+-rw-r--r--   0        0        0     2547 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/up/subscribe.py
+-rw-r--r--   0        0        0     2101 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/up/unsubscribe.py
+-rw-r--r--   0        0        0     1447 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/vip/add.py
+-rw-r--r--   0        0        0     1446 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/vip/remove.py
+-rw-r--r--   0        0        0     3017 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/vive_dynamic.py
+-rw-r--r--   0        0        0     1554 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/web_auth.py
+-rw-r--r--   0        0        0     1454 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/whitelist/add.py
+-rw-r--r--   0        0        0     1015 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/whitelist/close.py
+-rw-r--r--   0        0        0     1014 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/whitelist/open.py
+-rw-r--r--   0        0        0     1566 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/whitelist/remove.py
+-rw-r--r--   0        0        0     4026 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/event/bot_launch.py
+-rw-r--r--   0        0        0     1432 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/event/exception.py
+-rw-r--r--   0        0        0     1940 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/event/invited_join_group.py
+-rw-r--r--   0        0        0     1762 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/event/join_group.py
+-rw-r--r--   0        0        0     1923 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/event/leave_group.py
+-rw-r--r--   0        0        0     1291 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/event/mute.py
+-rw-r--r--   0        0        0     1475 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/event/new_friend.py
+-rw-r--r--   0        0        0      919 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/event/offline.py
+-rw-r--r--   0        0        0     1183 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/event/prem_change.py
+-rw-r--r--   0        0        0    16966 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/function/pusher/dynamic.py
+-rw-r--r--   0        0        0    15163 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/function/pusher/init.py
+-rw-r--r--   0        0        0    10666 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/function/pusher/live.py
+-rw-r--r--   0        0        0     2102 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/function/scheduler/refresh_token.py
+-rw-r--r--   0        0        0      946 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/function/scheduler/version_update.py
+-rw-r--r--   0        0        0     2856 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/model/bcut_asr.py
+-rw-r--r--   0        0        0      315 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/model/captcha.py
+-rw-r--r--   0        0        0     7708 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/model/config.py
+-rw-r--r--   0        0        0       93 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/model/exception.py
+-rw-r--r--   0        0        0     1742 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/model/fastapi.py
+-rw-r--r--   0        0        0      322 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/model/openai.py
+-rw-r--r--   0        0        0     4057 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/static/bot_config.exp.yaml
+-rw-r--r--   0        0        0     9159 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/static/mobile_style.js
+-rw-r--r--   0        0        0      684 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/static/mobile_style_bak.js
+-rw-r--r--   0        0        0      850 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/test.py
+-rw-r--r--   0        0        0      675 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/b23_extract.py
+-rw-r--r--   0        0        0     6184 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/bcut_asr.py
+-rw-r--r--   0        0        0      780 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/bilibili_parse.py
+-rw-r--r--   0        0        0     4760 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/bilibili_request.py
+-rw-r--r--   0        0        0    11279 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/browser_shot.py
+-rw-r--r--   0        0        0     1160 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/column_resolve.py
+-rw-r--r--   0        0        0      735 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/content_summarise.py
+-rw-r--r--   0        0        0     2165 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/detect_package.py
+-rw-r--r--   0        0        0     8979 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/draw_bili_image.py
+-rw-r--r--   0        0        0      551 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/dynamic_shot.py
+-rw-r--r--   0        0        0      310 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/fastapi.py
+-rw-r--r--   0        0        0     4384 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/fonts_provider.py
+-rw-r--r--   0        0        0     6183 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/openai.py
+-rw-r--r--   0        0        0     1103 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/pil_shot.py
+-rw-r--r--   0        0        0     5069 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/send_action.py
+-rw-r--r--   0        0        0     1867 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/strings.py
+-rw-r--r--   0        0        0     3030 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/text2image.py
+-rw-r--r--   0        0        0      516 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/time_tools.py
+-rw-r--r--   0        0        0     2474 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/uid_extract.py
+-rw-r--r--   0        0        0     5876 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/up_operation.py
+-rw-r--r--   0        0        0     1089 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/update_version.py
+-rw-r--r--   0        0        0     1666 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/verify_mah.py
+-rw-r--r--   0        0        0     3803 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/video_subtitle.py
+-rw-r--r--   0        0        0      713 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/wordcloud.py
+-rw-r--r--   0        0        0     1509 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/website/__init__.py
+-rw-r--r--   0        0        0      415 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/__init__.py
+-rw-r--r--   0        0        0     4953 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/auth.py
+-rw-r--r--   0        0        0     1266 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/config.py
+-rw-r--r--   0        0        0     2730 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/follow.py
+-rw-r--r--   0        0        0     1664 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/home.py
+-rw-r--r--   0        0        0     1459 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/user.py
+-rw-r--r--   0        0        0     4009 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/ws.py
+-rw-r--r--   0        0        0    87542 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/website/static/html/favicon.ico
+-rw-r--r--   0        0        0      306 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/website/static/html/index.html
+-rw-r--r--   0        0        0     1720 2023-06-14 07:43:35.421459 aunly-bbot-1.5.0b1/pyproject.toml
+-rw-r--r--   0        0        0     5120 2023-06-14 07:43:35.421459 aunly-bbot-1.5.0b1/readme.md
+-rw-r--r--   0        0        0     5720 1970-01-01 00:00:00.000000 aunly-bbot-1.5.0b1/PKG-INFO
```

### Comparing `aunly-bbot-1.4.1/LICENSE` & `aunly-bbot-1.5.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/bot.py` & `aunly-bbot-1.5.0b1/aunly_bbot/bot.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/cli/__init__.py` & `aunly-bbot-1.5.0b1/aunly_bbot/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/cli/api.py` & `aunly-bbot-1.5.0b1/aunly_bbot/cli/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from fastapi import FastAPI
 from fastapi.responses import Response
 from playwright.async_api import async_playwright
 from playwright.async_api._generated import BrowserContext
 from graiax.playwright.installer import install_playwright
 
 from ..utils.browser_shot import screenshot
-from ..utils.fonts_provider import get_font
+from ..utils.fonts_provider import font_init
 from ..utils.detect_package import is_package
 
 
 DYNAMIC_SHOT_CACHE = Path("data", "cache")
 DYNAMIC_SHOT_CACHE.mkdir(parents=True, exist_ok=True)
 os.environ["PLAYWRIGHT_BROWSERS_PATH"] = (
     "0" if is_package else Path(__file__).parent.parent.joinpath("static", "browser").as_posix()
@@ -23,30 +23,34 @@
 app = FastAPI(title="BBot Playwright API", version="0.1.0")
 
 
 @app.on_event("startup")
 async def init_playwright():
     global PLAYWRIGIT
     logger.info("正在下载字体...")
-    await get_font()
+    font_init()
     logger.success("字体下载完成！")
 
     await install_playwright(browser_type="firefox")
     pw = await async_playwright().start()
     ff = await pw.firefox.launch_persistent_context(
         Path("data").joinpath("browser"),
         device_scale_factor=1.5,
         user_agent=(
             "Mozilla/5.0 (Linux; Android 10; RMX1911) AppleWebKit/537.36 "
             "(KHTML, like Gecko) Chrome/100.0.4896.127 Mobile Safari/537.36"
         ),
+        # headless=False,
     )
     PLAYWRIGIT = ff
     logger.info("[Playwright] 正在获取浏览器版本")
-    page = await PLAYWRIGIT.new_page()
+    if len(PLAYWRIGIT.pages) > 0:
+        page = PLAYWRIGIT.pages[0]
+    else:
+        page = await PLAYWRIGIT.new_page()
     version = await page.evaluate("navigator.appVersion")
     logger.info(f"[BiliBili推送] 浏览器启动完成，当前版本 {version}")
     logger.debug(await PLAYWRIGIT.cookies())
 
 
 @app.get("/dynamic/{dynid}")
 async def get_up(dynid: str):
```

### Comparing `aunly-bbot-1.4.1/aunly_bbot/cli/config.py` & `aunly-bbot-1.5.0b1/aunly_bbot/cli/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,15 +284,15 @@
         else:
             click.secho("输入的 OpenAI Token 不合法（应以 sk- 开头）", fg="bright_red", bold=True)
             self.openai_api_token()
 
     def openai_model(self):
         openai_model = ListPrompt(
             "请选择 OpenAI 模型",
-            [Choice("gpt-3.5-turbo-0301"), Choice("gpt-4-0314"), Choice("gpt-4-32k-0314")],
+            [Choice("gpt-3.5-turbo-0613"), Choice("gpt-3.5-turbo-16k-0613"), Choice("gpt-4-0613")],
             allow_filter=False,
             annotation="使用键盘的 ↑ 和 ↓ 来选择, 按回车确认",
         ).prompt()
         self.config["Bilibili"]["openai_model"] = openai_model.name
 
     def openai_proxy(self):
         if openai_proxy_url := InputPrompt("请输入 OpenAI 代理地址（留空则不使用代理）: ").prompt():
@@ -302,21 +302,22 @@
             elif not openai_proxy_url.startswith("http"):
                 click.secho("输入的 OpenAI 代理地址不合法！仅可使用 http 代理", fg="bright_red", bold=True)
                 self.openai_proxy()
             self.config["Bilibili"]["openai_proxy"] = openai_proxy_url
 
     def bilibili_username(self):
         username = InputPrompt("请输入 Bilibili 用户名: （可用于 AI 总结时获取 Bilibili 的 AI 字幕）").prompt()
-        if not username:
-            click.secho("用户名不能为空！", fg="bright_red", bold=True)
-            self.bilibili_username()
+        if not username or username == "":
+            self.config["Bilibili"]["username"] = username
+            return click.secho("用户名为空，已关闭对应功能！", fg="bright_red", bold=True)
         elif not username.isdigit():
             click.secho("用户名不合法！", fg="bright_red", bold=True)
             self.bilibili_username()
         self.config["Bilibili"]["username"] = username
+        self.bilibili_password()
 
     def bilibili_password(self):
         password = InputPrompt("请输入 Bilibili 密码: ", is_password=True).prompt()
         if not password:
             click.secho("密码不能为空！", fg="bright_red", bold=True)
             self.bilibili_password()
         self.config["Bilibili"]["password"] = password
@@ -446,20 +447,19 @@
             self.config["admins"].append(int(admin))
 
     def log_level(self):
         self.config["log_level"] = (
             ListPrompt(
                 "请选择日志等级",
                 [
-                    Choice("DEBUG"),
                     Choice("INFO"),
+                    Choice("DEBUG"),
                     Choice("WARNING"),
                 ],
                 allow_filter=False,
-                default_select=1,
                 annotation="使用键盘的 ↑ 和 ↓ 来选择, 按回车确认",
             )
             .prompt()
             .name
         )
 
     def name(self):
```

### Comparing `aunly-bbot-1.4.1/aunly_bbot/core/__init__.py` & `aunly-bbot-1.5.0b1/aunly_bbot/core/__init__.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/core/announcement.py` & `aunly-bbot-1.5.0b1/aunly_bbot/core/announcement.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/core/bot_config.py` & `aunly-bbot-1.5.0b1/aunly_bbot/core/bot_config.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/core/control.py` & `aunly-bbot-1.5.0b1/aunly_bbot/core/control.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/core/data.py` & `aunly-bbot-1.5.0b1/aunly_bbot/core/data.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/core/group_config.py` & `aunly-bbot-1.5.0b1/aunly_bbot/core/group_config.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/core/log.py` & `aunly-bbot-1.5.0b1/aunly_bbot/core/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
     rotation="00:00",
     retention="3 days",
     compression="tar.xz",
     level="WARNING",
 )
 
 logger.success(f"成功重载 logger，当前日志等级为 {log_level}")
+logger.info(f"日志文件将会保存在 {LOGPATH} 中")
 
 # logger.trace("TRACE 等级将会输出至控制台")
 # logger.debug("DEBUG 等级将会输出至控制台")
 # logger.info("INFO 等级将会输出至控制台")
 # logger.success("SUCCESS 等级将会输出至控制台")
 # logger.warning('WARNING 等级将会输出至控制台')
 # logger.error("ERROR 等级将会输出至控制台")
```

### Comparing `aunly-bbot-1.4.1/aunly_bbot/core/subgroup_config.py` & `aunly-bbot-1.5.0b1/aunly_bbot/core/subgroup_config.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/__init__.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/__init__.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/admin/add.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/admin/add.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/admin/remove.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/admin/remove.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/announcement.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/announcement.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/configure/atall.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/configure/atall.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/configure/nick.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/configure/nick.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/content_resolve.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/content_resolve.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/init.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/init.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/menu/__init__.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/menu/__init__.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/quit_group.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/quit_group.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/status.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/status.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/subgroup/add.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/subgroup/add.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/subgroup/add_up.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/subgroup/add_up.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/subgroup/get_subgroup.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/subgroup/get_subgroup.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/subgroup/remove.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/subgroup/remove.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/subgroup/remove_up.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/subgroup/remove_up.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/up/get_subscribe.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/up/get_subscribe.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/up/subscribe.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/up/subscribe.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/up/unsubscribe.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/up/unsubscribe.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/vip/add.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/vip/add.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/vip/remove.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/vip/remove.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/vive_dynamic.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/vive_dynamic.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/web_auth.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/web_auth.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/whitelist/add.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/whitelist/add.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/whitelist/close.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/whitelist/close.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/whitelist/open.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/whitelist/open.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/command/whitelist/remove.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/whitelist/remove.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/event/bot_launch.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/event/bot_launch.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/event/exception.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/event/exception.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/event/invited_join_group.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/event/invited_join_group.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/event/join_group.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/event/join_group.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/event/leave_group.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/event/leave_group.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/event/mute.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/event/mute.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/event/new_friend.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/event/new_friend.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/event/offline.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/event/offline.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/event/prem_change.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/event/prem_change.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/pusher/dynamic.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/pusher/dynamic.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/pusher/init.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/pusher/init.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/pusher/live.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/pusher/live.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/scheduler/refresh_token.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/scheduler/refresh_token.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/function/scheduler/version_update.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/scheduler/version_update.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/model/bcut_asr.py` & `aunly-bbot-1.5.0b1/aunly_bbot/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/model/config.py` & `aunly-bbot-1.5.0b1/aunly_bbot/model/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,33 +42,34 @@
                 return enable
             raise KeyError
         except KeyError as key_err:
             raise ValueError("已启用 Debug 但未填入合法的群号") from key_err
 
 
 class _Bilibili(BaseModel, extra=Extra.ignore):
-    username: Optional[int]
+    username: Optional[str]
     password: Optional[str]
     use_login: bool = False
     use_browser: bool = True
     allow_fallback: bool = True
     mobile_style: bool = True
     concurrency: int = 5
     dynamic_font: str = "HarmonyOS_Sans_SC_Medium.ttf"
     dynamic_font_source: Literal["local", "remote"] = "local"
     openai_summarization: bool = False
     openai_api_token: Optional[str] = None
-    openai_model: str = "gpt-3.5-turbo"
+    openai_model: str = "gpt-3.5-turbo-0301"
     openai_proxy: Optional[AnyHttpUrl] = None
     openai_cooldown: int = 60
     openai_whitelist_users: Optional[list[int]] = None
     openai_promot_version: int = 2
     use_wordcloud: bool = False
     use_bcut_asr: bool = False
     asr_length_threshold: int = 60
+    captcha_address: Optional[AnyHttpUrl] = None
 
     # 验证是否可以登录
     @validator("use_login", always=True)
     def can_use_login(cls, use_login, values):
         if not use_login:
             return use_login
         click.secho("已检测到开启 BiliBili 登录模式，不推荐使用", fg="bright_yellow", bold=True)
```

### Comparing `aunly-bbot-1.4.1/aunly_bbot/model/fastapi.py` & `aunly-bbot-1.5.0b1/aunly_bbot/model/fastapi.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/static/bot_config.exp.yaml` & `aunly-bbot-1.5.0b1/aunly_bbot/static/bot_config.exp.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,15 @@
   openai_proxy: "http://localhost:7890"   # 请求 OpenAI 所用的代理
   openai_cooldown: 60                     # OpenAI 调用冷却时间（秒）
   openai_whitelist_users: []              # OpenAI 调用冷却白名单用户（即使在冷却时间内也可以调用）
   openai_promot_version: 2                # OpenAI 提示词版本，当前可选值: 1, 2
   use_wordcloud: true                     # 是否使用词云
   use_bcut_asr: true                      # 是否使用 BCut 接口进行 AI 语音识别
   asr_length_threshold: 60                # 调用语音识别的最小长度阈值（秒）
+  captcha_address: null                   # 验证码识别服务地址
 Event:
   mute: true                              # 是否向管理员发送被禁言的事件提醒。
   permchange: true                        # 是否向管理员发送权限变更的事件提醒。
   push: true                              # 是否向管理员发送推送的事件提醒。
   subscribe: true                         # 是否向管理员发送订阅的事件提醒。
 Webui:
   webui_host: "0.0.0.0"                   # WebUI 监听地址
```

### Comparing `aunly-bbot-1.4.1/aunly_bbot/static/mobile_style.js` & `aunly-bbot-1.5.0b1/aunly_bbot/static/mobile_style.js`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/static/mobile_style_bak.js` & `aunly-bbot-1.5.0b1/aunly_bbot/static/mobile_style_bak.js`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/test.py` & `aunly-bbot-1.5.0b1/aunly_bbot/test.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/utils/b23_extract.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/b23_extract.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/utils/bcut_asr.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/utils/bilibili_parse.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/bilibili_parse.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/utils/bilibili_request.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/utils/column_resolve.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/column_resolve.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/utils/content_summarise.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/content_summarise.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/utils/detect_package.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/detect_package.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/utils/draw_bili_image.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/utils/dynamic_shot.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/dynamic_shot.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/utils/fonts_provider.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/utils/openai.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/openai.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import httpx
 import random
 import asyncio
 import tiktoken_async
 
 from loguru import logger
+from httpx import Response
 from typing import Optional
 from collections import OrderedDict
-from httpx import HTTPError, Response
 
 from ..core.bot_config import BotConfig
 from ..model.openai import OpenAI, TokenUsage
 
-LIMIT_COUNT = {"gpt-3.5-turbo-0301": 3500, "gpt-4-0314": 7600, "gpt-4-32k-0314": 32200}.get(
-    BotConfig.Bilibili.openai_model or "gpt-3.5-turbo-0301", 3500
-)
+LIMIT_COUNT = {
+    "gpt-3.5-turbo-0613": 3500,
+    "gpt-3.5-turbo-16k-0613": 15000,
+    "gpt-4-0613": 7600,
+}.get(BotConfig.Bilibili.openai_model or "gpt-3.5-turbo-0613", 3500)
 
 if BotConfig.Bilibili.openai_summarization:
     logger.info("正在加载 OpenAI Token 计算模型")
     tiktoken_enc = asyncio.run(
         tiktoken_async.encoding_for_model(BotConfig.Bilibili.openai_model)
     )
     logger.info(f"{tiktoken_enc.name} 加载成功")
@@ -55,18 +57,18 @@
         )
     )
 
 
 def count_tokens(prompts: list[dict[str, str]]):
     """根据内容计算 token 数"""
 
-    if BotConfig.Bilibili.openai_model == "gpt-3.5-turbo-0301":
+    if BotConfig.Bilibili.openai_model.startswith("gpt-3.5-turbo"):
         tokens_per_message = 4
         tokens_per_name = -1
-    elif BotConfig.Bilibili.openai_model == "gpt-4":
+    elif BotConfig.Bilibili.openai_model.startswith("gpt-4"):
         tokens_per_message = 3
         tokens_per_name = 1
     else:
         raise ValueError(f"Unknown model name {BotConfig.Bilibili.openai_model}")
 
     num_tokens = 0
     for message in prompts:
```

### Comparing `aunly-bbot-1.4.1/aunly_bbot/utils/pil_shot.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/pil_shot.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/utils/send_action.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/send_action.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/utils/strings.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/strings.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/utils/text2image.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/text2image.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/utils/time_tools.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/time_tools.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/utils/uid_extract.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/uid_extract.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/utils/up_operation.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/up_operation.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/utils/update_version.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/update_version.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/utils/verify_mah.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/verify_mah.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/utils/video_subtitle.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/utils/wordcloud.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/wordcloud.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/website/__init__.py` & `aunly-bbot-1.5.0b1/aunly_bbot/website/__init__.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/website/api/router/auth.py` & `aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/auth.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/website/api/router/config.py` & `aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/config.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/website/api/router/follow.py` & `aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/follow.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/website/api/router/home.py` & `aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/home.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/website/api/router/user.py` & `aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/user.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/website/api/router/ws.py` & `aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/ws.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/aunly_bbot/website/static/html/favicon.ico` & `aunly-bbot-1.5.0b1/aunly_bbot/website/static/html/favicon.ico`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/pyproject.toml` & `aunly-bbot-1.5.0b1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aunly-bbot"
-version = "1.4.1"
+version = "1.5.0-beta1"
 description = "一个用于 QQ 群内高效推送哔哩哔哩 UP 动态及直播的机器人"
 readme = "readme.md"
 keywords = [
     "graia",
     "graiax",
     "bilibili",
     "qqbot",
@@ -22,20 +22,20 @@
 dependencies = [
     "graia-ariadne[standard]>=0.11.5",
     "peewee>=3.16.2",
     "pyyaml>=6.0",
     "bilireq>=0.2.6",
     "psutil>=5.9.5",
     "uvicorn>=0.22.0",
-    "sentry-sdk>=1.25.0",
+    "sentry-sdk>=1.25.1",
     "python-jose[cryptography]>=3.3.0",
     "passlib[bcrypt]>=1.7.4",
     "python-multipart>=0.0.6",
-    "fastapi>=0.96.0",
-    "websockets>=11.0.2",
+    "fastapi>=0.97.0",
+    "websockets>=11.0.3",
     "qrcode>=7.4.2",
     "pillow>=9.5.0",
     "noneprompt>=0.1.9",
     "minidynamicrender>=1.2.6",
     "lxml>=4.9.2",
     "tiktoken-async>=0.3.2",
 ]
@@ -46,19 +46,19 @@
 [project.urls]
 homepage = "https://github.com/djkcyl/BBot-Graia"
 repository = "https://github.com/djkcyl/BBot-Graia/tree/master/bbot"
 documentation = "https://github.com/djkcyl/BBot-Graia/blob/master/readme.md"
 
 [project.optional-dependencies]
 full = [
-    "graiax-playwright",
-    "graiax-text2img-playwright",
-    "wordcloud",
-    "jieba",
-    "edgegpt",
+    "graiax-playwright>=0.2.4",
+    "graiax-text2img-playwright>=0.4.0",
+    "wordcloud>=1.9.2",
+    "jieba>=0.42.1",
+    "edgegpt>=0.10.13",
 ]
 
 [project.scripts]
 bbot = "aunly_bbot.__main__:main"
 
 [tool.pdm.build]
 includes = [
@@ -66,15 +66,15 @@
 ]
 excludes = [
     "aunly_bbot/static/browser",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "yamllint>=1.31.0",
+    "yamllint>=1.32.0",
     "black>=23.3.0",
     "flake8>=6.0.0",
 ]
 
 [tool.black]
 line-length = 96
```

### Comparing `aunly-bbot-1.4.1/readme.md` & `aunly-bbot-1.5.0b1/readme.md`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.4.1/PKG-INFO` & `aunly-bbot-1.5.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aunly-bbot
-Version: 1.4.1
+Version: 1.5.0-beta1
 Summary: 一个用于 QQ 群内高效推送哔哩哔哩 UP 动态及直播的机器人
 License: AGPL3.0
 Keywords: graia,graiax,bilibili,qqbot,grpc,playwright,fastapi,bot,openai,chatgpt
 Author-email: djkcyl <cyl@cyllive.cn>
 Requires-Python: >=3.9,<4.0
 Provides-Extra: full
 Project-URL: documentation, https://github.com/djkcyl/BBot-Graia/blob/master/readme.md
```

