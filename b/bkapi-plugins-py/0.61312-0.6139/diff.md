# Comparing `tmp/bkapi-plugins-py-0.61312.tar.gz` & `tmp/bkapi-plugins-py-0.6139.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bkapi-plugins-py-0.61312.tar", last modified: Tue Jun 13 06:12:39 2023, max compression
+gzip compressed data, was "bkapi-plugins-py-0.6139.tar", last modified: Tue Jun 13 11:35:50 2023, max compression
```

## Comparing `bkapi-plugins-py-0.61312.tar` & `bkapi-plugins-py-0.6139.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 06:12:39.503454 bkapi-plugins-py-0.61312/
--rw-rw-rw-   0        0        0       39 2023-04-17 10:01:55.000000 bkapi-plugins-py-0.61312/MANIFEST.in
--rw-rw-rw-   0        0        0      259 2023-06-13 06:12:39.503454 bkapi-plugins-py-0.61312/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 06:12:39.484302 bkapi-plugins-py-0.61312/bkapi_plugins/
-drwxrwxrwx   0        0        0        0 2023-06-13 06:12:39.495706 bkapi-plugins-py-0.61312/bkapi_plugins/files/
--rw-rw-rw-   0        0        0      336 2023-06-13 06:12:33.000000 bkapi-plugins-py-0.61312/bkapi_plugins/files/node.sh
-drwxrwxrwx   0        0        0        0 2023-06-13 06:12:39.502159 bkapi-plugins-py-0.61312/bkapi_plugins_py.egg-info/
--rw-rw-rw-   0        0        0      259 2023-06-13 06:12:39.000000 bkapi-plugins-py-0.61312/bkapi_plugins_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-06-13 06:12:39.000000 bkapi-plugins-py-0.61312/bkapi_plugins_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 06:12:39.000000 bkapi-plugins-py-0.61312/bkapi_plugins_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 06:12:39.000000 bkapi-plugins-py-0.61312/bkapi_plugins_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 06:12:39.504447 bkapi-plugins-py-0.61312/setup.cfg
--rw-rw-rw-   0        0        0      892 2023-06-13 06:12:32.000000 bkapi-plugins-py-0.61312/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 11:35:50.348823 bkapi-plugins-py-0.6139/
+-rw-rw-rw-   0        0        0       39 2023-04-17 10:01:55.000000 bkapi-plugins-py-0.6139/MANIFEST.in
+-rw-rw-rw-   0        0        0      258 2023-06-13 11:35:50.349319 bkapi-plugins-py-0.6139/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-13 11:35:50.313813 bkapi-plugins-py-0.6139/bkapi_plugins/
+drwxrwxrwx   0        0        0        0 2023-06-13 11:35:50.327227 bkapi-plugins-py-0.6139/bkapi_plugins/files/
+-rw-rw-rw-   0        0        0  3450384 2023-06-12 11:54:31.000000 bkapi-plugins-py-0.6139/bkapi_plugins/files/nacos-k8s-1.0.0.tar.gz
+drwxrwxrwx   0        0        0        0 2023-06-13 11:35:50.347332 bkapi-plugins-py-0.6139/bkapi_plugins_py.egg-info/
+-rw-rw-rw-   0        0        0      258 2023-06-13 11:35:50.000000 bkapi-plugins-py-0.6139/bkapi_plugins_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-06-13 11:35:50.000000 bkapi-plugins-py-0.6139/bkapi_plugins_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 11:35:50.000000 bkapi-plugins-py-0.6139/bkapi_plugins_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 11:35:50.000000 bkapi-plugins-py-0.6139/bkapi_plugins_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 11:35:50.351805 bkapi-plugins-py-0.6139/setup.cfg
+-rw-rw-rw-   0        0        0      891 2023-06-13 11:35:44.000000 bkapi-plugins-py-0.6139/setup.py
```

### Comparing `bkapi-plugins-py-0.61312/setup.py` & `bkapi-plugins-py-0.6139/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 readme = ''
 
 setup(
     description='',
     long_description=readme,
     name='bkapi-plugins-py', # 包的名字
-    version='0.61312', # 版本号每次打包完要改一下
+    version='0.6139', # 版本号每次打包完要改一下
     python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*',
     author='fadewalk',
     license='Apach License 2.0',
     # packages=find_packages(),
     # namespace_packages=['bkapi_plugins'],
     package_dir={'': '.'},
     include_package_data=True,
```

