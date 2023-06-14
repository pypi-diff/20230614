# Comparing `tmp/cns-1.0.6.tar.gz` & `tmp/cns-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cns-1.0.6.tar", last modified: Wed Jun 14 08:24:22 2023, max compression
+gzip compressed data, was "cns-1.0.7.tar", last modified: Wed Jun 14 09:07:06 2023, max compression
```

## Comparing `cns-1.0.6.tar` & `cns-1.0.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 08:24:22.581443 cns-1.0.6/
--rw-rw-rw-   0        0        0      473 2023-06-14 03:11:25.000000 cns-1.0.6/LICENSE
--rw-rw-rw-   0        0        0       18 2023-06-14 08:00:32.000000 cns-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2133 2023-06-14 08:24:22.581443 cns-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1674 2023-06-14 08:19:36.000000 cns-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 08:24:22.581443 cns-1.0.6/cns/
--rw-rw-rw-   0        0        0    82944 2023-06-02 15:12:04.000000 cns-1.0.6/cns/DateTimeX.cp36-win32.pyd
--rw-rw-rw-   0        0        0    99840 2023-06-02 15:11:31.000000 cns-1.0.6/cns/DateTimeX.cp36-win_amd64.pyd
--rw-rw-rw-   0        0        0    88576 2023-06-02 15:13:09.000000 cns-1.0.6/cns/DateTimeX.cp39-win_amd64.pyd
--rw-rw-rw-   0        0        0   138752 2021-05-25 06:18:53.000000 cns-1.0.6/cns/SqlAdm.cp36-win_amd64.pyd
--rw-rw-rw-   0        0        0    53248 2020-11-17 06:13:06.000000 cns-1.0.6/cns/Xtoken.cp36-win_amd64.pyd
--rw-rw-rw-   0        0        0   162304 2021-05-14 09:02:50.000000 cns-1.0.6/cns/ZdyLogic.cp36-win_amd64.pyd
--rw-rw-rw-   0        0        0     1123 2023-06-14 08:14:59.000000 cns-1.0.6/cns/__init__.py
--rw-rw-rw-   0        0        0    68096 2020-08-06 08:59:36.000000 cns-1.0.6/cns/auto_dump.cp36-win_amd64.pyd
--rw-rw-rw-   0        0        0      714 2022-01-11 21:10:01.000000 cns-1.0.6/cns/dbcfg.py
--rw-rw-rw-   0        0        0    82432 2020-03-13 09:16:26.000000 cns-1.0.6/cns/lbsql.cp36-win_amd64.pyd
--rw-rw-rw-   0        0        0    52736 2020-08-27 02:31:12.000000 cns-1.0.6/cns/mailyanzheng.cp36-win_amd64.pyd
--rw-rw-rw-   0        0        0    88576 2023-04-17 01:55:50.000000 cns-1.0.6/cns/sql_str.cp36-win_amd64.pyd
--rw-rw-rw-   0        0        0    77312 2021-11-08 02:21:01.000000 cns-1.0.6/cns/str2sql.cp36-win_amd64.pyd
--rw-rw-rw-   0        0        0    81920 2020-08-27 07:07:44.000000 cns-1.0.6/cns/tpass.cp36-win_amd64.pyd
--rw-rw-rw-   0        0        0    62976 2020-09-15 11:09:19.000000 cns-1.0.6/cns/wxlogin.cp36-win_amd64.pyd
--rw-rw-rw-   0        0        0   148480 2022-12-28 07:55:05.000000 cns-1.0.6/cns/xdata.cp36-win_amd64.pyd
-drwxrwxrwx   0        0        0        0 2023-06-14 08:24:22.581443 cns-1.0.6/cns.egg-info/
--rw-rw-rw-   0        0        0     2133 2023-06-14 08:24:22.000000 cns-1.0.6/cns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      676 2023-06-14 08:24:22.000000 cns-1.0.6/cns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 08:24:22.000000 cns-1.0.6/cns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 08:24:22.000000 cns-1.0.6/cns.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-14 08:24:22.000000 cns-1.0.6/cns.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       75 2023-06-14 08:24:05.000000 cns-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 08:24:22.581443 cns-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      728 2023-06-14 08:24:02.000000 cns-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:24:22.581443 cns-1.0.6/tests/
--rw-rw-rw-   0        0        0     1347 2023-06-14 04:54:42.000000 cns-1.0.6/tests/TEST_DateTimeX.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:07:06.945825 cns-1.0.7/
+-rw-rw-rw-   0        0        0      473 2023-06-14 03:11:25.000000 cns-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0       18 2023-06-14 08:00:32.000000 cns-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2133 2023-06-14 09:07:06.945825 cns-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1674 2023-06-14 08:19:36.000000 cns-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 09:07:06.930200 cns-1.0.7/cns/
+-rw-rw-rw-   0        0        0    82944 2023-06-02 15:12:04.000000 cns-1.0.7/cns/DateTimeX.cp36-win32.pyd
+-rw-rw-rw-   0        0        0    99840 2023-06-02 15:11:31.000000 cns-1.0.7/cns/DateTimeX.cp36-win_amd64.pyd
+-rw-rw-rw-   0        0        0    88576 2023-06-02 15:13:09.000000 cns-1.0.7/cns/DateTimeX.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0   138752 2021-05-25 06:18:53.000000 cns-1.0.7/cns/SqlAdm.cp36-win_amd64.pyd
+-rw-rw-rw-   0        0        0    53248 2020-11-17 06:13:06.000000 cns-1.0.7/cns/Xtoken.cp36-win_amd64.pyd
+-rw-rw-rw-   0        0        0   162304 2021-05-14 09:02:50.000000 cns-1.0.7/cns/ZdyLogic.cp36-win_amd64.pyd
+-rw-rw-rw-   0        0        0     1123 2023-06-14 08:14:59.000000 cns-1.0.7/cns/__init__.py
+-rw-rw-rw-   0        0        0    68096 2020-08-06 08:59:36.000000 cns-1.0.7/cns/auto_dump.cp36-win_amd64.pyd
+-rw-rw-rw-   0        0        0      714 2022-01-11 21:10:01.000000 cns-1.0.7/cns/dbcfg.py
+-rw-rw-rw-   0        0        0    82432 2020-03-13 09:16:26.000000 cns-1.0.7/cns/lbsql.cp36-win_amd64.pyd
+-rw-rw-rw-   0        0        0    52736 2020-08-27 02:31:12.000000 cns-1.0.7/cns/mailyanzheng.cp36-win_amd64.pyd
+-rw-rw-rw-   0        0        0    88576 2023-04-17 01:55:50.000000 cns-1.0.7/cns/sql_str.cp36-win_amd64.pyd
+-rw-rw-rw-   0        0        0    77312 2021-11-08 02:21:01.000000 cns-1.0.7/cns/str2sql.cp36-win_amd64.pyd
+-rw-rw-rw-   0        0        0    81920 2020-08-27 07:07:44.000000 cns-1.0.7/cns/tpass.cp36-win_amd64.pyd
+-rw-rw-rw-   0        0        0    62976 2020-09-15 11:09:19.000000 cns-1.0.7/cns/wxlogin.cp36-win_amd64.pyd
+-rw-rw-rw-   0        0        0   148480 2022-12-28 07:55:05.000000 cns-1.0.7/cns/xdata.cp36-win_amd64.pyd
+drwxrwxrwx   0        0        0        0 2023-06-14 09:07:06.930200 cns-1.0.7/cns.egg-info/
+-rw-rw-rw-   0        0        0     2133 2023-06-14 09:07:06.000000 cns-1.0.7/cns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      676 2023-06-14 09:07:06.000000 cns-1.0.7/cns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 09:07:06.000000 cns-1.0.7/cns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-14 09:07:06.000000 cns-1.0.7/cns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-14 09:07:06.000000 cns-1.0.7/cns.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       75 2023-06-14 09:02:54.000000 cns-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 09:07:06.945825 cns-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      728 2023-06-14 09:02:40.000000 cns-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:07:06.930200 cns-1.0.7/tests/
+-rw-rw-rw-   0        0        0     1347 2023-06-14 04:54:42.000000 cns-1.0.7/tests/TEST_DateTimeX.py
```

### Comparing `cns-1.0.6/PKG-INFO` & `cns-1.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: cns
-Version: 1.0.6
+Version: 1.0.7
 Summary: 化繁为简工具包
 Home-page: https://cns.ink/example
 Author: rambo
 Author-email: 6566666@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.6,<=3.9
+Requires-Python: >=3.6,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cns
 常用的工具包，目前支持日期类 DateTimeX, 后续将不断增加更多
 
 ## 安装方法
```

### Comparing `cns-1.0.6/README.md` & `cns-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `cns-1.0.6/cns/__init__.py` & `cns-1.0.7/cns/__init__.py`

 * *Files identical despite different names*

### Comparing `cns-1.0.6/cns/dbcfg.py` & `cns-1.0.7/cns/dbcfg.py`

 * *Files identical despite different names*

### Comparing `cns-1.0.6/cns.egg-info/PKG-INFO` & `cns-1.0.7/cns.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: cns
-Version: 1.0.6
+Version: 1.0.7
 Summary: 化繁为简工具包
 Home-page: https://cns.ink/example
 Author: rambo
 Author-email: 6566666@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.6,<=3.9
+Requires-Python: >=3.6,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cns
 常用的工具包，目前支持日期类 DateTimeX, 后续将不断增加更多
 
 ## 安装方法
```

### Comparing `cns-1.0.6/cns.egg-info/SOURCES.txt` & `cns-1.0.7/cns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cns-1.0.6/setup.py` & `cns-1.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r',encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='cns',
-    version='1.0.6',
+    version='1.0.7',
     author='rambo',
     author_email='6566666@qq.com',
     description='化繁为简工具包',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://cns.ink/example',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: Microsoft :: Windows',
     ],
-    python_requires='>=3.6,<=3.9',
+    python_requires='>=3.6,<3.10',
     install_requires=[
         'dateutil',
     ],
 )
```

### Comparing `cns-1.0.6/tests/TEST_DateTimeX.py` & `cns-1.0.7/tests/TEST_DateTimeX.py`

 * *Files identical despite different names*

