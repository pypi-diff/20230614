# Comparing `tmp/yplib-1.0.6.tar.gz` & `tmp/yplib-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.0.6.tar", last modified: Wed Jun 14 00:04:33 2023, max compression
+gzip compressed data, was "dist\yplib-1.0.7.tar", last modified: Wed Jun 14 00:32:22 2023, max compression
```

## Comparing `yplib-1.0.6.tar` & `yplib-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 00:04:33.254350 yplib-1.0.6/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-14 00:04:33.253990 yplib-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 00:04:33.254350 yplib-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-14 00:01:40.000000 yplib-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 00:04:33.250644 yplib-1.0.6/yplib/
--rw-rw-rw-   0        0        0       87 2023-06-14 00:01:35.000000 yplib-1.0.6/yplib/__init__.py
--rw-rw-rw-   0        0        0     2815 2023-06-13 06:37:43.000000 yplib-1.0.6/yplib/file.py
--rw-rw-rw-   0        0        0    12648 2023-06-13 07:01:18.000000 yplib-1.0.6/yplib/index.py
--rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-1.0.6/yplib/line_stack_temp.py
--rw-rw-rw-   0        0        0     3362 2023-06-14 00:00:47.000000 yplib-1.0.6/yplib/test_my_fun.py
-drwxrwxrwx   0        0        0        0 2023-06-14 00:04:33.253016 yplib-1.0.6/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-14 00:04:33.000000 yplib-1.0.6/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-06-14 00:04:33.000000 yplib-1.0.6/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 00:04:33.000000 yplib-1.0.6/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 00:04:33.000000 yplib-1.0.6/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 00:32:22.882244 yplib-1.0.7/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-14 00:32:22.881595 yplib-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-1.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 00:32:22.882244 yplib-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-14 00:32:09.000000 yplib-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:32:22.878165 yplib-1.0.7/yplib/
+-rw-rw-rw-   0        0        0       87 2023-06-14 00:01:35.000000 yplib-1.0.7/yplib/__init__.py
+-rw-rw-rw-   0        0        0     3555 2023-06-14 00:31:24.000000 yplib-1.0.7/yplib/file.py
+-rw-rw-rw-   0        0        0    12559 2023-06-14 00:31:06.000000 yplib-1.0.7/yplib/index.py
+-rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-1.0.7/yplib/line_stack_temp.py
+-rw-rw-rw-   0        0        0     3495 2023-06-14 00:31:27.000000 yplib-1.0.7/yplib/test_my_fun.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:32:22.881019 yplib-1.0.7/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-14 00:32:22.000000 yplib-1.0.7/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-06-14 00:32:22.000000 yplib-1.0.7/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 00:32:22.000000 yplib-1.0.7/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 00:32:22.000000 yplib-1.0.7/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.0.6/LICENSE` & `yplib-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.0.6/PKG-INFO` & `yplib-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 1.0.6
+Version: 1.0.7
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-1.0.6/setup.py` & `yplib-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.0.6",
+  version="1.0.7",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-1.0.6/yplib/file.py` & `yplib-1.0.7/yplib/file.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,23 +14,45 @@
 
 
 # 是否包含指定的文件
 def contain_file(file_path=None, prefix=None, contain=None, suffix=None):
     return len(get_file(file_path, prefix, contain, suffix)) > 0
 
 
+# 在指定的文件夹中查找包含指定字符串的数据
+# file_path : 文件路径
+# find_str : 查找的字符串
+# from_last : 是否从文件的最后开始查找
+def get_file_data_line(file_path=None, find_str='find_str', from_last=True):
+    file_list = get_file(file_path)
+    for one_file in file_list:
+        one_list = to_list(one_file)
+        index = 0
+        if from_last:
+            index = len(one_list) - 1
+        while -1 < index < len(one_list):
+            one_line = one_list[index]
+            if from_last:
+                index -= 1
+            else:
+                index += 1
+            if one_line.find(find_str) > -1:
+                return one_line
+    return None
+
+
 # 查询指定文件夹下面的所有的文件信息, 也可以是指定的文件
 def get_file_all(file_path, list_data, prefix=None, contain=None, suffix=None):
     if os.path.isdir(file_path):
-        for root, dirnames, filenames in os.walk(file_path):
-            for filename in filenames:
-                if get_file_check(filename, prefix, contain, suffix):
-                    list_data.append(os.path.join(root, filename))
-            for dirname in dirnames:
-                get_file_all(os.path.join(root, dirname), list_data)
+        for root, dir_names, file_names in os.walk(file_path):
+            for file_name in file_names:
+                if get_file_check(file_name, prefix, contain, suffix):
+                    list_data.append(os.path.join(root, file_name))
+            for dir_name in dir_names:
+                get_file_all(os.path.join(root, dir_name), list_data)
     elif get_file_check(file_path, prefix, contain, suffix):
         list_data.append(file_path)
 
 
 # 检查文件是否符合要求
 def get_file_check(file_name='', prefix=None, contain=None, suffix=None):
     if file_name is None or file_name == '':
@@ -54,15 +76,15 @@
         else:
             s = False
     return p and c and s
 
 
 # 检查文件内容是否包含指定的字符串
 # 慎用,否则, 执行时间可能比较长
-def get_file_by_content(file_path='', contain_txt=None, prefix=None, contain=None, suffix=None):
+def find_file_by_content(file_path='', contain_txt=None, prefix=None, contain=None, suffix=None):
     list_file = get_file(file_path, prefix, contain, suffix)
     if len(list_file) == 0:
         to_log(f'no_matched_file : {file_path} , {contain_txt} , {prefix} , {contain} , {suffix}')
         return False
     if contain_txt is None:
         to_log(list_file)
         return True
@@ -74,7 +96,8 @@
                     if line.endswith('\n'):
                         line = line[0:-1]
                     to_log(one_file, line)
         except Exception as e:
             to_log(one_file, e)
             continue
 
+
```

### Comparing `yplib-1.0.6/yplib/index.py` & `yplib-1.0.7/yplib/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,18 +267,15 @@
             row_data = []
             for j in range(len(rows)):
                 row_data.append(str(rows[j]).strip())
             data_list.append(row_data)
         return data_list
     # 普通文件的解析
     file = open(file_name, 'r', encoding='utf-8')
-    for line in file.readlines():
-        line = line.strip()
-        data_list.append(line)
-    return data_list
+    return file.readlines()
 
 
 def to_excel(list_data, file_name, file_path='excel'):
     file_name = str(file_name)
     while file_path.endswith('/'):
         file_path = file_path[0:-1]
     check_file(file_path)
```

### Comparing `yplib-1.0.6/yplib/line_stack_temp.py` & `yplib-1.0.7/yplib/line_stack_temp.py`

 * *Files identical despite different names*

### Comparing `yplib-1.0.6/yplib/test_my_fun.py` & `yplib-1.0.7/yplib/test_my_fun.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 #     y_list.append(n)
 # #
 # to_chart(x_list, y_list)
 #
 # to_txt_data(x_list, 'operate')
 # to_txt_data(y_list, 'operate')
 
-# log_to_file(1)
+# to_log_file(1)
 # log_to_file(12)
 # log_to_file('yangpu')
 # print(str_to_int('yan123gpu'))
 # print(str_to_float('yan123gpu'))
 # print(str_to_float('yan123g.12pu'))
 
 #
@@ -121,14 +121,17 @@
 # hash.update(sign.encode('utf-8'))
 # data['sign'] = hash.hexdigest()
 #
 # print(data)
 
 
 
+# print(get_file_data_line(r'D:\notepad_file\202306\fasdfsadfaf.txt', 'a'))
+
+# get_file_data_line(r'D:\notepad_file\202306', 'a')
 # get_file_by_content(r'D:\notepad_file\202306', 'a')
 # print(get_file(r'D:\notepad_file\202306', 'a'))
 # print(get_file(r'D:\notepad_file\202306'))
 # print(get_file())
 # print(os.path.abspath('.'))
```

### Comparing `yplib-1.0.6/yplib.egg-info/PKG-INFO` & `yplib-1.0.7/yplib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 1.0.6
+Version: 1.0.7
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

