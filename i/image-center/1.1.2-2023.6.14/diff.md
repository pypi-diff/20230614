# Comparing `tmp/image_center-1.1.2.tar.gz` & `tmp/image_center-2023.6.14.tar.gz`

## Comparing `image_center-1.1.2.tar` & `image_center-2023.6.14.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    15319 2020-02-02 00:00:00.000000 image_center-1.1.2/image_center/__init__.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 image_center-1.1.2/image_center/__version__.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 image_center-1.1.2/image_center/conf.py
--rw-r--r--   0        0        0     4326 2020-02-02 00:00:00.000000 image_center-1.1.2/image_center/server.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 image_center-1.1.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 image_center-1.1.2/LICENSE
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 image_center-1.1.2/README.md
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 image_center-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 image_center-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    15319 2020-02-02 00:00:00.000000 image_center-2023.6.14/image_center/__init__.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 image_center-2023.6.14/image_center/__version__.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 image_center-2023.6.14/image_center/conf.py
+-rw-r--r--   0        0        0     4326 2020-02-02 00:00:00.000000 image_center-2023.6.14/image_center/server.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 image_center-2023.6.14/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 image_center-2023.6.14/LICENSE
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 image_center-2023.6.14/README.md
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 image_center-2023.6.14/pyproject.toml
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 image_center-2023.6.14/PKG-INFO
```

### Comparing `image_center-1.1.2/image_center/__init__.py` & `image_center-2023.6.14/image_center/__init__.py`

 * *Files identical despite different names*

### Comparing `image_center-1.1.2/image_center/conf.py` & `image_center-2023.6.14/image_center/conf.py`

 * *Files identical despite different names*

### Comparing `image_center-1.1.2/image_center/server.py` & `image_center-2023.6.14/image_center/server.py`

 * *Files identical despite different names*

### Comparing `image_center-1.1.2/.gitignore` & `image_center-2023.6.14/.gitignore`

 * *Files identical despite different names*

### Comparing `image_center-1.1.2/LICENSE` & `image_center-2023.6.14/LICENSE`

 * *Files identical despite different names*

### Comparing `image_center-1.1.2/README.md` & `image_center-2023.6.14/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # image-center
 图像识别定位某个元素在当前屏幕中的坐标；
 
 在自动化测试中获取到元素坐标之后，可以传入到键鼠工具，从而实现对目标元素的操作。
 
 ---
 
-**Documentation**: <a href="https://funny-test.github.io/image-center" target="_blank">https://funny-test.github.io/image-center</a>
+**Documentation**: <a href="https://funny-dream.github.io/image-center" target="_blank">https://funny-dream.github.io/image-center</a>
 
-**Source Code**: <a href="https://github.com/funny-test/image-center" target="_blank">https://github.com/funny-test/image-center</a>
+**Source Code**: <a href="https://github.com/funny-dream/image-center" target="_blank">https://github.com/funny-dream/image-center</a>
 
 ---
 
 ## 安装
 
 ```console
 pip install image-center
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # image-center å¾åè¯å«å®ä½æä¸ªåç´ å¨å½åå±å¹ä¸­çåæ ï¼
 å¨èªå¨åæµè¯ä¸­è·åå°åç´ åæ ä¹åï¼å¯ä»¥ä¼ å¥å°é®é¼ å·¥å·ï¼ä»èå®ç°å¯¹ç®æ åç´ çæä½ã
---- **Documentation**: https://funny-test.github.io/image-center **Source
-Code**: https://github.com/funny-test/image-center --- ## å®è£ ```console pip
-install image-center ```
+--- **Documentation**: https://funny-dream.github.io/image-center **Source
+Code**: https://github.com/funny-dream/image-center --- ## å®è£ ```console
+pip install image-center ```
 å¦ææ³å¨æ¬æºç´æ¥ä½¿ç¨å¾åè¯å«ï¼è¿éè¦å¨æ¬æºå®è£OpenCV
 ```shell sudo apt install python3-opencv ``` ## ä½¿ç¨è¯´æ
 æªåç®æ åç´ å¾çï¼å°å¾çä¿å­å°æä¸ªè·¯å¾ï¼ ```python from
 image_center import ImageCenter ImageCenter.find_image("~/Desktop/test.png")
 ``` è¿å `test.png` å¨å½åå±å¹ä¸­çä½ç½®ã ## RPCæå¡
 å¦æä¸æ³å¨æ¬æºå®è£OpenCVï¼æèä½ çæºå¨æ æ³å®è£OpenCVï¼å¯ä»¥å¨æå¡ç«¯å®è£OpenCVï¼å®è£æ¹æ³åä¸é¢ä¸æ ·ï¼ï¼
 æå¡ç«¯å¯å¨æ¹æ³ï¼ ```python from image_center.server import server from
```

### Comparing `image_center-1.1.2/pyproject.toml` & `image_center-2023.6.14/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -42,9 +42,9 @@
 [tool.hatch.build.targets.sdist]
 include = [
     "/image_center",
     "/README.md",
 ]
 
 [project.urls]
-Source = "https://github.com/funny-test/image-center"
-Documentation = "https://funny-test.github.io/image-center"
+Source = "https://github.com/funny-dream/image-center"
+Documentation = "https://funny-dream.github.io/image-center"
```

### Comparing `image_center-1.1.2/PKG-INFO` & `image_center-2023.6.14/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: image-center
-Version: 1.1.2
+Version: 2023.6.14
 Summary: image-center
-Project-URL: Source, https://github.com/funny-test/image-center
-Project-URL: Documentation, https://funny-test.github.io/image-center
+Project-URL: Source, https://github.com/funny-dream/image-center
+Project-URL: Documentation, https://funny-dream.github.io/image-center
 Author-email: mikigo <1964191531@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: pillow
@@ -21,17 +21,17 @@
 # image-center
 图像识别定位某个元素在当前屏幕中的坐标；
 
 在自动化测试中获取到元素坐标之后，可以传入到键鼠工具，从而实现对目标元素的操作。
 
 ---
 
-**Documentation**: <a href="https://funny-test.github.io/image-center" target="_blank">https://funny-test.github.io/image-center</a>
+**Documentation**: <a href="https://funny-dream.github.io/image-center" target="_blank">https://funny-dream.github.io/image-center</a>
 
-**Source Code**: <a href="https://github.com/funny-test/image-center" target="_blank">https://github.com/funny-test/image-center</a>
+**Source Code**: <a href="https://github.com/funny-dream/image-center" target="_blank">https://github.com/funny-dream/image-center</a>
 
 ---
 
 ## 安装
 
 ```console
 pip install image-center
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: image-center Version: 1.1.2 Summary: image-center
-Project-URL: Source, https://github.com/funny-test/image-center Project-URL:
-Documentation, https://funny-test.github.io/image-center Author-email: mikigo
-<1964191531@qq.com> License-File: LICENSE Classifier: License :: OSI Approved
-:: Apache Software License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.7
-Requires-Dist: pillow Requires-Dist: pyscreenshot Provides-Extra: doc Requires-
-Dist: mkdocs-material; extra == 'doc' Provides-Extra: test Requires-Dist:
-pytest; extra == 'test' Description-Content-Type: text/markdown # image-center
-å¾åè¯å«å®ä½æä¸ªåç´ å¨å½åå±å¹ä¸­çåæ ï¼
+Metadata-Version: 2.1 Name: image-center Version: 2023.6.14 Summary: image-
+center Project-URL: Source, https://github.com/funny-dream/image-center
+Project-URL: Documentation, https://funny-dream.github.io/image-center Author-
+email: mikigo <1964191531@qq.com> License-File: LICENSE Classifier: License ::
+OSI Approved :: Apache Software License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Requires-Python:
+>=3.7 Requires-Dist: pillow Requires-Dist: pyscreenshot Provides-Extra: doc
+Requires-Dist: mkdocs-material; extra == 'doc' Provides-Extra: test Requires-
+Dist: pytest; extra == 'test' Description-Content-Type: text/markdown # image-
+center å¾åè¯å«å®ä½æä¸ªåç´ å¨å½åå±å¹ä¸­çåæ ï¼
 å¨èªå¨åæµè¯ä¸­è·åå°åç´ åæ ä¹åï¼å¯ä»¥ä¼ å¥å°é®é¼ å·¥å·ï¼ä»èå®ç°å¯¹ç®æ åç´ çæä½ã
---- **Documentation**: https://funny-test.github.io/image-center **Source
-Code**: https://github.com/funny-test/image-center --- ## å®è£ ```console pip
-install image-center ```
+--- **Documentation**: https://funny-dream.github.io/image-center **Source
+Code**: https://github.com/funny-dream/image-center --- ## å®è£ ```console
+pip install image-center ```
 å¦ææ³å¨æ¬æºç´æ¥ä½¿ç¨å¾åè¯å«ï¼è¿éè¦å¨æ¬æºå®è£OpenCV
 ```shell sudo apt install python3-opencv ``` ## ä½¿ç¨è¯´æ
 æªåç®æ åç´ å¾çï¼å°å¾çä¿å­å°æä¸ªè·¯å¾ï¼ ```python from
 image_center import ImageCenter ImageCenter.find_image("~/Desktop/test.png")
 ``` è¿å `test.png` å¨å½åå±å¹ä¸­çä½ç½®ã ## RPCæå¡
 å¦æä¸æ³å¨æ¬æºå®è£OpenCVï¼æèä½ çæºå¨æ æ³å®è£OpenCVï¼å¯ä»¥å¨æå¡ç«¯å®è£OpenCVï¼å®è£æ¹æ³åä¸é¢ä¸æ ·ï¼ï¼
 æå¡ç«¯å¯å¨æ¹æ³ï¼ ```python from image_center.server import server from
```

