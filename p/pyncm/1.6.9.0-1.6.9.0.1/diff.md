# Comparing `tmp/pyncm-1.6.9.0.tar.gz` & `tmp/pyncm-1.6.9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyncm-1.6.9.0.tar", last modified: Sat Jun 10 00:56:23 2023, max compression
+gzip compressed data, was "pyncm-1.6.9.0.1.tar", last modified: Wed Jun 14 05:25:35 2023, max compression
```

## Comparing `pyncm-1.6.9.0.tar` & `pyncm-1.6.9.0.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:56:23.954317 pyncm-1.6.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-10 00:56:23.954317 pyncm-1.6.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:56:23.950317 pyncm-1.6.9.0/demos/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/demos/二维码登录.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/demos/云盘上传.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/demos/手机登录.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/demos/获取单曲下载链接.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/demos/足迹伪装.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:56:23.950317 pyncm-1.6.9.0/pyncm/
--rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27061 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:56:23.954317 pyncm-1.6.9.0/pyncm/apis/
--rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/album.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/artist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/cloudsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/login.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:56:23.954317 pyncm-1.6.9.0/pyncm/apis/miniprograms/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/miniprograms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/miniprograms/difm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/miniprograms/radio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/miniprograms/sportsfm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/miniprograms/zonefm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/playlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/track.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:56:23.954317 pyncm-1.6.9.0/pyncm/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/utils/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/utils/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/utils/lrcparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/utils/security.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:56:23.954317 pyncm-1.6.9.0/pyncm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-10 00:56:23.000000 pyncm-1.6.9.0/pyncm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-10 00:56:23.000000 pyncm-1.6.9.0/pyncm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 00:56:23.000000 pyncm-1.6.9.0/pyncm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-10 00:56:23.000000 pyncm-1.6.9.0/pyncm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 00:56:23.000000 pyncm-1.6.9.0/pyncm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-10 00:56:23.000000 pyncm-1.6.9.0/pyncm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 00:56:23.954317 pyncm-1.6.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:25:35.541209 pyncm-1.6.9.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-06-14 05:25:35.537208 pyncm-1.6.9.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:25:35.533208 pyncm-1.6.9.0.1/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/demos/二维码登录.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/demos/云盘上传.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/demos/手机登录.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/demos/获取单曲下载链接.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/demos/足迹伪装.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:25:35.537208 pyncm-1.6.9.0.1/pyncm/
+-rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28468 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:25:35.537208 pyncm-1.6.9.0.1/pyncm/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/album.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/artist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/cloudsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/login.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:25:35.537208 pyncm-1.6.9.0.1/pyncm/apis/miniprograms/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/miniprograms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/miniprograms/difm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/miniprograms/radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/miniprograms/sportsfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/miniprograms/zonefm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:25:35.537208 pyncm-1.6.9.0.1/pyncm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/utils/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/utils/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/utils/lrcparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/utils/security.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:25:35.537208 pyncm-1.6.9.0.1/pyncm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-06-14 05:25:35.000000 pyncm-1.6.9.0.1/pyncm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-14 05:25:35.000000 pyncm-1.6.9.0.1/pyncm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 05:25:35.000000 pyncm-1.6.9.0.1/pyncm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-14 05:25:35.000000 pyncm-1.6.9.0.1/pyncm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 05:25:35.000000 pyncm-1.6.9.0.1/pyncm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 05:25:35.000000 pyncm-1.6.9.0.1/pyncm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 05:25:35.541209 pyncm-1.6.9.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/setup.py
```

### Comparing `pyncm-1.6.9.0/LICENSE` & `pyncm-1.6.9.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/PKG-INFO` & `pyncm-1.6.9.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyncm
-Version: 1.6.9.0
+Version: 1.6.9.0.1
 Summary: NeteaseCloudMusic APIs for Python 3.x 适用于 Python 3 的网易云音乐 API
 Home-page: https://github.com/greats3an/pyncm
 Author: greats3an
 Author-email: greats3an@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyncm-1.6.9.0/README.md` & `pyncm-1.6.9.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/demos/__init__.py` & `pyncm-1.6.9.0.1/demos/__init__.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/demos/二维码登录.py` & `pyncm-1.6.9.0.1/demos/二维码登录.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/demos/云盘上传.py` & `pyncm-1.6.9.0.1/demos/云盘上传.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/demos/手机登录.py` & `pyncm-1.6.9.0.1/demos/手机登录.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/demos/足迹伪装.py` & `pyncm-1.6.9.0.1/demos/足迹伪装.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/pyncm/__init__.py` & `pyncm-1.6.9.0.1/pyncm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     >>> pyncm.SetNewSession(
             pyncm.LoadSessionFromString(save)
         )
 
 # 注意事项
     - (PR#11) 海外用户可能经历 460 "Cheating" 问题，可通过添加以下 Header 解决: `X-Real-IP = 118.88.88.88`    
 """
-__version__ = "1.6.9.0"
+__version__ = "1.6.9.0.1"
 
 from threading import current_thread
 from typing import Text, Union
 from time import time
 from .utils.crypto import EapiEncrypt, EapiDecrypt, HexCompose
 import requests, logging, json, os
 logger = logging.getLogger("pyncm.api")
```

### Comparing `pyncm-1.6.9.0/pyncm/__main__.py` & `pyncm-1.6.9.0.1/pyncm/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -178,15 +178,30 @@
                 self.finished_tasks += 1
                 return
             if type(task) == TrackDownloadTask:
                 try:
                     # Downloding source audio
                     dAudio = track.GetTrackAudioV1(task.audio.id, level=task.audio.level)
                     dAudio = dAudio.get("data", [{"url": ""}])[0]  # Dummy fallback value                
-                    assert dAudio["url"], "%s 无法下载，资源不存在" % task.song.Title                
+                    if not dAudio['url']:
+                        # Attempt to give some sort of explaination
+                        # 来自 https://neteasecloudmusicapi-docs.4everland.app/#/?id=%e8%8e%b7%e5%8f%96%e6%ad%8c%e6%9b%b2%e8%af%a6%e6%83%85
+                        ''' fee : enum                       
+                        0: 免费或无版权
+                        1: VIP 歌曲
+                        4: 购买专辑
+                        8: 非会员可免费播放低音质，会员可播放高音质及下载
+                        fee 为 1 或 8 的歌曲均可单独购买 2 元单曲
+                        '''
+                        fee = dAudio['fee']
+                        assert fee != 0,"可能无版权"
+                        assert fee != 1,"VIP歌曲，账户可能无权访问"
+                        assert fee != 4,"歌曲所在专辑需购买"
+                        assert fee != 8,"歌曲可能需要单独购买或以低音质加载"                        
+                        assert False, "未知原因 (fee=%d)" % fee
                     logger.info(
                         "开始下载 #%d / %d - %s - %s - %skbps - %s"
                         % (
                             task.index + 1,
                             task.total,
                             task.song.Title,
                             task.song.AlbumName,
@@ -593,16 +608,22 @@
             % (GetCurrentSession().nickname, GetCurrentSession().vipType)
         )
     if args.save:
         logger.info("保存登陆信息于 : %s" % args.save)
         open(args.save, "w").write(DumpSessionAsString(GetCurrentSession()))
         return 0
     if not GetCurrentSession().logged_in:
+        # deviceID doesn't seem to have a format,so to speak
+        # Meaning anything will work. 
+        # What we're trying to do here is to generate a UUID for
+        # the current machine so pyncm users won't be sharing the same one (i.e. id=pyncm!)        
+        import uuid,base64
+        GetCurrentSession().deviceId = base64.b64encode(uuid.getnode().to_bytes(48,"little")).decode()
         login.LoginViaAnonymousAccount()
-        logger.info("以匿名身份登陆成功，UID: %s" % GetCurrentSession().uid)
+        logger.info("以匿名身份登陆成功，deviceId=%s, UID: %s" % (GetCurrentSession().deviceId,GetCurrentSession().uid))
     executor = TaskPoolExecutorThread(max_workers=args.max_workers)
     executor.daemon = True
     executor.start()
 
     def enqueue_task(task):
         executor.task_queue.put(task)
```

### Comparing `pyncm-1.6.9.0/pyncm/apis/__init__.py` & `pyncm-1.6.9.0.1/pyncm/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/pyncm/apis/album.py` & `pyncm-1.6.9.0.1/pyncm/apis/album.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/pyncm/apis/artist.py` & `pyncm-1.6.9.0.1/pyncm/apis/artist.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/pyncm/apis/cloud.py` & `pyncm-1.6.9.0.1/pyncm/apis/cloud.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/pyncm/apis/cloudsearch.py` & `pyncm-1.6.9.0.1/pyncm/apis/cloudsearch.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/pyncm/apis/login.py` & `pyncm-1.6.9.0.1/pyncm/apis/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,27 +266,26 @@
     
     Notes:
         Session 默认使用 `pyncm!` 作为设备 ID
 
     Returns:
         dict
     '''
-    if deviceId:
-        GetCurrentSession().deviceId = deviceId
-    deviceId = GetCurrentSession().deviceId
+    if not deviceId:
+        deviceId = GetCurrentSession().deviceId    
     login_status = WeapiCryptoRequest(
         lambda: ("/api/register/anonimous" , {
         "username" : b64encode(
             ('%s %s' % (
                 deviceId,
                 cloudmusic_dll_encode_id(deviceId))).encode()
         ).decode()
         }
         )
-    )()
+    )()    
     assert login_status['code'] == 200,"匿名登陆失败"
     WriteLoginInfo({
         **login_status,
         'profile':{
             'nickname' : 'Anonymous',
             **login_status
         },
```

### Comparing `pyncm-1.6.9.0/pyncm/apis/miniprograms/difm.py` & `pyncm-1.6.9.0.1/pyncm/apis/miniprograms/difm.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/pyncm/apis/miniprograms/radio.py` & `pyncm-1.6.9.0.1/pyncm/apis/miniprograms/radio.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/pyncm/apis/miniprograms/sportsfm.py` & `pyncm-1.6.9.0.1/pyncm/apis/miniprograms/sportsfm.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/pyncm/apis/miniprograms/zonefm.py` & `pyncm-1.6.9.0.1/pyncm/apis/miniprograms/zonefm.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/pyncm/apis/playlist.py` & `pyncm-1.6.9.0.1/pyncm/apis/playlist.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/pyncm/apis/track.py` & `pyncm-1.6.9.0.1/pyncm/apis/track.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/pyncm/apis/user.py` & `pyncm-1.6.9.0.1/pyncm/apis/user.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/pyncm/apis/video.py` & `pyncm-1.6.9.0.1/pyncm/apis/video.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/pyncm/utils/__init__.py` & `pyncm-1.6.9.0.1/pyncm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/pyncm/utils/aes.py` & `pyncm-1.6.9.0.1/pyncm/utils/aes.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/pyncm/utils/crypto.py` & `pyncm-1.6.9.0.1/pyncm/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/pyncm/utils/helper.py` & `pyncm-1.6.9.0.1/pyncm/utils/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from functools import wraps
 from os import listdir,path
 import datetime,logging
 
 truncate_length = 64
 logger = logging.getLogger("pyncm.helper")
 
-def SubstituteWithFullwidth(string,sub=set('\x00\\/:<>|?*')):
+def SubstituteWithFullwidth(string,sub=set('\x00\\/:<>|?*"')):
     return "".join([c if not c in sub else chr(ord(c) + 0xFEE0) for c in string])
 
 def Default(default=None):    
     def preWrapper(func):
         @property
         @wraps(func)
         def wrapper(*a, **k):
```

### Comparing `pyncm-1.6.9.0/pyncm/utils/lrcparser.py` & `pyncm-1.6.9.0.1/pyncm/utils/lrcparser.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/pyncm/utils/security.py` & `pyncm-1.6.9.0.1/pyncm/utils/security.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/pyncm.egg-info/PKG-INFO` & `pyncm-1.6.9.0.1/pyncm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyncm
-Version: 1.6.9.0
+Version: 1.6.9.0.1
 Summary: NeteaseCloudMusic APIs for Python 3.x 适用于 Python 3 的网易云音乐 API
 Home-page: https://github.com/greats3an/pyncm
 Author: greats3an
 Author-email: greats3an@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyncm-1.6.9.0/pyncm.egg-info/SOURCES.txt` & `pyncm-1.6.9.0.1/pyncm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0/setup.py` & `pyncm-1.6.9.0.1/setup.py`

 * *Files identical despite different names*

