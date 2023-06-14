# Comparing `tmp/yplib-1.1.2.tar.gz` & `tmp/yplib-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.1.2.tar", last modified: Wed Jun 14 02:29:33 2023, max compression
+gzip compressed data, was "dist\yplib-1.1.3.tar", last modified: Wed Jun 14 02:50:52 2023, max compression
```

## Comparing `yplib-1.1.2.tar` & `yplib-1.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 02:29:33.728799 yplib-1.1.2/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.1.2/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-14 02:29:33.728531 yplib-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-1.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 02:29:33.729019 yplib-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-14 02:29:11.000000 yplib-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:29:33.724905 yplib-1.1.2/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.1.2/yplib/__init__.py
--rw-rw-rw-   0        0        0     7365 2023-06-14 02:28:55.000000 yplib-1.1.2/yplib/chart.py
--rw-rw-rw-   0        0        0     3779 2023-06-14 02:06:14.000000 yplib-1.1.2/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.1.2/yplib/file.py
--rw-rw-rw-   0        0        0    13524 2023-06-14 02:28:45.000000 yplib-1.1.2/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:29:33.726958 yplib-1.1.2/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-14 02:29:33.000000 yplib-1.1.2/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-14 02:29:33.000000 yplib-1.1.2/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 02:29:33.000000 yplib-1.1.2/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 02:29:33.000000 yplib-1.1.2/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 02:50:52.908613 yplib-1.1.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-14 02:50:52.908613 yplib-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 02:50:52.908613 yplib-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-14 02:50:33.000000 yplib-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:50:52.905450 yplib-1.1.3/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.1.3/yplib/__init__.py
+-rw-rw-rw-   0        0        0     8409 2023-06-14 02:42:42.000000 yplib-1.1.3/yplib/chart.py
+-rw-rw-rw-   0        0        0     5523 2023-06-14 02:48:14.000000 yplib-1.1.3/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.1.3/yplib/file.py
+-rw-rw-rw-   0        0        0    13524 2023-06-14 02:28:45.000000 yplib-1.1.3/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:50:52.908042 yplib-1.1.3/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-14 02:50:52.000000 yplib-1.1.3/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-14 02:50:52.000000 yplib-1.1.3/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 02:50:52.000000 yplib-1.1.3/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 02:50:52.000000 yplib-1.1.3/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.1.2/LICENSE` & `yplib-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.1.2/setup.py` & `yplib-1.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.1.2",
+  version="1.1.3",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
-  url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
   classifiers=[
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   ],
 )
```

### Comparing `yplib-1.1.2/yplib/chart.py` & `yplib-1.1.3/yplib/chart.py`

 * *Files 12% similar despite different names*

```diff
@@ -98,14 +98,46 @@
     else:
         data_html_list = data_list
 
     if data_html in html_list_one:
         html_list_one = html_list_one.replace(data_html, str(data_html_list))
     to_txt([html_list_one], str(chart_name), 'html', False, '.html')
 
+
+# 将数据整理成柱状图
+# 数据 : data = [
+#         { value: 1048, name: "Search Engine" },
+#         { value: 735, name: "Direct" },
+#         { value: 580, name: "Email" },
+#         { value: 484, name: "Union Ads" },
+#         { value: 300, name: "Video Ads" }
+#       ]
+# 或者
+# 数据 : data = [
+#         [ "Search Engine", 1048 ],
+#         [ "Direct", 735 ],
+#         [ "Email",580 ],
+#         [ "Union Ads",484 ],
+#         [ "Video Ads",300 ]
+#       ]
+def to_chart_bar(data_list, chart_name='bar'):
+    html_list_one = pie_html()
+    data_html = '-data-'
+    data_html_list = []
+    if isinstance(data_list[0], list):
+        for one in data_list:
+            if isinstance(one, list):
+                data_html_list.append({'name': one[0], 'value': one[1]})
+    else:
+        data_html_list = data_list
+
+    if data_html in html_list_one:
+        html_list_one = html_list_one.replace(data_html, str(data_html_list))
+    to_txt([html_list_one], str(chart_name), 'html', False, '.html')
+
 #
 # data = []
 # # for i in range(10):
 # #     data.append([uuid_random(), int(random.uniform(0, 1000))])
 # for i in range(10):
 #     one = {}
 #     one['name'] = uuid_random()
```

### Comparing `yplib-1.1.2/yplib/file.py` & `yplib-1.1.3/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.1.2/yplib/index.py` & `yplib-1.1.3/yplib/index.py`

 * *Files identical despite different names*

