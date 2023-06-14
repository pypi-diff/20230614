# Comparing `tmp/yplib-1.1.9.tar.gz` & `tmp/yplib-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.1.9.tar", last modified: Wed Jun 14 07:18:57 2023, max compression
+gzip compressed data, was "dist\yplib-1.2.0.tar", last modified: Wed Jun 14 08:21:14 2023, max compression
```

## Comparing `yplib-1.1.9.tar` & `yplib-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 07:18:57.007842 yplib-1.1.9/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.1.9/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-14 07:18:57.007842 yplib-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.1.9/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 07:18:57.008344 yplib-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-14 07:18:53.000000 yplib-1.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 07:18:57.005182 yplib-1.1.9/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.1.9/yplib/__init__.py
--rw-rw-rw-   0        0        0     8057 2023-06-14 07:18:46.000000 yplib-1.1.9/yplib/chart.py
--rw-rw-rw-   0        0        0     8327 2023-06-14 07:18:39.000000 yplib-1.1.9/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.1.9/yplib/file.py
--rw-rw-rw-   0        0        0    13492 2023-06-14 06:31:40.000000 yplib-1.1.9/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-14 07:18:57.006609 yplib-1.1.9/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-14 07:18:56.000000 yplib-1.1.9/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-14 07:18:56.000000 yplib-1.1.9/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 07:18:56.000000 yplib-1.1.9/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 07:18:56.000000 yplib-1.1.9/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 08:21:14.179980 yplib-1.2.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-14 08:21:14.179310 yplib-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 08:21:14.179980 yplib-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-14 08:21:00.000000 yplib-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:21:14.174676 yplib-1.2.0/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.2.0/yplib/__init__.py
+-rw-rw-rw-   0        0        0     8091 2023-06-14 08:20:27.000000 yplib-1.2.0/yplib/chart.py
+-rw-rw-rw-   0        0        0     8327 2023-06-14 07:18:39.000000 yplib-1.2.0/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.2.0/yplib/file.py
+-rw-rw-rw-   0        0        0    13492 2023-06-14 06:31:40.000000 yplib-1.2.0/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:21:14.177817 yplib-1.2.0/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-14 08:21:14.000000 yplib-1.2.0/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-14 08:21:14.000000 yplib-1.2.0/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 08:21:14.000000 yplib-1.2.0/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 08:21:14.000000 yplib-1.2.0/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.1.9/LICENSE` & `yplib-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.1.9/setup.py` & `yplib-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.1.9",
+  version="1.2.0",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.1.9/yplib/chart.py` & `yplib-1.2.0/yplib/chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,21 +175,21 @@
 # 数据 : data = [
 #        {x: "Search Engine", y: 1048 },
 #        {x: "Direct", y: 735 },
 #        {x: "Email", y:580 },
 #        {x: "Union Ads", y:484 },
 #        {x: "Video Ads", y:300 }
 #       }]
-def to_chart_bar(data_list, chart_name='bar'):
+def to_chart_bar(data_list, chart_name='bar', x_index=0, y_index=1):
     x_list = []
     y_list = []
     for one in data_list:
         if isinstance(one, list):
-            x_list.append(one[0])
-            y_list.append(one[1])
+            x_list.append(one[x_index])
+            y_list.append(one[y_index])
         else:
             x_list.append(one['x'])
             y_list.append(one['y'])
 
     insert_data_to_chart(html_data=bar_html(),
                          chart_name=chart_name,
                          x_list=x_list,
```

### Comparing `yplib-1.1.9/yplib/chart_html.py` & `yplib-1.2.0/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.1.9/yplib/file.py` & `yplib-1.2.0/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.1.9/yplib/index.py` & `yplib-1.2.0/yplib/index.py`

 * *Files identical despite different names*

