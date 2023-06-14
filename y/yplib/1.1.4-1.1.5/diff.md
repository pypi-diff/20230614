# Comparing `tmp/yplib-1.1.4.tar.gz` & `tmp/yplib-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.1.4.tar", last modified: Wed Jun 14 06:32:26 2023, max compression
+gzip compressed data, was "dist\yplib-1.1.5.tar", last modified: Wed Jun 14 06:35:32 2023, max compression
```

## Comparing `yplib-1.1.4.tar` & `yplib-1.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 06:32:26.219693 yplib-1.1.4/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.1.4/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-14 06:32:26.219416 yplib-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 06:32:26.219693 yplib-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-14 06:32:16.000000 yplib-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:32:26.216280 yplib-1.1.4/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.1.4/yplib/__init__.py
--rw-rw-rw-   0        0        0     8968 2023-06-14 06:31:53.000000 yplib-1.1.4/yplib/chart.py
--rw-rw-rw-   0        0        0     5664 2023-06-14 06:14:34.000000 yplib-1.1.4/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.1.4/yplib/file.py
--rw-rw-rw-   0        0        0    13492 2023-06-14 06:31:40.000000 yplib-1.1.4/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:32:26.218745 yplib-1.1.4/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-14 06:32:26.000000 yplib-1.1.4/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-14 06:32:26.000000 yplib-1.1.4/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 06:32:26.000000 yplib-1.1.4/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 06:32:26.000000 yplib-1.1.4/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 06:35:32.790868 yplib-1.1.5/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-14 06:35:32.790366 yplib-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 06:35:32.790868 yplib-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-14 06:35:21.000000 yplib-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:35:32.787382 yplib-1.1.5/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.1.5/yplib/__init__.py
+-rw-rw-rw-   0        0        0     9104 2023-06-14 06:35:12.000000 yplib-1.1.5/yplib/chart.py
+-rw-rw-rw-   0        0        0     5664 2023-06-14 06:14:34.000000 yplib-1.1.5/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.1.5/yplib/file.py
+-rw-rw-rw-   0        0        0    13492 2023-06-14 06:31:40.000000 yplib-1.1.5/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:35:32.789626 yplib-1.1.5/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-14 06:35:32.000000 yplib-1.1.5/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-14 06:35:32.000000 yplib-1.1.5/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 06:35:32.000000 yplib-1.1.5/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 06:35:32.000000 yplib-1.1.5/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.1.4/LICENSE` & `yplib-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.1.4/setup.py` & `yplib-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.1.4",
+  version="1.1.5",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.1.4/yplib/chart.py` & `yplib-1.1.5/yplib/chart.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,19 @@
         one_p = p_list[index]
         one_data = p_data_list[index]
         if one_data is None:
             continue
         one_p = f'-{one_p}-'
         if one_p in html_data:
             html_data = html_data.replace(one_p, str(one_data))
-    to_txt([html_data], str(chart_name), 'html', False, '.html')
+    to_txt(list_data=[html_data],
+           file_name=str(chart_name),
+           file_path='html',
+           fixed_name=False,
+           suffix='.html')
     # current_path = os.path.abspath(__file__)
     # html_list = open(current_path[0:current_path.find('__init__')] + 'line-stack-temp.html', 'r', encoding='utf-8').readlines()
 
 
 # 将数据整理成折线图
 # x轴数据 : x_list = ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
 # y轴数据 : y_list = [
@@ -170,15 +174,14 @@
 #     one = {}
 #     one['name'] = uuid_random()
 #     one['value'] = int(random.uniform(0, 1000))
 #     data.append(one)
 #
 # to_chart_pie(data)
 
-
 # print('start')
 # to_txt([1,2,3], 'p')
 # to_txt_file_name([1,2,3], 'p')
 #
 #
 # li = to_list('D:\code\python3\packaging_tutorial\yplib\data\p_20230612_095450_34779.txt')
 #
@@ -196,35 +199,35 @@
 # to_txt_data('yangpu12', 1)
 #
 # x_list = ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
 # y_list = json.loads(
 #     '[{"name":"Email","data":[120,132,101,134,90,230,210]},{"name":"Union Ads","data":[220,182,191,234,290,330,310]},{"name":"Video Ads","data":[150,232,201,154,190,330,410]},{"name":"Direct","data":[320,332,301,334,390,330,320]},{"name":"Search Engine","data":[820,932,901,934,1290,1330,1320]}]')
 #
 
-# # 将 list 转化成 图表的例子
-x_list = []
-y_list = []
-# # x 轴有 100 个
-# # 100 个横坐标
-for i in range(100):
-    x_list.append(i)
-#
-# 有 10 条线
-for i in range(10):  # 0 1 2 3 4 55
-    n = {}
-    n['name'] = str(int(random.uniform(0, 1000)))
-    data = []
-    # 每条线有 100 个纵坐标, 与 x_list 中的对应起来
-    for i in range(100):
-        data.append(int(random.uniform(0, 1000)))
-    n['data'] = data
-    n['hide'] = '1'
-    y_list.append(n)
-#
-to_chart(x_list, y_list)
+# # # 将 list 转化成 图表的例子
+# x_list = []
+# y_list = []
+# # # x 轴有 100 个
+# # # 100 个横坐标
+# for i in range(100):
+#     x_list.append(i)
+# #
+# # 有 10 条线
+# for i in range(10):  # 0 1 2 3 4 55
+#     n = {}
+#     n['name'] = str(int(random.uniform(0, 1000)))
+#     data = []
+#     # 每条线有 100 个纵坐标, 与 x_list 中的对应起来
+#     for i in range(100):
+#         data.append(int(random.uniform(0, 1000)))
+#     n['data'] = data
+#     n['hide'] = '1'
+#     y_list.append(n)
+# #
+# to_chart(x_list, y_list)
 #
 # to_txt_data(x_list, 'operate')
 # to_txt_data(y_list, 'operate')
 
 # to_log_file(1)
 # log_to_file(12)
 # log_to_file('yangpu')
```

### Comparing `yplib-1.1.4/yplib/chart_html.py` & `yplib-1.1.5/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.1.4/yplib/file.py` & `yplib-1.1.5/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.1.4/yplib/index.py` & `yplib-1.1.5/yplib/index.py`

 * *Files identical despite different names*

