# Comparing `tmp/karas_py-0.2.8.tar.gz` & `tmp/karas_py-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\karas_py-0.2.8.tar", last modified: Sun Jan  8 15:03:32 2023, max compression
+gzip compressed data, was "karas_py-0.2.9.tar", last modified: Wed Feb  1 01:54:10 2023, max compression
```

## Comparing `karas_py-0.2.8.tar` & `karas_py-0.2.9.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-01-08 15:03:32.176230 karas_py-0.2.8/
--rw-rw-rw-   0        0        0     2769 2023-01-08 15:03:32.176230 karas_py-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     1754 2023-01-08 14:24:56.000000 karas_py-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-01-08 15:03:32.165228 karas_py-0.2.8/karas/
--rw-rw-rw-   0        0        0    59125 2023-01-08 14:59:57.000000 karas_py-0.2.8/karas/__init__.py
--rw-rw-rw-   0        0        0     2084 2023-01-07 11:02:29.000000 karas_py-0.2.8/karas/box.py
--rw-rw-rw-   0        0        0     6448 2023-01-07 09:51:49.000000 karas_py-0.2.8/karas/chain.py
--rw-rw-rw-   0        0        0     9302 2023-01-07 11:03:55.000000 karas_py-0.2.8/karas/elements.py
--rw-rw-rw-   0        0        0    15202 2023-01-08 07:53:44.000000 karas_py-0.2.8/karas/event.py
--rw-rw-rw-   0        0        0     2118 2023-01-07 11:00:03.000000 karas_py-0.2.8/karas/exceptions.py
--rw-rw-rw-   0        0        0     3696 2023-01-07 11:04:13.000000 karas_py-0.2.8/karas/messages.py
--rw-rw-rw-   0        0        0      828 2023-01-07 11:08:16.000000 karas_py-0.2.8/karas/permission.py
--rw-rw-rw-   0        0        0     3329 2023-01-07 11:02:29.000000 karas_py-0.2.8/karas/sender.py
-drwxrwxrwx   0        0        0        0 2023-01-08 15:03:32.171230 karas_py-0.2.8/karas/util/
--rw-rw-rw-   0        0        0      126 2022-06-12 15:02:37.000000 karas_py-0.2.8/karas/util/Listener.py
--rw-rw-rw-   0        0        0     5678 2023-01-08 14:24:38.000000 karas_py-0.2.8/karas/util/Logger.py
--rw-rw-rw-   0        0        0     2147 2023-01-07 10:33:36.000000 karas_py-0.2.8/karas/util/__init__.py
--rw-rw-rw-   0        0        0     3181 2023-01-07 11:02:48.000000 karas_py-0.2.8/karas/util/network.py
--rw-rw-rw-   0        0        0     1521 2022-06-12 15:02:37.000000 karas_py-0.2.8/karas/util/sync.py
-drwxrwxrwx   0        0        0        0 2023-01-08 15:03:32.175231 karas_py-0.2.8/karas_py.egg-info/
--rw-rw-rw-   0        0        0     2769 2023-01-08 15:03:32.000000 karas_py-0.2.8/karas_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      438 2023-01-08 15:03:32.000000 karas_py-0.2.8/karas_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-08 15:03:32.000000 karas_py-0.2.8/karas_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-01-08 15:03:32.000000 karas_py-0.2.8/karas_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-01-08 15:03:32.000000 karas_py-0.2.8/karas_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-08 15:03:32.176230 karas_py-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      902 2023-01-03 03:54:04.000000 karas_py-0.2.8/setup.py
+drwxrwxrwx   0 shiro     (1000) shiro     (1000)        0 2023-02-01 01:54:10.630759 karas_py-0.2.9/
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)    35184 2022-06-12 15:02:36.000000 karas_py-0.2.9/LICENSE
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     2261 2023-02-01 01:54:10.629759 karas_py-0.2.9/PKG-INFO
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     1756 2023-02-01 01:54:02.000000 karas_py-0.2.9/README.md
+drwxrwxrwx   0 shiro     (1000) shiro     (1000)        0 2023-02-01 01:54:10.496758 karas_py-0.2.9/karas/
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)    59175 2023-02-01 01:53:34.000000 karas_py-0.2.9/karas/__init__.py
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     2111 2023-02-01 01:36:01.000000 karas_py-0.2.9/karas/box.py
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     6448 2023-01-07 09:51:49.000000 karas_py-0.2.9/karas/chain.py
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     9302 2023-01-07 11:03:55.000000 karas_py-0.2.9/karas/elements.py
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)    15447 2023-02-01 01:35:26.000000 karas_py-0.2.9/karas/event.py
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     2118 2023-01-07 11:00:03.000000 karas_py-0.2.9/karas/exceptions.py
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     3696 2023-01-07 11:04:13.000000 karas_py-0.2.9/karas/messages.py
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)      828 2023-01-07 11:08:16.000000 karas_py-0.2.9/karas/permission.py
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     3329 2023-01-07 11:02:29.000000 karas_py-0.2.9/karas/sender.py
+drwxrwxrwx   0 shiro     (1000) shiro     (1000)        0 2023-02-01 01:54:10.564758 karas_py-0.2.9/karas/util/
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)      126 2022-06-12 15:02:37.000000 karas_py-0.2.9/karas/util/Listener.py
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     5678 2023-01-08 14:24:38.000000 karas_py-0.2.9/karas/util/Logger.py
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     2147 2023-01-07 10:33:36.000000 karas_py-0.2.9/karas/util/__init__.py
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     3181 2023-01-07 11:02:48.000000 karas_py-0.2.9/karas/util/network.py
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     1521 2022-06-12 15:02:37.000000 karas_py-0.2.9/karas/util/sync.py
+drwxrwxrwx   0 shiro     (1000) shiro     (1000)        0 2023-02-01 01:54:10.617759 karas_py-0.2.9/karas_py.egg-info/
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     2261 2023-02-01 01:54:10.000000 karas_py-0.2.9/karas_py.egg-info/PKG-INFO
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)      446 2023-02-01 01:54:10.000000 karas_py-0.2.9/karas_py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)        1 2023-02-01 01:54:10.000000 karas_py-0.2.9/karas_py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)       15 2023-02-01 01:54:10.000000 karas_py-0.2.9/karas_py.egg-info/requires.txt
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)        6 2023-02-01 01:54:10.000000 karas_py-0.2.9/karas_py.egg-info/top_level.txt
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)       38 2023-02-01 01:54:10.631760 karas_py-0.2.9/setup.cfg
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)      902 2023-01-03 03:54:04.000000 karas_py-0.2.9/setup.py
```

### Comparing `karas_py-0.2.8/README.md` & `karas_py-0.2.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <div style="text-align: center">
     <h1>Karas</h1><br>
 <p>这是一个基于<a href="https://github.com/project-mirai/mirai-api-http">mirai-api-http</a>的轻量级，高性能qq消息处理与发送框架  </p>
 </div>
 
 ##  Version  
-![Mirai-API-API-Version](https://img.shields.io/badge/mirai--http--api-2.5.0-brightgreen.svg?style=plastic)
+![Mirai-API-API-Version](https://img.shields.io/badge/mirai--http--api->=2.5.0-brightgreen.svg?style=plastic)
 ![python-Version](https://img.shields.io/badge/python->=3.7-brightgreen.svg?style=plastic)
-![karas-Version](https://img.shields.io/badge/karas-0.2.8-brightgreen.svg?style=plastic)    
+![karas-Version](https://img.shields.io/badge/karas-0.2.9-brightgreen.svg?style=plastic)    
 ## 使用  
 - 使用pip安装本项目  
 ```shell script
 pip3 install karas_py
 ```  
 - 一个群聊复读机实例:  
 (async)
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 ****** Karas ******
 
 è¿æ¯ä¸ä¸ªåºäºmirai-api-
 httpçè½»éçº§ï¼é«æ§è½qqæ¶æ¯å¤çä¸åéæ¡æ¶
 ## Version ![Mirai-API-API-Version](https://img.shields.io/badge/mirai--http--
-api-2.5.0-brightgreen.svg?style=plastic) ![python-Version](https://
+api->=2.5.0-brightgreen.svg?style=plastic) ![python-Version](https://
 img.shields.io/badge/python->=3.7-brightgreen.svg?style=plastic) ![karas-
-Version](https://img.shields.io/badge/karas-0.2.8-
+Version](https://img.shields.io/badge/karas-0.2.9-
 brightgreen.svg?style=plastic) ## ä½¿ç¨ - ä½¿ç¨pipå®è£æ¬é¡¹ç® ```shell
 script pip3 install karas_py ``` - ä¸ä¸ªç¾¤èå¤è¯»æºå®ä¾: (async)
 ```python from karas.box import Yurine,MessageChain,Group yurine = Yurine
 ( host="localhost", port=8080, qq=114514, verifyKey="1919810" ) @yurine.listen
 ("GroupMessage") async def gm_event(group:Group, message: MessageChain): #
 async send message await yurine.sendGroup(group, message) yurine.run_forever()
 ``` (sync send message) ```python from karas.box import
```

### Comparing `karas_py-0.2.8/karas/__init__.py` & `karas_py-0.2.9/karas/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from karas.elements import ElementBase, File, FlashImage, GroupConfig, Image, MemberInfo, Plain, Source, Voice, \
     FriendProfile, MemberProfile, \
     BotProfile, UserProfile
 from karas.exceptions import *
 from karas.util.Logger import Logging
 from karas.util.network import error_throw, URL_Route, wrap_data_json
 
-__version__ = "0.2.8"
+__version__ = "0.2.9"
 
 
 async def _build_content_json(
         _type: str,
         _obj: Union[ReceptorBase, int],
         _quote: Optional[Source],
         _chain: List
@@ -261,28 +261,29 @@
         """事件监听器"""
         self._receiver_is_running = True
         while True:
             try:
                 _receive_data: Dict = data or await self.ws.receive_json()
             except TypeError:
                 if self.online:
-                    self.logging.warning(f"not valid response")
+                    self.logging.warning(f"invalid response")
                     continue
                 await asyncio.sleep(3)
             except Exception:
                 raise
             syncId = _receive_data.get("syncId")
             if syncId == "-1":
                 _parser = self.karas.event_parse(
                     _receive_data["data"], self.logging)
                 _event = await _parser.__anext__()
                 if isinstance(_event, Event):
                     if not self.online and isinstance(_event.event, BotOnlineEvent):
                         self.logging.info("bot online")
                         self.online = True
+                        await _parser.asend(False)
                     if isinstance(_event.event, BotOfflineEventActive):
                         self.logging.warning("Bot offline, waiting reload...")
                         self.online = self.online and False
                         await asyncio.sleep(3)
                         try:
                             await self._connect()
                         except BotNotFoundException:
```

### Comparing `karas_py-0.2.8/karas/box.py` & `karas_py-0.2.9/karas/box.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     GroupMuteAllEvent,
     GroupAllowAnonymousChatEvent,
     GroupAllowConfessTalkEvent,
     GroupAllowMemberInviteEvent,
     MemberJoinEvent,
     MemberLeaveEventKick,
     MemberLeaveEventQuit,
+    BotLeaveEventDisband,
     MemberCardChangeEvent,
     MemberSpecialTitleChangeEvent,
     MemberPermissionChangeEvent,
     MemberMuteEvent,
     MemberUnmuteEvent,
     MemberHonorChangeEvent,
     NewFriendRequestEvent,
```

### Comparing `karas_py-0.2.8/karas/chain.py` & `karas_py-0.2.9/karas/chain.py`

 * *Files identical despite different names*

### Comparing `karas_py-0.2.8/karas/elements.py` & `karas_py-0.2.9/karas/elements.py`

 * *Files identical despite different names*

### Comparing `karas_py-0.2.8/karas/event.py` & `karas_py-0.2.9/karas/event.py`

 * *Files 7% similar despite different names*

```diff
@@ -193,14 +193,21 @@
     operator: Member
     group: Group
 
     def __str__(self) -> str:
         return super().__str__() + f":{self.group}"
 
 
+class BotLeaveEventDisband(GroupEventBase):
+    """Bot因群主解散群而退出群, 操作人一定是群主"""
+    type: str = "BotLeaveEventDisband"
+    group: Group
+    operator: Member
+
+
 class GroupRecallEvent(GroupEventBase):
     """群消息撤回"""
     type: str = "GroupRecallEvent"
     authorId: int
     messageId: int
     time: int
     group: Group
@@ -486,14 +493,15 @@
 
     BotGroupPermissionChangeEvent: "BotGroupPermissionChangeEvent" = BotGroupPermissionChangeEvent
     BotMuteEvent: "BotMuteEvent" = BotMuteEvent
     BotUnmuteEvent: "BotUnmuteEvent" = BotUnmuteEvent
     BotJoinGroupEvent: "BotJoinGroupEvent" = BotJoinGroupEvent
     BotLeaveEventActive: "BotLeaveEventActive" = BotLeaveEventActive
     BotLeaveEventKick: "BotLeaveEventKick" = BotLeaveEventKick
+    BotLeaveEventDisband: "BotLeaveEventDisband" = BotLeaveEventDisband
     GroupRecallEvent: "GroupRecallEvent" = GroupRecallEvent
     FriendRecallEvent: "FriendRecallEvent" = FriendRecallEvent
     NudgeEvent: "NudgeEvent" = NudgeEvent
 
     GroupNameChangeEvent: "GroupNameChangeEvent" = GroupNameChangeEvent
     GroupEntranceAnnouncementChangeEvent: "GroupEntranceAnnouncementChangeEvent" = GroupEntranceAnnouncementChangeEvent
     GroupMuteAllEvent: "GroupMuteAllEvent" = GroupMuteAllEvent
@@ -523,12 +531,12 @@
         """将传进的原始数据转换成对应的事件对象
 
         Returns:
             Event: 一个已经被自动解析完成的事件对象
         """
         _type = kwargs.get("type")
         if _type in __events__.get("messageEvent"):
-            _messageEvent: "MessageBase" = MessageEnum[_type].value
+            _messageEvent = MessageEnum[_type].value
             return _messageEvent(**kwargs)
         else:
-            _event: "EventBase" = EventEnum[_type].value
+            _event = EventEnum[_type].value
             return Event(_event(**kwargs))
```

### Comparing `karas_py-0.2.8/karas/exceptions.py` & `karas_py-0.2.9/karas/exceptions.py`

 * *Files identical despite different names*

### Comparing `karas_py-0.2.8/karas/messages.py` & `karas_py-0.2.9/karas/messages.py`

 * *Files identical despite different names*

### Comparing `karas_py-0.2.8/karas/permission.py` & `karas_py-0.2.9/karas/permission.py`

 * *Files identical despite different names*

### Comparing `karas_py-0.2.8/karas/sender.py` & `karas_py-0.2.9/karas/sender.py`

 * *Files identical despite different names*

### Comparing `karas_py-0.2.8/karas/util/Logger.py` & `karas_py-0.2.9/karas/util/Logger.py`

 * *Files identical despite different names*

### Comparing `karas_py-0.2.8/karas/util/__init__.py` & `karas_py-0.2.9/karas/util/__init__.py`

 * *Files identical despite different names*

### Comparing `karas_py-0.2.8/karas/util/network.py` & `karas_py-0.2.9/karas/util/network.py`

 * *Files identical despite different names*

### Comparing `karas_py-0.2.8/karas/util/sync.py` & `karas_py-0.2.9/karas/util/sync.py`

 * *Files identical despite different names*

### Comparing `karas_py-0.2.8/setup.py` & `karas_py-0.2.9/setup.py`

 * *Files identical despite different names*

