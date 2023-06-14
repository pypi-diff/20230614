# Comparing `tmp/nonebot_plugin_l4d2_server-0.5.5.3.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.5.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.5.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.5.4.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.5.5.3.tar` & `nonebot_plugin_l4d2_server-0.5.5.4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    35149 2023-06-09 11:26:16.190864 nonebot_plugin_l4d2_server-0.5.5.3/LICENSE
--rw-r--r--   0        0        0    11703 2023-06-09 11:26:16.190864 nonebot_plugin_l4d2_server-0.5.5.3/README.md
--rw-r--r--   0        0        0    17513 2023-06-09 11:26:16.194865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0   158357 2023-06-09 11:26:16.194865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-06-09 11:26:16.194865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1590 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2135 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     6135 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6170 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1523 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     5506 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
--rw-r--r--   0        0        0     2408 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
--rw-r--r--   0        0        0     7874 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0      486 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
--rw-r--r--   0        0        0     1350 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/img/white.png
--rw-r--r--   0        0        0     8734 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1610 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3010 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1694 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      359 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3252 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      468 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0        0 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_data/database.py
--rw-r--r--   0        0        0     3232 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1295 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4097 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     1906 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
--rw-r--r--   0        0        0     1860 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
--rw-r--r--   0        0        0     2688 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_file/remote.py
--rw-r--r--   0        0        0     4148 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4007 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0     1038 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0     9524 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/image.py
--rw-r--r--   0        0        0     1073 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/one.py
--rw-r--r--   0        0        0      936 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     3799 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1387 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     7415 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
--rw-r--r--   0        0        0     3735 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1157 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0     1191 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    10855 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1615 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_server/index.py
--rw-r--r--   0        0        0     1248 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1359 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     4113 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
--rw-r--r--   0        0        0     1175 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
--rw-r--r--   0        0        0     2024 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_update/restart.py
--rw-r--r--   0        0        0     1417 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_update/update.py
--rw-r--r--   0        0        0     9728 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/command.py
--rw-r--r--   0        0        0     6275 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/config.py
--rw-r--r--   0        0        0     1620 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/message.py
--rw-r--r--   0        0        0      337 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
--rw-r--r--   0        0        0      992 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
--rw-r--r--   0        0        0     2133 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
--rw-r--r--   0        0        0     8928 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
--rw-r--r--   0        0        0     8575 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    14159 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1453 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/pyproject.toml
--rw-r--r--   0        0        0    13572 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.5.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-14 10:18:10.824905 nonebot_plugin_l4d2_server-0.5.5.4/LICENSE
+-rw-r--r--   0        0        0    11703 2023-06-14 10:18:10.824905 nonebot_plugin_l4d2_server-0.5.5.4/README.md
+-rw-r--r--   0        0        0    17513 2023-06-14 10:18:10.828904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0   158357 2023-06-14 10:18:10.828904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-06-14 10:18:10.828904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1590 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2135 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     6135 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6170 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1523 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     5506 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
+-rw-r--r--   0        0        0     2408 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
+-rw-r--r--   0        0        0     7874 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0      486 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
+-rw-r--r--   0        0        0     1350 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/img/white.png
+-rw-r--r--   0        0        0     8734 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1610 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3010 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1694 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      359 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3252 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      468 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_data/database.py
+-rw-r--r--   0        0        0     3232 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1295 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     4097 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     1906 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
+-rw-r--r--   0        0        0     1860 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
+-rw-r--r--   0        0        0     2688 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_file/remote.py
+-rw-r--r--   0        0        0     4148 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4007 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0     1038 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0     9524 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/image.py
+-rw-r--r--   0        0        0     1073 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/one.py
+-rw-r--r--   0        0        0      936 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     3799 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1387 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     7415 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
+-rw-r--r--   0        0        0     3735 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1157 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0     1191 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
+-rw-r--r--   0        0        0    10855 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     1615 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_server/index.py
+-rw-r--r--   0        0        0     1248 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1359 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     4113 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
+-rw-r--r--   0        0        0     1175 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
+-rw-r--r--   0        0        0     2024 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_update/restart.py
+-rw-r--r--   0        0        0     1434 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_update/update.py
+-rw-r--r--   0        0        0     9728 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/command.py
+-rw-r--r--   0        0        0     5753 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/config.py
+-rw-r--r--   0        0        0     1620 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/message.py
+-rw-r--r--   0        0        0      337 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
+-rw-r--r--   0        0        0      992 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
+-rw-r--r--   0        0        0     2133 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
+-rw-r--r--   0        0        0     8928 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
+-rw-r--r--   0        0        0     8575 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    14781 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1499 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/pyproject.toml
+-rw-r--r--   0        0        0    13572 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.5.4/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/LICENSE` & `nonebot_plugin_l4d2_server-0.5.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/README.md` & `nonebot_plugin_l4d2_server-0.5.5.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/img/white.png` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/img/white.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_file/input_json.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_file/input_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_file/remote.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_file/remote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/image.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/one.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/one.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_push/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_push/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_update/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_update/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_update/restart.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_update/restart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_update/update.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_update/update.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from git.exc import GitCommandError
 
 
 async def update_from_git(
     level: int = 0,
     repo_path: Union[str, Path, None] = None,
     log_config: dict = {
-        'key': '✨🐛',
+        'key': '✨🐛🎨⚡🍱♻️',
         'num': 7,
     },
     is_update: bool = True,
 ) -> List[str]:
     if repo_path is None:
         repo_path = Path(__file__).parents[2]
     repo = git.Repo(repo_path)  # type: ignore
```

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/command.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/command.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/config.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,23 +50,18 @@
     def update(self, **kwargs):
         for key, value in kwargs.items():
             if key in self.__fields__:
                 self.__setattr__(key, value)
 
 class L4d2Config(BaseModel):
     total_enable: bool = Field(True, alias='是否全局启用求生功能')
-    map_path: List[str] = Field([], alias='求生地图路径')
     web_username: str = Field('l4d2', alias='后台管理用户名')
     web_password: str = Field('admin', alias='后台管理密码')
     l4_style: str = Field("standard", alias='图片风格')
     l4_image: bool = Field(False , alias='是否启用图片')
-    # l4_file: List[str] = Field(	["/home/ubuntu/l4d2/coop"], alias='本地求生服务器地址')
-    # l4_host: List[str] = Field(['127.0.0.1'], alias='求生服务器地址')
-    # l4_port: List[str] = Field(['20715'], alias='求生服务器端口')
-    # l4_rcon: List[str] = Field(['114514'], alias='求生服务器rcon密码')
     
     l4_ipall: List[Dict[str,Union[str,int,bool]]] = Field(
         [{
         'id_rank':'1',
         'place': False,
         'location':'C:\\l4d2',
         'host':'127.0.0.1',
@@ -87,16 +82,14 @@
           alias='l4服务器ip集合')
     web_secret_key: str = Field('49c294d32f69b732ef6447c18379451ce1738922a75cd1d4812ef150318a2ed0',
                                 alias='后台管理token密钥')
     l4_master: List[str] = Field(['114514919'], alias='求生地图全局管理员qq')
     # l4_ip:bool = Field(False, alias='查询地图是否显示ip')
     l4_font: str = Field('simsun.ttc', alias='字体')
     l4_only:bool = Field(False, alias='下载地图是是否阻碍其他指令')
-    l4_tag: List[str] = Field(['呆呆','橘'], alias='查服的名')
-    l4_key: str = Field('q1145149191810', alias='key')
     l4_push_interval: int = Field(3, alias='定时任务间隔')
     l4_push_times: int = Field(10, alias='定时任务次数')
     group_config: Dict[int, L4d2GroupConfig] = Field({}, alias='分群配置')
 
     def update(self, **kwargs):
         for key, value in kwargs.items():
             if key in self.__fields__:
```

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/message.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/seach.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/seach.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/utils.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,28 +55,35 @@
                                      content='登录本后台管理所需要的用户名。')),
         InputPassword(label='后台管理密码', name='web_password', value='${web_password}',
                       labelRemark=Remark(shape='circle',
                                          content='登录本后台管理所需要的密码。')),
         InputText(label='后台管理token密钥', name='web_secret_key', value='${web_secret_key}',
                   labelRemark=Remark(shape='circle',
                                      content='用于本后台管理加密验证token的密钥。')),
-        InputText(label='查询key', name='l4_key', value='${l4_key}',
-                  labelRemark=Remark(shape='circle',
-                                     content='用于获取拓展功能的key,加q群399365126领取。')),
         InputText(label='字体', name='l4_font', value='${l4_font}',
                   labelRemark=Remark(shape='circle',
                                      content='机器人返回图片中文字的字体。')),
         Select(label='图片风格', name='l4_style', value='${l4_style}',source='${l4_styles}',
                   labelRemark=Remark(shape='circle',
                                      content='仅仅是批量查询的风格')),
+        Switch(label='是否优先上传地图', name='l4_only', value='${l4_only}', onText='开启', offText='关闭',
+               labelRemark=Remark(shape='circle',
+                                  content='开启时，上传地图会保证优先级，从而阻碍其他指令')),
         InputTag(label='查询的远程服务器tag', name='l4_tag', value='${l4_tag}',
                  enableBatchAdd=True,
                  placeholder='添加qq号', visibleOn='${total_enable}', joinValues=False, extractValue=True,
                  labelRemark=Remark(shape='circle',
                                     content='在这里加入的用户，才能上传地图')),
+        
+        InputNumber(label='定时推送间隔（min）', name='l4_push_interval', value='${l4_push_interval}',
+                  labelRemark=Remark(shape='circle',
+                                     content='设置好后，使用推送服务器定时指令，将以x分钟为间隔推送一次')),
+        InputNumber(label='定时推次数', name='l4_push_times', value='${l4_push_times}',
+                  labelRemark=Remark(shape='circle',
+                                     content='设置好后，将按照推送间隔时间推送x此')),        
         InputTag(label='求生上传地图用户', name='l4_master', value='${l4_master}',
                  enableBatchAdd=True,
                  placeholder='添加qq号', visibleOn='${total_enable}', joinValues=False, extractValue=True,
                  labelRemark=Remark(shape='circle',
                                     content='在这里加入的用户，才能上传地图')),
 
     ],
```

#### html2text {}

```diff
@@ -29,26 +29,32 @@
 content='ç»å½æ¬åå°ç®¡çæéè¦çç¨æ·åã')), InputPassword
 (label='åå°ç®¡çå¯ç ', name='web_password', value='${web_password}',
 labelRemark=Remark(shape='circle',
 content='ç»å½æ¬åå°ç®¡çæéè¦çå¯ç ã')), InputText
 (label='åå°ç®¡çtokenå¯é¥', name='web_secret_key', value='$
 {web_secret_key}', labelRemark=Remark(shape='circle',
 content='ç¨äºæ¬åå°ç®¡çå å¯éªè¯tokençå¯é¥ã')), InputText
-(label='æ¥è¯¢key', name='l4_key', value='${l4_key}', labelRemark=Remark
-(shape='circle',
-content='ç¨äºè·åæå±åè½çkey,å qç¾¤399365126é¢åã')), InputText
 (label='å­ä½', name='l4_font', value='${l4_font}', labelRemark=Remark
 (shape='circle', content='æºå¨äººè¿åå¾çä¸­æå­çå­ä½ã')), Select
 (label='å¾çé£æ ¼', name='l4_style', value='${l4_style}',source='$
 {l4_styles}', labelRemark=Remark(shape='circle',
-content='ä»ä»æ¯æ¹éæ¥è¯¢çé£æ ¼')), InputTag
-(label='æ¥è¯¢çè¿ç¨æå¡å¨tag', name='l4_tag', value='${l4_tag}',
+content='ä»ä»æ¯æ¹éæ¥è¯¢çé£æ ¼')), Switch
+(label='æ¯å¦ä¼åä¸ä¼ å°å¾', name='l4_only', value='${l4_only}',
+onText='å¼å¯', offText='å³é­', labelRemark=Remark(shape='circle',
+content='å¼å¯æ¶ï¼ä¸ä¼ å°å¾ä¼ä¿è¯ä¼åçº§ï¼ä»èé»ç¢å¶ä»æä»¤')),
+InputTag(label='æ¥è¯¢çè¿ç¨æå¡å¨tag', name='l4_tag', value='${l4_tag}',
 enableBatchAdd=True, placeholder='æ·»å qqå·', visibleOn='${total_enable}',
 joinValues=False, extractValue=True, labelRemark=Remark(shape='circle',
-content='å¨è¿éå å¥çç¨æ·ï¼æè½ä¸ä¼ å°å¾')), InputTag
+content='å¨è¿éå å¥çç¨æ·ï¼æè½ä¸ä¼ å°å¾')), InputNumber
+(label='å®æ¶æ¨éé´éï¼minï¼', name='l4_push_interval', value='$
+{l4_push_interval}', labelRemark=Remark(shape='circle',
+content='è®¾ç½®å¥½åï¼ä½¿ç¨æ¨éæå¡å¨å®æ¶æä»¤ï¼å°ä»¥xåéä¸ºé´éæ¨éä¸æ¬¡')),
+InputNumber(label='å®æ¶æ¨æ¬¡æ°', name='l4_push_times', value='$
+{l4_push_times}', labelRemark=Remark(shape='circle',
+content='è®¾ç½®å¥½åï¼å°æç§æ¨éé´éæ¶é´æ¨éxæ­¤')), InputTag
 (label='æ±çä¸ä¼ å°å¾ç¨æ·', name='l4_master', value='${l4_master}',
 enableBatchAdd=True, placeholder='æ·»å qqå·', visibleOn='${total_enable}',
 joinValues=False, extractValue=True, labelRemark=Remark(shape='circle',
 content='å¨è¿éå å¥çç¨æ·ï¼æè½ä¸ä¼ å°å¾')), ], actions=[Action
 (label='ä¿å­', level=LevelEnum.success, type='submit'), Action
 (label='éç½®', level=LevelEnum.warning, type='reset')] ) upload_map_form =
 Form( title='å¨å±éç½®', name='global_config', api='post:/l4d2/api/
```

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/pyproject.toml` & `nonebot_plugin_l4d2_server-0.5.5.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.5.5.3"
+version = "0.5.5.4"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
 include = [
     "LICENSE","README.md"
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_l4d2_server-0.5.5.3/PKG-INFO` & `nonebot_plugin_l4d2_server-0.5.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.5.5.3
+Version: 0.5.5.4
 Summary: L4D2 server related operations plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: steam,game,l4d2,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.5.3
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.5.4
 Summary: L4D2 server related operations plugin for NoneBot2 Home-page: https://
 github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
 steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
 Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

