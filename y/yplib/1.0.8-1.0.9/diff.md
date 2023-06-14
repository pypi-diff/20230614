# Comparing `tmp/yplib-1.0.8.tar.gz` & `tmp/yplib-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.0.8.tar", last modified: Wed Jun 14 00:35:16 2023, max compression
+gzip compressed data, was "dist\yplib-1.0.9.tar", last modified: Wed Jun 14 00:56:21 2023, max compression
```

## Comparing `yplib-1.0.8.tar` & `yplib-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 00:35:16.341557 yplib-1.0.8/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.0.8/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-14 00:35:16.341557 yplib-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 00:35:16.342358 yplib-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-14 00:34:41.000000 yplib-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 00:35:16.338777 yplib-1.0.8/yplib/
--rw-rw-rw-   0        0        0       87 2023-06-14 00:01:35.000000 yplib-1.0.8/yplib/__init__.py
--rw-rw-rw-   0        0        0     3555 2023-06-14 00:31:24.000000 yplib-1.0.8/yplib/file.py
--rw-rw-rw-   0        0        0    12648 2023-06-14 00:34:27.000000 yplib-1.0.8/yplib/index.py
--rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-1.0.8/yplib/line_stack_temp.py
--rw-rw-rw-   0        0        0     3495 2023-06-14 00:34:35.000000 yplib-1.0.8/yplib/test_my_fun.py
-drwxrwxrwx   0        0        0        0 2023-06-14 00:35:16.341235 yplib-1.0.8/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-14 00:35:16.000000 yplib-1.0.8/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-06-14 00:35:16.000000 yplib-1.0.8/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 00:35:16.000000 yplib-1.0.8/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 00:35:16.000000 yplib-1.0.8/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 00:56:21.202093 yplib-1.0.9/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-14 00:56:21.202093 yplib-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 00:56:21.202093 yplib-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-14 00:56:00.000000 yplib-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:56:21.199627 yplib-1.0.9/yplib/
+-rw-rw-rw-   0        0        0       87 2023-06-14 00:01:35.000000 yplib-1.0.9/yplib/__init__.py
+-rw-rw-rw-   0        0        0     3555 2023-06-14 00:31:24.000000 yplib-1.0.9/yplib/file.py
+-rw-rw-rw-   0        0        0    12664 2023-06-14 00:55:40.000000 yplib-1.0.9/yplib/index.py
+-rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-1.0.9/yplib/line_stack_temp.py
+-rw-rw-rw-   0        0        0     3517 2023-06-14 00:54:35.000000 yplib-1.0.9/yplib/test_my_fun.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:56:21.201665 yplib-1.0.9/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-14 00:56:21.000000 yplib-1.0.9/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-06-14 00:56:21.000000 yplib-1.0.9/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 00:56:21.000000 yplib-1.0.9/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 00:56:21.000000 yplib-1.0.9/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.0.8/LICENSE` & `yplib-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.0.8/PKG-INFO` & `yplib-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 1.0.8
+Version: 1.0.9
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-1.0.8/setup.py` & `yplib-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.0.8",
+  version="1.0.9",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-1.0.8/yplib/file.py` & `yplib-1.0.9/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.0.8/yplib/index.py` & `yplib-1.0.9/yplib/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,22 +31,22 @@
     return lo
 
 
 # 将 log 数据, 写入到文件
 def to_log_file(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
                 a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
     lo = to_log(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20)
-    to_txt([lo], datetime.today().strftime('%Y-%m-%d'), 'log', True)
+    to_txt([lo], datetime.today().strftime('%Y-%m-%d'), 'log', True, '.log')
 
 
 # 将 log 数据, 写入到固定文件中
 def to_log_txt(file_name, a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
                a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
     lo = to_log(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20)
-    to_txt([lo], file_name, 'log', True)
+    to_txt([lo], file_name, 'log', True, '.txt')
 
 
 # 将下划线命名转成驼峰命名
 # 例如 : user_id -> userId
 # 例如 : USER_ID -> userId
 def to_hump(a1=''):
     if a1 == '':
```

### Comparing `yplib-1.0.8/yplib/line_stack_temp.py` & `yplib-1.0.9/yplib/line_stack_temp.py`

 * *Files identical despite different names*

### Comparing `yplib-1.0.8/yplib/test_my_fun.py` & `yplib-1.0.9/yplib/test_my_fun.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 # hash.update(sign.encode('utf-8'))
 # data['sign'] = hash.hexdigest()
 #
 # print(data)
 
 
 
-# print(get_file_data_line(r'D:\notepad_file\202306\fasdfsadfaf.txt', 'a'))
+# print(get_file_data_line(r'D:\notepad_file\202306\fasdfsadfaf.txt', 'payout', from_last=False))
 
 # get_file_data_line(r'D:\notepad_file\202306', 'a')
 # get_file_by_content(r'D:\notepad_file\202306', 'a')
 # print(get_file(r'D:\notepad_file\202306', 'a'))
 # print(get_file(r'D:\notepad_file\202306'))
 # print(get_file())
 # print(os.path.abspath('.'))
```

### Comparing `yplib-1.0.8/yplib.egg-info/PKG-INFO` & `yplib-1.0.9/yplib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 1.0.8
+Version: 1.0.9
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

