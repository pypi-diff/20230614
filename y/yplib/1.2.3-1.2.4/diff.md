# Comparing `tmp/yplib-1.2.3.tar.gz` & `tmp/yplib-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.2.3.tar", last modified: Wed Jun 14 08:33:29 2023, max compression
+gzip compressed data, was "dist\yplib-1.2.4.tar", last modified: Wed Jun 14 08:43:12 2023, max compression
```

## Comparing `yplib-1.2.3.tar` & `yplib-1.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 08:33:29.605534 yplib-1.2.3/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.2.3/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-14 08:33:29.605145 yplib-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.2.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 08:33:29.605733 yplib-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-14 08:33:09.000000 yplib-1.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:33:29.602213 yplib-1.2.3/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.2.3/yplib/__init__.py
--rw-rw-rw-   0        0        0     8101 2023-06-14 08:23:22.000000 yplib-1.2.3/yplib/chart.py
--rw-rw-rw-   0        0        0     8327 2023-06-14 07:18:39.000000 yplib-1.2.3/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.2.3/yplib/file.py
--rw-rw-rw-   0        0        0    13793 2023-06-14 08:33:02.000000 yplib-1.2.3/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:33:29.604540 yplib-1.2.3/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-14 08:33:29.000000 yplib-1.2.3/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-14 08:33:29.000000 yplib-1.2.3/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 08:33:29.000000 yplib-1.2.3/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 08:33:29.000000 yplib-1.2.3/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 08:43:12.266115 yplib-1.2.4/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-14 08:43:12.265996 yplib-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.2.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 08:43:12.266523 yplib-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-14 08:42:21.000000 yplib-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:43:12.262181 yplib-1.2.4/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.2.4/yplib/__init__.py
+-rw-rw-rw-   0        0        0     8101 2023-06-14 08:23:22.000000 yplib-1.2.4/yplib/chart.py
+-rw-rw-rw-   0        0        0     7978 2023-06-14 08:42:03.000000 yplib-1.2.4/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.2.4/yplib/file.py
+-rw-rw-rw-   0        0        0    13793 2023-06-14 08:33:02.000000 yplib-1.2.4/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:43:12.265283 yplib-1.2.4/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-14 08:43:12.000000 yplib-1.2.4/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-14 08:43:12.000000 yplib-1.2.4/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 08:43:12.000000 yplib-1.2.4/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 08:43:12.000000 yplib-1.2.4/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.2.3/LICENSE` & `yplib-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.2.3/setup.py` & `yplib-1.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.2.3",
+  version="1.2.4",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.2.3/yplib/chart.py` & `yplib-1.2.4/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.2.3/yplib/chart_html.py` & `yplib-1.2.4/yplib/chart_html.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,28 +74,20 @@
 
 
 # 折线图的 html 模板代码
 def line_area_html():
     option = '{' \
              '  tooltip: {' \
              '    trigger: "axis",' \
-             '    position: function (pt) {' \
-             '      return [pt[0], "10%"];' \
-             '    }' \
              '  },' \
              '  title: {' \
-             '    left: "center",' \
              '    text: "-chart_name-"' \
              '  },' \
              '  toolbox: {' \
              '    feature: {' \
-             '      dataZoom: {' \
-             '        yAxisIndex: "none"' \
-             '      },' \
-             '      restore: {},' \
              '      saveAsImage: {}' \
              '    }' \
              '  },' \
              '    grid: {' \
              '        left: "30px",' \
              '        right: "40px",' \
              '        bottom: "80px",' \
@@ -104,15 +96,14 @@
              '  xAxis: {' \
              '    type: "category",' \
              '    boundaryGap: false,' \
              '    data: -x_list-' \
              '  },' \
              '  yAxis: {' \
              '    type: "value",' \
-             '    boundaryGap: [0, "100%"]' \
              '  },' \
              '    dataZoom: [' \
              '        {' \
              '            show: true,' \
              '            realtime: true,' \
              '        },' \
              '        {' \
```

### Comparing `yplib-1.2.3/yplib/file.py` & `yplib-1.2.4/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.2.3/yplib/index.py` & `yplib-1.2.4/yplib/index.py`

 * *Files identical despite different names*

