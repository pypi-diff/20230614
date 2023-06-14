# Comparing `tmp/yplib-1.0.7.tar.gz` & `tmp/yplib-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.0.7.tar", last modified: Wed Jun 14 00:32:22 2023, max compression
+gzip compressed data, was "dist\yplib-1.0.8.tar", last modified: Wed Jun 14 00:35:16 2023, max compression
```

## Comparing `yplib-1.0.7.tar` & `yplib-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 00:32:22.882244 yplib-1.0.7/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.0.7/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-14 00:32:22.881595 yplib-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-1.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 00:32:22.882244 yplib-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-14 00:32:09.000000 yplib-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 00:32:22.878165 yplib-1.0.7/yplib/
--rw-rw-rw-   0        0        0       87 2023-06-14 00:01:35.000000 yplib-1.0.7/yplib/__init__.py
--rw-rw-rw-   0        0        0     3555 2023-06-14 00:31:24.000000 yplib-1.0.7/yplib/file.py
--rw-rw-rw-   0        0        0    12559 2023-06-14 00:31:06.000000 yplib-1.0.7/yplib/index.py
--rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-1.0.7/yplib/line_stack_temp.py
--rw-rw-rw-   0        0        0     3495 2023-06-14 00:31:27.000000 yplib-1.0.7/yplib/test_my_fun.py
-drwxrwxrwx   0        0        0        0 2023-06-14 00:32:22.881019 yplib-1.0.7/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-14 00:32:22.000000 yplib-1.0.7/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-06-14 00:32:22.000000 yplib-1.0.7/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 00:32:22.000000 yplib-1.0.7/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 00:32:22.000000 yplib-1.0.7/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 00:35:16.341557 yplib-1.0.8/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-14 00:35:16.341557 yplib-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-1.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 00:35:16.342358 yplib-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-14 00:34:41.000000 yplib-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:35:16.338777 yplib-1.0.8/yplib/
+-rw-rw-rw-   0        0        0       87 2023-06-14 00:01:35.000000 yplib-1.0.8/yplib/__init__.py
+-rw-rw-rw-   0        0        0     3555 2023-06-14 00:31:24.000000 yplib-1.0.8/yplib/file.py
+-rw-rw-rw-   0        0        0    12648 2023-06-14 00:34:27.000000 yplib-1.0.8/yplib/index.py
+-rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-1.0.8/yplib/line_stack_temp.py
+-rw-rw-rw-   0        0        0     3495 2023-06-14 00:34:35.000000 yplib-1.0.8/yplib/test_my_fun.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:35:16.341235 yplib-1.0.8/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-14 00:35:16.000000 yplib-1.0.8/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-06-14 00:35:16.000000 yplib-1.0.8/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 00:35:16.000000 yplib-1.0.8/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 00:35:16.000000 yplib-1.0.8/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.0.7/LICENSE` & `yplib-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.0.7/PKG-INFO` & `yplib-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 1.0.7
+Version: 1.0.8
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-1.0.7/setup.py` & `yplib-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.0.7",
+  version="1.0.8",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-1.0.7/yplib/file.py` & `yplib-1.0.8/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.0.7/yplib/index.py` & `yplib-1.0.8/yplib/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,15 +267,18 @@
             row_data = []
             for j in range(len(rows)):
                 row_data.append(str(rows[j]).strip())
             data_list.append(row_data)
         return data_list
     # 普通文件的解析
     file = open(file_name, 'r', encoding='utf-8')
-    return file.readlines()
+    for line in file.readlines():
+        line = line.strip()
+        data_list.append(line)
+    return data_list
 
 
 def to_excel(list_data, file_name, file_path='excel'):
     file_name = str(file_name)
     while file_path.endswith('/'):
         file_path = file_path[0:-1]
     check_file(file_path)
```

### Comparing `yplib-1.0.7/yplib/line_stack_temp.py` & `yplib-1.0.8/yplib/line_stack_temp.py`

 * *Files identical despite different names*

### Comparing `yplib-1.0.7/yplib/test_my_fun.py` & `yplib-1.0.8/yplib/test_my_fun.py`

 * *Files identical despite different names*

### Comparing `yplib-1.0.7/yplib.egg-info/PKG-INFO` & `yplib-1.0.8/yplib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 1.0.7
+Version: 1.0.8
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

