# Comparing `tmp/yplib-1.1.6.tar.gz` & `tmp/yplib-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.1.6.tar", last modified: Wed Jun 14 06:41:14 2023, max compression
+gzip compressed data, was "dist\yplib-1.1.7.tar", last modified: Wed Jun 14 07:09:35 2023, max compression
```

## Comparing `yplib-1.1.6.tar` & `yplib-1.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 06:41:14.282556 yplib-1.1.6/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.1.6/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-14 06:41:14.282438 yplib-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 06:41:14.282556 yplib-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-14 06:41:10.000000 yplib-1.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:41:14.279601 yplib-1.1.6/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.1.6/yplib/__init__.py
--rw-rw-rw-   0        0        0     8855 2023-06-14 06:39:45.000000 yplib-1.1.6/yplib/chart.py
--rw-rw-rw-   0        0        0     5804 2023-06-14 06:40:22.000000 yplib-1.1.6/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.1.6/yplib/file.py
--rw-rw-rw-   0        0        0    13492 2023-06-14 06:31:40.000000 yplib-1.1.6/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:41:14.281942 yplib-1.1.6/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-14 06:41:14.000000 yplib-1.1.6/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-14 06:41:14.000000 yplib-1.1.6/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 06:41:14.000000 yplib-1.1.6/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 06:41:14.000000 yplib-1.1.6/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 07:09:35.491231 yplib-1.1.7/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.1.7/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-14 07:09:35.490719 yplib-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 07:09:35.491231 yplib-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-14 07:09:30.000000 yplib-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:09:35.487221 yplib-1.1.7/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.1.7/yplib/__init__.py
+-rw-rw-rw-   0        0        0     7656 2023-06-14 07:01:05.000000 yplib-1.1.7/yplib/chart.py
+-rw-rw-rw-   0        0        0     8074 2023-06-14 07:09:11.000000 yplib-1.1.7/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.1.7/yplib/file.py
+-rw-rw-rw-   0        0        0    13492 2023-06-14 06:31:40.000000 yplib-1.1.7/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:09:35.490323 yplib-1.1.7/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-14 07:09:35.000000 yplib-1.1.7/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-14 07:09:35.000000 yplib-1.1.7/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 07:09:35.000000 yplib-1.1.7/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 07:09:35.000000 yplib-1.1.7/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.1.6/LICENSE` & `yplib-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.1.6/setup.py` & `yplib-1.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.1.6",
+  version="1.1.7",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.1.6/yplib/chart.py` & `yplib-1.1.7/yplib/chart.py`

 * *Files 20% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 #                 data: [320, 332, 301, 334, 390, 330, 320],
 #             },
 #             {
 #                 name: 'Search Engine',
 #                 data: [820, 932, 901, 934, 1290, 1330, 1320],
 #             },
 #         ]
-def to_chart(x_list, y_list, chart_name='stack_line'):
+def to_chart(x_list, y_list, chart_name='line_stack'):
     # data: ['Email', 'Union Ads', 'Video Ads', 'Direct', 'Search Engine']
     legend_data = []
     legend_selected = {}
     for y_one in y_list:
         legend_data.append(y_one['name'])
         if 'hide' in y_one:
             legend_selected[y_one['name']] = 0
@@ -84,14 +84,53 @@
     insert_data_to_chart(html_data=line_stack_html(),
                          chart_name=chart_name,
                          x_list=x_list,
                          legend=legend,
                          series=series)
 
 
+# 将数据整理成折线图
+# 一条折线
+# 数据 : data_list = [
+#             ['2020-01-01', 132],
+#             ['2021-01-01', 181],
+#             ['2022-01-01', 147]
+#         ]
+def to_chart_one(list_data, chart_name='line'):
+    x_list = []
+    y_list = []
+    for d_one in list_data:
+        x_list.append(d_one[0])
+        y_list.append(d_one[1])
+    to_chart(x_list, [{'name': chart_name, 'data': y_list}], chart_name=chart_name)
+
+
+# legend_data.append(y_one['name'])
+#     if 'hide' in y_one:
+#         legend_selected[y_one['name']] = 0
+# legend = "data : " + str(legend_data) + ", selected : " + str(legend_selected)
+# # {
+# #     name: 'Email',
+# #     type: 'line',
+# #     stack: 'Total',
+# #     data: [120, 132, 101, 134, 90, 230, 210],
+# # }
+# series = []
+# for y_one in y_list:
+#     y_one['type'] = 'line'
+#     y_one['stack'] = 'Total'
+#     series.append(y_one)
+#
+# insert_data_to_chart(html_data=line_stack_html(),
+#                      chart_name=chart_name,
+#                      x_list=x_list,
+#                      legend=legend,
+#                      series=series)
+
+
 # 将数据整理成饼状图
 # 数据 : data = [
 #         { value: 1048, name: "Search Engine" },
 #         { value: 735, name: "Direct" },
 #         { value: 580, name: "Email" },
 #         { value: 484, name: "Union Ads" },
 #         { value: 300, name: "Video Ads" }
@@ -147,159 +186,63 @@
                          chart_name=chart_name,
                          x_list=x_list,
                          y_list=y_list)
 
 # data = []
 # # for i in range(10):
 # #     data.append([uuid_random(), int(random.uniform(0, 1000))])
-# for i in range(100):
+# for i in range(10000):
 #     one = {}
 #     one['x'] = uuid_random()
 #     one['y'] = int(random.uniform(0, 1000))
 #     data.append(one)
 #
 # to_chart_bar(data)
-#
+
 #
 #
 # data = []
 # # for i in range(10):
 # #     data.append([uuid_random(), int(random.uniform(0, 1000))])
 # for i in range(10):
 #     one = {}
 #     one['name'] = uuid_random()
 #     one['value'] = int(random.uniform(0, 1000))
 #     data.append(one)
 #
 # to_chart_pie(data)
 
-# print('start')
-# to_txt([1,2,3], 'p')
-# to_txt_file_name([1,2,3], 'p')
-#
-#
-# li = to_list('D:\code\python3\packaging_tutorial\yplib\data\p_20230612_095450_34779.txt')
-#
-# to_log()
-#
-# to_log()
-# to_log(1)
-# to_log(1, 2)
-# to_log(1, 2, [1, 2])
-# to_log_file(1, 2, [{'a': 2}])
-# to_log_txt('1.txt', 1, 2, [{'a': 2}])
-# to_txt([{'a': 2}])
-# to_txt_data('yangpu', 1)
-# to_txt_data('yangpu1', 1)
-# to_txt_data('yangpu12', 1)
-#
 # x_list = ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
 # y_list = json.loads(
 #     '[{"name":"Email","data":[120,132,101,134,90,230,210]},{"name":"Union Ads","data":[220,182,191,234,290,330,310]},{"name":"Video Ads","data":[150,232,201,154,190,330,410]},{"name":"Direct","data":[320,332,301,334,390,330,320]},{"name":"Search Engine","data":[820,932,901,934,1290,1330,1320]}]')
 #
 
 # # # 将 list 转化成 图表的例子
 # x_list = []
 # y_list = []
 # # # x 轴有 100 个
 # # # 100 个横坐标
 # for i in range(100):
 #     x_list.append(i)
 # #
 # # 有 10 条线
-# for i in range(10):  # 0 1 2 3 4 55
+# for i in range(1):  # 0 1 2 3 4 55
 #     n = {}
 #     n['name'] = str(int(random.uniform(0, 1000)))
 #     data = []
 #     # 每条线有 100 个纵坐标, 与 x_list 中的对应起来
 #     for i in range(100):
 #         data.append(int(random.uniform(0, 1000)))
 #     n['data'] = data
-#     n['hide'] = '1'
+#     # n['hide'] = '1'
 #     y_list.append(n)
 # #
 # to_chart(x_list, y_list)
 #
-# to_txt_data(x_list, 'operate')
-# to_txt_data(y_list, 'operate')
-
-# to_log_file(1)
-# log_to_file(12)
-# log_to_file('yangpu')
-# print(str_to_int('yan123gpu'))
-# print(str_to_float('yan123gpu'))
-# print(str_to_float('yan123g.12pu'))
-
-#
-# print(to_hump('user_id'))
-# print(to_hump('USER_ID'))
-# print(to_hump('userId'))
-# print(to_hump('user'))
-# print(to_hump(''))
-
-# print(to_hump_more('userId'))
-
-# print(to_underline('userId'))
-
-
-# print(uuid_random(5))
-# print(uuid_random(10))
-# print(uuid_random())
-# print(uuid_random(32))
-# print(uuid_random(64))
-# print(uuid_random(128))
-# print(uuid_random(127))
-# print(uuid_random(129))
-
-
-# print(to_int('a'))
-# print(to_int(2))
-# print(to_int(2.2))
-# print(to_int(2.2))
-
-# print(to_float('a'))
-# print(to_float(2))
-# print(to_float(2.2))
-# print(to_float(2.24))
-
-# print(to_date('2019-09'))
-# print(to_date('2019-09-08'))
-# print(to_date('2019-09-08 12'))
-# print(to_date('2019-09-08 12:13'))
-# print(to_datetime('2019-09-08 12:13:14'))
-# print(to_datetime('2019-09-08 12:13:14.789'))
-# print(to_datetime(1686537485))
-# print(to_datetime(1686537484467))
-# print(to_datetime(datetime.today()))
-#
-# print(do_md5())
-# print(do_md5())
-# print(do_md5('yangpu'))
-# print(do_md5('yangpu12'))
-#
-# log_msg = ''
-# headers = {'Content-Type': 'application/json;charset=utf-8'}
-# data = {}
-# data['merchantId'] = "merchantId"
-# data['currency'] = "IDR"
-# data['accType'] = "payout"
-# data['version'] = "1.0"
-# sign = sort_by_json_key(data)
-# print(sign)
-# hash = hashlib.sha256()
-# hash.update(sign.encode('utf-8'))
-# data['sign'] = hash.hexdigest()
-#
-# print(data)
-
-
-# print(get_file_data_line(r'D:\notepad_file\202306\fasdfsadfaf.txt', 'payout', from_last=False))
-
-# get_file_data_line(r'D:\notepad_file\202306', 'a')
-# get_file_by_content(r'D:\notepad_file\202306', 'a')
-# print(get_file(r'D:\notepad_file\202306', 'a'))
-# print(get_file(r'D:\notepad_file\202306'))
-# print(get_file())
-# print(os.path.abspath('.'))
 
+# data_list = []
+# for i in range(100000):
+#     data_list.append([i, int(random.uniform(0, 1000))])
+#
+# to_chart_one(data_list)
 
 # print('end')
```

### Comparing `yplib-1.1.6/yplib/chart_html.py` & `yplib-1.1.7/yplib/chart_html.py`

 * *Files 11% similar despite different names*

```diff
@@ -69,14 +69,83 @@
              '        -legend-,' \
              '    },' \
              '    series: -series-,' \
              '}'
     return chart_html(option)
 
 
+# 折线图的 html 模板代码
+def line_area_html():
+    option = '{' \
+             '  tooltip: {' \
+             '    trigger: "axis",' \
+             '    position: function (pt) {' \
+             '      return [pt[0], "10%"];' \
+             '    }' \
+             '  },' \
+             '  title: {' \
+             '    left: "center",' \
+             '    text: "-chart_name-"' \
+             '  },' \
+             '  toolbox: {' \
+             '    feature: {' \
+             '      dataZoom: {' \
+             '        yAxisIndex: "none"' \
+             '      },' \
+             '      restore: {},' \
+             '      saveAsImage: {}' \
+             '    }' \
+             '  },' \
+             '  xAxis: {' \
+             '    type: "category",' \
+             '    boundaryGap: false,' \
+             '    data: -x_list-' \
+             '  },' \
+             '  yAxis: {' \
+             '    type: "value",' \
+             '    boundaryGap: [0, "100%"]' \
+             '  },' \
+             '  dataZoom: [' \
+             '    {' \
+             '      type: "inside",' \
+             '      start: 0,' \
+             '      end: 10' \
+             '    },' \
+             '    {' \
+             '      start: 0,' \
+             '      end: 10' \
+             '    }' \
+             '  ],' \
+             '  series: [' \
+             '    {' \
+             '      type: "line",' \
+             '      symbol: "none",' \
+             '      sampling: "lttb",' \
+             '      itemStyle: {' \
+             '        color: "rgb(255, 70, 131)"' \
+             '      },' \
+             '      areaStyle: {' \
+             '        color: new echarts.graphic.LinearGradient(0, 0, 0, 1, [' \
+             '          {' \
+             '            offset: 0,' \
+             '            color: "rgb(255, 158, 68)"' \
+             '          },' \
+             '          {' \
+             '            offset: 1,' \
+             '            color: "rgb(255, 70, 131)"' \
+             '          }' \
+             '        ])' \
+             '      },' \
+             '      data: -y_list-' \
+             '    }' \
+             '  ]' \
+             '}'
+    return chart_html(option)
+
+
 # 饼图的 html 模板代码
 def pie_html():
     option = '{' \
              '  title: {' \
              '    text: "-chart_name-",' \
              '    left: 10' \
              '  },' \
```

### Comparing `yplib-1.1.6/yplib/file.py` & `yplib-1.1.7/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.1.6/yplib/index.py` & `yplib-1.1.7/yplib/index.py`

 * *Files identical despite different names*

