# Comparing `tmp/nonebot_plugin_smart_reply-0.0.8.tar.gz` & `tmp/nonebot_plugin_smart_reply-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_smart_reply-0.0.8.tar", last modified: Sun Sep 18 12:00:27 2022, max compression
+gzip compressed data, was "nonebot_plugin_smart_reply-0.0.9.tar", last modified: Mon Nov 21 14:06:32 2022, max compression
```

## Comparing `nonebot_plugin_smart_reply-0.0.8.tar` & `nonebot_plugin_smart_reply-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2022-09-18 12:00:27.709842 nonebot_plugin_smart_reply-0.0.8/
--rw-rw-rw-   0        0        0      308 2022-09-18 12:00:27.708836 nonebot_plugin_smart_reply-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      366 2022-06-18 06:47:22.000000 nonebot_plugin_smart_reply-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-09-18 12:00:27.671842 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/
--rw-rw-rw-   0        0        0     3281 2022-09-18 11:54:42.000000 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-18 12:00:27.668811 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/
-drwxrwxrwx   0        0        0        0 2022-09-18 12:00:27.707810 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/
--rw-rw-rw-   0        0        0    32921 2022-09-18 11:54:42.000000 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/cnm傻逼吃屎滚.aac
--rw-rw-rw-   0        0        0   122981 2022-09-18 11:54:42.000000 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊(振声!).aac
--rw-rw-rw-   0        0        0    67013 2022-09-18 11:54:42.000000 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊我超.aac
--rw-rw-rw-   0        0        0    42760 2022-09-18 11:54:42.000000 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/你是不是有毛病.aac
--rw-rw-rw-   0        0        0    36232 2022-09-18 11:54:42.000000 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/你正常一点.aac
--rw-rw-rw-   0        0        0    11615 2022-09-18 11:54:42.000000 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/傻逼.aac
--rw-rw-rw-   0        0        0    68879 2022-09-18 11:54:42.000000 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/南通啊.aac
--rw-rw-rw-   0        0        0    15206 2022-09-18 11:54:42.000000 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/去死吧.aac
--rw-rw-rw-   0        0        0   101527 2022-09-18 11:54:42.000000 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/变态啊.aac
--rw-rw-rw-   0        0        0   105258 2022-09-18 11:54:42.000000 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/啊你好烦啊.aac
--rw-rw-rw-   0        0        0     6491 2022-09-18 11:54:42.000000 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/我草泥马.aac
--rw-rw-rw-   0        0        0    15706 2022-09-18 11:54:42.000000 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/操你妈.aac
--rw-rw-rw-   0        0        0    96863 2022-09-18 11:54:42.000000 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/救命啊.aac
--rw-rw-rw-   0        0        0    14470 2022-09-18 11:54:42.000000 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/草泥马(慢).aac
--rw-rw-rw-   0        0        0    74476 2022-09-18 11:54:42.000000 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/非礼啊.aac
-drwxrwxrwx   0        0        0        0 2022-09-18 12:00:27.708836 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/json/
--rw-rw-rw-   0        0        0    81633 2022-09-18 11:54:42.000000 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/json/data.json
--rw-rw-rw-   0        0        0     3403 2022-09-18 11:54:42.000000 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/utils.py
-drwxrwxrwx   0        0        0        0 2022-09-18 12:00:27.677812 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply.egg-info/
--rw-rw-rw-   0        0        0      308 2022-09-18 12:00:27.000000 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1298 2022-09-18 12:00:27.000000 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-18 12:00:27.000000 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2022-09-18 12:00:27.000000 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2022-09-18 12:00:27.000000 nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-18 12:00:27.709842 nonebot_plugin_smart_reply-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      585 2022-09-18 11:59:04.000000 nonebot_plugin_smart_reply-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-21 14:06:32.872003 nonebot_plugin_smart_reply-0.0.9/
+-rw-rw-rw-   0        0        0      269 2022-11-21 14:06:32.871003 nonebot_plugin_smart_reply-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2022-06-18 06:47:22.000000 nonebot_plugin_smart_reply-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-11-21 14:06:32.814003 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/
+-rw-rw-rw-   0        0        0     3561 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-21 14:06:32.811004 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/
+drwxrwxrwx   0        0        0        0 2022-11-21 14:06:32.869003 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/
+-rw-rw-rw-   0        0        0    32921 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/cnm傻逼吃屎滚.aac
+-rw-rw-rw-   0        0        0   122981 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊(振声!).aac
+-rw-rw-rw-   0        0        0    67013 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊我超.aac
+-rw-rw-rw-   0        0        0    42760 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/你是不是有毛病.aac
+-rw-rw-rw-   0        0        0    36232 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/你正常一点.aac
+-rw-rw-rw-   0        0        0    11615 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/傻逼.aac
+-rw-rw-rw-   0        0        0    68879 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/南通啊.aac
+-rw-rw-rw-   0        0        0    15206 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/去死吧.aac
+-rw-rw-rw-   0        0        0   101527 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/变态啊.aac
+-rw-rw-rw-   0        0        0   105258 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/啊你好烦啊.aac
+-rw-rw-rw-   0        0        0     6491 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/我草泥马.aac
+-rw-rw-rw-   0        0        0    15706 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/操你妈.aac
+-rw-rw-rw-   0        0        0    96863 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/救命啊.aac
+-rw-rw-rw-   0        0        0    14470 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/草泥马(慢).aac
+-rw-rw-rw-   0        0        0    74476 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/非礼啊.aac
+drwxrwxrwx   0        0        0        0 2022-11-21 14:06:32.870003 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/json/
+-rw-rw-rw-   0        0        0    81633 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/json/data.json
+-rw-rw-rw-   0        0        0     3594 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/utils.py
+drwxrwxrwx   0        0        0        0 2022-11-21 14:06:32.842004 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply.egg-info/
+-rw-rw-rw-   0        0        0      269 2022-11-21 14:06:32.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1298 2022-11-21 14:06:32.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-21 14:06:32.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2022-11-21 14:06:32.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2022-11-21 14:06:32.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-11-21 14:06:32.872003 nonebot_plugin_smart_reply-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      585 2022-11-21 14:06:07.000000 nonebot_plugin_smart_reply-0.0.9/setup.py
```

### Comparing `nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/__init__.py` & `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from loguru import logger
 
 
 # 这个值为False时, 使用的是小爱同学, True时使用的是青云客api
 api_flag = True
 # 优先级1, 向下阻断, 需要艾特bot, 智能回复api切换指令, 目前有俩api, 分别是qinyunke_api和小爱同学, 默认qinyun
 api_switch = on_command("智障回复api切换", aliases={
-                        "ai切换", "api_switch","智能回复api切换"}, permission=SUPERUSER, rule=to_me(), block=True)
+                        "ai切换", "api_switch", "智能回复api切换"}, permission=SUPERUSER, rule=to_me(), block=True)
 # 优先级99, 条件: 艾特bot就触发
 ai = on_message(rule=to_me(), priority=99, block=False)
 # 优先级1, 不会向下阻断, 条件: 戳一戳bot触发
 poke_ = on_notice(rule=to_me(), block=False)
 
 
 @api_switch.handle()
@@ -58,16 +58,20 @@
     # 如果词库没有结果，则调用api获取智能回复
     if result == None:
         if api_flag:
             qinyun_url = f"http://api.qingyunke.com/api.php?key=free&appid=0&msg={msg}"
             message = await qinyun_reply(qinyun_url)
             logger.info("来自青云客的智能回复: " + message)
         else:
-            xiaoai_url = f"https://jintia.jintias.cn/api/xatx.php?msg={msg}"
+            xiaoai_url = f"https://apibug.cn/api/xiaoai/?msg={msg}&apiKey={apiKey}"
+            if apiKey == "寄":
+                await ai.finish("小爱同学apiKey未设置, 请联系SUPERUSERS在.env中设置")
             message = await xiaoice_reply(xiaoai_url)
+            if message == "寄":
+                await ai.finish("小爱同学apiKey错误, 请联系SUPERUSERS在.env中重新设置")
             logger.info("来自小爱同学的智能回复: " + message)
         await ai.finish(message=message)
     await ai.finish(Message(result))
 
 
 @poke_.handle()
 async def _poke_event(event: PokeNotifyEvent):
```

### Comparing `nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/cnm傻逼吃屎滚.aac` & `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/cnm傻逼吃屎滚.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊(振声!).aac` & `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊(振声!).aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊我超.aac` & `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊我超.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/你是不是有毛病.aac` & `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/你是不是有毛病.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/你正常一点.aac` & `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/你正常一点.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/傻逼.aac` & `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/傻逼.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/南通啊.aac` & `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/南通啊.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/去死吧.aac` & `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/去死吧.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/变态啊.aac` & `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/变态啊.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/啊你好烦啊.aac` & `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/啊你好烦啊.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/我草泥马.aac` & `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/我草泥马.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/操你妈.aac` & `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/操你妈.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/救命啊.aac` & `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/救命啊.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/草泥马(慢).aac` & `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/草泥马(慢).aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/audio/非礼啊.aac` & `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/非礼啊.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/resource/json/data.json` & `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/json/data.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply/utils.py` & `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,30 @@
 try:
     import ujson as json
 except ModuleNotFoundError:
     import json
 from httpx import AsyncClient
 import re
 
+try:
+    apiKey: str = nonebot.get_driver().config.xiaoai_apikey
+except:
+    apiKey: str = "寄"
 
-Bot_NICKNAME: str = list(nonebot.get_driver().config.nickname)[0]      # bot的nickname,可以换成你自己的
-Bot_MASTER: str = list(nonebot.get_driver().config.superusers)[0]      # bot的主人名称,也可以换成你自己的
+try:
+    Bot_NICKNAME: str = nonebot.get_driver(
+    ).config.Bot_NICKNAME     # bot的nickname,可以换成你自己的
+    Bot_MASTER: str = nonebot.get_driver().config.Bot_MASTER      # bot的主人名称,也可以换成你自己的
+except:
+    Bot_NICKNAME: str = "脑积水"
+    Bot_MASTER: str = "脑积水"
 # NICKNAME: str = "Hinata"
 # MASTER: str = "星野日向_Official"
 
 
-
 # 载入词库(这个词库有点涩)
 AnimeThesaurus = json.load(open(Path(os.path.join(os.path.dirname(
     __file__), "resource/json")) / "data.json", "r", encoding="utf8"))
 
 
 # 获取resource/audio下面的全部文件
 aac_file_path = os.path.join(os.path.dirname(__file__), "resource/audio")
@@ -59,33 +67,40 @@
     "再戳一下试试？",
     "正在关闭对您的所有服务...关闭成功",
     "啊呜，太舒服刚刚竟然睡着了。什么事？",
     "正在定位您的真实地址...定位成功。轰炸机已起飞",
 ]
 
 # 从字典里返还消息, 抄(借鉴)的zhenxun-bot
+
+
 async def get_chat_result(text: str, nickname: str) -> str:
     if len(text) < 7:
         keys = AnimeThesaurus.keys()
         for key in keys:
             if text.find(key) != -1:
                 return random.choice(AnimeThesaurus[key]).replace("你", nickname)
 
 # 从qinyunke_api拿到消息
+
+
 async def qinyun_reply(url):
     async with AsyncClient() as client:
         response = await client.get(url)
         # 这个api好像问道主人或者他叫什么名字会返回私活,这里replace掉部分
-        res = response.json()["content"].replace("林欣", Bot_MASTER).replace("{br}", "\n").replace("贾彦娟", Bot_MASTER).replace("周超辉", Bot_MASTER).replace("鑫总", Bot_MASTER).replace("张鑫", Bot_MASTER).replace("菲菲", Bot_NICKNAME).replace("dn", Bot_MASTER).replace("1938877131", "2749903559").replace("小燕", Bot_NICKNAME)
+        res = response.json()["content"].replace("林欣", Bot_MASTER).replace("{br}", "\n").replace("贾彦娟", Bot_MASTER).replace("周超辉", Bot_MASTER).replace(
+            "鑫总", Bot_MASTER).replace("张鑫", Bot_MASTER).replace("菲菲", Bot_NICKNAME).replace("dn", Bot_MASTER).replace("1938877131", "2749903559").replace("小燕", Bot_NICKNAME)
         res = re.sub(u"\\{.*?\\}", "", res)
         if "taobao" in res:
             res = Bot_NICKNAME + "暂时听不懂主人说的话呢"
         return res
 
 # 从小爱同学api拿到消息, 这个api私货比较少
+
+
 async def xiaoice_reply(url):
     async with AsyncClient() as client:
-        res = (await client.get(url)).text
-        res = res[res.find("{"):res.rfind("}")+1]
-        res = json.loads(res)
-        res = res["text"].replace("小爱", Bot_NICKNAME)
-        return res
+        res = (await client.get(url)).json()
+        if res["code"] == 200:
+            return (res["text"]).replace("小爱", Bot_NICKNAME)
+        else:
+            return "寄"
```

### Comparing `nonebot_plugin_smart_reply-0.0.8/nonebot_plugin_smart_reply.egg-info/SOURCES.txt` & `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.8/setup.py` & `nonebot_plugin_smart_reply-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 
 from setuptools import find_packages, setup
 name = 'nonebot_plugin_smart_reply'
 
 setup(
     name=name,  
-    version='0.0.8',
+    version='0.0.9',
     author="Special-Week",
     author_email='2385612749@qq.com',
     description="encapsulate logger",
     python_requires=">=3.8.*",
     packages=find_packages(),
     long_description="reply插件",
     url="https://github.com/Special-Week/nonebot_plugin_smart_reply",
```

