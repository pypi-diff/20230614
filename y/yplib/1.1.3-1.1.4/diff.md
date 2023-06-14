# Comparing `tmp/yplib-1.1.3.tar.gz` & `tmp/yplib-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.1.3.tar", last modified: Wed Jun 14 02:50:52 2023, max compression
+gzip compressed data, was "dist\yplib-1.1.4.tar", last modified: Wed Jun 14 06:32:26 2023, max compression
```

## Comparing `yplib-1.1.3.tar` & `yplib-1.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 02:50:52.908613 yplib-1.1.3/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.1.3/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-14 02:50:52.908613 yplib-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 02:50:52.908613 yplib-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-14 02:50:33.000000 yplib-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:50:52.905450 yplib-1.1.3/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.1.3/yplib/__init__.py
--rw-rw-rw-   0        0        0     8409 2023-06-14 02:42:42.000000 yplib-1.1.3/yplib/chart.py
--rw-rw-rw-   0        0        0     5523 2023-06-14 02:48:14.000000 yplib-1.1.3/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.1.3/yplib/file.py
--rw-rw-rw-   0        0        0    13524 2023-06-14 02:28:45.000000 yplib-1.1.3/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:50:52.908042 yplib-1.1.3/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-14 02:50:52.000000 yplib-1.1.3/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-14 02:50:52.000000 yplib-1.1.3/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 02:50:52.000000 yplib-1.1.3/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 02:50:52.000000 yplib-1.1.3/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 06:32:26.219693 yplib-1.1.4/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-14 06:32:26.219416 yplib-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 06:32:26.219693 yplib-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-14 06:32:16.000000 yplib-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:32:26.216280 yplib-1.1.4/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.1.4/yplib/__init__.py
+-rw-rw-rw-   0        0        0     8968 2023-06-14 06:31:53.000000 yplib-1.1.4/yplib/chart.py
+-rw-rw-rw-   0        0        0     5664 2023-06-14 06:14:34.000000 yplib-1.1.4/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.1.4/yplib/file.py
+-rw-rw-rw-   0        0        0    13492 2023-06-14 06:31:40.000000 yplib-1.1.4/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:32:26.218745 yplib-1.1.4/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-14 06:32:26.000000 yplib-1.1.4/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-14 06:32:26.000000 yplib-1.1.4/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 06:32:26.000000 yplib-1.1.4/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 06:32:26.000000 yplib-1.1.4/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.1.3/LICENSE` & `yplib-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.1.3/setup.py` & `yplib-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.1.3",
+  version="1.1.4",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.1.3/yplib/chart.py` & `yplib-1.1.4/yplib/chart.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,78 +1,91 @@
 from yplib.chart_html import *
 from yplib.index import *
 
 
+# 将 html 中的占位符 替换成数据
+# 并且 导出 生成后的 html 文件
+def insert_data_to_chart(html_data='',
+                         chart_name=None,
+                         x_list=None,
+                         y_list=None,
+                         legend=None,
+                         series=None):
+    p_list = [
+        'chart_name', 'x_list', 'y_list', 'legend', 'series'
+    ]
+    p_data_list = [
+        chart_name, x_list, y_list, legend, series
+    ]
+    for index in range(len(p_list)):
+        one_p = p_list[index]
+        one_data = p_data_list[index]
+        if one_data is None:
+            continue
+        one_p = f'-{one_p}-'
+        if one_p in html_data:
+            html_data = html_data.replace(one_p, str(one_data))
+    to_txt([html_data], str(chart_name), 'html', False, '.html')
+    # current_path = os.path.abspath(__file__)
+    # html_list = open(current_path[0:current_path.find('__init__')] + 'line-stack-temp.html', 'r', encoding='utf-8').readlines()
+
+
 # 将数据整理成折线图
 # x轴数据 : x_list = ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
 # y轴数据 : y_list = [
 #             {
 #                 name: 'Email',
-#                 selected: False,
+#                 hide: False,
 #                 data: [120, 132, 101, 134, 90, 230, 210],
 #             },
 #             {
 #                 name: 'Union Ads',
-#                 selected: 0,
+#                 hide: 0,
 #                 data: [220, 182, 191, 234, 290, 330, 310],
 #             },
 #             {
 #                 name: 'Video Ads',
+#                 hide: True,
 #                 data: [150, 232, 201, 154, 190, 330, 410],
 #             },
 #             {
 #                 name: 'Direct',
 #                 data: [320, 332, 301, 334, 390, 330, 320],
 #             },
 #             {
 #                 name: 'Search Engine',
 #                 data: [820, 932, 901, 934, 1290, 1330, 1320],
 #             },
 #         ]
 def to_chart(x_list, y_list, chart_name='stack_line'):
-    # current_path = os.path.abspath(__file__)
-    # html_list = open(current_path[0:current_path.find('__init__')] + 'line-stack-temp.html', 'r', encoding='utf-8').readlines()
-    html_list_one = line_stack_html()
-    chart_name_html = '-chart_name-'
-    x_list_html = '-x_list-'
-    legend_html = '-legend-'
-    series_html = '-series-'
-    r_list = []
     # data: ['Email', 'Union Ads', 'Video Ads', 'Direct', 'Search Engine']
     legend_data = []
     legend_selected = {}
     for y_one in y_list:
         legend_data.append(y_one['name'])
-        if 'selected' in y_one:
-            legend_selected[y_one['name']] = 'false'
+        if 'hide' in y_one:
+            legend_selected[y_one['name']] = 0
     legend = "data : " + str(legend_data) + ", selected : " + str(legend_selected)
     # {
     #     name: 'Email',
     #     type: 'line',
     #     stack: 'Total',
     #     data: [120, 132, 101, 134, 90, 230, 210],
     # }
     series = []
     for y_one in y_list:
         y_one['type'] = 'line'
         y_one['stack'] = 'Total'
         series.append(y_one)
 
-    one_line = html_list_one
-    if chart_name_html in one_line:
-        one_line = one_line.replace(chart_name_html, str(chart_name))
-    if x_list_html in one_line:
-        # ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
-        one_line = one_line.replace(x_list_html, str(x_list))
-    if legend_html in one_line:
-        one_line = one_line.replace(legend_html, str(legend))
-    if series_html in one_line:
-        one_line = one_line.replace(series_html, str(series))
-    r_list.append(one_line)
-    to_txt(r_list, str(chart_name), 'html', False, '.html')
+    insert_data_to_chart(html_data=line_stack_html(),
+                         chart_name=chart_name,
+                         x_list=x_list,
+                         legend=legend,
+                         series=series)
 
 
 # 将数据整理成饼状图
 # 数据 : data = [
 #         { value: 1048, name: "Search Engine" },
 #         { value: 735, name: "Direct" },
 #         { value: 580, name: "Email" },
@@ -84,60 +97,75 @@
 #         [ "Search Engine", 1048 ],
 #         [ "Direct", 735 ],
 #         [ "Email",580 ],
 #         [ "Union Ads",484 ],
 #         [ "Video Ads",300 ]
 #       ]
 def to_chart_pie(data_list, chart_name='pie'):
-    html_list_one = pie_html()
-    data_html = '-data-'
-    data_html_list = []
+    x_list = []
     if isinstance(data_list[0], list):
         for one in data_list:
-            if isinstance(one, list):
-                data_html_list.append({'name': one[0], 'value': one[1]})
+            x_list.append({'name': one[0], 'value': one[1]})
     else:
-        data_html_list = data_list
-
-    if data_html in html_list_one:
-        html_list_one = html_list_one.replace(data_html, str(data_html_list))
-    to_txt([html_list_one], str(chart_name), 'html', False, '.html')
+        x_list = data_list
+    insert_data_to_chart(html_data=pie_html(),
+                         chart_name=chart_name,
+                         x_list=x_list)
 
 
 # 将数据整理成柱状图
 # 数据 : data = [
-#         { value: 1048, name: "Search Engine" },
-#         { value: 735, name: "Direct" },
-#         { value: 580, name: "Email" },
-#         { value: 484, name: "Union Ads" },
-#         { value: 300, name: "Video Ads" }
-#       ]
-# 或者
-# 数据 : data = [
 #         [ "Search Engine", 1048 ],
 #         [ "Direct", 735 ],
 #         [ "Email",580 ],
 #         [ "Union Ads",484 ],
 #         [ "Video Ads",300 ]
 #       ]
+# 或者
+# 数据 : data = [
+#        {x: "Search Engine", y: 1048 },
+#        {x: "Direct", y: 735 },
+#        {x: "Email", y:580 },
+#        {x: "Union Ads", y:484 },
+#        {x: "Video Ads", y:300 }
+#       }]
 def to_chart_bar(data_list, chart_name='bar'):
-    html_list_one = pie_html()
-    data_html = '-data-'
-    data_html_list = []
-    if isinstance(data_list[0], list):
-        for one in data_list:
-            if isinstance(one, list):
-                data_html_list.append({'name': one[0], 'value': one[1]})
-    else:
-        data_html_list = data_list
-
-    if data_html in html_list_one:
-        html_list_one = html_list_one.replace(data_html, str(data_html_list))
+    html_list_one = bar_html()
+    x_list_html = '-x_list-'
+    y_list_html = '-y_list-'
+    x_html_list = []
+    y_html_list = []
+    for one in data_list:
+        if isinstance(one, list):
+            x_html_list.append(one[0])
+            y_html_list.append(one[1])
+        else:
+            x_html_list.append(one['x'])
+            y_html_list.append(one['y'])
+
+    if x_list_html in html_list_one:
+        html_list_one = html_list_one.replace(x_list_html, str(x_html_list))
+    if y_list_html in html_list_one:
+        html_list_one = html_list_one.replace(y_list_html, str(y_html_list))
     to_txt([html_list_one], str(chart_name), 'html', False, '.html')
 
+
+#
+# data = []
+# # for i in range(10):
+# #     data.append([uuid_random(), int(random.uniform(0, 1000))])
+# for i in range(10):
+#     one = {}
+#     one['x'] = uuid_random()
+#     one['y'] = int(random.uniform(0, 1000))
+#     data.append(one)
+#
+# to_chart_bar(data)
+#
+#
 #
 # data = []
 # # for i in range(10):
 # #     data.append([uuid_random(), int(random.uniform(0, 1000))])
 # for i in range(10):
 #     one = {}
 #     one['name'] = uuid_random()
@@ -169,33 +197,34 @@
 #
 # x_list = ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
 # y_list = json.loads(
 #     '[{"name":"Email","data":[120,132,101,134,90,230,210]},{"name":"Union Ads","data":[220,182,191,234,290,330,310]},{"name":"Video Ads","data":[150,232,201,154,190,330,410]},{"name":"Direct","data":[320,332,301,334,390,330,320]},{"name":"Search Engine","data":[820,932,901,934,1290,1330,1320]}]')
 #
 
 # # 将 list 转化成 图表的例子
-# x_list = []
-# y_list = []
+x_list = []
+y_list = []
 # # x 轴有 100 个
 # # 100 个横坐标
-# for i in range(100):
-#     x_list.append(i)
+for i in range(100):
+    x_list.append(i)
+#
+# 有 10 条线
+for i in range(10):  # 0 1 2 3 4 55
+    n = {}
+    n['name'] = str(int(random.uniform(0, 1000)))
+    data = []
+    # 每条线有 100 个纵坐标, 与 x_list 中的对应起来
+    for i in range(100):
+        data.append(int(random.uniform(0, 1000)))
+    n['data'] = data
+    n['hide'] = '1'
+    y_list.append(n)
 #
-# # 有 10 条线
-# for i in range(10):  # 0 1 2 3 4 55
-#     n = {}
-#     n['name'] = str(int(random.uniform(0, 1000)))
-#     data = []
-#     # 每条线有 100 个纵坐标, 与 x_list 中的对应起来
-#     for i in range(100):
-#         data.append(int(random.uniform(0, 1000)))
-#     n['data'] = data
-#     y_list.append(n)
-# #
-# to_chart(x_list, y_list)
+to_chart(x_list, y_list)
 #
 # to_txt_data(x_list, 'operate')
 # to_txt_data(y_list, 'operate')
 
 # to_log_file(1)
 # log_to_file(12)
 # log_to_file('yangpu')
```

### Comparing `yplib-1.1.3/yplib/chart_html.py` & `yplib-1.1.4/yplib/chart_html.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,14 +72,18 @@
              '}'
     return chart_html(option)
 
 
 # 饼图的 html 模板代码
 def pie_html():
     option = '{' \
+             '  title: {' \
+             '    text: "-chart_name-",' \
+             '    left: 10' \
+             '  },' \
              '  tooltip: {' \
              '    trigger: "item"' \
              '  },' \
              '  legend: {' \
              '    top: "5%",' \
              '    left: "center"' \
              '  },' \
@@ -99,26 +103,26 @@
              '          fontSize: 30,' \
              '          fontWeight: "bold"' \
              '        }' \
              '      },' \
              '      labelLine: {' \
              '        show: true' \
              '      },' \
-             '      data: -data-' \
+             '      data: -x_list-' \
              '    }' \
              '  ]' \
              '}'
     return chart_html(option)
 
 
 # 柱状的 html 模板代码
 def bar_html():
     option = '{' \
              '  title: {' \
-             '    text: "",' \
+             '    text: "-chart_name-",' \
              '    left: 10' \
              '  },' \
              '  toolbox: {' \
              '    feature: {' \
              '      dataZoom: {' \
              '        yAxisIndex: false' \
              '      },' \
```

### Comparing `yplib-1.1.3/yplib/file.py` & `yplib-1.1.4/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.1.3/yplib/index.py` & `yplib-1.1.4/yplib/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 import xlrd
 import xlwt
 import time
 import re
 import random
 import hashlib
-from yplib.chart_html import *
 
 
 # 记录日志, 如果是对象会转化为 json
 def to_log(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
            a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
     l = [a1, a2, a3, a4, a5, a6, a7, a8, a9, a10,
          a11, a12, a13, a14, a15, a16, a17, a18, a19, a20]
```

