# Comparing `tmp/clife_svc-1.13.tar.gz` & `tmp/clife_svc-1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\clife_svc-1.13.tar", last modified: Tue Jun 13 07:22:14 2023, max compression
+gzip compressed data, was "dist\clife_svc-1.14.tar", last modified: Wed Jun 14 01:54:50 2023, max compression
```

## Comparing `clife_svc-1.13.tar` & `clife_svc-1.14.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 07:22:14.000000 clife_svc-1.13/
-drwxrwxrwx   0        0        0        0 2023-06-13 07:22:14.000000 clife_svc-1.13/clife_svc/
--rw-rw-rw-   0        0        0    11780 2023-06-13 07:15:59.000000 clife_svc-1.13/clife_svc/application.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:22:14.000000 clife_svc-1.13/clife_svc/config/
--rw-rw-rw-   0        0        0     2078 2023-01-13 06:38:28.000000 clife_svc-1.13/clife_svc/config/configmap.py
--rw-rw-rw-   0        0        0     5582 2023-04-27 09:54:37.000000 clife_svc-1.13/clife_svc/config/disconf.py
--rw-rw-rw-   0        0        0        0 2023-01-13 06:18:27.000000 clife_svc-1.13/clife_svc/config/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:22:14.000000 clife_svc-1.13/clife_svc/errors/
--rw-rw-rw-   0        0        0     3589 2022-09-01 09:09:26.000000 clife_svc-1.13/clife_svc/errors/error_code.py
--rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.13/clife_svc/errors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:22:14.000000 clife_svc-1.13/clife_svc/libs/
--rw-rw-rw-   0        0        0      284 2021-12-23 09:51:21.000000 clife_svc-1.13/clife_svc/libs/context.py
--rw-rw-rw-   0        0        0    14499 2023-06-13 07:17:16.000000 clife_svc-1.13/clife_svc/libs/http_request.py
--rw-rw-rw-   0        0        0     2649 2023-05-15 11:06:18.000000 clife_svc-1.13/clife_svc/libs/log.py
--rw-rw-rw-   0        0        0     3510 2023-06-13 07:17:16.000000 clife_svc-1.13/clife_svc/libs/mq_handler.py
--rw-rw-rw-   0        0        0     1282 2023-01-13 07:00:07.000000 clife_svc-1.13/clife_svc/libs/utils.py
--rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.13/clife_svc/libs/__init__.py
--rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.13/clife_svc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:22:14.000000 clife_svc-1.13/clife_svc.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-13 07:22:14.000000 clife_svc-1.13/clife_svc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      420 2023-06-13 07:22:14.000000 clife_svc-1.13/clife_svc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      141 2023-06-13 07:22:14.000000 clife_svc-1.13/clife_svc.egg-info/requires.txt
--rw-rw-rw-   0        0        0      535 2023-06-13 07:22:14.000000 clife_svc-1.13/clife_svc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2023-06-13 07:22:14.000000 clife_svc-1.13/clife_svc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      420 2023-06-13 07:22:14.000000 clife_svc-1.13/PKG-INFO
--rw-rw-rw-   0        0        0       12 2021-12-20 11:08:06.000000 clife_svc-1.13/README.md
--rw-rw-rw-   0        0        0       42 2023-06-13 07:22:14.000000 clife_svc-1.13/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-06-13 07:19:32.000000 clife_svc-1.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:50.000000 clife_svc-1.14/
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:50.000000 clife_svc-1.14/clife_svc/
+-rw-rw-rw-   0        0        0    11780 2023-06-13 07:15:59.000000 clife_svc-1.14/clife_svc/application.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:50.000000 clife_svc-1.14/clife_svc/config/
+-rw-rw-rw-   0        0        0     2078 2023-01-13 06:38:28.000000 clife_svc-1.14/clife_svc/config/configmap.py
+-rw-rw-rw-   0        0        0     5582 2023-04-27 09:54:37.000000 clife_svc-1.14/clife_svc/config/disconf.py
+-rw-rw-rw-   0        0        0        0 2023-01-13 06:18:27.000000 clife_svc-1.14/clife_svc/config/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:50.000000 clife_svc-1.14/clife_svc/errors/
+-rw-rw-rw-   0        0        0     3589 2022-09-01 09:09:26.000000 clife_svc-1.14/clife_svc/errors/error_code.py
+-rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.14/clife_svc/errors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:50.000000 clife_svc-1.14/clife_svc/libs/
+-rw-rw-rw-   0        0        0      284 2021-12-23 09:51:21.000000 clife_svc-1.14/clife_svc/libs/context.py
+-rw-rw-rw-   0        0        0    14499 2023-06-13 07:17:16.000000 clife_svc-1.14/clife_svc/libs/http_request.py
+-rw-rw-rw-   0        0        0     2649 2023-05-15 11:06:18.000000 clife_svc-1.14/clife_svc/libs/log.py
+-rw-rw-rw-   0        0        0     3510 2023-06-13 07:17:16.000000 clife_svc-1.14/clife_svc/libs/mq_handler.py
+-rw-rw-rw-   0        0        0     1282 2023-01-13 07:00:07.000000 clife_svc-1.14/clife_svc/libs/utils.py
+-rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.14/clife_svc/libs/__init__.py
+-rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.14/clife_svc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:50.000000 clife_svc-1.14/clife_svc.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-14 01:54:50.000000 clife_svc-1.14/clife_svc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      420 2023-06-14 01:54:50.000000 clife_svc-1.14/clife_svc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      141 2023-06-14 01:54:50.000000 clife_svc-1.14/clife_svc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      535 2023-06-14 01:54:50.000000 clife_svc-1.14/clife_svc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2023-06-14 01:54:50.000000 clife_svc-1.14/clife_svc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      420 2023-06-14 01:54:50.000000 clife_svc-1.14/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2021-12-20 11:08:06.000000 clife_svc-1.14/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 01:54:50.000000 clife_svc-1.14/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-06-14 01:54:48.000000 clife_svc-1.14/setup.py
```

### Comparing `clife_svc-1.13/clife_svc/application.py` & `clife_svc-1.14/clife_svc/application.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.13/clife_svc/config/configmap.py` & `clife_svc-1.14/clife_svc/config/configmap.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.13/clife_svc/config/disconf.py` & `clife_svc-1.14/clife_svc/config/disconf.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.13/clife_svc/errors/error_code.py` & `clife_svc-1.14/clife_svc/errors/error_code.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.13/clife_svc/libs/http_request.py` & `clife_svc-1.14/clife_svc/libs/http_request.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.13/clife_svc/libs/log.py` & `clife_svc-1.14/clife_svc/libs/log.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.13/clife_svc/libs/mq_handler.py` & `clife_svc-1.14/clife_svc/libs/mq_handler.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.13/clife_svc/libs/utils.py` & `clife_svc-1.14/clife_svc/libs/utils.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.13/clife_svc.egg-info/SOURCES.txt` & `clife_svc-1.14/clife_svc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clife_svc-1.13/setup.py` & `clife_svc-1.14/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         if line.startswith('-e git+'):
             dependency_links.append(line.replace('-e ', ''))
         else:
             requirements.append(line)
 
 setuptools.setup(
     name='clife_svc',   # 需要打包的名字,即本模块要发布的名字
-    version='1.13',     # 版本
+    version='1.14',     # 版本
     author='andy.hu',  # 作者名
     author_email='hlp0@163.com',  # 作者邮件
     description='A module for service',   # 简要描述
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='',       # 项目地址,一般是代码托管的网站
     packages=setuptools.find_packages(),
```

