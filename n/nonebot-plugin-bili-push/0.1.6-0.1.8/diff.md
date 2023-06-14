# Comparing `tmp/nonebot_plugin_bili_push-0.1.6.tar.gz` & `tmp/nonebot_plugin_bili_push-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bili_push-0.1.6.tar", last modified: Wed Jun 14 03:32:03 2023, max compression
+gzip compressed data, was "nonebot_plugin_bili_push-0.1.8.tar", last modified: Wed Jun 14 06:38:30 2023, max compression
```

## Comparing `nonebot_plugin_bili_push-0.1.6.tar` & `nonebot_plugin_bili_push-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 03:32:03.173886 nonebot_plugin_bili_push-0.1.6/
--rw-rw-rw-   0        0        0     1078 2023-06-13 02:14:36.000000 nonebot_plugin_bili_push-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      268 2023-06-14 03:32:03.172883 nonebot_plugin_bili_push-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1694 2023-06-14 03:27:08.000000 nonebot_plugin_bili_push-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 03:32:03.159883 nonebot_plugin_bili_push-0.1.6/nonebot_plugin_bili_push/
--rw-rw-rw-   0        0        0   102059 2023-06-14 03:27:18.000000 nonebot_plugin_bili_push-0.1.6/nonebot_plugin_bili_push/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:32:03.170884 nonebot_plugin_bili_push-0.1.6/nonebot_plugin_bili_push.egg-info/
--rw-rw-rw-   0        0        0      268 2023-06-14 03:32:03.000000 nonebot_plugin_bili_push-0.1.6/nonebot_plugin_bili_push.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-14 03:32:03.000000 nonebot_plugin_bili_push-0.1.6/nonebot_plugin_bili_push.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 03:32:03.000000 nonebot_plugin_bili_push-0.1.6/nonebot_plugin_bili_push.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      111 2023-06-14 03:32:03.000000 nonebot_plugin_bili_push-0.1.6/nonebot_plugin_bili_push.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-14 03:32:03.000000 nonebot_plugin_bili_push-0.1.6/nonebot_plugin_bili_push.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 03:32:03.173886 nonebot_plugin_bili_push-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1069 2023-06-14 03:31:53.000000 nonebot_plugin_bili_push-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:38:30.748955 nonebot_plugin_bili_push-0.1.8/
+-rw-rw-rw-   0        0        0     1078 2023-06-13 02:14:36.000000 nonebot_plugin_bili_push-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      268 2023-06-14 06:38:30.747956 nonebot_plugin_bili_push-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1694 2023-06-14 03:27:08.000000 nonebot_plugin_bili_push-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 06:38:30.736955 nonebot_plugin_bili_push-0.1.8/nonebot_plugin_bili_push/
+-rw-rw-rw-   0        0        0    98887 2023-06-14 06:16:44.000000 nonebot_plugin_bili_push-0.1.8/nonebot_plugin_bili_push/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:38:30.745954 nonebot_plugin_bili_push-0.1.8/nonebot_plugin_bili_push.egg-info/
+-rw-rw-rw-   0        0        0      268 2023-06-14 06:38:30.000000 nonebot_plugin_bili_push-0.1.8/nonebot_plugin_bili_push.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-06-14 06:38:30.000000 nonebot_plugin_bili_push-0.1.8/nonebot_plugin_bili_push.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 06:38:30.000000 nonebot_plugin_bili_push-0.1.8/nonebot_plugin_bili_push.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      111 2023-06-14 06:38:30.000000 nonebot_plugin_bili_push-0.1.8/nonebot_plugin_bili_push.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-14 06:38:30.000000 nonebot_plugin_bili_push-0.1.8/nonebot_plugin_bili_push.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 06:38:30.749954 nonebot_plugin_bili_push-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1069 2023-06-14 06:38:18.000000 nonebot_plugin_bili_push-0.1.8/setup.py
```

### Comparing `nonebot_plugin_bili_push-0.1.6/LICENSE` & `nonebot_plugin_bili_push-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bili_push-0.1.6/README.md` & `nonebot_plugin_bili_push-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bili_push-0.1.6/nonebot_plugin_bili_push/__init__.py` & `nonebot_plugin_bili_push-0.1.8/nonebot_plugin_bili_push/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import os
+import requests
 import re
 from PIL import Image, ImageDraw, ImageFont
 from io import BytesIO
 import json
 from nonebot.adapters.onebot.v11 import Bot, MessageEvent, GroupMessageEvent, MessageSegment
 from nonebot import on_command
 import sqlite3
 from nonebot.adapters.onebot.v11 import GROUP_ADMIN, GROUP_OWNER
 import random
-from nonebot import require, logger
+from nonebot import require
 import nonebot
 from nonebot.plugin import PluginMetadata
-import httpx
-import asyncio
 
 require("nonebot_plugin_apscheduler")
 from nonebot_plugin_apscheduler import scheduler
 
 config = nonebot.get_driver().config
 # 读取配置
 #
@@ -38,31 +37,14 @@
 #
 # 配置4：
 # 是否使用api来获取emoji图像
 # 为True时使用api，为False时不使用api，为空时自动选择。
 # bilipush_emojiapi=True
 #
 
-
-def get_api(url: str, type: str = "json"):
-    if type == "json":
-        async def fetch(url):
-            async with httpx.AsyncClient(http2=True) as client:
-                response = await client.get(url)
-            return response.text
-        return_data = asyncio.get_event_loop().run_until_complete(fetch(apiurl))
-        return return_data
-
-    elif type == "image":
-        return httpx.get(apiurl).read()
-    return
-
-
-
-
 # 配置1：
 try:
     adminqq = config.superusers
     adminqq = list(adminqq)
 except:
     adminqq = []
 # 配置2：
@@ -77,15 +59,15 @@
     apiurl = "http://cdn.kanon.ink"
 # 配置4：
 try:
     use_api = config.bilipush_emojiapi
 except:
     try:
         get_url = apiurl + "/json/config?name=ping"
-        return_json = get_api(get_url, "json")
+        return_json = json.loads(requests.get(get_url).text)
         if return_json["code"] == 0:
             use_api = True
         else:
             use_api = False
     except:
         use_api = False
 
@@ -101,44 +83,37 @@
     supported_adapters={"~onebot.v11"},
     # 支持的适配器集合，其中 `~` 在此处代表前缀 `nonebot.adapters.`，其余适配器亦按此格式填写。
     # 若插件可以保证兼容所有适配器（即仅使用基本适配器功能）可不填写，否则应该列出插件支持的适配器。
 )
 
 # 创建基础参数
 returnpath = ""
-dbpath = basepath + 'botsdb/'
-configpart = dbpath + 'config/'
-fontdb = configpart + 'font.db'
-livedb = dbpath + "live/Kanon_push.db"
-emojidbname = dbpath + 'emoji/emoji.db'
-dbpath = basepath + 'botsdb/'
-pushlistdb = dbpath + "live/push_list.db"
-livelistdb = dbpath + "live/livelist.db"
-heartdb = basepath + 'local-ImgCache/heart.db'
-configpart = dbpath + 'config/'
-groupconfigdb = configpart + 'groupconfig.db'
+plugin_dbpath = basepath + 'db/bili_push/'
+if not os.path.exists(plugin_dbpath):
+    os.makedirs(plugin_dbpath)
+livedb = plugin_dbpath + "bili_push.db"
+heartdb = plugin_dbpath + "heart.db"
 half_text = ["A", "B", "C", "D", "E", "F", "G", "H", "I", "J", "K", "L", "M", "N", "O", "P", "Q", "R", "S", "T", "U",
              "V", "W", "X", "Y", "Z", "a", "b", "c", "d", "e", "f", "g", "h", "i", "j", "k", "l", "m", "n", "o", "p",
              "q", "r", "s", "t", "u", "v", "w", "x", "y", "z", "1", "2", "3", "4", "5", "6", "7", "8", "9", "0", ",",
              ".", "/", "\\", "[", "]", "(", ")", "!", "+", "-", "*", "！", "？", "。", "，", "{", "}", "、", "‘", "“",
              '"', "'", "！", " "]
 
 
-
-
 def get_emoji(emoji):
     cachepath = basepath + "cache/emoji/"
     if not os.path.exists(cachepath):
         os.makedirs(cachepath)
     cachepath = cachepath + emoji + ".png"
     if not cachepath.exists():
         if use_api:
             url = apiurl + "/api/emoji?imageid=" + emoji
             try:
-                return_image = get_api(url, "image")
+                return_image = requests.get(url)
+                return_image = Image.open(BytesIO(return_image.content))
                 return_image.save(cachepath)
             except:
                 print("api出错，请联系开发者")
                 # api出错时直接打印文字
                 return_image = Image.new("RGBA", (100, 100), color=(0, 0, 0, 0))
                 paste_image = draw_text(emoji, 100, 10)
                 return_image.paste(paste_image, (0, 0), mask=paste_image)
@@ -371,29 +346,18 @@
                     # 粘贴biliemoji
                     for emoji_info in biliemoji_infos:
                         emoji_name = emoji_info["emoji_name"]
                         if emoji_name == biliemoji_name:
                             emoji_url = emoji_info["url"]
                             x_num += 1
             if biliemoji_name == "":
-                conn = sqlite3.connect(emojidbname)
-                cursor = conn.cursor()
-                cursor.execute('select * from emoji where emoji = "' + fort + '"')
-                data = cursor.fetchone()
-                cursor.close()
-                conn.close()
-                if data is None:
-                    # 打印文字
+                if not is_emoji(fort):
                     if fort in half_text:
                         x_num -= 0.4
-                else:
-                    # 打印表情
-                    if not is_emoji(fort):
-                        if fort in half_text:
-                            x_num -= 0.4
+
     x = int((textlen + 1) * size)
     y = int((y_num + 1) * size * 1.2)
 
     image = Image.new("RGBA", size=(x, y), color=(0, 0, 0, 0))  # 生成透明图片
     draw_image = ImageDraw.Draw(image)
     fortsize = size
     font = ImageFont.truetype(font=fontfile, size=fortsize)
@@ -676,21 +640,16 @@
                                             paste_image = paste_image.resize((int(fortsize * 1.2), int(fortsize * 1.2)))
                                             draw_image.paste(paste_image,
                                                              (int(x + print_x * fortsize), int(y + print_y * fortsize)))
                                             print_x += 0.5
 
                             if emoji_code == "":
                                 # 检测是否半格字符
-                                conn = sqlite3.connect(emojidbname)
-                                cursor = conn.cursor()
-                                cursor.execute('select * from emoji where emoji = "' + text + '"')
-                                data = cursor.fetchone()
-                                cursor.close()
-                                conn.close()
-                                if data is None:
+                                if not is_emoji(font):
+
                                     # 打印文字
                                     draw.text(xy=(int(x + print_x * fortsize), int(y + print_y * fortsize)), text=text,
                                               fill=(0, 0, 0), font=cache_font)
                                     if text in half_text:
                                         print_x -= 0.4
                                 else:
                                     # 打印表情
@@ -761,24 +720,15 @@
                                                 draw_image.paste(paste_image,
                                                                  (int(x + print_x * fortsize),
                                                                   int(y + print_y * fortsize)))
                                                 print_x += 0.5
 
                                 if emoji_code == "":
                                     # 检测是否半格字符
-                                    conn = sqlite3.connect(emojidbname)
-                                    cursor = conn.cursor()
-                                    try:
-                                        cursor.execute('select * from emoji where emoji = "' + text + '"')
-                                        data = cursor.fetchone()
-                                    except:
-                                        data = None
-                                    cursor.close()
-                                    conn.close()
-                                    if data is None:
+                                    if not is_emoji(font):
                                         # 打印文字
                                         draw.text(xy=(int(x + print_x * fortsize), int(y + print_y * fortsize)),
                                                   text=text,
                                                   fill=(100, 100, 100), font=cache_font)
                                         if text in half_text:
                                             print_x -= 0.4
                                     else:
@@ -1429,21 +1379,15 @@
                                     paste_image = paste_image.resize((int(fortsize * 1.2), int(fortsize * 1.2)))
                                     draw_image.paste(paste_image,
                                                      (int(x + print_x * fortsize), int(y + print_y * fortsize)))
                                     print_x += 0.5
 
                     if emoji_code == "":
                         # 检测是否半格字符
-                        conn = sqlite3.connect(emojidbname)
-                        cursor = conn.cursor()
-                        cursor.execute('select * from emoji where emoji = "' + text + '"')
-                        data = cursor.fetchone()
-                        cursor.close()
-                        conn.close()
-                        if data is None:
+                        if not is_emoji(font):
                             # 打印文字
                             draw.text(xy=(int(x + print_x * fortsize), int(y + print_y * fortsize)), text=text,
                                       fill=(0, 0, 0), font=font)
                             if text in half_text:
                                 print_x -= 0.4
                         else:
                             # 打印表情
@@ -1520,21 +1464,15 @@
                                     paste_image = paste_image.resize((int(fortsize * 1.2), int(fortsize * 1.2)))
                                     draw_image.paste(paste_image,
                                                      (int(x + print_x * fortsize), int(y + print_y * fortsize)))
                                     print_x += 0.5
 
                     if emoji_code == "":
                         # 检测是否半格字符
-                        conn = sqlite3.connect(emojidbname)
-                        cursor = conn.cursor()
-                        cursor.execute('select * from emoji where emoji = "' + text + '"')
-                        data = cursor.fetchone()
-                        cursor.close()
-                        conn.close()
-                        if data is None:
+                        if not is_emoji(font):
                             # 打印文字
                             draw.text(xy=(int(x + print_x * fortsize), int(y + print_y * fortsize)), text=text,
                                       fill=(0, 0, 0), font=cache_font)
                             if text in half_text:
                                 print_x -= 0.4
                         else:
                             # 打印表情
@@ -1598,21 +1536,15 @@
                                     paste_image = paste_image.resize((int(fortsize * 1.2), int(fortsize * 1.2)))
                                     draw_image.paste(paste_image,
                                                      (int(x + print_x * fortsize), int(y + print_y * fortsize)))
                                     print_x += 0.5
 
                     if emoji_code == "":
                         # 检测是否半格字符
-                        conn = sqlite3.connect(emojidbname)
-                        cursor = conn.cursor()
-                        cursor.execute('select * from emoji where emoji = "' + text + '"')
-                        data = cursor.fetchone()
-                        cursor.close()
-                        conn.close()
-                        if data is None:
+                        if not is_emoji(font):
                             # 打印文字
                             draw.text(xy=(int(x + print_x * fortsize), int(y + print_y * fortsize)), text=text,
                                       fill=(100, 100, 100), font=cache_font)
                             if text in half_text:
                                 print_x -= 0.4
                         else:
                             # 打印表情
@@ -1636,15 +1568,15 @@
 
 
 @get_new.handle()
 async def _(bot: Bot, messageevent: MessageEvent):
     print("bili-push_command")
     returnpath = ""
     code = 0
-    qq = int(messageevent.get_user_id())
+    qq = str(messageevent.get_user_id())
     message = messageevent.get_message()
     message = str(message)
     commands = get_commands(message)
     command = str(commands[0])
     command = command.removeprefix("/")
     if len(commands) >= 2:
         command2 = commands[1]
@@ -1792,14 +1724,25 @@
                     returnjson = json.loads(returnjson)
                     returncode = returnjson["code"]
                     if returncode == 0:
                         print('获取动态图片并发送')
                         # 获取动态id并保存
                         return_datas = returnjson["data"]["cards"]
 
+                        try:
+                            conn = sqlite3.connect(livedb)
+                            cursor = conn.cursor()
+                            cursor.execute('create table ' + groupcode +
+                                           '(dynamicid int(10) primary key, uid varchar(10))')
+                            cursor.close()
+                            conn.commit()
+                            conn.close()
+                        except:
+                            print()
+
                         conn = sqlite3.connect(livedb)
                         cursor = conn.cursor()
                         for return_data in return_datas:
                             dynamicid = str(return_data["desc"]["dynamic_id"])
                             cursor.execute(
                                 "replace into "+groupcode+"(dynamicid,uid) values('" + dynamicid + "','" + uid + "')")
                         cursor.close()
@@ -1939,15 +1882,15 @@
 
     groups = await nonebot.get_bot().get_group_list()
     grouplist = []
     for memberinfo in groups:
         grouplist.append(str(memberinfo['group_id']))
 
     # ############获取动态############s
-    run = False  # 代码折叠
+    run = True  # 代码折叠
     if run:
         print('---------获取更新的动态----------')
         print("获取订阅列表")
         try:
             # 数据库文件 如果文件不存在，会自动在当前目录中创建
             conn = sqlite3.connect(livedb)
             cursor = conn.cursor()
@@ -2035,33 +1978,14 @@
         cursor = conn.cursor()
         cursor.execute("SELECT * FROM subscriptionlist")
         subscriptions = cursor.fetchall()
         cursor.close()
         conn.commit()
         conn.close()
 
-        # 添加邦推送
-        conn = sqlite3.connect(groupconfigdb)
-        cursor = conn.cursor()
-        cursor.execute("select * from groupconfig where bilibilidynamic = 'on'")
-        configs = cursor.fetchall()
-        cursor.close()
-        conn.commit()
-        conn.close()
-
-        for config in configs:
-            groupcode = str(config[0])
-            uids = ["1459104794", "171818544", "354218272"]
-            for uid in uids:
-                subscription = []
-                subscription.append("data")
-                subscription.append(groupcode)
-                subscription.append(uid)
-                subscriptions.append(subscription)
-
         if not subscriptions:
             print("无订阅")
         else:
             for subscription in subscriptions:
                 groupcode = subscription[1]
                 uid = str(subscription[2])
                 # 判断是否本bot以及是否主bot
```

### Comparing `nonebot_plugin_bili_push-0.1.6/setup.py` & `nonebot_plugin_bili_push-0.1.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         'nonebot_adapter_onebot>=2.2.3',
         'nonebot_plugin_apscheduler>=0.2.0'
     ]
     return reqs
 
 
 setup(name='nonebot_plugin_bili_push',
-      version='0.1.6',
+      version='0.1.8',
       description='nonebot2 plugin',
       author='SuperGuGuGu',
       author_email='13680478000@163.com',
       url='https://github.com/SuperGuGuGu/nonebot_plugin_bili_push',
       packages=find_packages(),
       python_requires=">=3.8",
       install_requires=get_install_requires(),
```

