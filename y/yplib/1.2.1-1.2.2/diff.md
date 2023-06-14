# Comparing `tmp/yplib-1.2.1.tar.gz` & `tmp/yplib-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.2.1.tar", last modified: Wed Jun 14 08:23:48 2023, max compression
+gzip compressed data, was "dist\yplib-1.2.2.tar", last modified: Wed Jun 14 08:29:21 2023, max compression
```

## Comparing `yplib-1.2.1.tar` & `yplib-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 08:23:48.785631 yplib-1.2.1/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.2.1/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-14 08:23:48.785631 yplib-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 08:23:48.786443 yplib-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-14 08:23:33.000000 yplib-1.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:23:48.781960 yplib-1.2.1/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.2.1/yplib/__init__.py
--rw-rw-rw-   0        0        0     8101 2023-06-14 08:23:22.000000 yplib-1.2.1/yplib/chart.py
--rw-rw-rw-   0        0        0     8327 2023-06-14 07:18:39.000000 yplib-1.2.1/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.2.1/yplib/file.py
--rw-rw-rw-   0        0        0    13492 2023-06-14 06:31:40.000000 yplib-1.2.1/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:23:48.784571 yplib-1.2.1/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-14 08:23:48.000000 yplib-1.2.1/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-14 08:23:48.000000 yplib-1.2.1/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 08:23:48.000000 yplib-1.2.1/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 08:23:48.000000 yplib-1.2.1/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 08:29:21.913043 yplib-1.2.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-14 08:29:21.912541 yplib-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 08:29:21.913043 yplib-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-14 08:27:19.000000 yplib-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:29:21.909677 yplib-1.2.2/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.2.2/yplib/__init__.py
+-rw-rw-rw-   0        0        0     8101 2023-06-14 08:23:22.000000 yplib-1.2.2/yplib/chart.py
+-rw-rw-rw-   0        0        0     8327 2023-06-14 07:18:39.000000 yplib-1.2.2/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.2.2/yplib/file.py
+-rw-rw-rw-   0        0        0    13785 2023-06-14 08:27:02.000000 yplib-1.2.2/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:29:21.911693 yplib-1.2.2/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-14 08:29:21.000000 yplib-1.2.2/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-14 08:29:21.000000 yplib-1.2.2/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 08:29:21.000000 yplib-1.2.2/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 08:29:21.000000 yplib-1.2.2/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.2.1/LICENSE` & `yplib-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.2.1/setup.py` & `yplib-1.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.2.1",
+  version="1.2.2",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.2.1/yplib/chart.py` & `yplib-1.2.2/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.2.1/yplib/chart_html.py` & `yplib-1.2.2/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.2.1/yplib/file.py` & `yplib-1.2.2/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.2.1/yplib/index.py` & `yplib-1.2.2/yplib/index.py`

 * *Files 3% similar despite different names*

```diff
@@ -195,14 +195,19 @@
                                       weeks=weeks)
 
 
 def to_date(s=None):
     return to_datetime(s, True)[0:10]
 
 
+def date_add(s=None, days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0):
+    return datetime_add(s=s, days=days, seconds=seconds, microseconds=microseconds, milliseconds=milliseconds, minutes=minutes, hours=hours,
+                        weeks=weeks)[0:10]
+
+
 # 将 list 中的数据以 json 或者基本类型的形式写入到文件中
 # list_data : 数组数据, 也可以不是数组
 # file_name : 文件名
 # fixed_name : 是否固定文件名
 # file_path : 文件路径
 def to_txt(list_data, file_name='txt', file_path='txt', fixed_name=False, suffix='.txt'):
     file_name = str(file_name)
```

