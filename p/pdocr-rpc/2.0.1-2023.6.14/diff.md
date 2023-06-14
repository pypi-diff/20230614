# Comparing `tmp/pdocr_rpc-2.0.1.tar.gz` & `tmp/pdocr_rpc-2023.6.14.tar.gz`

## Comparing `pdocr_rpc-2.0.1.tar` & `pdocr_rpc-2023.6.14.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     6441 2020-02-02 00:00:00.000000 pdocr_rpc-2.0.1/pdocr_rpc/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pdocr_rpc-2.0.1/pdocr_rpc/__version__.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 pdocr_rpc-2.0.1/pdocr_rpc/conf.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 pdocr_rpc-2.0.1/pdocr_rpc/server.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pdocr_rpc-2.0.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pdocr_rpc-2.0.1/LICENSE
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 pdocr_rpc-2.0.1/README.md
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 pdocr_rpc-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 pdocr_rpc-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6441 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.14/pdocr_rpc/__init__.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.14/pdocr_rpc/__version__.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.14/pdocr_rpc/conf.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.14/pdocr_rpc/server.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.14/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.14/LICENSE
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.14/README.md
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.14/pyproject.toml
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.14/PKG-INFO
```

### Comparing `pdocr_rpc-2.0.1/pdocr_rpc/__init__.py` & `pdocr_rpc-2023.6.14/pdocr_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2.0.1/pdocr_rpc/conf.py` & `pdocr_rpc-2023.6.14/pdocr_rpc/conf.py`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2.0.1/pdocr_rpc/server.py` & `pdocr_rpc-2023.6.14/pdocr_rpc/server.py`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2.0.1/LICENSE` & `pdocr_rpc-2023.6.14/LICENSE`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2.0.1/README.md` & `pdocr_rpc-2023.6.14/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 因为 `PaddleOCR` 安装**太重**了，如果你的使用场景是需要经常安装，那绝对是一个痛苦的事情，你要是知道它每次安装要装多少东西你肯定会忍不住摇头；
 
 而在服务端一次性安装部署之后，客户端就可以零成本的使用，非常的方便。
 
 ---
 
-**Documentation**: <a href="https://funny-test.github.io/pdocr-rpc" target="_blank">https://funny-test.github.io/pdocr-rpc</a>
+**Documentation**: <a href="https://funny-dream.github.io/pdocr-rpc" target="_blank">https://funny-dream.github.io/pdocr-rpc</a>
 
-**Source Code**: <a href="https://github.com/funny-test/pdocr-rpc" target="_blank">https://github.com/funny-test/pdocr-rpc</a>
+**Source Code**: <a href="https://github.com/funny-dream/pdocr-rpc" target="_blank">https://github.com/funny-dream/pdocr-rpc</a>
 
 ---
 
 ## 1、服务端
 
 ### 服务端安装
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 # pdocr-rpc åºäº `PaddleOCR` å°è£ç `RPC`
 æå¡ï¼åå«å®¢æ·ç«¯åæå¡ç«¯ã
 å®¢æ·ç«¯æä¾äºä¸ä¸ªç®åæç¨çå½æ°
 `ocr`ï¼éè¿ä¸åçåæ°æ§å¶è¿åä¸åçå¼ã
 **ä¸ºä»ä¹è¦åææå¡ç«¯åå®¢æ·ç«¯ï¼** å ä¸º `PaddleOCR`
 å®è£**å¤ªé**äºï¼å¦æä½ çä½¿ç¨åºæ¯æ¯éè¦ç»å¸¸å®è£ï¼é£ç»å¯¹æ¯ä¸ä¸ªçè¦çäºæï¼ä½ è¦æ¯ç¥éå®æ¯æ¬¡å®è£è¦è£å¤å°ä¸è¥¿ä½ è¯å®ä¼å¿ä¸ä½æå¤´ï¼
 èå¨æå¡ç«¯ä¸æ¬¡æ§å®è£é¨ç½²ä¹åï¼å®¢æ·ç«¯å°±å¯ä»¥é¶ææ¬çä½¿ç¨ï¼éå¸¸çæ¹ä¾¿ã
---- **Documentation**: https://funny-test.github.io/pdocr-rpc **Source Code**:
-https://github.com/funny-test/pdocr-rpc --- ## 1ãæå¡ç«¯ ###
+--- **Documentation**: https://funny-dream.github.io/pdocr-rpc **Source Code**:
+https://github.com/funny-dream/pdocr-rpc --- ## 1ãæå¡ç«¯ ###
 æå¡ç«¯å®è£ ```console pip install pdocr-rpc[server] ``` ###
 æå¡ç«¯å¯å¨æå¡
 éææ°å»ºä¸ä¸ª`py`æä»¶ï¼åç§°ä½ å¯ä»¥èªå®ä¹ï¼æ¯å¦ï¼`ocr_server.py`ï¼
 åå¥ä»¥ä¸åå®¹ï¼ ```python # ocr_server.py from pdocr_rpc.server import
 server server() ``` é»è®¤ç«¯å£å·ä¸º `8890` å¦æä½ æ³ä¿®æ¹ç«¯å£ï¼
 ```python from pdocr_rpc.server import server from pdocr_rpc.conf import
 setting setting.PORT = 8888 server() ``` ## 2ãå®¢æ·ç«¯ ### å®¢æ·ç«¯å®è£
```

### Comparing `pdocr_rpc-2.0.1/pyproject.toml` & `pdocr_rpc-2023.6.14/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pdocr-rpc"
 authors = [
@@ -42,9 +43,9 @@
 [tool.hatch.build.targets.sdist]
 include = [
     "/pdocr_rpc",
     "/README.md",
 ]
 
 [project.urls]
-Source = "https://github.com/funny-test/pdocr-rpc"
-Documentation = "https://funny-test.github.io/pdocr-rpc"
+Source = "https://github.com/funny-dream/pdocr-rpc"
+Documentation = "https://funny-dream.github.io/pdocr-rpc"
```

### Comparing `pdocr_rpc-2.0.1/PKG-INFO` & `pdocr_rpc-2023.6.14/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pdocr-rpc
-Version: 2.0.1
+Version: 2023.6.14
 Summary: PaddleOCR-RPC
-Project-URL: Source, https://github.com/funny-test/pdocr-rpc
-Project-URL: Documentation, https://funny-test.github.io/pdocr-rpc
+Project-URL: Source, https://github.com/funny-dream/pdocr-rpc
+Project-URL: Documentation, https://funny-dream.github.io/pdocr-rpc
 Author-email: mikigo <1964191531@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: pillow; sys_platform == 'win32'
@@ -31,17 +31,17 @@
 
 因为 `PaddleOCR` 安装**太重**了，如果你的使用场景是需要经常安装，那绝对是一个痛苦的事情，你要是知道它每次安装要装多少东西你肯定会忍不住摇头；
 
 而在服务端一次性安装部署之后，客户端就可以零成本的使用，非常的方便。
 
 ---
 
-**Documentation**: <a href="https://funny-test.github.io/pdocr-rpc" target="_blank">https://funny-test.github.io/pdocr-rpc</a>
+**Documentation**: <a href="https://funny-dream.github.io/pdocr-rpc" target="_blank">https://funny-dream.github.io/pdocr-rpc</a>
 
-**Source Code**: <a href="https://github.com/funny-test/pdocr-rpc" target="_blank">https://github.com/funny-test/pdocr-rpc</a>
+**Source Code**: <a href="https://github.com/funny-dream/pdocr-rpc" target="_blank">https://github.com/funny-dream/pdocr-rpc</a>
 
 ---
 
 ## 1、服务端
 
 ### 服务端安装
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pdocr-rpc Version: 2.0.1 Summary: PaddleOCR-RPC
-Project-URL: Source, https://github.com/funny-test/pdocr-rpc Project-URL:
-Documentation, https://funny-test.github.io/pdocr-rpc Author-email: mikigo
+Metadata-Version: 2.1 Name: pdocr-rpc Version: 2023.6.14 Summary: PaddleOCR-RPC
+Project-URL: Source, https://github.com/funny-dream/pdocr-rpc Project-URL:
+Documentation, https://funny-dream.github.io/pdocr-rpc Author-email: mikigo
 <1964191531@qq.com> License-File: LICENSE Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.7
 Requires-Dist: pillow; sys_platform == 'win32' Requires-Dist: pyscreenshot;
 sys_platform == 'linux' Provides-Extra: doc Requires-Dist: mkdocs-material;
 extra == 'doc' Provides-Extra: server Requires-Dist: paddleocr>=2.0.1; extra ==
 'server' Requires-Dist: paddlepaddle; extra == 'server' Provides-Extra: test
@@ -12,16 +12,16 @@
 # pdocr-rpc åºäº `PaddleOCR` å°è£ç `RPC`
 æå¡ï¼åå«å®¢æ·ç«¯åæå¡ç«¯ã
 å®¢æ·ç«¯æä¾äºä¸ä¸ªç®åæç¨çå½æ°
 `ocr`ï¼éè¿ä¸åçåæ°æ§å¶è¿åä¸åçå¼ã
 **ä¸ºä»ä¹è¦åææå¡ç«¯åå®¢æ·ç«¯ï¼** å ä¸º `PaddleOCR`
 å®è£**å¤ªé**äºï¼å¦æä½ çä½¿ç¨åºæ¯æ¯éè¦ç»å¸¸å®è£ï¼é£ç»å¯¹æ¯ä¸ä¸ªçè¦çäºæï¼ä½ è¦æ¯ç¥éå®æ¯æ¬¡å®è£è¦è£å¤å°ä¸è¥¿ä½ è¯å®ä¼å¿ä¸ä½æå¤´ï¼
 èå¨æå¡ç«¯ä¸æ¬¡æ§å®è£é¨ç½²ä¹åï¼å®¢æ·ç«¯å°±å¯ä»¥é¶ææ¬çä½¿ç¨ï¼éå¸¸çæ¹ä¾¿ã
---- **Documentation**: https://funny-test.github.io/pdocr-rpc **Source Code**:
-https://github.com/funny-test/pdocr-rpc --- ## 1ãæå¡ç«¯ ###
+--- **Documentation**: https://funny-dream.github.io/pdocr-rpc **Source Code**:
+https://github.com/funny-dream/pdocr-rpc --- ## 1ãæå¡ç«¯ ###
 æå¡ç«¯å®è£ ```console pip install pdocr-rpc[server] ``` ###
 æå¡ç«¯å¯å¨æå¡
 éææ°å»ºä¸ä¸ª`py`æä»¶ï¼åç§°ä½ å¯ä»¥èªå®ä¹ï¼æ¯å¦ï¼`ocr_server.py`ï¼
 åå¥ä»¥ä¸åå®¹ï¼ ```python # ocr_server.py from pdocr_rpc.server import
 server server() ``` é»è®¤ç«¯å£å·ä¸º `8890` å¦æä½ æ³ä¿®æ¹ç«¯å£ï¼
 ```python from pdocr_rpc.server import server from pdocr_rpc.conf import
 setting setting.PORT = 8888 server() ``` ## 2ãå®¢æ·ç«¯ ### å®¢æ·ç«¯å®è£
```

