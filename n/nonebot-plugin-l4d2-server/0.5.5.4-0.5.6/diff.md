# Comparing `tmp/nonebot_plugin_l4d2_server-0.5.5.4.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.5.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.6.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.5.5.4.tar` & `nonebot_plugin_l4d2_server-0.5.6.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    35149 2023-06-14 10:18:10.824905 nonebot_plugin_l4d2_server-0.5.5.4/LICENSE
--rw-r--r--   0        0        0    11703 2023-06-14 10:18:10.824905 nonebot_plugin_l4d2_server-0.5.5.4/README.md
--rw-r--r--   0        0        0    17513 2023-06-14 10:18:10.828904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0   158357 2023-06-14 10:18:10.828904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-06-14 10:18:10.828904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1590 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2135 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     6135 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6170 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1523 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     5506 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
--rw-r--r--   0        0        0     2408 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
--rw-r--r--   0        0        0     7874 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0      486 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
--rw-r--r--   0        0        0     1350 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/img/white.png
--rw-r--r--   0        0        0     8734 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1610 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3010 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1694 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      359 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3252 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      468 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0        0 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_data/database.py
--rw-r--r--   0        0        0     3232 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1295 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4097 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     1906 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
--rw-r--r--   0        0        0     1860 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
--rw-r--r--   0        0        0     2688 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_file/remote.py
--rw-r--r--   0        0        0     4148 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4007 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0     1038 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0     9524 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/image.py
--rw-r--r--   0        0        0     1073 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/one.py
--rw-r--r--   0        0        0      936 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     3799 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1387 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     7415 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
--rw-r--r--   0        0        0     3735 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1157 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0     1191 2023-06-14 10:18:10.832904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    10855 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1615 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_server/index.py
--rw-r--r--   0        0        0     1248 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1359 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     4113 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
--rw-r--r--   0        0        0     1175 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
--rw-r--r--   0        0        0     2024 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_update/restart.py
--rw-r--r--   0        0        0     1434 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_update/update.py
--rw-r--r--   0        0        0     9728 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/command.py
--rw-r--r--   0        0        0     5753 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/config.py
--rw-r--r--   0        0        0     1620 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/message.py
--rw-r--r--   0        0        0      337 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
--rw-r--r--   0        0        0      992 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
--rw-r--r--   0        0        0     2133 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
--rw-r--r--   0        0        0     8928 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
--rw-r--r--   0        0        0     8575 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    14781 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1499 2023-06-14 10:18:10.836904 nonebot_plugin_l4d2_server-0.5.5.4/pyproject.toml
--rw-r--r--   0        0        0    13572 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.5.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-14 12:38:37.817076 nonebot_plugin_l4d2_server-0.5.6/LICENSE
+-rw-r--r--   0        0        0    11703 2023-06-14 12:38:37.817076 nonebot_plugin_l4d2_server-0.5.6/README.md
+-rw-r--r--   0        0        0    17650 2023-06-14 12:38:37.821076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0   158357 2023-06-14 12:38:37.821076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-06-14 12:38:37.821076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1590 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2135 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     6135 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6170 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1523 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     5506 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
+-rw-r--r--   0        0        0     2408 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
+-rw-r--r--   0        0        0     7874 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0      486 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
+-rw-r--r--   0        0        0     1350 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/img/white.png
+-rw-r--r--   0        0        0     8734 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1610 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3010 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1694 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      359 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3252 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      468 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0        0 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_data/database.py
+-rw-r--r--   0        0        0     3232 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1295 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     4097 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     1906 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
+-rw-r--r--   0        0        0     1860 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
+-rw-r--r--   0        0        0     2688 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_file/remote.py
+-rw-r--r--   0        0        0     4148 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4007 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0     1038 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0     9524 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/image.py
+-rw-r--r--   0        0        0     1073 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/one.py
+-rw-r--r--   0        0        0      936 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     3799 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1387 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     7415 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
+-rw-r--r--   0        0        0     3735 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1157 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0     1191 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
+-rw-r--r--   0        0        0    10855 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     1615 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_server/index.py
+-rw-r--r--   0        0        0     1248 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1359 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     4113 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
+-rw-r--r--   0        0        0     1175 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
+-rw-r--r--   0        0        0     2024 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_update/restart.py
+-rw-r--r--   0        0        0     1434 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_update/update.py
+-rw-r--r--   0        0        0     9342 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/command.py
+-rw-r--r--   0        0        0     5753 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/config.py
+-rw-r--r--   0        0        0     1620 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/message.py
+-rw-r--r--   0        0        0      337 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
+-rw-r--r--   0        0        0      992 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
+-rw-r--r--   0        0        0     2133 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
+-rw-r--r--   0        0        0     8928 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
+-rw-r--r--   0        0        0     8575 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    14781 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1475 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0    13527 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.6/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/LICENSE` & `nonebot_plugin_l4d2_server-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/README.md` & `nonebot_plugin_l4d2_server-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,22 @@
 from .l4d2_utils.txt_to_img import mode_txt_to_img
 # from .l4d2_server import RCONClient
 scheduler = require("nonebot_plugin_apscheduler").scheduler
 
 driver = get_driver()
 
 
-__version__ = "0.5.5"
+__version__ = "0.5.6"
 __plugin_meta__ = PluginMetadata(
     name="求生之路小助手",
     description='群内对有关求生之路的查询和操作',
     usage='求生服务器操作指令',
+    type="application",
+    homepage="https://github.com/Agnes4m/nonebot_plugin_l4d2_server",
+    supported_adapters={"~onebot.v11"},
     extra={
         "version": __version__,
         "author": "Agnes4m <Z735803792@163.com>",
     },
 )
```

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/data/img/white.png` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/img/white.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_file/input_json.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_file/input_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_file/remote.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_file/remote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/image.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/one.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/one.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_push/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_push/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_update/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_update/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_update/restart.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_update/restart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_update/update.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_update/update.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/command.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/command.py`

 * *Files 9% similar despite different names*

```diff
@@ -121,44 +121,36 @@
 
 
     
 async def get_des_ip():
     global ALL_HOST
     global ANNE_IP
     global matchers
-    if l4_config.l4_tag == None:
-        pass
-    else:
-        # try:
-        #     qq = l4_config.l4_master[0]
-        # except:
-        #     qq = list(nonebot.get_bot().config.superusers)[0]
-        # ALL_HOST.update(await seach_map(msg = l4_config.l4_tag,qq = qq, key=l4_config.l4_key,mode='ip'))
-        def count_ips(ip_dict:dict):
-            global ANNE_IP
-            for key, value in ip_dict.items():
-                if key in ['error_','success_']:
-                    ip_dict.pop(key)
-                    break
-                count = len(value)
-                logger.info(f'已加载：{key} | {count}个')
-                if key == '云':
-                    ANNE_IP = {key:value}
+    def count_ips(ip_dict:dict):
+        global ANNE_IP
+        for key, value in ip_dict.items():
+            if key in ['error_','success_']:
+                ip_dict.pop(key)
+                break
+            count = len(value)
+            logger.info(f'已加载：{key} | {count}个')
+            if key == '云':
+                ANNE_IP = {key:value}
         sleep(1)
-        count_ips(ALL_HOST)
-        ip_anne_list=[] 
-        try:
-            ips = ALL_HOST['云']
-            ip_anne_list = []
-            for one_ip in ips:
-                host,port = split_maohao(one_ip['ip'])
-                ip_anne_list.append((one_ip['id'],host,port))
-        except KeyError:
-            pass
-        await get_read_ip(ip_anne_list)
+    count_ips(ALL_HOST)
+    ip_anne_list=[] 
+    try:
+        ips = ALL_HOST['云']
+        ip_anne_list = []
+        for one_ip in ips:
+            host,port = split_maohao(one_ip['ip'])
+            ip_anne_list.append((one_ip['id'],host,port))
+    except KeyError:
+        pass
+    await get_read_ip(ip_anne_list)
 
         
     @tan_jian.handle()
     async def _(matcher:Matcher,event:MessageEvent):
         msg = await get_tan_jian(ip_anne_list,1)
         await matcher.finish(msg)
```

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/config.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/message.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/seach.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/seach.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_utils/utils.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/pyproject.toml` & `nonebot_plugin_l4d2_server-0.5.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.5.5.4"
+version = "0.5.6"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
@@ -19,27 +19,26 @@
 ]
 include = [
     "LICENSE","README.md"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-nonebot2 = "^2.0.0rc4"
+nonebot2 = "^2.0.0"
 nonebot-adapter-onebot = ">=2.1.5"
 nonebot_plugin_htmlrender = "^0.2.0.1"
 nonebot_plugin_txt2img = ">=0.3.0"
 nonebot_plugin_apscheduler = "^0.2.0"
 asyncio = ">=3.4.3"
 jinja2 = ">=3.0.0"
 srctools="^2.3.9"
 httpx = ">=0.23.3"
 beautifulsoup4 = ">=4.8.0"
 rcon = "^2.1.0"
 pillow = "^9.3.0"
-aiohttp = "^3.8.3"
 pyunpack = "^0.3.0"
 "ruamel.yaml" = "^0.17.21"
 rarfile = "^4.0"
 patool = "^1.12"
 python-a2s = "^1.3.0"
 amis-python = "^1.0.6"
 jieba = "^0.42.1"
```

### Comparing `nonebot_plugin_l4d2_server-0.5.5.4/PKG-INFO` & `nonebot_plugin_l4d2_server-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.5.5.4
+Version: 0.5.6
 Summary: L4D2 server related operations plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: steam,game,l4d2,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
@@ -12,25 +12,24 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: amis-python (>=1.0.6,<2.0.0)
 Requires-Dist: asyncio (>=3.4.3)
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
 Requires-Dist: beautifulsoup4 (>=4.8.0)
 Requires-Dist: gitpython (>=3.1.27)
 Requires-Dist: httpx (>=0.23.3)
 Requires-Dist: jieba (>=0.42.1,<0.43.0)
 Requires-Dist: jinja2 (>=3.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.5)
-Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
 Requires-Dist: nonebot_plugin_htmlrender (>=0.2.0.1,<0.3.0.0)
 Requires-Dist: nonebot_plugin_txt2img (>=0.3.0)
 Requires-Dist: pandas (>=1.5.2)
 Requires-Dist: patool (>=1.12,<2.0)
 Requires-Dist: pillow (>=9.3.0,<10.0.0)
 Requires-Dist: python-a2s (>=1.3.0,<2.0.0)
```

#### html2text {}

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.5.4
-Summary: L4D2 server related operations plugin for NoneBot2 Home-page: https://
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.6 Summary:
+L4D2 server related operations plugin for NoneBot2 Home-page: https://
 github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
 steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
 Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiohttp (>=3.8.3,<4.0.0) Requires-Dist: amis-python
-(>=1.0.6,<2.0.0) Requires-Dist: asyncio (>=3.4.3) Requires-Dist: attrs
-(>=23.1.0,<24.0.0) Requires-Dist: beautifulsoup4 (>=4.8.0) Requires-Dist:
-gitpython (>=3.1.27) Requires-Dist: httpx (>=0.23.3) Requires-Dist: jieba
-(>=0.42.1,<0.43.0) Requires-Dist: jinja2 (>=3.0.0) Requires-Dist: nonebot-
-adapter-onebot (>=2.1.5) Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0) Requires-
-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0) Requires-Dist:
+Requires-Dist: amis-python (>=1.0.6,<2.0.0) Requires-Dist: asyncio (>=3.4.3)
+Requires-Dist: attrs (>=23.1.0,<24.0.0) Requires-Dist: beautifulsoup4 (>=4.8.0)
+Requires-Dist: gitpython (>=3.1.27) Requires-Dist: httpx (>=0.23.3) Requires-
+Dist: jieba (>=0.42.1,<0.43.0) Requires-Dist: jinja2 (>=3.0.0) Requires-Dist:
+nonebot-adapter-onebot (>=2.1.5) Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
+Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0) Requires-Dist:
 nonebot_plugin_htmlrender (>=0.2.0.1,<0.3.0.0) Requires-Dist:
 nonebot_plugin_txt2img (>=0.3.0) Requires-Dist: pandas (>=1.5.2) Requires-Dist:
 patool (>=1.12,<2.0) Requires-Dist: pillow (>=9.3.0,<10.0.0) Requires-Dist:
 python-a2s (>=1.3.0,<2.0.0) Requires-Dist: python-jose (>=3.3.0,<4.0.0)
 Requires-Dist: pyunpack (>=0.3.0,<0.4.0) Requires-Dist: rarfile (>=4.0,<5.0)
 Requires-Dist: rcon (>=2.1.0,<3.0.0) Requires-Dist: ruamel.yaml
 (>=0.17.21,<0.18.0) Requires-Dist: srctools (>=2.3.9,<3.0.0) Project-URL:
```

