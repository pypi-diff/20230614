# Comparing `tmp/nonebot_plugin_game_collection-2.1.8.tar.gz` & `tmp/nonebot_plugin_game_collection-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_game_collection-2.1.8.tar", last modified: Tue Jun  6 06:37:35 2023, max compression
+gzip compressed data, was "nonebot_plugin_game_collection-2.1.9.tar", last modified: Tue Jun  6 13:30:49 2023, max compression
```

## Comparing `nonebot_plugin_game_collection-2.1.8.tar` & `nonebot_plugin_game_collection-2.1.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 06:37:35.700514 nonebot_plugin_game_collection-2.1.8/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.1.8/LICENSE
--rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0      376 2023-06-06 06:37:35.700014 nonebot_plugin_game_collection-2.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 06:37:35.638736 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/
--rw-rw-rw-   0        0        0    17451 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/Account.py
--rw-rw-rw-   0        0        0    50095 2023-06-06 06:35:38.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/Game.py
-drwxrwxrwx   0        0        0        0 2023-06-06 06:37:35.656477 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/HorseRace/
--rw-rw-rw-   0        0        0    15602 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/HorseRace/events_main.py
--rw-rw-rw-   0        0        0     6399 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/HorseRace/horse.py
--rw-rw-rw-   0        0        0     5151 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/HorseRace/race_group.py
--rw-rw-rw-   0        0        0     9187 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/HorseRace/start.py
--rw-rw-rw-   0        0        0    11410 2023-06-04 13:24:05.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/Manager.py
--rw-rw-rw-   0        0        0    20170 2023-06-04 13:24:04.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/Market.py
--rw-rw-rw-   0        0        0    16156 2023-06-05 10:03:35.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/Prop.py
--rw-rw-rw-   0        0        0    30875 2023-06-05 12:54:00.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/__init__.py
--rw-rw-rw-   0        0        0     3249 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/config.py
-drwxrwxrwx   0        0        0        0 2023-06-06 06:37:35.663483 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/data/
--rw-rw-rw-   0        0        0      525 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/data/api.py
--rw-rw-rw-   0        0        0     5589 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/data/data.py
--rw-rw-rw-   0        0        0      102 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/data/run.py
-drwxrwxrwx   0        0        0        0 2023-06-06 06:37:35.668987 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/
--rw-rw-rw-   0        0        0      171 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/element_library.json
-drwxrwxrwx   0        0        0        0 2023-06-06 06:37:35.690007 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/
--rw-rw-rw-   0        0        0     5488 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/Stand.json
--rw-rw-rw-   0        0        0     4549 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
--rw-rw-rw-   0        0        0     1757 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
--rw-rw-rw-   0        0        0      906 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/基础事件.json
--rw-rw-rw-   0        0        0     2717 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
--rw-rw-rw-   0        0        0     1257 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
--rw-rw-rw-   0        0        0    22637 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/群友日常.json
--rw-rw-rw-   0        0        0     4751 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
--rw-rw-rw-   0        0        0     1010 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
--rw-rw-rw-   0        0        0     2253 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
--rw-rw-rw-   0        0        0    12958 2023-06-04 12:00:23.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/menu_data.json
--rw-rw-rw-   0        0        0     5375 2023-06-04 11:46:30.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/props_library.json
-drwxrwxrwx   0        0        0        0 2023-06-06 06:37:35.693008 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/subprocess/
--rw-rw-rw-   0        0        0     2245 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
-drwxrwxrwx   0        0        0        0 2023-06-06 06:37:35.698012 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/utils/
--rw-rw-rw-   0        0        0     1321 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/utils/avatar.py
--rw-rw-rw-   0        0        0     7133 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/utils/chart.py
--rw-rw-rw-   0        0        0     1619 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-06 06:37:35.647969 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection.egg-info/
--rw-rw-rw-   0        0        0      376 2023-06-06 06:37:35.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2038 2023-06-06 06:37:35.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 06:37:35.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-06-06 06:37:35.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-06-06 06:37:35.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 06:37:35.701014 nonebot_plugin_game_collection-2.1.8/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-06-06 06:37:31.000000 nonebot_plugin_game_collection-2.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 13:30:49.837005 nonebot_plugin_game_collection-2.1.9/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.1.9/LICENSE
+-rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      376 2023-06-06 13:30:49.836505 nonebot_plugin_game_collection-2.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 13:30:49.770448 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/
+-rw-rw-rw-   0        0        0    17451 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/Account.py
+-rw-rw-rw-   0        0        0    50156 2023-06-06 13:16:15.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/Game.py
+drwxrwxrwx   0        0        0        0 2023-06-06 13:30:49.788963 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/HorseRace/
+-rw-rw-rw-   0        0        0    15602 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/HorseRace/events_main.py
+-rw-rw-rw-   0        0        0     6399 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/HorseRace/horse.py
+-rw-rw-rw-   0        0        0     5151 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/HorseRace/race_group.py
+-rw-rw-rw-   0        0        0     9187 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/HorseRace/start.py
+-rw-rw-rw-   0        0        0    11410 2023-06-04 13:24:05.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/Manager.py
+-rw-rw-rw-   0        0        0    20170 2023-06-04 13:24:04.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/Market.py
+-rw-rw-rw-   0        0        0    16157 2023-06-06 13:24:53.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/Prop.py
+-rw-rw-rw-   0        0        0    30876 2023-06-06 12:22:52.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/__init__.py
+-rw-rw-rw-   0        0        0     3249 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/config.py
+drwxrwxrwx   0        0        0        0 2023-06-06 13:30:49.795970 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/data/
+-rw-rw-rw-   0        0        0      525 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/data/api.py
+-rw-rw-rw-   0        0        0     5589 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/data/data.py
+-rw-rw-rw-   0        0        0      102 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/data/run.py
+drwxrwxrwx   0        0        0        0 2023-06-06 13:30:49.801474 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/
+-rw-rw-rw-   0        0        0      171 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/element_library.json
+drwxrwxrwx   0        0        0        0 2023-06-06 13:30:49.824995 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/
+-rw-rw-rw-   0        0        0     5488 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/Stand.json
+-rw-rw-rw-   0        0        0     4549 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
+-rw-rw-rw-   0        0        0     1757 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
+-rw-rw-rw-   0        0        0      906 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/基础事件.json
+-rw-rw-rw-   0        0        0     2717 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
+-rw-rw-rw-   0        0        0     1257 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
+-rw-rw-rw-   0        0        0    22637 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/群友日常.json
+-rw-rw-rw-   0        0        0     4751 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
+-rw-rw-rw-   0        0        0     1010 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
+-rw-rw-rw-   0        0        0     2253 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
+-rw-rw-rw-   0        0        0    12958 2023-06-04 12:00:23.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/menu_data.json
+-rw-rw-rw-   0        0        0     5357 2023-06-06 13:25:50.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/props_library.json
+drwxrwxrwx   0        0        0        0 2023-06-06 13:30:49.826996 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/subprocess/
+-rw-rw-rw-   0        0        0     2245 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
+drwxrwxrwx   0        0        0        0 2023-06-06 13:30:49.834503 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/utils/
+-rw-rw-rw-   0        0        0     1321 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/utils/avatar.py
+-rw-rw-rw-   0        0        0     7133 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/utils/chart.py
+-rw-rw-rw-   0        0        0     1619 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-06 13:30:49.780456 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-06-06 13:30:49.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2038 2023-06-06 13:30:49.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 13:30:49.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-06-06 13:30:49.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-06-06 13:30:49.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 13:30:49.837505 nonebot_plugin_game_collection-2.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-06-06 13:27:00.000000 nonebot_plugin_game_collection-2.1.9/setup.py
```

### Comparing `nonebot_plugin_game_collection-2.1.8/LICENSE` & `nonebot_plugin_game_collection-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/README.md` & `nonebot_plugin_game_collection-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/Account.py` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/Account.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/Game.py` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/Game.py`

 * *Files 2% similar despite different names*

```diff
@@ -373,16 +373,17 @@
 
 current_games:Dict[int,Session] = {}
 
 def accept(event:GroupMessageEvent):
     """
     接受挑战
     """
+    group_id = event.group_id
     global current_games
-    session = current_games[event.group_id]
+    session = current_games[group_id]
     if msg := session.try_join_game(event):
         return None if msg == " " else msg
     group_account = Manager.locate_user(event)[1]
     if session.info["game"] == "random":
         session.gold = random.randint(0, 0 if(mingold := min(group_account.gold,session.info["gold"])) < 0 else mingold) if session.gold == -1 else session.gold
         game = random.choice(["russian","dice","poker","lucky_number","cantrell"])
         if game == "russian":
@@ -392,16 +393,22 @@
         elif game == "poker":
             session.info = poker_info()
         elif game == "lucky_number":
             session.info = lucky_number_info(session.gold)
         elif game == "cantrell":
             session.info = cantrell_info(session.gold)
     elif group_account.gold <  session.gold:
-        del current_games[event.group_id]
+        del current_games[group_id]
         return Message(MessageSegment.at(event.user_id) + f"你的金币不足以接受这场对决！\n——你还有{group_account.gold}枚金币。")
+
+    bet_limit = min(
+        user_data[session.player1_id].group_accounts[group_id].gold,
+        user_data[session.player2_id].group_accounts[group_id].gold)
+    bet_limit = bet_limit if bet_limit > 0 else 0
+    session.info["bet_limit"] = bet_limit
     session.next = session.player1_id
     return acceptmessage(session)
 
 def acceptmessage(session:Session):
     """
     生成接受挑战的提示信息
     """
@@ -1000,18 +1007,15 @@
     猜数字
     """
     group_id = event.group_id
     global current_games
     session = current_games[group_id]
     if msg := session.shot_check(event):
         return None if msg == " " else msg
-    session.info.setdefault("max",(maxgold if (maxgold := min(
-        user_data[session.player1_id].group_accounts[group_id].gold,
-        user_data[session.player2_id].group_accounts[group_id].gold)) > 0 else 0 ))
-    session.gold = min(session.info["gold"] * session.round, session.info["max"])
+    session.gold = min(session.info["gold"] * session.round, session.info["bet_limit"])
     session.nextround()
     TrueN = session.info["number"]
     if N > TrueN:
         return f"{N}比这个数字大\n金额：{session.gold}"
     if N < TrueN:
         return f"{N}比这个数字小\n金额：{session.gold}"
     session.win = event.user_id
@@ -1155,15 +1159,16 @@
 def cantrell(event:GroupMessageEvent, gold:int ,times:int = 1):
     """
     发起游戏：港式五张
     """
     flag, msg = start(event, gold, max_bet_gold * 10)
     if flag == False:
         return msg
-    session = current_games[event.group_id]
+    group_id = event.group_id
+    session = current_games[group_id]
     session.gold = gold
     if times == 1:
         session.info = cantrell_info(gold)
     else:
         session.info = happy_cantrell_info(gold,times)
     return (f"随机牌堆已生成\n"
             f"开局金额：{gold}\n"
@@ -1198,20 +1203,28 @@
     加注
     """
     group_id = event.group_id
     global current_games
     session = current_games[group_id]
     if msg := session.shot_check(event):
         return None if msg == " " else msg
+    if gold > max_bet_gold:
+        return MessageSegment.at(event.user_id) + f"加注金额不能超过{max_bet_gold}"
+    if gold > session.info["bet_limit"]:
+        gold = session.info["bet_limit"]
     expose = session.round / 2
     if expose == int(expose):
         session.nextround()
         session.time += 120
         expose = int(expose) + 3
-        session.gold += session.info["round_gold"]
+        if gold > session.info["round_gold"]:
+            session.gold += gold
+        else:
+            session.gold += session.info["round_gold"]
+        session.info["bet_limit"] -= gold
         msg = (
             f'玩家：{user_data[session.player1_id].group_accounts[group_id].nickname}\n'
             "手牌：\n"
             "|"
             + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in session.info["hand1"][0:expose]]) + (5 - expose)*"   |"
             "\n——————————————\n"
             f'玩家：{user_data[session.player2_id].group_accounts[group_id].nickname}\n'
@@ -1222,21 +1235,17 @@
         if expose == 5:
             if session.info["pt1"][0] > session.info["pt2"][0]:
                 session.win = session.player1_id
             else:
                 session.win = session.player2_id
             await end(bot, event)
         else:
-            return MessageSegment.image(text_to_png(f"您已跟注{session.info['round_gold']}金币\n" + msg,30))
+            return MessageSegment.image(text_to_png(f"您已跟注{gold}金币\n" + msg,30))
     else:
-        if gold > max_bet_gold:
-            return MessageSegment.at(event.user_id) + f"加注金额不能超过{max_bet_gold}"
-        group_account = Manager.locate_user(event)[1]
-        if gold + session.gold > group_account.gold:
-            return Message(MessageSegment.at(event.user_id) + f"你没有足够的金币。\n——你还有{group_account.gold - session.gold}枚金币。")
+        session.info["bet_limit"] -= gold
         session.nextround()
         session.time += 120
         session.info["round_gold"] = gold
         return MessageSegment.at(event.user_id) + f"您已加注{gold}金币"
 
 """+++++++++++++++++
 ——————————
```

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/HorseRace/events_main.py` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/HorseRace/events_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/HorseRace/horse.py` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/HorseRace/horse.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/HorseRace/race_group.py` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/HorseRace/race_group.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/HorseRace/start.py` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/HorseRace/start.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/Manager.py` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/Manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/Market.py` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/Market.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/Prop.py` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/Prop.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,15 +394,15 @@
 
         props["63101"] -= 1
         if props["63101"] < 1:
             del props["63101"]
 
         gold = group_account.gold
 
-        if random.randint(0,2) > 0:
+        if random.randint(0,2) == 0:
             user.gold += gold
             group_account.gold += gold
             return f"你获得了{gold}金币"
         else:
             user.gold -= gold
             group_account.gold -= gold
             user.props.setdefault("53101",0)
```

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/__init__.py` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -383,15 +383,15 @@
         gold = bet_gold
         times = 1
     else:
         test = len(arg)
         if test == 1:
             gold = arg[0]
             if gold.isdigit():
-                gold = int(arg)
+                gold = int(gold)
             else:
                 gold = bet_gold
             times = 1
         else:
             gold = arg[0]
             if gold.isdigit():
                 gold = int(gold)
```

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/config.py` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/data/api.py` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/data/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/data/data.py` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/data/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/Stand.json` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/Stand.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/基础事件.json` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/基础事件.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/群友日常.json` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/群友日常.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/menu_data.json` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/menu_data.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/props_library.json` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/props_library.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9958333333333332%*

 * *Differences: {"'63101'": "{'intro': '有33.3%的概率获得金币，66.6%的概率失去金币。没有上限', 'des': '奖励翻倍，惩罚翻倍。'}"}*

```diff
@@ -151,16 +151,16 @@
         "des": "\u201c\u94bb\u77f3\u6709\u4ec0\u4e48\u7528\uff1f\u201d\n\u201c\u6ca1\u7528\u3002\u201d",
         "intro": "\u65e0\u6bd4\u73cd\u8d35\u7684\u94bb\u77f3\uff0c\u53ea\u6709\u5343\u5206\u4e4b\u4e94\u7684\u6982\u7387\u83b7\u5f97\uff0c\u4ee5\u540e\u53ef\u80fd\u6709\u7528\u3002",
         "name": "\u94bb\u77f3",
         "rare": 6
     },
     "63101": {
         "color": "#FF3300",
-        "des": "\u6210\u529f\u7387\u7ffb\u500d\uff0c\u5956\u52b1\u7ffb\u500d\uff0c\u60e9\u7f5a\u7ffb\u500d\u3002",
-        "intro": "\u670966.6%\u7684\u6982\u7387\u83b7\u5f97\u91d1\u5e01\uff0c33.3%\u7684\u6982\u7387\u5931\u53bb\u91d1\u5e01\u3002\u6ca1\u6709\u4e0a\u9650",
+        "des": "\u5956\u52b1\u7ffb\u500d\uff0c\u60e9\u7f5a\u7ffb\u500d\u3002",
+        "intro": "\u670933.3%\u7684\u6982\u7387\u83b7\u5f97\u91d1\u5e01\uff0c66.6%\u7684\u6982\u7387\u5931\u53bb\u91d1\u5e01\u3002\u6ca1\u6709\u4e0a\u9650",
         "name": "\u8d85\u7ea7\u5e78\u8fd0\u786c\u5e01",
         "rare": 6
     },
     "63102": {
         "color": "#006633",
         "des": "\u4e8b\u4e86\u62c2\u8863\u53bb\uff0c\u6df1\u85cf\u8eab\u4e0e\u540d\u3002",
         "intro": "\u6e05\u7a7a\u81ea\u5df1\u7684\u91d1\u5e01\uff0c\u80a1\u7968",
```

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/subprocess/ohlc.py` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/subprocess/ohlc.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/utils/avatar.py` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/utils/chart.py` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/utils/chart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/utils/utils.py` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection.egg-info/SOURCES.txt` & `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.8/setup.py` & `nonebot_plugin_game_collection-2.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_game_collection',
-version='2.1.8',
+version='2.1.9',
 description='改自nonebot_plugin_russian合并了nonebot_plugin_horserace还有一些自编玩法的小游戏合集。',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_game_collection","nonebot_plugin_game_collection.*"]),
```

