# Comparing `tmp/yplib-1.1.7.tar.gz` & `tmp/yplib-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.1.7.tar", last modified: Wed Jun 14 07:09:35 2023, max compression
+gzip compressed data, was "dist\yplib-1.1.8.tar", last modified: Wed Jun 14 07:15:00 2023, max compression
```

## Comparing `yplib-1.1.7.tar` & `yplib-1.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 07:09:35.491231 yplib-1.1.7/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.1.7/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-14 07:09:35.490719 yplib-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 07:09:35.491231 yplib-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-14 07:09:30.000000 yplib-1.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 07:09:35.487221 yplib-1.1.7/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.1.7/yplib/__init__.py
--rw-rw-rw-   0        0        0     7656 2023-06-14 07:01:05.000000 yplib-1.1.7/yplib/chart.py
--rw-rw-rw-   0        0        0     8074 2023-06-14 07:09:11.000000 yplib-1.1.7/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.1.7/yplib/file.py
--rw-rw-rw-   0        0        0    13492 2023-06-14 06:31:40.000000 yplib-1.1.7/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-14 07:09:35.490323 yplib-1.1.7/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-14 07:09:35.000000 yplib-1.1.7/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-14 07:09:35.000000 yplib-1.1.7/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 07:09:35.000000 yplib-1.1.7/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 07:09:35.000000 yplib-1.1.7/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 07:15:00.159998 yplib-1.1.8/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.1.8/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-14 07:15:00.159998 yplib-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 07:15:00.159998 yplib-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-14 07:14:45.000000 yplib-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:15:00.156210 yplib-1.1.8/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.1.8/yplib/__init__.py
+-rw-rw-rw-   0        0        0     8030 2023-06-14 07:14:39.000000 yplib-1.1.8/yplib/chart.py
+-rw-rw-rw-   0        0        0     8298 2023-06-14 07:14:33.000000 yplib-1.1.8/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.1.8/yplib/file.py
+-rw-rw-rw-   0        0        0    13492 2023-06-14 06:31:40.000000 yplib-1.1.8/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:15:00.159225 yplib-1.1.8/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-14 07:15:00.000000 yplib-1.1.8/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-14 07:15:00.000000 yplib-1.1.8/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 07:15:00.000000 yplib-1.1.8/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 07:15:00.000000 yplib-1.1.8/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.1.7/LICENSE` & `yplib-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.1.7/setup.py` & `yplib-1.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.1.7",
+  version="1.1.8",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.1.7/yplib/chart.py` & `yplib-1.1.8/yplib/chart.py`

 * *Files 12% similar despite different names*

```diff
@@ -91,21 +91,29 @@
 # 将数据整理成折线图
 # 一条折线
 # 数据 : data_list = [
 #             ['2020-01-01', 132],
 #             ['2021-01-01', 181],
 #             ['2022-01-01', 147]
 #         ]
-def to_chart_one(list_data, chart_name='line'):
+# x_index : x 轴数据的下标
+# y_index : y 轴数据的下标
+def to_chart_one(list_data, chart_name='line', is_area=False, x_index=0, y_index=1):
     x_list = []
     y_list = []
     for d_one in list_data:
-        x_list.append(d_one[0])
-        y_list.append(d_one[1])
-    to_chart(x_list, [{'name': chart_name, 'data': y_list}], chart_name=chart_name)
+        x_list.append(d_one[x_index])
+        y_list.append(d_one[y_index])
+    if is_area:
+        insert_data_to_chart(html_data=line_area_html(),
+                             chart_name=chart_name,
+                             x_list=x_list,
+                             y_list=y_list)
+    else:
+        to_chart(x_list, [{'name': chart_name, 'data': y_list}], chart_name=chart_name)
 
 
 # legend_data.append(y_one['name'])
 #     if 'hide' in y_one:
 #         legend_selected[y_one['name']] = 0
 # legend = "data : " + str(legend_data) + ", selected : " + str(legend_selected)
 # # {
@@ -239,10 +247,10 @@
 # to_chart(x_list, y_list)
 #
 
 # data_list = []
 # for i in range(100000):
 #     data_list.append([i, int(random.uniform(0, 1000))])
 #
-# to_chart_one(data_list)
+# to_chart_one(list_data=data_list, is_area=True)
 
 # print('end')
```

### Comparing `yplib-1.1.7/yplib/chart_html.py` & `yplib-1.1.8/yplib/chart_html.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,20 @@
              '      dataZoom: {' \
              '        yAxisIndex: "none"' \
              '      },' \
              '      restore: {},' \
              '      saveAsImage: {}' \
              '    }' \
              '  },' \
+             '    grid: {' \
+             '        left: "30px",' \
+             '        right: "40px",' \
+             '        bottom: "80px",' \
+             '        containLabel: true,' \
+             '    },' \
              '  xAxis: {' \
              '    type: "category",' \
              '    boundaryGap: false,' \
              '    data: -x_list-' \
              '  },' \
              '  yAxis: {' \
              '    type: "value",' \
```

### Comparing `yplib-1.1.7/yplib/file.py` & `yplib-1.1.8/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.1.7/yplib/index.py` & `yplib-1.1.8/yplib/index.py`

 * *Files identical despite different names*

