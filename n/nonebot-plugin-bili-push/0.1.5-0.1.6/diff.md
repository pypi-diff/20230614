# Comparing `tmp/nonebot_plugin_bili_push-0.1.5.tar.gz` & `tmp/nonebot_plugin_bili_push-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bili_push-0.1.5.tar", last modified: Tue Jun 13 10:12:07 2023, max compression
+gzip compressed data, was "nonebot_plugin_bili_push-0.1.6.tar", last modified: Wed Jun 14 03:32:03 2023, max compression
```

## Comparing `nonebot_plugin_bili_push-0.1.5.tar` & `nonebot_plugin_bili_push-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 10:12:07.090541 nonebot_plugin_bili_push-0.1.5/
--rw-rw-rw-   0        0        0     1078 2023-06-13 02:14:36.000000 nonebot_plugin_bili_push-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      268 2023-06-13 10:12:07.089540 nonebot_plugin_bili_push-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1663 2023-06-13 09:23:15.000000 nonebot_plugin_bili_push-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 10:12:07.075543 nonebot_plugin_bili_push-0.1.5/nonebot_plugin_bili_push/
--rw-rw-rw-   0        0        0   101668 2023-06-13 10:10:25.000000 nonebot_plugin_bili_push-0.1.5/nonebot_plugin_bili_push/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 10:12:07.087540 nonebot_plugin_bili_push-0.1.5/nonebot_plugin_bili_push.egg-info/
--rw-rw-rw-   0        0        0      268 2023-06-13 10:12:06.000000 nonebot_plugin_bili_push-0.1.5/nonebot_plugin_bili_push.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-13 10:12:07.000000 nonebot_plugin_bili_push-0.1.5/nonebot_plugin_bili_push.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 10:12:06.000000 nonebot_plugin_bili_push-0.1.5/nonebot_plugin_bili_push.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2023-06-13 10:12:06.000000 nonebot_plugin_bili_push-0.1.5/nonebot_plugin_bili_push.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-13 10:12:06.000000 nonebot_plugin_bili_push-0.1.5/nonebot_plugin_bili_push.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 10:12:07.090541 nonebot_plugin_bili_push-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      794 2023-06-13 10:11:37.000000 nonebot_plugin_bili_push-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:32:03.173886 nonebot_plugin_bili_push-0.1.6/
+-rw-rw-rw-   0        0        0     1078 2023-06-13 02:14:36.000000 nonebot_plugin_bili_push-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      268 2023-06-14 03:32:03.172883 nonebot_plugin_bili_push-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1694 2023-06-14 03:27:08.000000 nonebot_plugin_bili_push-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 03:32:03.159883 nonebot_plugin_bili_push-0.1.6/nonebot_plugin_bili_push/
+-rw-rw-rw-   0        0        0   102059 2023-06-14 03:27:18.000000 nonebot_plugin_bili_push-0.1.6/nonebot_plugin_bili_push/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:32:03.170884 nonebot_plugin_bili_push-0.1.6/nonebot_plugin_bili_push.egg-info/
+-rw-rw-rw-   0        0        0      268 2023-06-14 03:32:03.000000 nonebot_plugin_bili_push-0.1.6/nonebot_plugin_bili_push.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-06-14 03:32:03.000000 nonebot_plugin_bili_push-0.1.6/nonebot_plugin_bili_push.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 03:32:03.000000 nonebot_plugin_bili_push-0.1.6/nonebot_plugin_bili_push.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      111 2023-06-14 03:32:03.000000 nonebot_plugin_bili_push-0.1.6/nonebot_plugin_bili_push.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-14 03:32:03.000000 nonebot_plugin_bili_push-0.1.6/nonebot_plugin_bili_push.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 03:32:03.173886 nonebot_plugin_bili_push-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1069 2023-06-14 03:31:53.000000 nonebot_plugin_bili_push-0.1.6/setup.py
```

### Comparing `nonebot_plugin_bili_push-0.1.5/LICENSE` & `nonebot_plugin_bili_push-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bili_push-0.1.5/README.md` & `nonebot_plugin_bili_push-0.1.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-<div align="center">
-  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/supergugugu/1.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
-  <br>
-  <p><img src="https://github.com/2.png" width="240" alt="NoneBotPluginText"></p>
-</div>
-
-<div align="center">
-
-# nonebot-plugin-bili-push
- B订阅推送插件 
-</div>
-
-## 示例
-
-![输入图片描述](README_md_files/9cf89890-0952-11ee-8733-25d9c7397331.jpeg?v=1&type=image)
-![输入图片描述](README_md_files/7fd7ee50-0952-11ee-8733-25d9c7397331.jpeg?v=1&type=image)
-
-
-## 安装
-（以下方法三选一）
-
-~~一.命令行安装：（未就绪）~~
-
-    nb plugin install nonebot-plugin-bili-push
- 二.使用插件文件安装：（不推荐）
- 1.下载插件文件，放到plugins文件夹。
-2.修改pyproject.toml使其可以加载插件
-
-三.pip安装：（不推荐）
-1.执行此命令
-
-    pip install nonebot-plugin-bili-push
-2.修改pyproject.toml使其可以加载插件
-
-    plugins = [”nonebot-plugin-bili-push“]
- 
-## 配置
-在 nonebot2 项目的`.env`文件中选填配置
-配置管理员账户，只有管理员才能添加订阅
-
-    SUPERUSERS=["12345678"] # 配置 NoneBot 超级用户
-插件数据存放位置，默认为 “./”。
-
-    bilipush_basepath="./"
-## 参考内容
-Mirai动态绘制插件 [BilibiliDynamic MiraiPlugin](https://github.com/Colter23/bilibili-dynamic-mirai-plugin)
-
-## 交流
--   交流群[鸽子窝里有鸽子（291788927）](https://qm.qq.com/cgi-bin/qm/qr?k=QhOk7Z2jaXBOnAFfRafEy9g5WoiETQhy&jump_from=webapi&authKey=fCvx/auG+QynlI8bcFNs4Csr2soR8UjzuwLqrDN9F8LDwJrwePKoe89psqpozg/m)
--   有疑问或者建议都可以进群详谈。
+<div align="center">
+  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/supergugugu/1.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+  <br>
+  <p><img src="https://github.com/2.png" width="240" alt="NoneBotPluginText"></p>
+</div>
+
+<div align="center">
+
+# nonebot-plugin-bili-push
+ B订阅推送插件 
+</div>
+
+## 示例
+
+![输入图片描述](README_md_files/9cf89890-0952-11ee-8733-25d9c7397331.jpeg?v=1&type=image)
+![输入图片描述](README_md_files/7fd7ee50-0952-11ee-8733-25d9c7397331.jpeg?v=1&type=image)
+
+
+## 安装
+（以下方法三选一）
+
+一.命令行安装：
+
+    nb plugin install nonebot-plugin-bili-push
+ 二.使用插件文件安装：（不推荐）
+ 1.下载插件文件，放到plugins文件夹。
+2.修改pyproject.toml使其可以加载插件
+
+三.pip安装：（不推荐）
+1.执行此命令
+
+    pip install nonebot-plugin-bili-push
+2.修改pyproject.toml使其可以加载插件
+
+    plugins = [”nonebot-plugin-bili-push“]
+ 
+## 配置
+在 nonebot2 项目的`.env`文件中选填配置
+配置管理员账户，只有管理员才能添加订阅
+
+    SUPERUSERS=["12345678"] # 配置 NoneBot 超级用户
+插件数据存放位置，默认为 “./”。
+
+    bilipush_basepath="./"
+## 参考内容
+Mirai动态绘制插件 [BilibiliDynamic MiraiPlugin](https://github.com/Colter23/bilibili-dynamic-mirai-plugin)
+
+## 交流
+-   交流群[鸽子窝里有鸽子（291788927）](https://qm.qq.com/cgi-bin/qm/qr?k=QhOk7Z2jaXBOnAFfRafEy9g5WoiETQhy&jump_from=webapi&authKey=fCvx/auG+QynlI8bcFNs4Csr2soR8UjzuwLqrDN9F8LDwJrwePKoe89psqpozg/m)
+-   有疑问或者建议都可以进群详谈。
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                 # nonebot-plugin-bili-push Bè®¢éæ¨éæä»¶
 ## ç¤ºä¾ ![è¾å¥å¾çæè¿°](README_md_files/9cf89890-0952-11ee-8733-
 25d9c7397331.jpeg?v=1&type=image) ![è¾å¥å¾çæè¿°](README_md_files/
 7fd7ee50-0952-11ee-8733-25d9c7397331.jpeg?v=1&type=image) ## å®è£
-ï¼ä»¥ä¸æ¹æ³ä¸éä¸ï¼ ~~ä¸.å½ä»¤è¡å®è£ï¼ï¼æªå°±ç»ªï¼~~ nb plugin
-install nonebot-plugin-bili-push äº.ä½¿ç¨æä»¶æä»¶å®è£ï¼ï¼ä¸æ¨èï¼
+ï¼ä»¥ä¸æ¹æ³ä¸éä¸ï¼ ä¸.å½ä»¤è¡å®è£ï¼ nb plugin install nonebot-
+plugin-bili-push äº.ä½¿ç¨æä»¶æä»¶å®è£ï¼ï¼ä¸æ¨èï¼
 1.ä¸è½½æä»¶æä»¶ï¼æ¾å°pluginsæä»¶å¤¹ã
 2.ä¿®æ¹pyproject.tomlä½¿å¶å¯ä»¥å è½½æä»¶ ä¸.pipå®è£ï¼ï¼ä¸æ¨èï¼
 1.æ§è¡æ­¤å½ä»¤ pip install nonebot-plugin-bili-push
 2.ä¿®æ¹pyproject.tomlä½¿å¶å¯ä»¥å è½½æä»¶ plugins = [ânonebot-plugin-
 bili-pushâ] ## éç½® å¨ nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­éå¡«éç½®
 éç½®ç®¡çåè´¦æ·ï¼åªæç®¡çåæè½æ·»å è®¢é SUPERUSERS=
 ["12345678"] # éç½® NoneBot è¶çº§ç¨æ· æä»¶æ°æ®å­æ¾ä½ç½®ï¼é»è®¤ä¸º
```

### Comparing `nonebot_plugin_bili_push-0.1.5/nonebot_plugin_bili_push/__init__.py` & `nonebot_plugin_bili_push-0.1.6/nonebot_plugin_bili_push/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
-import requests
 import re
 from PIL import Image, ImageDraw, ImageFont
 from io import BytesIO
 import json
 from nonebot.adapters.onebot.v11 import Bot, MessageEvent, GroupMessageEvent, MessageSegment
 from nonebot import on_command
 import sqlite3
 from nonebot.adapters.onebot.v11 import GROUP_ADMIN, GROUP_OWNER
 import random
-from nonebot import require
+from nonebot import require, logger
 import nonebot
 from nonebot.plugin import PluginMetadata
+import httpx
+import asyncio
 
 require("nonebot_plugin_apscheduler")
 from nonebot_plugin_apscheduler import scheduler
 
 config = nonebot.get_driver().config
 # 读取配置
 #
@@ -37,14 +38,31 @@
 #
 # 配置4：
 # 是否使用api来获取emoji图像
 # 为True时使用api，为False时不使用api，为空时自动选择。
 # bilipush_emojiapi=True
 #
 
+
+def get_api(url: str, type: str = "json"):
+    if type == "json":
+        async def fetch(url):
+            async with httpx.AsyncClient(http2=True) as client:
+                response = await client.get(url)
+            return response.text
+        return_data = asyncio.get_event_loop().run_until_complete(fetch(apiurl))
+        return return_data
+
+    elif type == "image":
+        return httpx.get(apiurl).read()
+    return
+
+
+
+
 # 配置1：
 try:
     adminqq = config.superusers
     adminqq = list(adminqq)
 except:
     adminqq = []
 # 配置2：
@@ -59,15 +77,15 @@
     apiurl = "http://cdn.kanon.ink"
 # 配置4：
 try:
     use_api = config.bilipush_emojiapi
 except:
     try:
         get_url = apiurl + "/json/config?name=ping"
-        return_json = json.loads(requests.get(get_url).text)
+        return_json = get_api(get_url, "json")
         if return_json["code"] == 0:
             use_api = True
         else:
             use_api = False
     except:
         use_api = False
 
@@ -101,25 +119,26 @@
 half_text = ["A", "B", "C", "D", "E", "F", "G", "H", "I", "J", "K", "L", "M", "N", "O", "P", "Q", "R", "S", "T", "U",
              "V", "W", "X", "Y", "Z", "a", "b", "c", "d", "e", "f", "g", "h", "i", "j", "k", "l", "m", "n", "o", "p",
              "q", "r", "s", "t", "u", "v", "w", "x", "y", "z", "1", "2", "3", "4", "5", "6", "7", "8", "9", "0", ",",
              ".", "/", "\\", "[", "]", "(", ")", "!", "+", "-", "*", "！", "？", "。", "，", "{", "}", "、", "‘", "“",
              '"', "'", "！", " "]
 
 
+
+
 def get_emoji(emoji):
     cachepath = basepath + "cache/emoji/"
     if not os.path.exists(cachepath):
         os.makedirs(cachepath)
     cachepath = cachepath + emoji + ".png"
     if not cachepath.exists():
         if use_api:
             url = apiurl + "/api/emoji?imageid=" + emoji
             try:
-                return_image = requests.get(url)
-                return_image = Image.open(BytesIO(return_image.content))
+                return_image = get_api(url, "image")
                 return_image.save(cachepath)
             except:
                 print("api出错，请联系开发者")
                 # api出错时直接打印文字
                 return_image = Image.new("RGBA", (100, 100), color=(0, 0, 0, 0))
                 paste_image = draw_text(emoji, 100, 10)
                 return_image.paste(paste_image, (0, 0), mask=paste_image)
```

### Comparing `nonebot_plugin_bili_push-0.1.5/setup.py` & `nonebot_plugin_bili_push-0.1.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 from setuptools import setup, find_packages
 
 
+# def get_install_requires():
+#     reqs = [
+#         'pillow>=9.5.0',
+#         'httpx>=0.24.1',
+#         'h2>=4.1.0',
+#         'nonebot2>=2.0.0',
+#         'nonebot_adapter_onebot>=2.2.3',
+#         'nonebot_plugin_apscheduler>=0.2.0'
+#     ]
+#     return reqs
+
 def get_install_requires():
     reqs = [
         'pillow>=9.5.0',
-        'requests>=2.30.0',
-        'nonebot2>=2.0.0rc3',
+        'requests>=2.31.0',
+        'nonebot2>=2.0.0',
         'nonebot_adapter_onebot>=2.2.3',
         'nonebot_plugin_apscheduler>=0.2.0'
     ]
     return reqs
 
 
 setup(name='nonebot_plugin_bili_push',
-      version='0.1.5',
+      version='0.1.6',
       description='nonebot2 plugin',
       author='SuperGuGuGu',
       author_email='13680478000@163.com',
       url='https://github.com/SuperGuGuGu/nonebot_plugin_bili_push',
       packages=find_packages(),
       python_requires=">=3.8",
       install_requires=get_install_requires(),
```

