# Comparing `tmp/ming6131-0.0.0.8.tar.gz` & `tmp/ming6131-0.0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ming6131-0.0.0.8.tar", last modified: Tue Oct 25 02:34:49 2022, max compression
+gzip compressed data, was "ming6131-0.0.0.9.tar", last modified: Tue Oct 25 02:51:59 2022, max compression
```

## Comparing `ming6131-0.0.0.8.tar` & `ming6131-0.0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-10-25 02:34:49.975932 ming6131-0.0.0.8/
--rw-rw-rw-   0        0        0      482 2022-10-25 02:34:49.975932 ming6131-0.0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-10-25 01:53:20.000000 ming6131-0.0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-10-25 02:34:49.960909 ming6131-0.0.0.8/ming6131/
--rw-rw-rw-   0        0        0        0 2022-10-21 05:20:45.000000 ming6131-0.0.0.8/ming6131/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-25 02:34:49.971807 ming6131-0.0.0.8/ming6131/image/
--rw-rw-rw-   0        0        0     2129 2022-10-25 01:49:41.000000 ming6131-0.0.0.8/ming6131/image/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-25 02:34:49.973868 ming6131-0.0.0.8/ming6131/text/
--rw-rw-rw-   0        0        0      613 2022-10-25 01:49:41.000000 ming6131-0.0.0.8/ming6131/text/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-25 02:34:49.970789 ming6131-0.0.0.8/ming6131.egg-info/
--rw-rw-rw-   0        0        0      482 2022-10-25 02:34:49.000000 ming6131-0.0.0.8/ming6131.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2022-10-25 02:34:49.000000 ming6131-0.0.0.8/ming6131.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-25 02:34:49.000000 ming6131-0.0.0.8/ming6131.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2022-10-25 02:34:49.000000 ming6131-0.0.0.8/ming6131.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2022-10-25 02:34:49.000000 ming6131-0.0.0.8/ming6131.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-25 02:34:49.976814 ming6131-0.0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1392 2022-10-25 02:34:37.000000 ming6131-0.0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-25 02:51:59.439984 ming6131-0.0.0.9/
+-rw-rw-rw-   0        0        0      482 2022-10-25 02:51:59.439984 ming6131-0.0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2022-10-25 01:53:20.000000 ming6131-0.0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-10-25 02:51:59.421988 ming6131-0.0.0.9/ming6131/
+-rw-rw-rw-   0        0        0        0 2022-10-21 05:20:45.000000 ming6131-0.0.0.9/ming6131/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-25 02:51:59.434986 ming6131-0.0.0.9/ming6131/image/
+-rw-rw-rw-   0        0        0     2147 2022-10-25 02:51:27.000000 ming6131-0.0.0.9/ming6131/image/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-25 02:51:59.436985 ming6131-0.0.0.9/ming6131/text/
+-rw-rw-rw-   0        0        0      613 2022-10-25 01:49:41.000000 ming6131-0.0.0.9/ming6131/text/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-25 02:51:59.432988 ming6131-0.0.0.9/ming6131.egg-info/
+-rw-rw-rw-   0        0        0      482 2022-10-25 02:51:59.000000 ming6131-0.0.0.9/ming6131.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2022-10-25 02:51:59.000000 ming6131-0.0.0.9/ming6131.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-25 02:51:59.000000 ming6131-0.0.0.9/ming6131.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2022-10-25 02:51:59.000000 ming6131-0.0.0.9/ming6131.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2022-10-25 02:51:59.000000 ming6131-0.0.0.9/ming6131.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-10-25 02:51:59.440989 ming6131-0.0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1392 2022-10-25 02:51:53.000000 ming6131-0.0.0.9/setup.py
```

### Comparing `ming6131-0.0.0.8/ming6131/image/__init__.py` & `ming6131-0.0.0.9/ming6131/image/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from PIL import Image, ImageDraw, ImageFont
-from ming6131 import text
+import ming6131.text
 
 def fontPng(imagesize,text,ttf,fill,path,spacing=10):
     '''
     使text文本内容的字号与行数自适应指定的画布大小，
     返回文本居中的透明背景的PNG图片
         如果要使图片有颜色，可将以下代码中mode参数改成RGB，具体百度
         Image.new(mode='RGB', size=imagesize)
@@ -26,15 +26,15 @@
     draw_table = ImageDraw.Draw(im=image)
 
 
     # 位置
     xy = (0, 0)
 
     rw = 1
-    itext = text.tomultiline(text, rw)
+    itext = ming6131.text.tomultiline(text, rw)
 
     for ftSize in range(fontsize[0], fontsize[1]):
 
         # 字体
         font = ImageFont.truetype(ttf, ftSize)
         # 获取字体大小
         size = draw_table.multiline_textbbox(xy=xy, text=itext, font=font, spacing=spacing)
@@ -44,15 +44,15 @@
         if w <= imageW and h <= imageH:
             finalText = itext
             finalFont = font
             fw,fh = w,h
 
         elif w > imageW and h <= imageH:
             rw += 1
-            itext = tomultiline(text, rw)
+            itext = ming6131.text.tomultiline(text, rw)
         elif w > imageW and h > imageH:
             break
         elif h > imageH:
             break
     text = finalText
     font = finalFont
     x = (imageW-fw)/2
```

### Comparing `ming6131-0.0.0.8/ming6131/text/__init__.py` & `ming6131-0.0.0.9/ming6131/text/__init__.py`

 * *Files identical despite different names*

### Comparing `ming6131-0.0.0.8/setup.py` & `ming6131-0.0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='ming6131',  # 包名
-    version='0.0.0.8',  # 版本
+    version='0.0.0.9',  # 版本
     description="",  # 包简介
     long_description=open('README.md').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='',  # 作者
     author_email='',  # 作者邮件
     maintainer='',  # 维护者
     maintainer_email='',  # 维护者邮件
```

