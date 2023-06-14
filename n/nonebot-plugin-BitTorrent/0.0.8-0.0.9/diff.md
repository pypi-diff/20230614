# Comparing `tmp/nonebot_plugin_BitTorrent-0.0.8.tar.gz` & `tmp/nonebot_plugin_BitTorrent-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_BitTorrent-0.0.8.tar", last modified: Tue May 23 19:24:39 2023, max compression
+gzip compressed data, was "nonebot_plugin_BitTorrent-0.0.9.tar", last modified: Tue Jun  6 15:08:23 2023, max compression
```

## Comparing `nonebot_plugin_BitTorrent-0.0.8.tar` & `nonebot_plugin_BitTorrent-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 19:24:39.585351 nonebot_plugin_BitTorrent-0.0.8/
--rw-rw-rw-   0        0        0     1064 2022-06-17 16:08:47.000000 nonebot_plugin_BitTorrent-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      305 2023-05-23 19:24:39.584352 nonebot_plugin_BitTorrent-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1150 2022-06-23 16:37:02.000000 nonebot_plugin_BitTorrent-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 19:24:39.572568 nonebot_plugin_BitTorrent-0.0.8/nonebot_plugin_BitTorrent/
--rw-rw-rw-   0        0        0      502 2023-05-23 19:24:17.000000 nonebot_plugin_BitTorrent-0.0.8/nonebot_plugin_BitTorrent/__init__.py
--rw-rw-rw-   0        0        0     6162 2023-05-23 19:17:30.000000 nonebot_plugin_BitTorrent-0.0.8/nonebot_plugin_BitTorrent/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-23 19:24:39.582831 nonebot_plugin_BitTorrent-0.0.8/nonebot_plugin_BitTorrent.egg-info/
--rw-rw-rw-   0        0        0      305 2023-05-23 19:24:39.000000 nonebot_plugin_BitTorrent-0.0.8/nonebot_plugin_BitTorrent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-05-23 19:24:39.000000 nonebot_plugin_BitTorrent-0.0.8/nonebot_plugin_BitTorrent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 19:24:39.000000 nonebot_plugin_BitTorrent-0.0.8/nonebot_plugin_BitTorrent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-23 19:24:39.000000 nonebot_plugin_BitTorrent-0.0.8/nonebot_plugin_BitTorrent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-05-23 19:24:39.000000 nonebot_plugin_BitTorrent-0.0.8/nonebot_plugin_BitTorrent.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 19:24:39.585351 nonebot_plugin_BitTorrent-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      534 2023-05-23 19:23:27.000000 nonebot_plugin_BitTorrent-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 15:08:23.673879 nonebot_plugin_BitTorrent-0.0.9/
+-rw-rw-rw-   0        0        0     1064 2022-06-17 16:08:47.000000 nonebot_plugin_BitTorrent-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      305 2023-06-06 15:08:23.672878 nonebot_plugin_BitTorrent-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1150 2022-06-23 16:37:02.000000 nonebot_plugin_BitTorrent-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 15:08:23.665879 nonebot_plugin_BitTorrent-0.0.9/nonebot_plugin_BitTorrent/
+-rw-rw-rw-   0        0        0      643 2023-06-06 15:07:20.000000 nonebot_plugin_BitTorrent-0.0.9/nonebot_plugin_BitTorrent/__init__.py
+-rw-rw-rw-   0        0        0     6162 2023-06-06 15:06:47.000000 nonebot_plugin_BitTorrent-0.0.9/nonebot_plugin_BitTorrent/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-06 15:08:23.671878 nonebot_plugin_BitTorrent-0.0.9/nonebot_plugin_BitTorrent.egg-info/
+-rw-rw-rw-   0        0        0      305 2023-06-06 15:08:23.000000 nonebot_plugin_BitTorrent-0.0.9/nonebot_plugin_BitTorrent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-06-06 15:08:23.000000 nonebot_plugin_BitTorrent-0.0.9/nonebot_plugin_BitTorrent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 15:08:23.000000 nonebot_plugin_BitTorrent-0.0.9/nonebot_plugin_BitTorrent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-06 15:08:23.000000 nonebot_plugin_BitTorrent-0.0.9/nonebot_plugin_BitTorrent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-06-06 15:08:23.000000 nonebot_plugin_BitTorrent-0.0.9/nonebot_plugin_BitTorrent.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 15:08:23.673879 nonebot_plugin_BitTorrent-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      534 2023-06-06 15:08:14.000000 nonebot_plugin_BitTorrent-0.0.9/setup.py
```

### Comparing `nonebot_plugin_BitTorrent-0.0.8/LICENSE` & `nonebot_plugin_BitTorrent-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_BitTorrent-0.0.8/README.md` & `nonebot_plugin_BitTorrent-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_BitTorrent-0.0.8/nonebot_plugin_BitTorrent/utils.py` & `nonebot_plugin_BitTorrent-0.0.9/nonebot_plugin_BitTorrent/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_BitTorrent-0.0.8/setup.py` & `nonebot_plugin_BitTorrent-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 
 from setuptools import find_packages, setup
 name = 'nonebot_plugin_BitTorrent'
 
 setup(
     name=name,  
-    version='0.0.8',
+    version='0.0.9',
     author="Special-Week",
     author_email='2749903559@qq.com',
     description="encapsulate logger",
     python_requires=">=3.8.0",
     packages=find_packages(),
     long_description="nonebot2磁力搜索插件",
     url="https://github.com/Special-Week/nonebot_plugin_BitTorrent",
```

