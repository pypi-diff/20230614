# Comparing `tmp/DigiCore-1.0.3.tar.gz` & `tmp/DigiCore-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\DigiCore-1.0.3.tar", last modified: Wed Jun 14 06:39:15 2023, max compression
+gzip compressed data, was "dist\DigiCore-1.0.4.tar", last modified: Wed Jun 14 08:48:52 2023, max compression
```

## Comparing `DigiCore-1.0.3.tar` & `DigiCore-1.0.4.tar`

### file list

```diff
@@ -1,35 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 06:39:15.140298 DigiCore-1.0.3/
-drwxrwxrwx   0        0        0        0 2023-06-14 06:39:15.124551 DigiCore-1.0.3/DigiCore.egg-info/
--rw-rw-rw-   0        0        0     4014 2023-06-14 06:39:15.000000 DigiCore-1.0.3/DigiCore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      653 2023-06-14 06:39:15.000000 DigiCore-1.0.3/DigiCore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 06:39:15.000000 DigiCore-1.0.3/DigiCore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      663 2023-06-14 06:39:15.000000 DigiCore-1.0.3/DigiCore.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 06:39:15.000000 DigiCore-1.0.3/DigiCore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-06-14 06:39:15.000000 DigiCore-1.0.3/DigiCore.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1104 2023-05-20 03:41:32.000000 DigiCore-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     4014 2023-06-14 06:39:15.140298 DigiCore-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2670 2023-05-20 03:41:32.000000 DigiCore-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 06:39:15.126779 DigiCore-1.0.3/digiCore/
--rw-rw-rw-   0        0        0     1382 2023-05-20 06:50:26.000000 DigiCore-1.0.3/digiCore/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:39:15.126779 DigiCore-1.0.3/digiCore/dingding/
--rw-rw-rw-   0        0        0      130 2023-05-20 03:41:32.000000 DigiCore-1.0.3/digiCore/dingding/__init__.py
--rw-rw-rw-   0        0        0     1015 2023-05-23 01:25:52.000000 DigiCore-1.0.3/digiCore/dingding/dingding_model.py
--rw-rw-rw-   0        0        0     3747 2023-06-07 01:34:09.000000 DigiCore-1.0.3/digiCore/dingding/send_to_group.py
--rw-rw-rw-   0        0        0     4901 2023-06-14 02:12:46.000000 DigiCore-1.0.3/digiCore/dsd_kafka.py
--rw-rw-rw-   0        0        0     3673 2023-06-14 02:12:46.000000 DigiCore-1.0.3/digiCore/dsd_mongodb.py
--rw-rw-rw-   0        0        0     6853 2023-06-14 02:12:46.000000 DigiCore-1.0.3/digiCore/dsd_mysql.py
--rw-rw-rw-   0        0        0     3919 2023-05-20 07:33:42.000000 DigiCore-1.0.3/digiCore/dsd_redis.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:39:15.140298 DigiCore-1.0.3/digiCore/kingdee/
--rw-rw-rw-   0        0        0      553 2023-06-14 06:38:53.000000 DigiCore-1.0.3/digiCore/kingdee/__init__.py
--rw-rw-rw-   0        0        0     9953 2023-06-14 02:12:46.000000 DigiCore-1.0.3/digiCore/kingdee/kingdee_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:39:15.140298 DigiCore-1.0.3/digiCore/lingxing/
--rw-rw-rw-   0        0        0      130 2023-05-20 03:41:32.000000 DigiCore-1.0.3/digiCore/lingxing/__init__.py
--rw-rw-rw-   0        0        0     4167 2023-06-14 02:12:46.000000 DigiCore-1.0.3/digiCore/lingxing/api_scheduler.py
--rw-rw-rw-   0        0        0      786 2023-05-20 03:41:55.000000 DigiCore-1.0.3/digiCore/status_code.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:39:15.140298 DigiCore-1.0.3/digiCore/test/
--rw-rw-rw-   0        0        0      130 2023-05-20 03:41:32.000000 DigiCore-1.0.3/digiCore/test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:39:15.140298 DigiCore-1.0.3/digiCore/utils/
--rw-rw-rw-   0        0        0       25 2023-06-07 01:34:09.000000 DigiCore-1.0.3/digiCore/utils/__init__.py
--rw-rw-rw-   0        0        0     5351 2023-06-14 02:12:46.000000 DigiCore-1.0.3/digiCore/utils/utils.py
--rw-rw-rw-   0        0        0       42 2023-06-14 06:39:15.140298 DigiCore-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     3118 2023-06-14 06:38:53.000000 DigiCore-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:48:52.009566 DigiCore-1.0.4/
+drwxrwxrwx   0        0        0        0 2023-06-14 08:48:52.007058 DigiCore-1.0.4/DigiCore.egg-info/
+-rw-rw-rw-   0        0        0     4014 2023-06-14 08:48:51.000000 DigiCore-1.0.4/DigiCore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      444 2023-06-14 08:48:51.000000 DigiCore-1.0.4/DigiCore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 08:48:51.000000 DigiCore-1.0.4/DigiCore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      585 2023-06-14 08:48:51.000000 DigiCore-1.0.4/DigiCore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-14 08:48:51.000000 DigiCore-1.0.4/DigiCore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-06-14 08:48:18.000000 DigiCore-1.0.4/DigiCore.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1104 2023-05-20 03:41:32.000000 DigiCore-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     4014 2023-06-14 08:48:52.009566 DigiCore-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2670 2023-05-20 03:41:32.000000 DigiCore-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 08:48:52.009566 DigiCore-1.0.4/digiCore/
+-rw-rw-rw-   0        0        0     1382 2023-05-20 06:50:26.000000 DigiCore-1.0.4/digiCore/__init__.py
+-rw-rw-rw-   0        0        0     4901 2023-06-14 02:12:46.000000 DigiCore-1.0.4/digiCore/dsd_kafka.py
+-rw-rw-rw-   0        0        0     3673 2023-06-14 02:12:46.000000 DigiCore-1.0.4/digiCore/dsd_mongodb.py
+-rw-rw-rw-   0        0        0     6853 2023-06-14 02:12:46.000000 DigiCore-1.0.4/digiCore/dsd_mysql.py
+-rw-rw-rw-   0        0        0     3919 2023-05-20 07:33:42.000000 DigiCore-1.0.4/digiCore/dsd_redis.py
+-rw-rw-rw-   0        0        0     4161 2023-06-14 08:34:47.000000 DigiCore-1.0.4/digiCore/lingxing_api_scheduler.py
+-rw-rw-rw-   0        0        0     1015 2023-05-23 01:25:52.000000 DigiCore-1.0.4/digiCore/model.py
+-rw-rw-rw-   0        0        0     3738 2023-06-14 08:39:17.000000 DigiCore-1.0.4/digiCore/send_to_group.py
+-rw-rw-rw-   0        0        0      786 2023-05-20 03:41:55.000000 DigiCore-1.0.4/digiCore/status_code.py
+-rw-rw-rw-   0        0        0     5351 2023-06-14 02:12:46.000000 DigiCore-1.0.4/digiCore/utils.py
+-rw-rw-rw-   0        0        0       42 2023-06-14 08:48:52.009566 DigiCore-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     3015 2023-06-14 08:48:13.000000 DigiCore-1.0.4/setup.py
```

### Comparing `DigiCore-1.0.3/DigiCore.egg-info/PKG-INFO` & `DigiCore-1.0.4/DigiCore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DigiCore
-Version: 1.0.3
+Version: 1.0.4
 Summary: DigiCore是一个基于Python的数字化支持部第三方库，旨在为数据处理和开发提供完备的工具集和服务。
 Home-page: UNKNOWN
 Author: yarm
 Author-email: yangyang@doocn.com
 License: MIT License
 Keywords: digicore是服务于道诚集团数字化支持部的自建第三方库项目
 Platform: any
```

### Comparing `DigiCore-1.0.3/DigiCore.egg-info/requires.txt` & `DigiCore-1.0.4/DigiCore.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 colorama==0.4.6
 confluent-kafka==2.1.1
 crypto==1.4.1
 DBUtils==3.0.3
 dnspython==2.3.0
 et-xmlfile==1.1.0
 idna==3.4
-kingdee.cdp.webapi.sdk@ file:///kingdee.cdp.webapi.sdk-8.0.3-py3-none-any.whl
 loguru==0.7.0
 lz4==4.3.2
 Naked==0.1.32
 numpy==1.24.3
 openpyxl==3.1.2
 orjson==3.8.12
 package-name==0.1
```

### Comparing `DigiCore-1.0.3/LICENSE` & `DigiCore-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.3/PKG-INFO` & `DigiCore-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DigiCore
-Version: 1.0.3
+Version: 1.0.4
 Summary: DigiCore是一个基于Python的数字化支持部第三方库，旨在为数据处理和开发提供完备的工具集和服务。
 Home-page: UNKNOWN
 Author: yarm
 Author-email: yangyang@doocn.com
 License: MIT License
 Keywords: digicore是服务于道诚集团数字化支持部的自建第三方库项目
 Platform: any
```

### Comparing `DigiCore-1.0.3/README.md` & `DigiCore-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.3/digiCore/__init__.py` & `DigiCore-1.0.4/digiCore/__init__.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.3/digiCore/dingding/dingding_model.py` & `DigiCore-1.0.4/digiCore/model.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.3/digiCore/dingding/send_to_group.py` & `DigiCore-1.0.4/digiCore/send_to_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # _*_ coding:utf-8 _*_
 from loguru import logger
 import json
 import requests
-from dingding_model import Text, TextMsg, AtMobile, Markdown, MarkdownMsg, Link, LinkMsg
+from model import Text, TextMsg, AtMobile, Markdown, MarkdownMsg, Link, LinkMsg
 from digiCore import Decorate
 
 
 class SendToGroup():
     """
     1、将消息发送到群
     2、消息类型包括
```

### Comparing `DigiCore-1.0.3/digiCore/dsd_kafka.py` & `DigiCore-1.0.4/digiCore/dsd_kafka.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.3/digiCore/dsd_mongodb.py` & `DigiCore-1.0.4/digiCore/dsd_mongodb.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.3/digiCore/dsd_mysql.py` & `DigiCore-1.0.4/digiCore/dsd_mysql.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.3/digiCore/dsd_redis.py` & `DigiCore-1.0.4/digiCore/dsd_redis.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.3/digiCore/lingxing/api_scheduler.py` & `DigiCore-1.0.4/digiCore/lingxing_api_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # @File : common-lingxing-sign-api
 # @Desc :
 import copy
 import time
 import urllib
 from typing import Union
 from orjson import orjson
-from digiCore.utils.utils import EncryptTool
+from digiCore.utils import EncryptTool
 
 
 class SignBase(object):
 
     @classmethod
     def generate_sign(cls, encrypt_key: str, request_params: dict) -> str:
         """
```

### Comparing `DigiCore-1.0.3/digiCore/status_code.py` & `DigiCore-1.0.4/digiCore/status_code.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.3/digiCore/utils/utils.py` & `DigiCore-1.0.4/digiCore/utils.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.3/setup.py` & `DigiCore-1.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # @Author : 杨洋
 # @Email ： yangyang@doocn.com
 # @File : DigiCore
 # @Desc :
 
 from pathlib import Path
 
-import chardet
 from setuptools import find_packages, setup
 
 here = Path(__file__).resolve().parent
 README = (here / "README.md").read_text(encoding="utf-8")
 
 excluded_packages = ["tests", "tests.*"]
 
@@ -37,15 +36,14 @@
 "colorama==0.4.6",
 "confluent-kafka==2.1.1",
 "crypto==1.4.1",
 "DBUtils==3.0.3",
 "dnspython==2.3.0",
 "et-xmlfile==1.1.0",
 "idna==3.4",
-"kingdee.cdp.webapi.sdk @ file:///kingdee.cdp.webapi.sdk-8.0.3-py3-none-any.whl",
 "loguru==0.7.0",
 "lz4==4.3.2",
 "Naked==0.1.32",
 "numpy==1.24.3",
 "openpyxl==3.1.2",
 "orjson==3.8.12",
 "package-name==0.1",
@@ -62,21 +60,19 @@
 "requests==2.30.0",
 "shellescape==3.8.1",
 "six==1.16.0",
 "typing_extensions==4.5.0",
 "tzdata==2023.3",
 "urllib3==2.0.2",
 "win32-setctime==1.1.0"
-
-
 ]
 
 setup(
     name="DigiCore",
-    version="1.0.3",
+    version="1.0.4",
     description="DigiCore是一个基于Python的数字化支持部第三方库，旨在为数据处理和开发提供完备的工具集和服务。",
     long_description=README,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
```

