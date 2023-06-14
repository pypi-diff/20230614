# Comparing `tmp/nonebot-plugin-pcrjjc-0.1.8.tar.gz` & `tmp/nonebot-plugin-pcrjjc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-pcrjjc-0.1.8.tar", last modified: Tue Jun 13 13:38:08 2023, max compression
+gzip compressed data, was "nonebot-plugin-pcrjjc-0.2.0.tar", last modified: Wed Jun 14 13:19:53 2023, max compression
```

## Comparing `nonebot-plugin-pcrjjc-0.1.8.tar` & `nonebot-plugin-pcrjjc-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 13:38:08.573063 nonebot-plugin-pcrjjc-0.1.8/
--rw-rw-rw-   0        0        0    35171 2023-06-10 05:18:04.000000 nonebot-plugin-pcrjjc-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     2699 2023-06-13 13:38:08.571074 nonebot-plugin-pcrjjc-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1835 2023-06-10 08:28:10.000000 nonebot-plugin-pcrjjc-0.1.8/README.md
--rw-rw-rw-   0        0        0     1583 2023-06-13 13:34:28.000000 nonebot-plugin-pcrjjc-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-13 13:38:08.574059 nonebot-plugin-pcrjjc-0.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-13 13:38:08.080239 nonebot-plugin-pcrjjc-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 13:38:08.233734 nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc/
--rw-rw-rw-   0        0        0    39835 2023-06-13 07:52:32.000000 nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc/__init__.py
--rw-rw-rw-   0        0        0     2785 2023-06-08 22:14:57.000000 nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc/aiorequests.py
--rw-rw-rw-   0        0        0     6481 2023-06-09 05:09:18.000000 nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc/bsgamesdk.py
--rw-rw-rw-   0        0        0      840 2023-06-10 23:26:37.000000 nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc/config.py
-drwxrwxrwx   0        0        0        0 2023-06-13 13:38:08.288733 nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc/fonts/
--rw-rw-rw-   0        0        0  8390148 2023-03-11 01:34:30.000000 nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc/fonts/SourceHanSansCN-Medium.otf
--rw-rw-rw-   0        0        0     9200 2023-06-10 08:05:10.000000 nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc/pcrclient.py
--rw-rw-rw-   0        0        0     7909 2023-06-13 13:31:09.000000 nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc/query.py
--rw-rw-rw-   0        0        0      438 2023-06-09 05:01:11.000000 nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc/rsacr.py
--rw-rw-rw-   0        0        0     2357 2023-06-08 23:35:29.000000 nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc/text2img.py
-drwxrwxrwx   0        0        0        0 2023-06-13 13:38:08.282739 nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc.egg-info/
--rw-rw-rw-   0        0        0     2699 2023-06-13 13:38:08.000000 nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      636 2023-06-13 13:38:08.000000 nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 13:38:08.000000 nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      187 2023-06-13 13:38:08.000000 nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-13 13:38:08.000000 nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 13:19:52.938463 nonebot-plugin-pcrjjc-0.2.0/
+-rw-rw-rw-   0        0        0    35171 2023-06-10 05:18:04.000000 nonebot-plugin-pcrjjc-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2702 2023-06-14 13:19:52.937615 nonebot-plugin-pcrjjc-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1838 2023-06-14 13:19:25.000000 nonebot-plugin-pcrjjc-0.2.0/README.md
+-rw-rw-rw-   0        0        0     1583 2023-06-14 10:44:30.000000 nonebot-plugin-pcrjjc-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 13:19:52.938463 nonebot-plugin-pcrjjc-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-14 13:19:52.882614 nonebot-plugin-pcrjjc-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-14 13:19:52.908614 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/
+-rw-rw-rw-   0        0        0    39835 2023-06-13 07:52:32.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/__init__.py
+-rw-rw-rw-   0        0        0     2785 2023-06-08 22:14:57.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/aiorequests.py
+-rw-rw-rw-   0        0        0     6022 2023-06-14 11:47:54.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/bsgamesdk.py
+-rw-rw-rw-   0        0        0      856 2023-06-14 10:44:45.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/config.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:19:52.924438 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/fonts/
+-rw-rw-rw-   0        0        0  8390148 2023-03-11 01:34:30.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/fonts/SourceHanSansCN-Medium.otf
+-rw-rw-rw-   0        0        0     9200 2023-06-10 08:05:10.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/pcrclient.py
+-rw-rw-rw-   0        0        0     8186 2023-06-14 11:47:48.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/query.py
+-rw-rw-rw-   0        0        0      438 2023-06-09 05:01:11.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/rsacr.py
+-rw-rw-rw-   0        0        0     2357 2023-06-08 23:35:29.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/text2img.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:19:52.921217 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc.egg-info/
+-rw-rw-rw-   0        0        0     2702 2023-06-14 13:19:52.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2023-06-14 13:19:52.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 13:19:52.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      187 2023-06-14 13:19:52.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-14 13:19:52.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc.egg-info/top_level.txt
```

### Comparing `nonebot-plugin-pcrjjc-0.1.8/LICENSE` & `nonebot-plugin-pcrjjc-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.8/PKG-INFO` & `nonebot-plugin-pcrjjc-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pcrjjc
-Version: 0.1.8
+Version: 0.2.0
 Summary: pcrjjc排名监测插件
 Author-email: reine-ishyanami <2402979195@qq.com>
 License: AGPL-3
 Project-URL: Homepage, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc
 Project-URL: Bug Tracker, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc/issues
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -51,18 +51,18 @@
 
 
 
 ### 配置项
 
 **在nonebot2项目中的`.env`开头的文件添加下表配置项，其中非必填项可不填**
 
-|     配置项     |   类型    | 是否必填 | 默认值  |              说明              |
-| :------------: | :-------: | :------: | :-----: | :----------------------------: |
+|     配置项     |   类型    | 是否必填 |   默认值   |              说明              |
+| :------------: | :-------: | :------: |:-------:| :----------------------------: |
 |   SUPERUSERS   | list[str] |   True   |         | 超级用户QQ号，示例：["114514"] |
-|      OTTO      |   bool    |  False   |  False  | 是否自动过验证码（不建议修改） |
+|      OTTO      |   bool    |  False   |  True   | 是否自动过验证码（不建议修改） |
 |    VERSION     |    str    |  False   | "6.2.0" |          客户端版本号          |
 |    MAX_PRI     |    int    |  False   |    0    |          最大私聊人数          |
 |   MAX_PCRID    |    int    |  False   |    8    |       每人绑定的最大数量       |
 |  MAX_HISTORY   |    int    |  False   |   50    |        单人最多历史记录        |
 | NOTICE_CD_MIN  |    int    |  False   |   10    |  上线提醒时间间隔（单位：分）  |
 | REFRESH_SECOND |    int    |  False   |    3    |    排名刷新频率（单位：秒）    |
```

### Comparing `nonebot-plugin-pcrjjc-0.1.8/README.md` & `nonebot-plugin-pcrjjc-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -32,18 +32,18 @@
 
 
 
 ### 配置项
 
 **在nonebot2项目中的`.env`开头的文件添加下表配置项，其中非必填项可不填**
 
-|     配置项     |   类型    | 是否必填 | 默认值  |              说明              |
-| :------------: | :-------: | :------: | :-----: | :----------------------------: |
+|     配置项     |   类型    | 是否必填 |   默认值   |              说明              |
+| :------------: | :-------: | :------: |:-------:| :----------------------------: |
 |   SUPERUSERS   | list[str] |   True   |         | 超级用户QQ号，示例：["114514"] |
-|      OTTO      |   bool    |  False   |  False  | 是否自动过验证码（不建议修改） |
+|      OTTO      |   bool    |  False   |  True   | 是否自动过验证码（不建议修改） |
 |    VERSION     |    str    |  False   | "6.2.0" |          客户端版本号          |
 |    MAX_PRI     |    int    |  False   |    0    |          最大私聊人数          |
 |   MAX_PCRID    |    int    |  False   |    8    |       每人绑定的最大数量       |
 |  MAX_HISTORY   |    int    |  False   |   50    |        单人最多历史记录        |
 | NOTICE_CD_MIN  |    int    |  False   |   10    |  上线提醒时间间隔（单位：分）  |
 | REFRESH_SECOND |    int    |  False   |    3    |    排名刷新频率（单位：秒）    |
```

### Comparing `nonebot-plugin-pcrjjc-0.1.8/pyproject.toml` & `nonebot-plugin-pcrjjc-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-pcrjjc"
-version = "0.1.8"
+version = "0.2.0"
 authors = [
     {name="reine-ishyanami", email="2402979195@qq.com"}
 ]
 description = "pcrjjc排名监测插件"
 readme = "README.md"
 license = { text = "AGPL-3" }
 requires-python = ">=3.10, <4.0"
```

### Comparing `nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc/__init__.py` & `nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc/aiorequests.py` & `nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/aiorequests.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc/bsgamesdk.py` & `nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/bsgamesdk.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,30 +82,15 @@
     data = set_sign(data)
     return await send_post(bili_login + "api/client/start_captcha", data)
 
 
 async def login(bili_account, bili_pwd, captcha_verifier):
     logger.info('logging in with acc = {}, pwd = {}', bili_account, bili_pwd)
     login_sta = await login1(bili_account, bili_pwd)
-    if "access_key" in login_sta:
-        return login_sta
-
-    otto = False
-    try:
-        otto = await captcha_verifier()
-    except:  # 兼容原版手动过码
-        pass
-    if otto:
-        cap = await captcha_verifier(True, True)
-        if cap == "manual":
-            otto = False
-        else:
-            login_sta = await login2(bili_account, bili_pwd, cap["challenge"], cap['gt_user_id'], cap['validate'])
-            if "access_key" in login_sta:
-                await captcha_verifier(0)
-            return login_sta
+    # if "access_key" in login_sta:
+    #     return login_sta
 
-    if not otto:
+    if login_sta['code'] == 200_000:
         cap = await captcha()
-        captcha_done = await captcha_verifier(cap['gt'], cap['challenge'], cap['gt_user_id'])
-        login_sta = await login2(bili_account, bili_pwd, cap["challenge"], cap['gt_user_id'], captcha_done)
+        challenge, gt_user_id, captcha_done = await captcha_verifier(cap['gt'], cap['challenge'], cap['gt_user_id'])
+        login_sta = await login2(bili_account, bili_pwd, challenge, gt_user_id, captcha_done)
         return login_sta
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc/fonts/SourceHanSansCN-Medium.otf` & `nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/fonts/SourceHanSansCN-Medium.otf`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc/pcrclient.py` & `nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/pcrclient.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc/query.py` & `nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -120,82 +120,77 @@
         await bot.send_private_msg(user_id=admin, message=f'thread{ordd}: Changed to auto')
     try:
         captcha_lck.release()
     except:
         pass
 
 
-async def captcha_verifier(*args):
-    global otto
-    if len(args) == 0:
-        return otto
-    global captcha_cnt
-    if len(args) == 1 and type(args[0]) == int:
-        captcha_cnt = args[0]
-        return captcha_cnt
-
-    global ac_first, validating
-    global validate, captcha_lck
+async def captcha_verifier(gt: str, challenge: str, userid: str):
+    global otto, captcha_cnt, ac_first, validating, validate, captcha_lck
+    # global otto, ac_first, validating, validate, captcha_lck
     if not ac_first:
         await captcha_lck.acquire()
         ac_first = True
 
     validating = True
+
+    # 非自动过码
     if not otto:
-        gt = args[0]
-        challenge = args[1]
-        userid = args[2]
         online_url_head = f"https://help.tencentbot.top/geetest_/?"
         url = f"captcha_type=1&challenge={challenge}&gt={gt}&userid={userid}&gs=1"
         await bot.send_private_msg(
             user_id=admin,
             message=f'pcr账号登录需要验证码，请完成以下链接中的验证内容后将第1个方框的内容点击复制，并加上"validate{ordd} "前缀发送给机器人完成验证'
                     f'\n示例：validate{ordd} 123456789\n您也可以发送 validate{ordd} auto 命令bot自动过验证码'
                     f'\n验证链接头：{online_url_head}'
                     f'\n链接：{url}'
                     f'\n为避免tx网页安全验证使验证码过期，请手动拼接链接头和链接'
         )
         await captcha_lck.acquire()
         validating = False
-        return validate
+        return challenge, gt, validate
 
     while captcha_cnt < 5:
         captcha_cnt += 1
         try:
             logger.info('测试新版自动过码中，当前尝试第{}次。', captcha_cnt)
-
-            await asyncio.sleep(1)
-            uuid = loads(await (await get(url="https://pcrd.tencentbot.top/geetest")).content)["uuid"]
-            logger.info('uuid={}', uuid)
+            url = f"https://pcrd.tencentbot.top/geetest_renew?captcha_type=1&challenge={challenge}&gt={gt}&userid={userid}&gs=1"
+            header = {"Content-Type": "application/json", "User-Agent": "pcrjjc/0.2.0"}
+            res = await (await get(url=url, headers=header)).content
+            res = loads(res)
+            uuid = res["uuid"]
+            msg = [f"uuid={uuid}"]
 
             ccnt = 0
-            while ccnt < 3:
+            while ccnt < 10:
                 ccnt += 1
                 await asyncio.sleep(5)
-                res = await (await get(url=f"https://pcrd.tencentbot.top/check/{uuid}")).content
+                res = await (await get(url=f"https://pcrd.tencentbot.top/check/{uuid}", headers=header)).content
                 res = loads(res)
                 if "queue_num" in res:
                     nu = res["queue_num"]
-                    logger.info("queue_num={}", nu)
-                    tim = min(int(nu), 3) * 5
-                    logger.info("sleep={}", tim)
-                    await asyncio.sleep(tim)
+                    msg.append(f"queue_num={nu}")
+                    tim = min(int(nu), 3) * 10
+                    msg.append(f"sleep={tim}")
+                    logger.info("pcrjjc2:{}", msg)
+                    msg = []
                 else:
                     info = res["info"]
                     if info in ["fail", "url invalid"]:
                         break
                     elif info == "in running":
                         await asyncio.sleep(5)
-                    else:
+                    elif 'validate' in info:
                         logger.info('info={}', info)
                         validating = False
-                        return info
+                        return info["challenge"], info["gt_user_id"], info["validate"]
+                if ccnt > 10:
+                    raise Exception("Captcha Failed")
         except:
             pass
-
     if captcha_cnt >= 5:
         otto = False
         await bot.send_private_msg(user_id=admin,
                                    message=f'thread{ordd}: 自动过码多次尝试失败，可能为服务器错误，自动切换为手动。\n确实服务器无误后，可发送 validate{ordd} auto重新触发自动过码。')
         await bot.send_private_msg(user_id=admin, message=f'thread{ordd}: Changed to manual')
         validating = False
         return "manual"
```

### Comparing `nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc/text2img.py` & `nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/text2img.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO` & `nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pcrjjc
-Version: 0.1.8
+Version: 0.2.0
 Summary: pcrjjc排名监测插件
 Author-email: reine-ishyanami <2402979195@qq.com>
 License: AGPL-3
 Project-URL: Homepage, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc
 Project-URL: Bug Tracker, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc/issues
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -51,18 +51,18 @@
 
 
 
 ### 配置项
 
 **在nonebot2项目中的`.env`开头的文件添加下表配置项，其中非必填项可不填**
 
-|     配置项     |   类型    | 是否必填 | 默认值  |              说明              |
-| :------------: | :-------: | :------: | :-----: | :----------------------------: |
+|     配置项     |   类型    | 是否必填 |   默认值   |              说明              |
+| :------------: | :-------: | :------: |:-------:| :----------------------------: |
 |   SUPERUSERS   | list[str] |   True   |         | 超级用户QQ号，示例：["114514"] |
-|      OTTO      |   bool    |  False   |  False  | 是否自动过验证码（不建议修改） |
+|      OTTO      |   bool    |  False   |  True   | 是否自动过验证码（不建议修改） |
 |    VERSION     |    str    |  False   | "6.2.0" |          客户端版本号          |
 |    MAX_PRI     |    int    |  False   |    0    |          最大私聊人数          |
 |   MAX_PCRID    |    int    |  False   |    8    |       每人绑定的最大数量       |
 |  MAX_HISTORY   |    int    |  False   |   50    |        单人最多历史记录        |
 | NOTICE_CD_MIN  |    int    |  False   |   10    |  上线提醒时间间隔（单位：分）  |
 | REFRESH_SECOND |    int    |  False   |    3    |    排名刷新频率（单位：秒）    |
```

### Comparing `nonebot-plugin-pcrjjc-0.1.8/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt` & `nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

