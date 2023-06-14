# Comparing `tmp/fast_model_server-1.0.0.1-py2.py3-none-any.whl.zip` & `tmp/fast_model_server-1.1.0.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 35103 bytes, number of entries: 36
+Zip file size: 41546 bytes, number of entries: 44
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-13 00:53 fast_model_server/__init__.py
 -rw-rw-r--  2.0 unx     3880 b- defN 23-Jun-13 00:53 fast_model_server/application.py
 -rw-rw-r--  2.0 unx     1836 b- defN 23-Jun-13 15:35 fast_model_server/common.py
 -rw-rw-r--  2.0 unx    15304 b- defN 23-Jun-13 15:35 fast_model_server/create.py
 -rw-rw-r--  2.0 unx    11823 b- defN 23-Jun-13 15:35 fast_model_server/main.py
 -rw-rw-r--  2.0 unx      343 b- defN 23-Jun-13 15:35 fast_model_server/router_service.py
 -rw-r--r--  2.0 unx      975 b- defN 23-Jun-13 03:10 fast_model_server/template/router/common.py.template
@@ -17,22 +17,30 @@
 -rw-rw-r--  2.0 unx     1519 b- defN 23-Jun-13 15:48 fast_model_server/utils/redis_cache.py
 -rw-rw-r--  2.0 unx     2011 b- defN 23-Jun-13 15:48 fast_model_server/utils/redis_connection.py
 -rw-rw-r--  2.0 unx     1903 b- defN 23-Jun-13 15:50 fast_model_server/utils/redis_lock.py
 -rw-rw-r--  2.0 unx     2589 b- defN 23-Jun-13 15:48 fast_model_server/utils/redis_msg_queue.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-13 00:53 fast_model_server/utils/bdcrawler/__init__.py
 -rw-r--r--  2.0 unx     3965 b- defN 23-Jun-13 00:53 fast_model_server/utils/bdcrawler/crawler.config.json
 -rw-rw-r--  2.0 unx    11207 b- defN 23-Jun-13 02:24 fast_model_server/utils/bdcrawler/crawler.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jun-14 06:23 fast_model_server/utils/llm_model_access/__init__.py
+-rw-rw-r--  2.0 unx      120 b- defN 23-Jun-14 06:28 fast_model_server/utils/llm_model_access/embeddings/__init__.py
+-rw-rw-r--  2.0 unx     3188 b- defN 23-Jun-14 06:33 fast_model_server/utils/llm_model_access/embeddings/fschat.py
+-rw-rw-r--  2.0 unx     2023 b- defN 23-Jun-14 06:33 fast_model_server/utils/llm_model_access/embeddings/rocketqa.py
+-rw-rw-r--  2.0 unx      121 b- defN 23-Jun-14 06:46 fast_model_server/utils/llm_model_access/llms/__init__.py
+-rw-rw-r--  2.0 unx     4958 b- defN 23-Jun-14 06:33 fast_model_server/utils/llm_model_access/llms/fschat.py
+-rw-rw-r--  2.0 unx      122 b- defN 23-Jun-14 06:41 fast_model_server/utils/llm_model_access/rankers/__init__.py
+-rw-rw-r--  2.0 unx     2691 b- defN 23-Jun-14 06:41 fast_model_server/utils/llm_model_access/rankers/rocketqa.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-13 00:53 fast_model_server/utils/model_access/__init__.py
 -rw-rw-r--  2.0 unx    15399 b- defN 23-Jun-13 02:25 fast_model_server/utils/model_access/model_access.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-13 00:53 fast_model_server/utils/model_manage/__init__.py
 -rw-r--r--  2.0 unx       90 b- defN 23-Jun-13 00:53 fast_model_server/utils/model_manage/model_manage.config.json
 -rw-rw-r--  2.0 unx     4722 b- defN 23-Jun-13 15:57 fast_model_server/utils/model_manage/model_manage.py
 -rw-r--r--  2.0 unx      648 b- defN 23-Jun-13 00:53 fast_model_server/utils/model_manage/pack.sh
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-13 00:53 fast_model_server/utils/rule/__init__.py
 -rw-rw-r--  2.0 unx     4059 b- defN 23-Jun-13 16:01 fast_model_server/utils/rule/rule.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-13 00:53 fast_model_server/utils/rule/test/__init__.py
 -rw-rw-r--  2.0 unx     1464 b- defN 23-Jun-13 15:45 fast_model_server/utils/rule/test/test_rule.py
--rw-rw-r--  2.0 unx     2711 b- defN 23-Jun-13 16:01 fast_model_server-1.0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Jun-13 16:01 fast_model_server-1.0.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       18 b- defN 23-Jun-13 16:01 fast_model_server-1.0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3534 b- defN 23-Jun-13 16:01 fast_model_server-1.0.0.1.dist-info/RECORD
-36 files, 95866 bytes uncompressed, 29213 bytes compressed:  69.5%
+-rw-rw-r--  2.0 unx     2727 b- defN 23-Jun-14 06:47 fast_model_server-1.1.0.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jun-14 06:47 fast_model_server-1.1.0.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       18 b- defN 23-Jun-14 06:47 fast_model_server-1.1.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4455 b- defN 23-Jun-14 06:47 fast_model_server-1.1.0.0.dist-info/RECORD
+44 files, 110026 bytes uncompressed, 34106 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -60,14 +60,38 @@
 
 Filename: fast_model_server/utils/bdcrawler/crawler.config.json
 Comment: 
 
 Filename: fast_model_server/utils/bdcrawler/crawler.py
 Comment: 
 
+Filename: fast_model_server/utils/llm_model_access/__init__.py
+Comment: 
+
+Filename: fast_model_server/utils/llm_model_access/embeddings/__init__.py
+Comment: 
+
+Filename: fast_model_server/utils/llm_model_access/embeddings/fschat.py
+Comment: 
+
+Filename: fast_model_server/utils/llm_model_access/embeddings/rocketqa.py
+Comment: 
+
+Filename: fast_model_server/utils/llm_model_access/llms/__init__.py
+Comment: 
+
+Filename: fast_model_server/utils/llm_model_access/llms/fschat.py
+Comment: 
+
+Filename: fast_model_server/utils/llm_model_access/rankers/__init__.py
+Comment: 
+
+Filename: fast_model_server/utils/llm_model_access/rankers/rocketqa.py
+Comment: 
+
 Filename: fast_model_server/utils/model_access/__init__.py
 Comment: 
 
 Filename: fast_model_server/utils/model_access/model_access.py
 Comment: 
 
 Filename: fast_model_server/utils/model_manage/__init__.py
@@ -90,20 +114,20 @@
 
 Filename: fast_model_server/utils/rule/test/__init__.py
 Comment: 
 
 Filename: fast_model_server/utils/rule/test/test_rule.py
 Comment: 
 
-Filename: fast_model_server-1.0.0.1.dist-info/METADATA
+Filename: fast_model_server-1.1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: fast_model_server-1.0.0.1.dist-info/WHEEL
+Filename: fast_model_server-1.1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: fast_model_server-1.0.0.1.dist-info/top_level.txt
+Filename: fast_model_server-1.1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fast_model_server-1.0.0.1.dist-info/RECORD
+Filename: fast_model_server-1.1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fast_model_server-1.0.0.1.dist-info/METADATA` & `fast_model_server-1.1.0.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-model-server
-Version: 1.0.0.1
+Version: 1.1.0.0
 Summary: python基础服务框架
 Home-page: https://codeup.aliyun.com/64650c96168f0a5963451dec/lib/fast-model-server/blob/master/README.md
 Author: yes_bobo
 Author-email: fb_linux@163.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -13,21 +13,21 @@
 Description-Content-Type: text/markdown
 Requires-Dist: fastapi (==0.63.0)
 Requires-Dist: uvicorn (==0.15.0)
 Requires-Dist: pydantic (==1.8.2)
 Requires-Dist: typing (==3.7.4.3)
 Requires-Dist: aiofiles (==0.8.0)
 Requires-Dist: rule-engine (==3.5.0)
+Requires-Dist: langchain (==0.0.194)
 Requires-Dist: dash (==2.7.1)
 Requires-Dist: bce-python-sdk
 Requires-Dist: httpx
 Requires-Dist: tqdm
 Requires-Dist: redis
 Requires-Dist: networkx
-Requires-Dist: jieba
 
 Fast[API] Model Server
 ===
 python服务框架
 
 快速开始
 ---
```

## Comparing `fast_model_server-1.0.0.1.dist-info/RECORD` & `fast_model_server-1.1.0.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -16,21 +16,29 @@
 fast_model_server/utils/redis_cache.py,sha256=b9sSkbWbfsnAqRuBhn9nAFdQZEF53aHhrDHHIvCz8bw,1519
 fast_model_server/utils/redis_connection.py,sha256=EYQr_PVsW5Hko7QxLtRfSJoi9u3Y02tFK7H3sQB4wYY,2011
 fast_model_server/utils/redis_lock.py,sha256=EWoPTQzngtMYpxt-va1MCpik8clsxUVgBkF1ZzG-eLw,1903
 fast_model_server/utils/redis_msg_queue.py,sha256=cYuJQePtIDxNwMj3dwlcRLNFSN2HKGo30A2dzagGtjM,2589
 fast_model_server/utils/bdcrawler/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fast_model_server/utils/bdcrawler/crawler.config.json,sha256=_-qPug446dsdDizK2O2g0TdE9S3DBmXGQD1YF8_zjE4,3965
 fast_model_server/utils/bdcrawler/crawler.py,sha256=0_F-ddIKnmui2n754i13u5f0A00JdUXGGgSbc-_A0Sg,11207
+fast_model_server/utils/llm_model_access/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+fast_model_server/utils/llm_model_access/embeddings/__init__.py,sha256=2skmITnWC_F-PuV6p5aU8nK1xuqlXtYxiABTQlxCZ4Q,120
+fast_model_server/utils/llm_model_access/embeddings/fschat.py,sha256=a437d2-vwiTS-ZljYQynWgn6cfr3VZOgTppAB5OkGVg,3188
+fast_model_server/utils/llm_model_access/embeddings/rocketqa.py,sha256=CjZ6VfkXTFyTZkZ5bvNiicq9hqS24URjPMycx3NQu4s,2023
+fast_model_server/utils/llm_model_access/llms/__init__.py,sha256=SG3TPKwAsP5xxRHQlQikMzxcwXQavSHRl4fvNYRyyuM,121
+fast_model_server/utils/llm_model_access/llms/fschat.py,sha256=mr2ECqS8rxpuDZCzA6iq3hMZNi0-4TE0NufLjLLe3k0,4958
+fast_model_server/utils/llm_model_access/rankers/__init__.py,sha256=hxM9CLVVeqCh4DYJXOBCYTOt_GKeVrugl_umQB7RJnc,122
+fast_model_server/utils/llm_model_access/rankers/rocketqa.py,sha256=ldkaf1kDdTINjWJMoYoOxlFiM2TzreLdrfSaJxgdRFs,2691
 fast_model_server/utils/model_access/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fast_model_server/utils/model_access/model_access.py,sha256=qkjRyIFmrHP8vqMhJ8La_-Vj9UQXayApz-Q0-XFSR_w,15399
 fast_model_server/utils/model_manage/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fast_model_server/utils/model_manage/model_manage.config.json,sha256=7IUID818YotaZquUQSvSozv1fn3qf-t7-0Sa5ulwVMo,90
 fast_model_server/utils/model_manage/model_manage.py,sha256=k593aX4Z7EgA9O0Il2TFxLUKeQI2i35nc6dVh1CdHmo,4722
 fast_model_server/utils/model_manage/pack.sh,sha256=NJ76Y6snY5ngmIOmm8g2ZeALETRbpDmRZ9Zyy2D-c28,648
 fast_model_server/utils/rule/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fast_model_server/utils/rule/rule.py,sha256=sq8K2HorzeGAaxb3FSatgUIl0DF6xy7Xgbp4Sfj7ZXk,4059
 fast_model_server/utils/rule/test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fast_model_server/utils/rule/test/test_rule.py,sha256=CzysHmPMJ3hLDouzWm-er0QLDb4ojBEKVaVllFhTo_8,1464
-fast_model_server-1.0.0.1.dist-info/METADATA,sha256=eSvKm7P7P9aLdfcy3lqCQ7sLeMuv6yD69CiZlnhz3Z8,2711
-fast_model_server-1.0.0.1.dist-info/WHEEL,sha256=oh0NKYrTcu1i1-wgrI1cnhkjYIi8WJ-8qd9Jrr5_y4E,110
-fast_model_server-1.0.0.1.dist-info/top_level.txt,sha256=v0z-TTFnnZC-On43gY1hMZaNWjxGkerzZ4eaqcrqbBo,18
-fast_model_server-1.0.0.1.dist-info/RECORD,,
+fast_model_server-1.1.0.0.dist-info/METADATA,sha256=LFXPqRXz3GHrR6JDBp1q9dF1OVWbgG0yzSSYNl4iM2k,2727
+fast_model_server-1.1.0.0.dist-info/WHEEL,sha256=oh0NKYrTcu1i1-wgrI1cnhkjYIi8WJ-8qd9Jrr5_y4E,110
+fast_model_server-1.1.0.0.dist-info/top_level.txt,sha256=v0z-TTFnnZC-On43gY1hMZaNWjxGkerzZ4eaqcrqbBo,18
+fast_model_server-1.1.0.0.dist-info/RECORD,,
```

