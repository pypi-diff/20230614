# Comparing `tmp/betweens-1.2.1rc3.tar.gz` & `tmp/betweens-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betweens-1.2.1rc3.tar", last modified: Wed Jun 14 08:07:28 2023, max compression
+gzip compressed data, was "betweens-1.2.2.tar", last modified: Wed Jun 14 08:16:01 2023, max compression
```

## Comparing `betweens-1.2.1rc3.tar` & `betweens-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 08:07:28.505014 betweens-1.2.1rc3/
--rw-rw-rw-   0        0        0     1091 2023-05-03 12:21:47.000000 betweens-1.2.1rc3/LICENSE
--rw-rw-rw-   0        0        0       13 2023-05-04 10:16:44.000000 betweens-1.2.1rc3/MANIFEST.in
--rw-rw-rw-   0        0        0     1780 2023-06-14 08:07:28.505014 betweens-1.2.1rc3/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-05-08 10:56:31.000000 betweens-1.2.1rc3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 08:07:28.505014 betweens-1.2.1rc3/betweens/
--rw-rw-rw-   0        0        0      311 2023-05-05 10:33:20.000000 betweens-1.2.1rc3/betweens/__init__.py
--rw-rw-rw-   0        0        0     3905 2023-05-08 10:52:21.000000 betweens-1.2.1rc3/betweens/betweens.py
--rw-rw-rw-   0        0        0      128 2023-05-05 10:18:08.000000 betweens-1.2.1rc3/betweens/version.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:07:28.505014 betweens-1.2.1rc3/betweens.egg-info/
--rw-rw-rw-   0        0        0     1780 2023-06-14 08:07:28.000000 betweens-1.2.1rc3/betweens.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-06-14 08:07:28.000000 betweens-1.2.1rc3/betweens.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 08:07:28.000000 betweens-1.2.1rc3/betweens.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 08:07:28.000000 betweens-1.2.1rc3/betweens.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      670 2023-06-14 08:05:13.000000 betweens-1.2.1rc3/new.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 08:07:28.505014 betweens-1.2.1rc3/setup.cfg
--rw-rw-rw-   0        0        0     2240 2023-06-14 08:07:15.000000 betweens-1.2.1rc3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:16:01.677154 betweens-1.2.2/
+-rw-rw-rw-   0        0        0     1091 2023-05-03 12:21:47.000000 betweens-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0       13 2023-05-04 10:16:44.000000 betweens-1.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1777 2023-06-14 08:16:01.677154 betweens-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-05-08 10:56:31.000000 betweens-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 08:16:01.661518 betweens-1.2.2/betweens/
+-rw-rw-rw-   0        0        0      311 2023-05-05 10:33:20.000000 betweens-1.2.2/betweens/__init__.py
+-rw-rw-rw-   0        0        0     3905 2023-05-08 10:52:21.000000 betweens-1.2.2/betweens/betweens.py
+-rw-rw-rw-   0        0        0      128 2023-05-05 10:18:08.000000 betweens-1.2.2/betweens/version.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:16:01.677154 betweens-1.2.2/betweens.egg-info/
+-rw-rw-rw-   0        0        0     1777 2023-06-14 08:16:01.000000 betweens-1.2.2/betweens.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-06-14 08:16:01.000000 betweens-1.2.2/betweens.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 08:16:01.000000 betweens-1.2.2/betweens.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-14 08:16:01.000000 betweens-1.2.2/betweens.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      697 2023-06-14 08:14:54.000000 betweens-1.2.2/new.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 08:16:01.677154 betweens-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     2237 2023-06-14 08:15:48.000000 betweens-1.2.2/setup.py
```

### Comparing `betweens-1.2.1rc3/LICENSE` & `betweens-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `betweens-1.2.1rc3/PKG-INFO` & `betweens-1.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betweens
-Version: 1.2.1rc3
+Version: 1.2.2
 Summary: 0.0.1:
 Author: yuanbaoge
 Author-email: yuanbaoge@outlook.com
 Keywords: pimm source manager
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `betweens-1.2.1rc3/betweens/betweens.py` & `betweens-1.2.2/betweens/betweens.py`

 * *Files identical despite different names*

### Comparing `betweens-1.2.1rc3/betweens.egg-info/PKG-INFO` & `betweens-1.2.2/betweens.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betweens
-Version: 1.2.1rc3
+Version: 1.2.2
 Summary: 0.0.1:
 Author: yuanbaoge
 Author-email: yuanbaoge@outlook.com
 Keywords: pimm source manager
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `betweens-1.2.1rc3/new.txt` & `betweens-1.2.2/new.txt`

 * *Files 9% similar despite different names*

```diff
@@ -45,12 +45,15 @@
 
 1.1.2:
 UpDate File.
 
 1.2.0:
 Optimized setup.py
 
-1.2.1.dev1:
+1.2.1rc1-1.2.1rc3:
 Optimized setup.py and README.md
 
 1.2.1:
-UpDate File.
+UpDate File.
+
+1.2.2:
+Nothing.
```

### Comparing `betweens-1.2.1rc3/setup.py` & `betweens-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 with open(path.join(this_directory, 'new.txt'), encoding='utf-8') as f:
     description = f.read()
 
 setup(name='betweens', # 包名称
       packages=find_packages(), # 需要处理的包目录
-      version='1.2.1rc3', # 版本
+      version='1.2.2', # 版本
       classifiers=[
           'Development Status :: 4 - Beta',
           'License :: OSI Approved :: MIT License',
           'Programming Language :: Python', 'Intended Audience :: Developers',
           'Operating System :: OS Independent',
           'License :: OSI Approved :: Common Public License',
           'License :: OSI Approved :: W3C License',
```

