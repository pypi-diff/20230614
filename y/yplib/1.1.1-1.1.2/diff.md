# Comparing `tmp/yplib-1.1.1.tar.gz` & `tmp/yplib-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.1.1.tar", last modified: Wed Jun 14 02:06:42 2023, max compression
+gzip compressed data, was "dist\yplib-1.1.2.tar", last modified: Wed Jun 14 02:29:33 2023, max compression
```

## Comparing `yplib-1.1.1.tar` & `yplib-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 02:06:42.061242 yplib-1.1.1/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.1.1/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-14 02:06:42.061123 yplib-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 02:06:42.061694 yplib-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-14 02:06:28.000000 yplib-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:06:42.058074 yplib-1.1.1/yplib/
--rw-rw-rw-   0        0        0      119 2023-06-14 01:52:25.000000 yplib-1.1.1/yplib/__init__.py
--rw-rw-rw-   0        0        0     3779 2023-06-14 02:06:14.000000 yplib-1.1.1/yplib/chart_html.py
--rw-rw-rw-   0        0        0     3555 2023-06-14 00:31:24.000000 yplib-1.1.1/yplib/file.py
--rw-rw-rw-   0        0        0    12635 2023-06-14 01:52:29.000000 yplib-1.1.1/yplib/index.py
--rw-rw-rw-   0        0        0     3517 2023-06-14 01:54:39.000000 yplib-1.1.1/yplib/test_my_fun.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:06:42.060433 yplib-1.1.1/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-14 02:06:41.000000 yplib-1.1.1/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-06-14 02:06:42.000000 yplib-1.1.1/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 02:06:42.000000 yplib-1.1.1/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 02:06:42.000000 yplib-1.1.1/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 02:29:33.728799 yplib-1.1.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-14 02:29:33.728531 yplib-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-1.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 02:29:33.729019 yplib-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-14 02:29:11.000000 yplib-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:29:33.724905 yplib-1.1.2/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.1.2/yplib/__init__.py
+-rw-rw-rw-   0        0        0     7365 2023-06-14 02:28:55.000000 yplib-1.1.2/yplib/chart.py
+-rw-rw-rw-   0        0        0     3779 2023-06-14 02:06:14.000000 yplib-1.1.2/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.1.2/yplib/file.py
+-rw-rw-rw-   0        0        0    13524 2023-06-14 02:28:45.000000 yplib-1.1.2/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:29:33.726958 yplib-1.1.2/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-14 02:29:33.000000 yplib-1.1.2/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-14 02:29:33.000000 yplib-1.1.2/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 02:29:33.000000 yplib-1.1.2/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 02:29:33.000000 yplib-1.1.2/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.1.1/LICENSE` & `yplib-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.1.1/PKG-INFO` & `yplib-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 1.1.1
+Version: 1.1.2
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-1.1.1/setup.py` & `yplib-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.1.1",
+  version="1.1.2",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-1.1.1/yplib/chart_html.py` & `yplib-1.1.2/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.1.1/yplib/index.py` & `yplib-1.1.2/yplib/index.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datetime import datetime
 from datetime import timedelta
 
 import xlrd
 import xlwt
 import time
 import re
-# import random
+import random
 import hashlib
 from yplib.chart_html import *
 
 
 # 记录日志, 如果是对象会转化为 json
 def to_log(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
            a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
@@ -307,75 +307,137 @@
                 s = str(one_data)
             sh.write(m, n, s)  # 写入A3，数值等于1
         m += 1
     # 5. 保存
     # myWorkbook.save('5002200.xls')
     w_b.save(file_path + '/' + get_file_name(file_name, '.xls'))
 
+# print('start')
+# to_txt([1,2,3], 'p')
+# to_txt_file_name([1,2,3], 'p')
+#
+#
+# li = to_list('D:\code\python3\packaging_tutorial\yplib\data\p_20230612_095450_34779.txt')
+#
+# to_log()
+#
+# to_log()
+# to_log(1)
+# to_log(1, 2)
+# to_log(1, 2, [1, 2])
+# to_log_file(1, 2, [{'a': 2}])
+# to_log_txt('1.txt', 1, 2, [{'a': 2}])
+# to_txt([{'a': 2}])
+# to_txt_data('yangpu', 1)
+# to_txt_data('yangpu1', 1)
+# to_txt_data('yangpu12', 1)
+#
+# x_list = ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
+# y_list = json.loads(
+#     '[{"name":"Email","data":[120,132,101,134,90,230,210]},{"name":"Union Ads","data":[220,182,191,234,290,330,310]},{"name":"Video Ads","data":[150,232,201,154,190,330,410]},{"name":"Direct","data":[320,332,301,334,390,330,320]},{"name":"Search Engine","data":[820,932,901,934,1290,1330,1320]}]')
+#
+
+# # 将 list 转化成 图表的例子
+# x_list = []
+# y_list = []
+# # x 轴有 100 个
+# # 100 个横坐标
+# for i in range(100):
+#     x_list.append(i)
+#
+# # 有 10 条线
+# for i in range(10):  # 0 1 2 3 4 55
+#     n = {}
+#     n['name'] = str(int(random.uniform(0, 1000)))
+#     data = []
+#     # 每条线有 100 个纵坐标, 与 x_list 中的对应起来
+#     for i in range(100):
+#         data.append(int(random.uniform(0, 1000)))
+#     n['data'] = data
+#     y_list.append(n)
+# #
+# to_chart(x_list, y_list)
+#
+# to_txt_data(x_list, 'operate')
+# to_txt_data(y_list, 'operate')
+
+# to_log_file(1)
+# log_to_file(12)
+# log_to_file('yangpu')
+# print(str_to_int('yan123gpu'))
+# print(str_to_float('yan123gpu'))
+# print(str_to_float('yan123g.12pu'))
+
+#
+# print(to_hump('user_id'))
+# print(to_hump('USER_ID'))
+# print(to_hump('userId'))
+# print(to_hump('user'))
+# print(to_hump(''))
+
+# print(to_hump_more('userId'))
+
+# print(to_underline('userId'))
+
+
+# print(uuid_random(5))
+# print(uuid_random(10))
+# print(uuid_random())
+# print(uuid_random(32))
+# print(uuid_random(64))
+# print(uuid_random(128))
+# print(uuid_random(127))
+# print(uuid_random(129))
+
+
+# print(to_int('a'))
+# print(to_int(2))
+# print(to_int(2.2))
+# print(to_int(2.2))
+
+# print(to_float('a'))
+# print(to_float(2))
+# print(to_float(2.2))
+# print(to_float(2.24))
+
+# print(to_date('2019-09'))
+# print(to_date('2019-09-08'))
+# print(to_date('2019-09-08 12'))
+# print(to_date('2019-09-08 12:13'))
+# print(to_datetime('2019-09-08 12:13:14'))
+# print(to_datetime('2019-09-08 12:13:14.789'))
+# print(to_datetime(1686537485))
+# print(to_datetime(1686537484467))
+# print(to_datetime(datetime.today()))
+#
+# print(do_md5())
+# print(do_md5())
+# print(do_md5('yangpu'))
+# print(do_md5('yangpu12'))
+#
+# log_msg = ''
+# headers = {'Content-Type': 'application/json;charset=utf-8'}
+# data = {}
+# data['merchantId'] = "merchantId"
+# data['currency'] = "IDR"
+# data['accType'] = "payout"
+# data['version'] = "1.0"
+# sign = sort_by_json_key(data)
+# print(sign)
+# hash = hashlib.sha256()
+# hash.update(sign.encode('utf-8'))
+# data['sign'] = hash.hexdigest()
+#
+# print(data)
+
+
+# print(get_file_data_line(r'D:\notepad_file\202306\fasdfsadfaf.txt', 'payout', from_last=False))
+
+# get_file_data_line(r'D:\notepad_file\202306', 'a')
+# get_file_by_content(r'D:\notepad_file\202306', 'a')
+# print(get_file(r'D:\notepad_file\202306', 'a'))
+# print(get_file(r'D:\notepad_file\202306'))
+# print(get_file())
+# print(os.path.abspath('.'))
 
-# 将数据整理成折线图
-# x轴数据 : x_list = ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
-# y轴数据 : y_list = [
-#             {
-#                 name: 'Email',
-#                 selected: False,
-#                 data: [120, 132, 101, 134, 90, 230, 210],
-#             },
-#             {
-#                 name: 'Union Ads',
-#                 selected: 0,
-#                 data: [220, 182, 191, 234, 290, 330, 310],
-#             },
-#             {
-#                 name: 'Video Ads',
-#                 data: [150, 232, 201, 154, 190, 330, 410],
-#             },
-#             {
-#                 name: 'Direct',
-#                 data: [320, 332, 301, 334, 390, 330, 320],
-#             },
-#             {
-#                 name: 'Search Engine',
-#                 data: [820, 932, 901, 934, 1290, 1330, 1320],
-#             },
-#         ]
-def to_chart(x_list, y_list, chart_name='stack_line'):
-    # current_path = os.path.abspath(__file__)
-    # html_list = open(current_path[0:current_path.find('__init__')] + 'line-stack-temp.html', 'r', encoding='utf-8').readlines()
-    html_list_one = line_stack_html()
-    chart_name_html = '-chart_name-'
-    x_list_html = '-x_list-'
-    legend_html = '-legend-'
-    series_html = '-series-'
-    r_list = []
-    # data: ['Email', 'Union Ads', 'Video Ads', 'Direct', 'Search Engine']
-    legend_data = []
-    legend_selected = {}
-    for y_one in y_list:
-        legend_data.append(y_one['name'])
-        if 'selected' in y_one:
-            legend_selected[y_one['name']] = 'false'
-    legend = "data : " + str(legend_data) + ", selected : " + str(legend_selected)
-    # {
-    #     name: 'Email',
-    #     type: 'line',
-    #     stack: 'Total',
-    #     data: [120, 132, 101, 134, 90, 230, 210],
-    # }
-    series = []
-    for y_one in y_list:
-        y_one['type'] = 'line'
-        y_one['stack'] = 'Total'
-        series.append(y_one)
-
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
+
+# print('end')
```

### Comparing `yplib-1.1.1/yplib.egg-info/PKG-INFO` & `yplib-1.1.2/yplib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 1.1.1
+Version: 1.1.2
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

