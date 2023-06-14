# Comparing `tmp/yplib-1.1.5.tar.gz` & `tmp/yplib-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.1.5.tar", last modified: Wed Jun 14 06:35:32 2023, max compression
+gzip compressed data, was "dist\yplib-1.1.6.tar", last modified: Wed Jun 14 06:41:14 2023, max compression
```

## Comparing `yplib-1.1.5.tar` & `yplib-1.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 06:35:32.790868 yplib-1.1.5/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.1.5/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-14 06:35:32.790366 yplib-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 06:35:32.790868 yplib-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-14 06:35:21.000000 yplib-1.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:35:32.787382 yplib-1.1.5/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.1.5/yplib/__init__.py
--rw-rw-rw-   0        0        0     9104 2023-06-14 06:35:12.000000 yplib-1.1.5/yplib/chart.py
--rw-rw-rw-   0        0        0     5664 2023-06-14 06:14:34.000000 yplib-1.1.5/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.1.5/yplib/file.py
--rw-rw-rw-   0        0        0    13492 2023-06-14 06:31:40.000000 yplib-1.1.5/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:35:32.789626 yplib-1.1.5/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-14 06:35:32.000000 yplib-1.1.5/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-14 06:35:32.000000 yplib-1.1.5/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 06:35:32.000000 yplib-1.1.5/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 06:35:32.000000 yplib-1.1.5/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 06:41:14.282556 yplib-1.1.6/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-14 06:41:14.282438 yplib-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 06:41:14.282556 yplib-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-14 06:41:10.000000 yplib-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:41:14.279601 yplib-1.1.6/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.1.6/yplib/__init__.py
+-rw-rw-rw-   0        0        0     8855 2023-06-14 06:39:45.000000 yplib-1.1.6/yplib/chart.py
+-rw-rw-rw-   0        0        0     5804 2023-06-14 06:40:22.000000 yplib-1.1.6/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.1.6/yplib/file.py
+-rw-rw-rw-   0        0        0    13492 2023-06-14 06:31:40.000000 yplib-1.1.6/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:41:14.281942 yplib-1.1.6/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-14 06:41:14.000000 yplib-1.1.6/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-14 06:41:14.000000 yplib-1.1.6/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 06:41:14.000000 yplib-1.1.6/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 06:41:14.000000 yplib-1.1.6/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.1.5/LICENSE` & `yplib-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.1.5/setup.py` & `yplib-1.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.1.5",
+  version="1.1.6",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.1.5/yplib/chart.py` & `yplib-1.1.6/yplib/chart.py`

 * *Files 5% similar despite different names*

```diff
@@ -129,39 +129,33 @@
 #        {x: "Search Engine", y: 1048 },
 #        {x: "Direct", y: 735 },
 #        {x: "Email", y:580 },
 #        {x: "Union Ads", y:484 },
 #        {x: "Video Ads", y:300 }
 #       }]
 def to_chart_bar(data_list, chart_name='bar'):
-    html_list_one = bar_html()
-    x_list_html = '-x_list-'
-    y_list_html = '-y_list-'
-    x_html_list = []
-    y_html_list = []
+    x_list = []
+    y_list = []
     for one in data_list:
         if isinstance(one, list):
-            x_html_list.append(one[0])
-            y_html_list.append(one[1])
+            x_list.append(one[0])
+            y_list.append(one[1])
         else:
-            x_html_list.append(one['x'])
-            y_html_list.append(one['y'])
+            x_list.append(one['x'])
+            y_list.append(one['y'])
 
-    if x_list_html in html_list_one:
-        html_list_one = html_list_one.replace(x_list_html, str(x_html_list))
-    if y_list_html in html_list_one:
-        html_list_one = html_list_one.replace(y_list_html, str(y_html_list))
-    to_txt([html_list_one], str(chart_name), 'html', False, '.html')
+    insert_data_to_chart(html_data=bar_html(),
+                         chart_name=chart_name,
+                         x_list=x_list,
+                         y_list=y_list)
 
-
-#
 # data = []
 # # for i in range(10):
 # #     data.append([uuid_random(), int(random.uniform(0, 1000))])
-# for i in range(10):
+# for i in range(100):
 #     one = {}
 #     one['x'] = uuid_random()
 #     one['y'] = int(random.uniform(0, 1000))
 #     data.append(one)
 #
 # to_chart_bar(data)
 #
```

### Comparing `yplib-1.1.5/yplib/chart_html.py` & `yplib-1.1.6/yplib/chart_html.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,17 +133,20 @@
              '  },' \
              '  tooltip: {' \
              '    trigger: "axis",' \
              '    axisPointer: {' \
              '      type: "shadow"' \
              '    }' \
              '  },' \
-             '  grid: {' \
-             '    bottom: 90' \
-             '  },' \
+             '    grid: {' \
+             '        left: "30px",' \
+             '        right: "40px",' \
+             '        bottom: "80px",' \
+             '        containLabel: true,' \
+             '    },' \
              '  dataZoom: [' \
              '    {' \
              '      type: "inside"' \
              '    },' \
              '    {' \
              '      type: "slider"' \
              '    }' \
```

### Comparing `yplib-1.1.5/yplib/file.py` & `yplib-1.1.6/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.1.5/yplib/index.py` & `yplib-1.1.6/yplib/index.py`

 * *Files identical despite different names*

