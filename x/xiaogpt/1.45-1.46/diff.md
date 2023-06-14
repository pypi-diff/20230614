# Comparing `tmp/xiaogpt-1.45.tar.gz` & `tmp/xiaogpt-1.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaogpt-1.45.tar", last modified: Tue May 30 12:09:42 2023, max compression
+gzip compressed data, was "xiaogpt-1.46.tar", last modified: Wed Jun 14 02:11:02 2023, max compression
```

## Comparing `xiaogpt-1.45.tar` & `xiaogpt-1.46.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-05-30 12:09:33.756188 xiaogpt-1.45/LICENSE
--rw-r--r--   0        0        0    11390 2023-05-30 12:09:33.756188 xiaogpt-1.45/README.md
--rw-r--r--   0        0        0      919 2023-05-30 12:09:42.272281 xiaogpt-1.45/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-30 12:09:33.756188 xiaogpt-1.45/xiaogpt/__init__.py
--rw-r--r--   0        0        0       61 2023-05-30 12:09:33.756188 xiaogpt-1.45/xiaogpt/__main__.py
--rw-r--r--   0        0        0      639 2023-05-30 12:09:33.756188 xiaogpt-1.45/xiaogpt/bot/__init__.py
--rw-r--r--   0        0        0      554 2023-05-30 12:09:33.756188 xiaogpt-1.45/xiaogpt/bot/base_bot.py
--rw-r--r--   0        0        0     3275 2023-05-30 12:09:33.756188 xiaogpt-1.45/xiaogpt/bot/chatgptapi_bot.py
--rw-r--r--   0        0        0     1605 2023-05-30 12:09:33.756188 xiaogpt-1.45/xiaogpt/bot/gpt3_bot.py
--rw-r--r--   0        0        0     1996 2023-05-30 12:09:33.756188 xiaogpt-1.45/xiaogpt/bot/newbing_bot.py
--rw-r--r--   0        0        0     3415 2023-05-30 12:09:33.756188 xiaogpt-1.45/xiaogpt/cli.py
--rw-r--r--   0        0        0     5263 2023-05-30 12:09:33.756188 xiaogpt-1.45/xiaogpt/config.py
--rw-r--r--   0        0        0     2071 2023-05-30 12:09:33.756188 xiaogpt-1.45/xiaogpt/utils.py
--rw-r--r--   0        0        0    18548 2023-05-30 12:09:33.756188 xiaogpt-1.45/xiaogpt/xiaogpt.py
--rw-r--r--   0        0        0    11976 1970-01-01 00:00:00.000000 xiaogpt-1.45/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-14 02:10:51.461803 xiaogpt-1.46/LICENSE
+-rw-r--r--   0        0        0    11480 2023-06-14 02:10:51.461803 xiaogpt-1.46/README.md
+-rw-r--r--   0        0        0      919 2023-06-14 02:11:02.441948 xiaogpt-1.46/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-14 02:10:51.461803 xiaogpt-1.46/xiaogpt/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-14 02:10:51.461803 xiaogpt-1.46/xiaogpt/__main__.py
+-rw-r--r--   0        0        0      639 2023-06-14 02:10:51.461803 xiaogpt-1.46/xiaogpt/bot/__init__.py
+-rw-r--r--   0        0        0      554 2023-06-14 02:10:51.461803 xiaogpt-1.46/xiaogpt/bot/base_bot.py
+-rw-r--r--   0        0        0     3280 2023-06-14 02:10:51.461803 xiaogpt-1.46/xiaogpt/bot/chatgptapi_bot.py
+-rw-r--r--   0        0        0     1605 2023-06-14 02:10:51.461803 xiaogpt-1.46/xiaogpt/bot/gpt3_bot.py
+-rw-r--r--   0        0        0     1996 2023-06-14 02:10:51.461803 xiaogpt-1.46/xiaogpt/bot/newbing_bot.py
+-rw-r--r--   0        0        0     3415 2023-06-14 02:10:51.461803 xiaogpt-1.46/xiaogpt/cli.py
+-rw-r--r--   0        0        0     5318 2023-06-14 02:10:51.461803 xiaogpt-1.46/xiaogpt/config.py
+-rw-r--r--   0        0        0     2071 2023-06-14 02:10:51.461803 xiaogpt-1.46/xiaogpt/utils.py
+-rw-r--r--   0        0        0    18548 2023-06-14 02:10:51.461803 xiaogpt-1.46/xiaogpt/xiaogpt.py
+-rw-r--r--   0        0        0    12066 1970-01-01 00:00:00.000000 xiaogpt-1.46/PKG-INFO
```

### Comparing `xiaogpt-1.45/LICENSE` & `xiaogpt-1.46/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.45/README.md` & `xiaogpt-1.46/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ## Windows 获取小米音响DID
 
 1. `pip install miservice_fork`
 2. `set MI_USER=xxxx`
 3. `set MI_PASS=xxx`
 4. 得到did
 5. `set MI_DID=xxxx`
-6. 具体可参考 `一键启动.bat` 脚本
+6. 具体可参考 `one_click.bat` 脚本
 - 如果获取did报错时，请更换一下无线网络，有很大概率解决问题。
 
 ## 一点原理
 
 [不用 root 使用小爱同学和 ChatGPT 交互折腾记](https://github.com/yihong0618/gitblog/issues/258)
 
 ## 准备
@@ -153,22 +153,22 @@
 
 [这里]: https://github.com/acheong08/EdgeGPT#getting-authentication-required
 
 ## 注意
 
 1. 请开启小爱同学的蓝牙
 2. 如果要更改提示词和 PROMPT 在代码最上面自行更改
-3. 目前已知 LX04 和 L05B L05C 可能需要使用 `--use_command`
+3. 目前已知 LX04、X10A 和 L05B L05C 可能需要使用 `--use_command`，否则可能会出现终端能输出GPT的回复但小爱同学不回答GPT的情况
 
 ## QA
 
 1. 用破解么？不用
 2. 你做这玩意也没用啊？确实。。。但是挺好玩的，有用对你来说没用，对我们来说不一定呀
 3. 想把它变得更好？PR Issue always welcome.
-4. 还有问题？提 Issuse 哈哈
+4. 还有问题？提 Issue 哈哈
 
 ## 视频教程
 https://www.youtube.com/watch?v=K4YA8YwzOOA
 
 ## Docker
 
 ### 常规用法
```

### Comparing `xiaogpt-1.45/pyproject.toml` & `xiaogpt-1.46/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "openai",
     "aiohttp",
     "rich",
     "edge-tts>=6.1.3",
     "EdgeGPT==0.1.26",
 ]
 dynamic = []
-version = "1.45"
+version = "1.46"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/yihong0618/xiaogpt"
```

### Comparing `xiaogpt-1.45/xiaogpt/bot/__init__.py` & `xiaogpt-1.46/xiaogpt/bot/__init__.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.45/xiaogpt/bot/base_bot.py` & `xiaogpt-1.46/xiaogpt/bot/base_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.45/xiaogpt/bot/chatgptapi_bot.py` & `xiaogpt-1.46/xiaogpt/bot/chatgptapi_bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from rich import print
 
 from xiaogpt.bot.base_bot import BaseBot
 from xiaogpt.utils import split_sentences
 
 
 class ChatGPTBot(BaseBot):
-    default_options = {"model": "gpt-3.5-turbo"}
+    default_options = {"model": "gpt-3.5-turbo-0613"}
 
     def __init__(
         self,
         openai_key: str,
         api_base: str | None = None,
         proxy: str | None = None,
         deployment_id: str | None = None,
```

### Comparing `xiaogpt-1.45/xiaogpt/bot/gpt3_bot.py` & `xiaogpt-1.46/xiaogpt/bot/gpt3_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.45/xiaogpt/bot/newbing_bot.py` & `xiaogpt-1.46/xiaogpt/bot/newbing_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.45/xiaogpt/cli.py` & `xiaogpt-1.46/xiaogpt/cli.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.45/xiaogpt/config.py` & `xiaogpt-1.46/xiaogpt/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "L17A": ("7-3", "7-4"),
     "X08E": ("7-3", "7-4"),
     "LX05A": ("5-1", "5-5"),  # 小爱红外版
     "LX5A": ("5-1", "5-5"),  # 小爱红外版
     "L07A": ("5-1", "5-5"),  # Redmi小爱音箱Play(l7a)
     "L15A": ("7-3", "7-4"),
     "X6A": ("7-3", "7-4"),  # 小米智能家庭屏6
+    "X10A": ("7-3", "7-4"),  # 小米智能家庭屏10
     # add more here
 }
 
 EDGE_TTS_DICT = {
     "用英语": "en-US-AriaNeural",
     "用日语": "ja-JP-NanamiNeural",
     "用法语": "fr-BE-CharlineNeural",
```

### Comparing `xiaogpt-1.45/xiaogpt/utils.py` & `xiaogpt-1.46/xiaogpt/utils.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.45/xiaogpt/xiaogpt.py` & `xiaogpt-1.46/xiaogpt/xiaogpt.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.45/PKG-INFO` & `xiaogpt-1.46/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaogpt
-Version: 1.45
+Version: 1.46
 Summary: Play ChatGPT with xiaomi AI speaker
 Author-Email: yihong0618 <zouzou0208@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/yihong0618/xiaogpt
@@ -40,15 +40,15 @@
 ## Windows 获取小米音响DID
 
 1. `pip install miservice_fork`
 2. `set MI_USER=xxxx`
 3. `set MI_PASS=xxx`
 4. 得到did
 5. `set MI_DID=xxxx`
-6. 具体可参考 `一键启动.bat` 脚本
+6. 具体可参考 `one_click.bat` 脚本
 - 如果获取did报错时，请更换一下无线网络，有很大概率解决问题。
 
 ## 一点原理
 
 [不用 root 使用小爱同学和 ChatGPT 交互折腾记](https://github.com/yihong0618/gitblog/issues/258)
 
 ## 准备
@@ -172,22 +172,22 @@
 
 [这里]: https://github.com/acheong08/EdgeGPT#getting-authentication-required
 
 ## 注意
 
 1. 请开启小爱同学的蓝牙
 2. 如果要更改提示词和 PROMPT 在代码最上面自行更改
-3. 目前已知 LX04 和 L05B L05C 可能需要使用 `--use_command`
+3. 目前已知 LX04、X10A 和 L05B L05C 可能需要使用 `--use_command`，否则可能会出现终端能输出GPT的回复但小爱同学不回答GPT的情况
 
 ## QA
 
 1. 用破解么？不用
 2. 你做这玩意也没用啊？确实。。。但是挺好玩的，有用对你来说没用，对我们来说不一定呀
 3. 想把它变得更好？PR Issue always welcome.
-4. 还有问题？提 Issuse 哈哈
+4. 还有问题？提 Issue 哈哈
 
 ## 视频教程
 https://www.youtube.com/watch?v=K4YA8YwzOOA
 
 ## Docker
 
 ### 常规用法
```

