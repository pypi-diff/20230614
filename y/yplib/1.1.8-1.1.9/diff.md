# Comparing `tmp/yplib-1.1.8.tar.gz` & `tmp/yplib-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.1.8.tar", last modified: Wed Jun 14 07:15:00 2023, max compression
+gzip compressed data, was "dist\yplib-1.1.9.tar", last modified: Wed Jun 14 07:18:57 2023, max compression
```

## Comparing `yplib-1.1.8.tar` & `yplib-1.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 07:15:00.159998 yplib-1.1.8/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.1.8/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-14 07:15:00.159998 yplib-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.1.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 07:15:00.159998 yplib-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-14 07:14:45.000000 yplib-1.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 07:15:00.156210 yplib-1.1.8/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.1.8/yplib/__init__.py
--rw-rw-rw-   0        0        0     8030 2023-06-14 07:14:39.000000 yplib-1.1.8/yplib/chart.py
--rw-rw-rw-   0        0        0     8298 2023-06-14 07:14:33.000000 yplib-1.1.8/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.1.8/yplib/file.py
--rw-rw-rw-   0        0        0    13492 2023-06-14 06:31:40.000000 yplib-1.1.8/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-14 07:15:00.159225 yplib-1.1.8/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-14 07:15:00.000000 yplib-1.1.8/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-14 07:15:00.000000 yplib-1.1.8/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 07:15:00.000000 yplib-1.1.8/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 07:15:00.000000 yplib-1.1.8/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 07:18:57.007842 yplib-1.1.9/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-14 07:18:57.007842 yplib-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 07:18:57.008344 yplib-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-14 07:18:53.000000 yplib-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:18:57.005182 yplib-1.1.9/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.1.9/yplib/__init__.py
+-rw-rw-rw-   0        0        0     8057 2023-06-14 07:18:46.000000 yplib-1.1.9/yplib/chart.py
+-rw-rw-rw-   0        0        0     8327 2023-06-14 07:18:39.000000 yplib-1.1.9/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.1.9/yplib/file.py
+-rw-rw-rw-   0        0        0    13492 2023-06-14 06:31:40.000000 yplib-1.1.9/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:18:57.006609 yplib-1.1.9/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-14 07:18:56.000000 yplib-1.1.9/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-14 07:18:56.000000 yplib-1.1.9/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 07:18:56.000000 yplib-1.1.9/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 07:18:56.000000 yplib-1.1.9/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.1.8/LICENSE` & `yplib-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.1.8/setup.py` & `yplib-1.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.1.8",
+  version="1.1.9",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.1.8/yplib/chart.py` & `yplib-1.1.9/yplib/chart.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,15 +242,16 @@
 #         data.append(int(random.uniform(0, 1000)))
 #     n['data'] = data
 #     # n['hide'] = '1'
 #     y_list.append(n)
 # #
 # to_chart(x_list, y_list)
 #
-
+#
 # data_list = []
-# for i in range(100000):
+# for i in range(10000):
 #     data_list.append([i, int(random.uniform(0, 1000))])
 #
+# to_chart_one(data_list)
 # to_chart_one(list_data=data_list, is_area=True)
 
 # print('end')
```

### Comparing `yplib-1.1.8/yplib/chart_html.py` & `yplib-1.1.9/yplib/chart_html.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,25 +106,24 @@
              '    boundaryGap: false,' \
              '    data: -x_list-' \
              '  },' \
              '  yAxis: {' \
              '    type: "value",' \
              '    boundaryGap: [0, "100%"]' \
              '  },' \
-             '  dataZoom: [' \
-             '    {' \
-             '      type: "inside",' \
-             '      start: 0,' \
-             '      end: 10' \
-             '    },' \
-             '    {' \
-             '      start: 0,' \
-             '      end: 10' \
-             '    }' \
-             '  ],' \
+             '    dataZoom: [' \
+             '        {' \
+             '            show: true,' \
+             '            realtime: true,' \
+             '        },' \
+             '        {' \
+             '            type: "inside",' \
+             '            realtime: true,' \
+             '        },' \
+             '    ],' \
              '  series: [' \
              '    {' \
              '      type: "line",' \
              '      symbol: "none",' \
              '      sampling: "lttb",' \
              '      itemStyle: {' \
              '        color: "rgb(255, 70, 131)"' \
```

### Comparing `yplib-1.1.8/yplib/file.py` & `yplib-1.1.9/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.1.8/yplib/index.py` & `yplib-1.1.9/yplib/index.py`

 * *Files identical despite different names*

