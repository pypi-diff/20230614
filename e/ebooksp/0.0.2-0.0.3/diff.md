# Comparing `tmp/ebooksp-0.0.2.tar.gz` & `tmp/ebooksp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebooksp-0.0.2.tar", last modified: Tue Jun 13 11:20:02 2023, max compression
+gzip compressed data, was "ebooksp-0.0.3.tar", last modified: Wed Jun 14 02:00:39 2023, max compression
```

## Comparing `ebooksp-0.0.2.tar` & `ebooksp-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-13 11:20:02.112329 ebooksp-0.0.2/
--rw-r--r--   0 bo         (501) staff       (20)    11357 2023-06-13 11:17:27.000000 ebooksp-0.0.2/LICENSE
--rw-r--r--   0 bo         (501) staff       (20)     1025 2023-06-13 11:20:02.112208 ebooksp-0.0.2/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)      567 2023-06-13 11:19:50.000000 ebooksp-0.0.2/README.md
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-13 11:20:02.111492 ebooksp-0.0.2/ebooksp/
--rw-r--r--   0 bo         (501) staff       (20)      667 2023-06-13 11:19:50.000000 ebooksp-0.0.2/ebooksp/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     2014 2023-06-13 11:17:27.000000 ebooksp-0.0.2/ebooksp/ebook_convert_format.py
--rw-r--r--   0 bo         (501) staff       (20)     1215 2023-06-13 11:17:27.000000 ebooksp-0.0.2/ebooksp/ebook_to_text.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-13 11:20:02.112052 ebooksp-0.0.2/ebooksp.egg-info/
--rw-r--r--   0 bo         (501) staff       (20)     1025 2023-06-13 11:20:01.000000 ebooksp-0.0.2/ebooksp.egg-info/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)      257 2023-06-13 11:20:02.000000 ebooksp-0.0.2/ebooksp.egg-info/SOURCES.txt
--rw-r--r--   0 bo         (501) staff       (20)        1 2023-06-13 11:20:01.000000 ebooksp-0.0.2/ebooksp.egg-info/dependency_links.txt
--rw-r--r--   0 bo         (501) staff       (20)       13 2023-06-13 11:20:02.000000 ebooksp-0.0.2/ebooksp.egg-info/requires.txt
--rw-r--r--   0 bo         (501) staff       (20)        8 2023-06-13 11:20:02.000000 ebooksp-0.0.2/ebooksp.egg-info/top_level.txt
--rw-r--r--   0 bo         (501) staff       (20)       38 2023-06-13 11:20:02.112375 ebooksp-0.0.2/setup.cfg
--rw-r--r--   0 bo         (501) staff       (20)      791 2023-06-13 11:19:50.000000 ebooksp-0.0.2/setup.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-14 02:00:39.201402 ebooksp-0.0.3/
+-rw-r--r--   0 bo         (501) staff       (20)    11357 2023-06-13 11:17:27.000000 ebooksp-0.0.3/LICENSE
+-rw-r--r--   0 bo         (501) staff       (20)     1025 2023-06-14 02:00:39.201292 ebooksp-0.0.3/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)      567 2023-06-13 11:19:50.000000 ebooksp-0.0.3/README.md
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-14 02:00:39.200561 ebooksp-0.0.3/ebooksp/
+-rw-r--r--   0 bo         (501) staff       (20)      667 2023-06-13 11:19:50.000000 ebooksp-0.0.3/ebooksp/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     2023 2023-06-14 01:56:52.000000 ebooksp-0.0.3/ebooksp/ebook_convert_format.py
+-rw-r--r--   0 bo         (501) staff       (20)     1301 2023-06-14 02:00:03.000000 ebooksp-0.0.3/ebooksp/ebook_to_text.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-14 02:00:39.201135 ebooksp-0.0.3/ebooksp.egg-info/
+-rw-r--r--   0 bo         (501) staff       (20)     1025 2023-06-14 02:00:38.000000 ebooksp-0.0.3/ebooksp.egg-info/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)      257 2023-06-14 02:00:39.000000 ebooksp-0.0.3/ebooksp.egg-info/SOURCES.txt
+-rw-r--r--   0 bo         (501) staff       (20)        1 2023-06-14 02:00:38.000000 ebooksp-0.0.3/ebooksp.egg-info/dependency_links.txt
+-rw-r--r--   0 bo         (501) staff       (20)       13 2023-06-14 02:00:39.000000 ebooksp-0.0.3/ebooksp.egg-info/requires.txt
+-rw-r--r--   0 bo         (501) staff       (20)        8 2023-06-14 02:00:39.000000 ebooksp-0.0.3/ebooksp.egg-info/top_level.txt
+-rw-r--r--   0 bo         (501) staff       (20)       38 2023-06-14 02:00:39.201439 ebooksp-0.0.3/setup.cfg
+-rw-r--r--   0 bo         (501) staff       (20)      791 2023-06-14 02:00:03.000000 ebooksp-0.0.3/setup.py
```

### Comparing `ebooksp-0.0.2/LICENSE` & `ebooksp-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ebooksp-0.0.2/PKG-INFO` & `ebooksp-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebooksp
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Conversion Tool for e-book
 Home-page: https://gitee.com/maxbanana
 Author: hongbo liu
 Author-email: 782027465@qq.com
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ebooksp-0.0.2/README.md` & `ebooksp-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ebooksp-0.0.2/ebooksp/__init__.py` & `ebooksp-0.0.3/ebooksp/__init__.py`

 * *Files identical despite different names*

### Comparing `ebooksp-0.0.2/ebooksp/ebook_convert_format.py` & `ebooksp-0.0.3/ebooksp/ebook_convert_format.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 def check_type(ebook_path: str):
     type_list = ['epub', 'mobi', 'azw3', 'azw']
     if isinstance(ebook_path, str):
         tag = False
         for t in type_list:
-            if t.endswith('.' + t):
+            if ebook_path.endswith('.' + t):
                 tag = True
                 break
         if not tag:
             raise ValueError(f'the formats supported by e-books include {type_list}')
     else:
         raise ValueError(f'ebook need require a str, not a {type(ebook_path)}')
```

### Comparing `ebooksp-0.0.2/ebooksp/ebook_to_text.py` & `ebooksp-0.0.3/ebooksp/ebook_to_text.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,32 +2,33 @@
 # @Time : 2023/6/13 18:00 
 # @Author : 刘洪波
 import subprocess
 import epubs
 from ebook_convert_format import ebook_convert_format
 
 
-def ebook_to_text(ebook_input: str, delete=True, timeout=60):
+def ebook_to_text(ebook_input: str, delete=True, timeout=60, func=None):
     """
     电子书转文本
     转换过程中会自动生成电子书的epub版本，路径和原电子书路径相同
     :param ebook_input: 电子书路径
     :param delete: 是否删除电子书的epub版本，
     :param timeout: 超时
+    :param func: 解析html的函数，默认使用自有函数
     :return:
     """
     epub_book = ebook_input
     if not ebook_input.endswith('.epub'):
         type_list = ['mobi', 'azw3', 'azw']
         for t in type_list:
             tt = '.' + t
             if ebook_input.endswith(tt):
                 epub_book = ebook_input.split(tt)[0] + '.epub'
         ebook_convert_format(ebook_input, epub_book, timeout)
-    res = epubs.to_text(epub_book)
+    res = epubs.to_text(epub_book, func=func)
     if delete:
         delete_epub(epub_book, timeout)
     return res
 
 
 def delete_epub(epub_path: str, timeout=60):
     """删除epub book"""
```

### Comparing `ebooksp-0.0.2/ebooksp.egg-info/PKG-INFO` & `ebooksp-0.0.3/ebooksp.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebooksp
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Conversion Tool for e-book
 Home-page: https://gitee.com/maxbanana
 Author: hongbo liu
 Author-email: 782027465@qq.com
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ebooksp-0.0.2/setup.py` & `ebooksp-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='ebooksp',
-    version='0.0.2',
+    version='0.0.3',
     packages=setuptools.find_packages(),
     url='https://gitee.com/maxbanana',
     license='Apache',
     author='hongbo liu',
     author_email='782027465@qq.com',
     description='A Conversion Tool for e-book',
     long_description=long_description,
```

