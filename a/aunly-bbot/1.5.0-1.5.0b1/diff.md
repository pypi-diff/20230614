# Comparing `tmp/aunly-bbot-1.5.0.tar.gz` & `tmp/aunly-bbot-1.5.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aunly-bbot-1.5.0.tar", last modified: Wed Jun 14 15:14:29 2023, max compression
+gzip compressed data, was "aunly-bbot-1.5.0b1.tar", last modified: Wed Jun 14 07:43:49 2023, max compression
```

## Comparing `aunly-bbot-1.5.0.tar` & `aunly-bbot-1.5.0b1.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rwxr-xr-x   0        0        0    34523 2023-06-14 15:14:14.070269 aunly-bbot-1.5.0/LICENSE
--rw-r--r--   0        0        0       61 2023-06-14 15:14:14.070269 aunly-bbot-1.5.0/aunly_bbot/__main__.py
--rw-r--r--   0        0        0     3361 2023-06-14 15:14:14.070269 aunly-bbot-1.5.0/aunly_bbot/bot.py
--rw-r--r--   0        0        0     1753 2023-06-14 15:14:14.070269 aunly-bbot-1.5.0/aunly_bbot/cli/__init__.py
--rw-r--r--   0        0        0     2302 2023-06-14 15:14:14.070269 aunly-bbot-1.5.0/aunly_bbot/cli/api.py
--rw-r--r--   0        0        0    22667 2023-06-14 15:14:14.070269 aunly-bbot-1.5.0/aunly_bbot/cli/config.py
--rw-r--r--   0        0        0      401 2023-06-14 15:14:14.070269 aunly-bbot-1.5.0/aunly_bbot/cli/run.py
--rw-r--r--   0        0        0     1981 2023-06-14 15:14:14.070269 aunly-bbot-1.5.0/aunly_bbot/core/__init__.py
--rw-r--r--   0        0        0     3054 2023-06-14 15:14:14.070269 aunly-bbot-1.5.0/aunly_bbot/core/announcement.py
--rw-r--r--   0        0        0      944 2023-06-14 15:14:14.070269 aunly-bbot-1.5.0/aunly_bbot/core/bot_config.py
--rw-r--r--   0        0        0      162 2023-06-14 15:14:14.070269 aunly-bbot-1.5.0/aunly_bbot/core/context.py
--rw-r--r--   0        0        0     5470 2023-06-14 15:14:14.070269 aunly-bbot-1.5.0/aunly_bbot/core/control.py
--rw-r--r--   0        0        0    10888 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/core/data.py
--rw-r--r--   0        0        0     1796 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/core/group_config.py
--rw-r--r--   0        0        0     2620 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/core/log.py
--rw-r--r--   0        0        0     2957 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/core/subgroup_config.py
--rw-r--r--   0        0        0     1996 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/__init__.py
--rw-r--r--   0        0        0      322 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/add_talk.py
--rw-r--r--   0        0        0     1526 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/admin/add.py
--rw-r--r--   0        0        0     1523 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/admin/remove.py
--rw-r--r--   0        0        0     1088 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/announcement.py
--rw-r--r--   0        0        0     2264 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/configure/atall.py
--rw-r--r--   0        0        0     2316 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/configure/nick.py
--rwxr-xr-x   0        0        0    13750 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/content_resolve.py
--rw-r--r--   0        0        0     1415 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/init.py
--rw-r--r--   0        0        0     2480 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/menu/__init__.py
--rw-r--r--   0        0        0     2491 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/quit_group.py
--rw-r--r--   0        0        0     1068 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/status.py
--rw-r--r--   0        0        0     1456 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/subgroup/add.py
--rw-r--r--   0        0        0     2455 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/subgroup/add_up.py
--rw-r--r--   0        0        0     1336 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/subgroup/get_subgroup.py
--rw-r--r--   0        0        0     1355 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/subgroup/remove.py
--rw-r--r--   0        0        0     2259 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/subgroup/remove_up.py
--rw-r--r--   0        0        0     1666 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/up/get_subscribe.py
--rw-r--r--   0        0        0     2547 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/up/subscribe.py
--rw-r--r--   0        0        0     2101 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/up/unsubscribe.py
--rw-r--r--   0        0        0     1447 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/vip/add.py
--rw-r--r--   0        0        0     1446 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/vip/remove.py
--rw-r--r--   0        0        0     3017 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/vive_dynamic.py
--rw-r--r--   0        0        0     1554 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/web_auth.py
--rw-r--r--   0        0        0     1454 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/whitelist/add.py
--rw-r--r--   0        0        0     1015 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/whitelist/close.py
--rw-r--r--   0        0        0     1014 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/whitelist/open.py
--rw-r--r--   0        0        0     1566 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/command/whitelist/remove.py
--rw-r--r--   0        0        0     4026 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/event/bot_launch.py
--rw-r--r--   0        0        0     1432 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/event/exception.py
--rw-r--r--   0        0        0     1940 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/event/invited_join_group.py
--rw-r--r--   0        0        0     1762 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/event/join_group.py
--rw-r--r--   0        0        0     1923 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/event/leave_group.py
--rw-r--r--   0        0        0     1291 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/event/mute.py
--rw-r--r--   0        0        0     1475 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/event/new_friend.py
--rw-r--r--   0        0        0      919 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/event/offline.py
--rw-r--r--   0        0        0     1183 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/event/prem_change.py
--rw-r--r--   0        0        0    16966 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/pusher/dynamic.py
--rw-r--r--   0        0        0    15163 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/pusher/init.py
--rw-r--r--   0        0        0    10666 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/pusher/live.py
--rw-r--r--   0        0        0     2102 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/scheduler/refresh_token.py
--rw-r--r--   0        0        0      946 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/function/scheduler/version_update.py
--rw-r--r--   0        0        0     2856 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/model/bcut_asr.py
--rw-r--r--   0        0        0      315 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/model/captcha.py
--rw-r--r--   0        0        0     7773 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/model/config.py
--rw-r--r--   0        0        0       93 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/model/exception.py
--rw-r--r--   0        0        0     1742 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/model/fastapi.py
--rw-r--r--   0        0        0      322 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/model/openai.py
--rw-r--r--   0        0        0     4066 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/static/bot_config.exp.yaml
--rw-r--r--   0        0        0     9159 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/static/mobile_style.js
--rw-r--r--   0        0        0      684 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/static/mobile_style_bak.js
--rw-r--r--   0        0        0      850 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/test.py
--rw-r--r--   0        0        0      675 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/utils/b23_extract.py
--rw-r--r--   0        0        0     6184 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/utils/bcut_asr.py
--rw-r--r--   0        0        0      780 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/utils/bilibili_parse.py
--rw-r--r--   0        0        0     4760 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/utils/bilibili_request.py
--rw-r--r--   0        0        0    11279 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/utils/browser_shot.py
--rw-r--r--   0        0        0     1160 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/utils/column_resolve.py
--rw-r--r--   0        0        0      735 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/utils/content_summarise.py
--rw-r--r--   0        0        0     2165 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/utils/detect_package.py
--rw-r--r--   0        0        0     8979 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/utils/draw_bili_image.py
--rw-r--r--   0        0        0      551 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/utils/dynamic_shot.py
--rw-r--r--   0        0        0      310 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/utils/fastapi.py
--rw-r--r--   0        0        0     4384 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/utils/fonts_provider.py
--rw-r--r--   0        0        0     6183 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/utils/openai.py
--rw-r--r--   0        0        0     1103 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/utils/pil_shot.py
--rw-r--r--   0        0        0     5069 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/utils/send_action.py
--rw-r--r--   0        0        0     1867 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/utils/strings.py
--rw-r--r--   0        0        0     3030 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/utils/text2image.py
--rw-r--r--   0        0        0      516 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/utils/time_tools.py
--rw-r--r--   0        0        0     2474 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/utils/uid_extract.py
--rw-r--r--   0        0        0     5876 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/utils/up_operation.py
--rw-r--r--   0        0        0     1089 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/utils/update_version.py
--rw-r--r--   0        0        0     1666 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/utils/verify_mah.py
--rw-r--r--   0        0        0     3803 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/utils/video_subtitle.py
--rw-r--r--   0        0        0      713 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/utils/wordcloud.py
--rw-r--r--   0        0        0     1509 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/website/__init__.py
--rw-r--r--   0        0        0      415 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/website/api/router/__init__.py
--rw-r--r--   0        0        0     4953 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/website/api/router/auth.py
--rw-r--r--   0        0        0     1266 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/website/api/router/config.py
--rw-r--r--   0        0        0     2730 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/website/api/router/follow.py
--rw-r--r--   0        0        0     1664 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/website/api/router/home.py
--rw-r--r--   0        0        0     1459 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/website/api/router/user.py
--rw-r--r--   0        0        0     4009 2023-06-14 15:14:14.074269 aunly-bbot-1.5.0/aunly_bbot/website/api/router/ws.py
--rw-r--r--   0        0        0    87542 2023-06-14 15:14:14.078269 aunly-bbot-1.5.0/aunly_bbot/website/static/html/favicon.ico
--rw-r--r--   0        0        0      306 2023-06-14 15:14:14.078269 aunly-bbot-1.5.0/aunly_bbot/website/static/html/index.html
--rw-r--r--   0        0        0     1714 2023-06-14 15:14:14.082269 aunly-bbot-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     5120 2023-06-14 15:14:14.082269 aunly-bbot-1.5.0/readme.md
--rw-r--r--   0        0        0     5714 1970-01-01 00:00:00.000000 aunly-bbot-1.5.0/PKG-INFO
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

### Comparing `aunly-bbot-1.5.0/LICENSE` & `aunly-bbot-1.5.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/bot.py` & `aunly-bbot-1.5.0b1/aunly_bbot/bot.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/cli/__init__.py` & `aunly-bbot-1.5.0b1/aunly_bbot/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/cli/api.py` & `aunly-bbot-1.5.0b1/aunly_bbot/cli/api.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/cli/config.py` & `aunly-bbot-1.5.0b1/aunly_bbot/cli/config.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/core/__init__.py` & `aunly-bbot-1.5.0b1/aunly_bbot/core/__init__.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/core/announcement.py` & `aunly-bbot-1.5.0b1/aunly_bbot/core/announcement.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/core/bot_config.py` & `aunly-bbot-1.5.0b1/aunly_bbot/core/bot_config.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/core/control.py` & `aunly-bbot-1.5.0b1/aunly_bbot/core/control.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/core/data.py` & `aunly-bbot-1.5.0b1/aunly_bbot/core/data.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/core/group_config.py` & `aunly-bbot-1.5.0b1/aunly_bbot/core/group_config.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/core/log.py` & `aunly-bbot-1.5.0b1/aunly_bbot/core/log.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/core/subgroup_config.py` & `aunly-bbot-1.5.0b1/aunly_bbot/core/subgroup_config.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/__init__.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/__init__.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/admin/add.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/admin/add.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/admin/remove.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/admin/remove.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/announcement.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/announcement.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/configure/atall.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/configure/atall.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/configure/nick.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/configure/nick.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/content_resolve.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/content_resolve.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/init.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/init.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/menu/__init__.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/menu/__init__.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/quit_group.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/quit_group.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/status.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/status.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/subgroup/add.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/subgroup/add.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/subgroup/add_up.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/subgroup/add_up.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/subgroup/get_subgroup.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/subgroup/get_subgroup.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/subgroup/remove.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/subgroup/remove.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/subgroup/remove_up.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/subgroup/remove_up.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/up/get_subscribe.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/up/get_subscribe.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/up/subscribe.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/up/subscribe.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/up/unsubscribe.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/up/unsubscribe.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/vip/add.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/vip/add.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/vip/remove.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/vip/remove.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/vive_dynamic.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/vive_dynamic.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/web_auth.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/web_auth.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/whitelist/add.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/whitelist/add.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/whitelist/close.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/whitelist/close.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/whitelist/open.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/whitelist/open.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/command/whitelist/remove.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/command/whitelist/remove.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/event/bot_launch.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/event/bot_launch.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/event/exception.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/event/exception.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/event/invited_join_group.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/event/invited_join_group.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/event/join_group.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/event/join_group.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/event/leave_group.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/event/leave_group.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/event/mute.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/event/mute.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/event/new_friend.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/event/new_friend.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/event/offline.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/event/offline.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/event/prem_change.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/event/prem_change.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/pusher/dynamic.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/pusher/dynamic.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/pusher/init.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/pusher/init.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/pusher/live.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/pusher/live.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/scheduler/refresh_token.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/scheduler/refresh_token.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/function/scheduler/version_update.py` & `aunly-bbot-1.5.0b1/aunly_bbot/function/scheduler/version_update.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/model/bcut_asr.py` & `aunly-bbot-1.5.0b1/aunly_bbot/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/model/config.py` & `aunly-bbot-1.5.0b1/aunly_bbot/model/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,17 +61,15 @@
     openai_proxy: Optional[AnyHttpUrl] = None
     openai_cooldown: int = 60
     openai_whitelist_users: Optional[list[int]] = None
     openai_promot_version: int = 2
     use_wordcloud: bool = False
     use_bcut_asr: bool = False
     asr_length_threshold: int = 60
-    captcha_address: Optional[AnyHttpUrl] = AnyHttpUrl(
-        "https://bbot-captcha:6082", scheme="https"
-    )
+    captcha_address: Optional[AnyHttpUrl] = None
 
     # 验证是否可以登录
     @validator("use_login", always=True)
     def can_use_login(cls, use_login, values):
         if not use_login:
             return use_login
         click.secho("已检测到开启 BiliBili 登录模式，不推荐使用", fg="bright_yellow", bold=True)
```

### Comparing `aunly-bbot-1.5.0/aunly_bbot/model/fastapi.py` & `aunly-bbot-1.5.0b1/aunly_bbot/model/fastapi.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/static/bot_config.exp.yaml` & `aunly-bbot-1.5.0b1/aunly_bbot/static/bot_config.exp.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   openai_proxy: "http://localhost:7890"   # 请求 OpenAI 所用的代理
   openai_cooldown: 60                     # OpenAI 调用冷却时间（秒）
   openai_whitelist_users: []              # OpenAI 调用冷却白名单用户（即使在冷却时间内也可以调用）
   openai_promot_version: 2                # OpenAI 提示词版本，当前可选值: 1, 2
   use_wordcloud: true                     # 是否使用词云
   use_bcut_asr: true                      # 是否使用 BCut 接口进行 AI 语音识别
   asr_length_threshold: 60                # 调用语音识别的最小长度阈值（秒）
-  captcha_address: "https://captcha-cd.ngworks.cn" # 验证码识别服务地址
+  captcha_address: null                   # 验证码识别服务地址
 Event:
   mute: true                              # 是否向管理员发送被禁言的事件提醒。
   permchange: true                        # 是否向管理员发送权限变更的事件提醒。
   push: true                              # 是否向管理员发送推送的事件提醒。
   subscribe: true                         # 是否向管理员发送订阅的事件提醒。
 Webui:
   webui_host: "0.0.0.0"                   # WebUI 监听地址
```

### Comparing `aunly-bbot-1.5.0/aunly_bbot/static/mobile_style.js` & `aunly-bbot-1.5.0b1/aunly_bbot/static/mobile_style.js`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/static/mobile_style_bak.js` & `aunly-bbot-1.5.0b1/aunly_bbot/static/mobile_style_bak.js`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/test.py` & `aunly-bbot-1.5.0b1/aunly_bbot/test.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/utils/b23_extract.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/b23_extract.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/utils/bcut_asr.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/utils/bilibili_parse.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/bilibili_parse.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/utils/bilibili_request.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/utils/browser_shot.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/browser_shot.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/utils/column_resolve.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/column_resolve.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/utils/content_summarise.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/content_summarise.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/utils/detect_package.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/detect_package.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/utils/draw_bili_image.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/utils/dynamic_shot.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/dynamic_shot.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/utils/fonts_provider.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/utils/openai.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/openai.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/utils/pil_shot.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/pil_shot.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/utils/send_action.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/send_action.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/utils/strings.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/strings.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/utils/text2image.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/text2image.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/utils/time_tools.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/time_tools.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/utils/uid_extract.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/uid_extract.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/utils/up_operation.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/up_operation.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/utils/update_version.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/update_version.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/utils/verify_mah.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/verify_mah.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/utils/video_subtitle.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/utils/wordcloud.py` & `aunly-bbot-1.5.0b1/aunly_bbot/utils/wordcloud.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/website/__init__.py` & `aunly-bbot-1.5.0b1/aunly_bbot/website/__init__.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/website/api/router/auth.py` & `aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/auth.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/website/api/router/config.py` & `aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/config.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/website/api/router/follow.py` & `aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/follow.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/website/api/router/home.py` & `aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/home.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/website/api/router/user.py` & `aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/user.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/website/api/router/ws.py` & `aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/ws.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/aunly_bbot/website/static/html/favicon.ico` & `aunly-bbot-1.5.0b1/aunly_bbot/website/static/html/favicon.ico`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/pyproject.toml` & `aunly-bbot-1.5.0b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aunly-bbot"
-version = "1.5.0"
+version = "1.5.0-beta1"
 description = "一个用于 QQ 群内高效推送哔哩哔哩 UP 动态及直播的机器人"
 readme = "readme.md"
 keywords = [
     "graia",
     "graiax",
     "bilibili",
     "qqbot",
```

### Comparing `aunly-bbot-1.5.0/readme.md` & `aunly-bbot-1.5.0b1/readme.md`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0/PKG-INFO` & `aunly-bbot-1.5.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aunly-bbot
-Version: 1.5.0
+Version: 1.5.0-beta1
 Summary: 一个用于 QQ 群内高效推送哔哩哔哩 UP 动态及直播的机器人
 License: AGPL3.0
 Keywords: graia,graiax,bilibili,qqbot,grpc,playwright,fastapi,bot,openai,chatgpt
 Author-email: djkcyl <cyl@cyllive.cn>
 Requires-Python: >=3.9,<4.0
 Provides-Extra: full
 Project-URL: documentation, https://github.com/djkcyl/BBot-Graia/blob/master/readme.md
```

