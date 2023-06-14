# Comparing `tmp/QBsimpleAPI-0.0.1.tar.gz` & `tmp/QBsimpleAPI-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QBsimpleAPI-0.0.1.tar", last modified: Wed Jun 14 21:24:37 2023, max compression
+gzip compressed data, was "QBsimpleAPI-0.0.2.tar", last modified: Wed Jun 14 21:45:35 2023, max compression
```

## Comparing `QBsimpleAPI-0.0.1.tar` & `QBsimpleAPI-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 21:24:37.059936 QBsimpleAPI-0.0.1/
--rw-rw-rw-   0        0        0     1084 2023-05-15 11:24:29.000000 QBsimpleAPI-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      480 2023-06-14 21:24:37.058949 QBsimpleAPI-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 21:24:37.044887 QBsimpleAPI-0.0.1/QBsimpleAPI.egg-info/
--rw-rw-rw-   0        0        0      480 2023-06-14 21:24:36.000000 QBsimpleAPI-0.0.1/QBsimpleAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-06-14 21:24:36.000000 QBsimpleAPI-0.0.1/QBsimpleAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 21:24:36.000000 QBsimpleAPI-0.0.1/QBsimpleAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-14 21:24:36.000000 QBsimpleAPI-0.0.1/QBsimpleAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-06-14 21:24:36.000000 QBsimpleAPI-0.0.1/QBsimpleAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       71 2023-05-15 11:24:29.000000 QBsimpleAPI-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 21:24:37.053936 QBsimpleAPI-0.0.1/qBittorrentWebUIsimpleAPI/
--rw-rw-rw-   0        0        0     3683 2023-06-06 07:35:08.000000 QBsimpleAPI-0.0.1/qBittorrentWebUIsimpleAPI/QBsimpleAPI.py
--rw-rw-rw-   0        0        0       26 2023-06-06 06:17:08.000000 QBsimpleAPI-0.0.1/qBittorrentWebUIsimpleAPI/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-14 21:24:37.059936 QBsimpleAPI-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      748 2023-06-14 21:22:57.000000 QBsimpleAPI-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 21:45:35.056671 QBsimpleAPI-0.0.2/
+-rw-rw-rw-   0        0        0     1084 2023-05-15 11:24:29.000000 QBsimpleAPI-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      464 2023-06-14 21:45:35.053661 QBsimpleAPI-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 21:45:35.034078 QBsimpleAPI-0.0.2/QBsimpleAPI/
+-rw-rw-rw-   0        0        0     3683 2023-06-06 07:35:08.000000 QBsimpleAPI-0.0.2/QBsimpleAPI/QBsimpleAPI.py
+-rw-rw-rw-   0        0        0       26 2023-06-06 06:17:08.000000 QBsimpleAPI-0.0.2/QBsimpleAPI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 21:45:35.050141 QBsimpleAPI-0.0.2/QBsimpleAPI.egg-info/
+-rw-rw-rw-   0        0        0      464 2023-06-14 21:45:34.000000 QBsimpleAPI-0.0.2/QBsimpleAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-06-14 21:45:34.000000 QBsimpleAPI-0.0.2/QBsimpleAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 21:45:34.000000 QBsimpleAPI-0.0.2/QBsimpleAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-14 21:45:34.000000 QBsimpleAPI-0.0.2/QBsimpleAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-14 21:45:34.000000 QBsimpleAPI-0.0.2/QBsimpleAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       55 2023-06-14 21:42:32.000000 QBsimpleAPI-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 21:45:35.057671 QBsimpleAPI-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      748 2023-06-14 21:44:50.000000 QBsimpleAPI-0.0.2/setup.py
```

### Comparing `QBsimpleAPI-0.0.1/LICENSE` & `QBsimpleAPI-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `QBsimpleAPI-0.0.1/qBittorrentWebUIsimpleAPI/QBsimpleAPI.py` & `QBsimpleAPI-0.0.2/QBsimpleAPI/QBsimpleAPI.py`

 * *Files identical despite different names*

### Comparing `QBsimpleAPI-0.0.1/setup.py` & `QBsimpleAPI-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r",encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 requirements = ["bs4","requests"] # 这里填依赖包信息
-VERSION="0.0.1"
+VERSION="0.0.2"
 
 setup(
     name="QBsimpleAPI",
     version=VERSION,
     author="slexce",
     author_email="sim69732@gmail.com",
     description="用于与qbittorrent webui通讯的简易api接口",
```

