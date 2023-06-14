# Comparing `tmp/xToolkit-0.0.84.tar.gz` & `tmp/xToolkit-0.0.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xToolkit-0.0.84.tar", last modified: Wed May 17 07:42:36 2023, max compression
+gzip compressed data, was "dist\xToolkit-0.0.85.tar", last modified: Wed Jun 14 02:27:44 2023, max compression
```

## Comparing `xToolkit-0.0.84.tar` & `xToolkit-0.0.85.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.797854 xToolkit-0.0.84/
--rw-rw-rw-   0        0        0    25597 2023-05-17 07:42:36.797854 xToolkit-0.0.84/PKG-INFO
--rw-rw-rw-   0        0        0    25307 2023-05-17 07:34:59.000000 xToolkit-0.0.84/README.md
--rw-rw-rw-   0        0        0       42 2023-05-17 07:42:36.797854 xToolkit-0.0.84/setup.cfg
--rw-rw-rw-   0        0        0     1145 2023-05-17 07:37:10.000000 xToolkit-0.0.84/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.694696 xToolkit-0.0.84/xToolkit/
--rw-rw-rw-   0        0        0      558 2022-07-06 09:57:21.000000 xToolkit-0.0.84/xToolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.705722 xToolkit-0.0.84/xToolkit/xdatetime/
--rw-rw-rw-   0        0        0      313 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xdatetime/__init__.py
--rw-rw-rw-   0        0        0     3289 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xdatetime/api.py
-drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.727514 xToolkit-0.0.84/xToolkit/xdatetime/xdatetime/
--rw-rw-rw-   0        0        0      260 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xdatetime/xdatetime/__init__.py
--rw-rw-rw-   0        0        0    13012 2022-07-06 08:51:30.000000 xToolkit-0.0.84/xToolkit/xdatetime/xdatetime/xdatetime.py
-drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.731945 xToolkit-0.0.84/xToolkit/xfile/
--rw-rw-rw-   0        0        0      320 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xfile/__init__.py
--rw-rw-rw-   0        0        0      976 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xfile/api.py
-drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.734944 xToolkit-0.0.84/xToolkit/xfile/dispose/
--rw-rw-rw-   0        0        0      260 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xfile/dispose/__init__.py
--rw-rw-rw-   0        0        0     4771 2022-07-06 09:15:56.000000 xToolkit-0.0.84/xToolkit/xfile/dispose/dispose.py
-drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.748558 xToolkit-0.0.84/xToolkit/xhotchpotch/
--rw-rw-rw-   0        0        0      356 2022-07-06 09:43:23.000000 xToolkit-0.0.84/xToolkit/xhotchpotch/__init__.py
--rw-rw-rw-   0        0        0      907 2022-07-07 01:20:46.000000 xToolkit-0.0.84/xToolkit/xhotchpotch/api.py
-drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.759631 xToolkit-0.0.84/xToolkit/xhotchpotch/dispose/
--rw-rw-rw-   0        0        0        0 2022-07-06 09:19:47.000000 xToolkit-0.0.84/xToolkit/xhotchpotch/dispose/__init__.py
--rw-rw-rw-   0        0        0     1773 2022-07-07 01:20:46.000000 xToolkit-0.0.84/xToolkit/xhotchpotch/dispose/dispose.py
-drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.766071 xToolkit-0.0.84/xToolkit/xlist/
--rw-rw-rw-   0        0        0      329 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xlist/__init__.py
--rw-rw-rw-   0        0        0      903 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xlist/api.py
-drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.769071 xToolkit-0.0.84/xToolkit/xlist/dispose/
--rw-rw-rw-   0        0        0      268 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xlist/dispose/__init__.py
--rw-rw-rw-   0        0        0     1636 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xlist/dispose/dispose.py
-drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.773073 xToolkit-0.0.84/xToolkit/xstring/
--rw-rw-rw-   0        0        0      338 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xstring/__init__.py
--rw-rw-rw-   0        0        0     1818 2023-05-17 07:33:53.000000 xToolkit-0.0.84/xToolkit/xstring/api.py
-drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.780142 xToolkit-0.0.84/xToolkit/xstring/check/
--rw-rw-rw-   0        0        0      255 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xstring/check/__init__.py
--rw-rw-rw-   0        0        0    12135 2023-05-17 07:33:53.000000 xToolkit-0.0.84/xToolkit/xstring/check/check.py
-drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.783151 xToolkit-0.0.84/xToolkit/xstring/dispose/
--rw-rw-rw-   0        0        0      260 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xstring/dispose/__init__.py
--rw-rw-rw-   0        0        0     5693 2022-07-06 08:41:33.000000 xToolkit-0.0.84/xToolkit/xstring/dispose/dispose.py
--rw-rw-rw-   0        0        0     3648 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xstring/xstring.py
-drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.786109 xToolkit-0.0.84/xToolkit/xthreading/
--rw-rw-rw-   0        0        0      293 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xthreading/__init__.py
--rw-rw-rw-   0        0        0     1727 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xthreading/xthread.py
-drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.796186 xToolkit-0.0.84/xToolkit/xtoolkit/
--rw-rw-rw-   0        0        0      254 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xtoolkit/__init__.py
--rw-rw-rw-   0        0        0     3108 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xtoolkit/judgement.py
--rw-rw-rw-   0        0        0      441 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xtoolkit/xtoolkit.py
-drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.702724 xToolkit-0.0.84/xToolkit.egg-info/
--rw-rw-rw-   0        0        0    25597 2023-05-17 07:42:36.000000 xToolkit-0.0.84/xToolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1091 2023-05-17 07:42:36.000000 xToolkit-0.0.84/xToolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 07:42:36.000000 xToolkit-0.0.84/xToolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-05-17 07:42:36.000000 xToolkit-0.0.84/xToolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-17 07:42:36.000000 xToolkit-0.0.84/xToolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.625615 xToolkit-0.0.85/
+-rw-rw-rw-   0        0        0    25986 2023-06-14 02:27:44.625615 xToolkit-0.0.85/PKG-INFO
+-rw-rw-rw-   0        0        0    25696 2023-06-12 08:08:30.000000 xToolkit-0.0.85/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 02:27:44.625615 xToolkit-0.0.85/setup.cfg
+-rw-rw-rw-   0        0        0     1145 2023-06-14 02:27:34.000000 xToolkit-0.0.85/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.543453 xToolkit-0.0.85/xToolkit/
+-rw-rw-rw-   0        0        0      558 2022-07-06 09:57:21.000000 xToolkit-0.0.85/xToolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.552447 xToolkit-0.0.85/xToolkit/xdatetime/
+-rw-rw-rw-   0        0        0      313 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xdatetime/__init__.py
+-rw-rw-rw-   0        0        0     3289 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xdatetime/api.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.555472 xToolkit-0.0.85/xToolkit/xdatetime/xdatetime/
+-rw-rw-rw-   0        0        0      260 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xdatetime/xdatetime/__init__.py
+-rw-rw-rw-   0        0        0    13012 2022-07-06 08:51:30.000000 xToolkit-0.0.85/xToolkit/xdatetime/xdatetime/xdatetime.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.558501 xToolkit-0.0.85/xToolkit/xfile/
+-rw-rw-rw-   0        0        0      320 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xfile/__init__.py
+-rw-rw-rw-   0        0        0      976 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xfile/api.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.562500 xToolkit-0.0.85/xToolkit/xfile/dispose/
+-rw-rw-rw-   0        0        0      260 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xfile/dispose/__init__.py
+-rw-rw-rw-   0        0        0     4771 2022-07-06 09:15:56.000000 xToolkit-0.0.85/xToolkit/xfile/dispose/dispose.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.568500 xToolkit-0.0.85/xToolkit/xhotchpotch/
+-rw-rw-rw-   0        0        0      356 2022-07-06 09:43:23.000000 xToolkit-0.0.85/xToolkit/xhotchpotch/__init__.py
+-rw-rw-rw-   0        0        0      907 2022-07-07 01:20:46.000000 xToolkit-0.0.85/xToolkit/xhotchpotch/api.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.573306 xToolkit-0.0.85/xToolkit/xhotchpotch/dispose/
+-rw-rw-rw-   0        0        0        0 2022-07-06 09:19:47.000000 xToolkit-0.0.85/xToolkit/xhotchpotch/dispose/__init__.py
+-rw-rw-rw-   0        0        0     1773 2022-07-07 01:20:46.000000 xToolkit-0.0.85/xToolkit/xhotchpotch/dispose/dispose.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.586511 xToolkit-0.0.85/xToolkit/xlist/
+-rw-rw-rw-   0        0        0      329 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xlist/__init__.py
+-rw-rw-rw-   0        0        0      903 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xlist/api.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.590863 xToolkit-0.0.85/xToolkit/xlist/dispose/
+-rw-rw-rw-   0        0        0      268 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xlist/dispose/__init__.py
+-rw-rw-rw-   0        0        0     1636 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xlist/dispose/dispose.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.595052 xToolkit-0.0.85/xToolkit/xstring/
+-rw-rw-rw-   0        0        0      338 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xstring/__init__.py
+-rw-rw-rw-   0        0        0     1818 2023-05-17 07:33:53.000000 xToolkit-0.0.85/xToolkit/xstring/api.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.608459 xToolkit-0.0.85/xToolkit/xstring/check/
+-rw-rw-rw-   0        0        0      255 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xstring/check/__init__.py
+-rw-rw-rw-   0        0        0    13737 2023-06-14 02:23:04.000000 xToolkit-0.0.85/xToolkit/xstring/check/check.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.610460 xToolkit-0.0.85/xToolkit/xstring/dispose/
+-rw-rw-rw-   0        0        0      260 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xstring/dispose/__init__.py
+-rw-rw-rw-   0        0        0     5693 2022-07-06 08:41:33.000000 xToolkit-0.0.85/xToolkit/xstring/dispose/dispose.py
+-rw-rw-rw-   0        0        0     3648 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xstring/xstring.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.613461 xToolkit-0.0.85/xToolkit/xthreading/
+-rw-rw-rw-   0        0        0      293 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xthreading/__init__.py
+-rw-rw-rw-   0        0        0     1727 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xthreading/xthread.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.623617 xToolkit-0.0.85/xToolkit/xtoolkit/
+-rw-rw-rw-   0        0        0      254 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xtoolkit/__init__.py
+-rw-rw-rw-   0        0        0     3108 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xtoolkit/judgement.py
+-rw-rw-rw-   0        0        0      441 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xtoolkit/xtoolkit.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.549445 xToolkit-0.0.85/xToolkit.egg-info/
+-rw-rw-rw-   0        0        0    25986 2023-06-14 02:27:44.000000 xToolkit-0.0.85/xToolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1091 2023-06-14 02:27:44.000000 xToolkit-0.0.85/xToolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 02:27:44.000000 xToolkit-0.0.85/xToolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-06-14 02:27:44.000000 xToolkit-0.0.85/xToolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-14 02:27:44.000000 xToolkit-0.0.85/xToolkit.egg-info/top_level.txt
```

### Comparing `xToolkit-0.0.84/PKG-INFO` & `xToolkit-0.0.85/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: xToolkit
-Version: 0.0.84
-Summary: UNKNOWN
-Home-page: https://github.com/xionglihong/xToolkit
-Author: xionglihong
-Author-email: xionglihong@163.com
-License: GNU General Public License v3.0
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 # 1 什么是xToolkit库
 
 库xToolkit的中文名字叫Ｘ工具集．是python内置库的一个扩展库.把python的datetime,string,list,dist，xthread等数据结构进行了系统库功能的扩展。
 
 安装方法(利用阿里云的pypi源安装会比默认的pypi快很多)：
 
 ```shell
@@ -596,14 +585,15 @@
         # 参数校验
         parameter = {
             "rests_license": ParameterVerify(request, "rests_license", rule="is_url_list"),
             "limit": ParameterVerify(request, "limit", rule="is_int"),
             "shopping_sign": ParameterVerify(request, "shopping_sign", rule="casual"),  # 商店标识
             "title": ParameterVerify(request, "title", rule="casual"),
             "distribution": ParameterVerify(request, "distribution", rule="is_choices", choices=["快递", "线下取货"]),
+            "phoenix": ParameterVerify(request, "cn123451", regular="cn\d{6}(?!\d)"),  # 微鳯号
         }
 
         for key, item in parameter.items():
             if item is False:
                 return GlobalReturn(code=10001, msg="{}为{}，格式错误".format(key, item))
 
         return GlobalReturn(**OperationOrderForm().select_order_list(request=request, **parameter))
@@ -641,14 +631,15 @@
 | is_casual_list          | 任意列表         | 列表里面的值不进行校验，只能确保整体是一个列表 |
 
 参数说明 xstring.formative(parameter, **kwargs)：
 
 - parameter 为需要校验的参数名称
 - is_blank 是否可以为空，如果可以为空，不进行规则校验，直接返回空字符串，如果用户传了，就进行规则校验
 - rule 为正则标识，如果rule为is_choices，必须传choices，choices为枚举值，choices的类型为列表
+- regular 为自定义正则表达式，如果传入自定义正则表达式就使用用户的正则表达式
 
 
 
 ## 3.3 多线程模块xthread
 
 ### 3.3.1 多线程模块
 
@@ -914,9 +905,9 @@
 
 2022年05月17日 V0.0.84
 
 - 复合参数校验添加自定义正则表达式校验
 
 开发计划：
 
-- 无
-
+- 加入微鳯号校验，经纬度格式校验，版本号，大陆联系号码正则表达式校验
+- 密码校验改为必须包含数字和字母，可以包含字符，6到18位
```

### Comparing `xToolkit-0.0.84/README.md` & `xToolkit-0.0.85/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: xToolkit
+Version: 0.0.85
+Summary: UNKNOWN
+Home-page: https://github.com/xionglihong/xToolkit
+Author: xionglihong
+Author-email: xionglihong@163.com
+License: GNU General Public License v3.0
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
 # 1 什么是xToolkit库
 
 库xToolkit的中文名字叫Ｘ工具集．是python内置库的一个扩展库.把python的datetime,string,list,dist，xthread等数据结构进行了系统库功能的扩展。
 
 安装方法(利用阿里云的pypi源安装会比默认的pypi快很多)：
 
 ```shell
@@ -585,14 +596,15 @@
         # 参数校验
         parameter = {
             "rests_license": ParameterVerify(request, "rests_license", rule="is_url_list"),
             "limit": ParameterVerify(request, "limit", rule="is_int"),
             "shopping_sign": ParameterVerify(request, "shopping_sign", rule="casual"),  # 商店标识
             "title": ParameterVerify(request, "title", rule="casual"),
             "distribution": ParameterVerify(request, "distribution", rule="is_choices", choices=["快递", "线下取货"]),
+            "phoenix": ParameterVerify(request, "cn123451", regular="cn\d{6}(?!\d)"),  # 微鳯号
         }
 
         for key, item in parameter.items():
             if item is False:
                 return GlobalReturn(code=10001, msg="{}为{}，格式错误".format(key, item))
 
         return GlobalReturn(**OperationOrderForm().select_order_list(request=request, **parameter))
@@ -630,14 +642,15 @@
 | is_casual_list          | 任意列表         | 列表里面的值不进行校验，只能确保整体是一个列表 |
 
 参数说明 xstring.formative(parameter, **kwargs)：
 
 - parameter 为需要校验的参数名称
 - is_blank 是否可以为空，如果可以为空，不进行规则校验，直接返回空字符串，如果用户传了，就进行规则校验
 - rule 为正则标识，如果rule为is_choices，必须传choices，choices为枚举值，choices的类型为列表
+- regular 为自定义正则表达式，如果传入自定义正则表达式就使用用户的正则表达式
 
 
 
 ## 3.3 多线程模块xthread
 
 ### 3.3.1 多线程模块
 
@@ -903,8 +916,10 @@
 
 2022年05月17日 V0.0.84
 
 - 复合参数校验添加自定义正则表达式校验
 
 开发计划：
 
-- 无
+- 加入微鳯号校验，经纬度格式校验，版本号，大陆联系号码正则表达式校验
+- 密码校验改为必须包含数字和字母，可以包含字符，6到18位
+
```

### Comparing `xToolkit-0.0.84/setup.py` & `xToolkit-0.0.85/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.84'
+VERSION = '0.0.85'
 
 # 导入信息说明文档
 with open("README.md", "r", encoding="UTF-8") as fh:
     long_description = fh.read()
 
 setup(
     name='xToolkit',
```

### Comparing `xToolkit-0.0.84/xToolkit/__init__.py` & `xToolkit-0.0.85/xToolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.84/xToolkit/xdatetime/api.py` & `xToolkit-0.0.85/xToolkit/xdatetime/api.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.84/xToolkit/xdatetime/xdatetime/xdatetime.py` & `xToolkit-0.0.85/xToolkit/xdatetime/xdatetime/xdatetime.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.84/xToolkit/xfile/api.py` & `xToolkit-0.0.85/xToolkit/xfile/api.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.84/xToolkit/xfile/dispose/dispose.py` & `xToolkit-0.0.85/xToolkit/xfile/dispose/dispose.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.84/xToolkit/xhotchpotch/api.py` & `xToolkit-0.0.85/xToolkit/xhotchpotch/api.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.84/xToolkit/xhotchpotch/dispose/dispose.py` & `xToolkit-0.0.85/xToolkit/xhotchpotch/dispose/dispose.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.84/xToolkit/xlist/api.py` & `xToolkit-0.0.85/xToolkit/xlist/api.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.84/xToolkit/xlist/dispose/dispose.py` & `xToolkit-0.0.85/xToolkit/xlist/dispose/dispose.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.84/xToolkit/xstring/api.py` & `xToolkit-0.0.85/xToolkit/xstring/api.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.84/xToolkit/xstring/check/check.py` & `xToolkit-0.0.85/xToolkit/xstring/check/check.py`

 * *Files 10% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 
     # 密码
     @property
     def is_user_password(self):
         """
         包含6-18位字符，必须包含字母与数字，可以包含特殊字符
         """
-        expression = "^(?![0-9]+$)(?![a-zA-Z]+$)[0-9A-Za-z\\W]{6,18}$"
+        expression = "^(?![0-9]+$)(?![a-zA-Z]+$)[0-9A-Za-z\W]{6,18}$"
         return self.__regular_expression(expression)
 
     # 邮箱
     @property
     def is_mailbox(self):
         """
         第一种：只允许英文字母、数字、下划线、英文句号、以及中划线组成
@@ -175,21 +175,68 @@
         工号格式为 4个大写字母+8位数字
         """
         expression = "^[A-Z]{4}\d{8}"
         return self.__regular_expression(expression)
 
     # ip地址
     @property
-    def ip_address(self):
+    def is_ip_address(self):
         """
         ip地址,ip4
         """
         expression = "^(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$"
         return self.__regular_expression(expression)
 
+    # 经纬度
+    @property
+    def is_longitude_latitude(self):
+        print("-")
+        """
+        经纬度，格式为：纬度，经度
+        其中纬度的范围在-90到90之间，经度的范围在-180到180之间
+        """
+        expression = "^[-]?([1-8]?\d(\.\d+)?|90(\.0+)?)\s*[,]\s*[-]?(180(\.0+)?|((1[0-7]\d)|([1-9]?\d))(\.\d+)?)$"
+        return self.__regular_expression(expression)
+
+    # 微鳯号
+    @property
+    def is_phoenix(self):
+        """
+        cn开头，后面有且只有6位数
+        """
+        expression = "cn\d{6}(?!\d)"
+        return self.__regular_expression(expression)
+
+    # 验证码
+    @property
+    def is_verification_code(self):
+        """
+        4位，数字和字母
+        """
+        expression = "^[a-zA-Z0-9]{4}$"
+        return self.__regular_expression(expression)
+
+    # 版本号
+    @property
+    def is_version(self):
+        """
+        版本号 格式为 V0.0.1
+        """
+        expression = "^V[0-99]\.[0-99]\.[1-99]$"
+        return self.__regular_expression(expression)
+
+    # 电话号码
+    @property
+    def is_contact_information(self):
+        """
+        包括中国大陆的手机号码和固定电话号码
+        """
+        expression = "^(((\d{3,4}-)?[0-9]{7,8})|(1(3|4|5|6|7|8|9)\d{9}))$"
+        return self.__regular_expression(expression)
+
 
 # 高级校验模块
 class FormativeCheck(CheckData):
     """
     高级校验模块
 
     接收用户的参数并进行校验
@@ -201,25 +248,28 @@
 
     def __init__(self, parameter):
         super().__init__(parameter)
         self.parameter = parameter
         self.rule_usual_list = [
             "is_car_number", "is_identity_card", "is_int_or_float", "is_int",  # 车牌号,身份证,整形或浮点型,整形
             "is_datetime_string", "is_url", "is_phone", "is_bank_number",  # 时间字符串,url地址,手机号,银行卡
-            "is_user_name", "is_user_password", "is_mailbox", "ip_address",  # 用户姓名,密码,邮箱,ip地址
+            "is_user_name", "is_user_password", "is_mailbox", "is_ip_address",  # 用户姓名,密码,邮箱,ip地址
+            "is_longitude_latitude", "is_phoenix", "is_verification_code",  # 经纬度,微鳯号,验证码,电话号码
+            "is_version", "is_contact_information",  # 版本号,电话号码
         ]
         self.rule_list_list = ["{}_list".format(key) for key in self.rule_usual_list]
 
     # 正则校验
     def regular(self, rule, **kwargs):
         """
         正则校验
         """
         if rule in self.rule_usual_list:
             return eval("self.{}".format(rule))
+
         # JSON
         elif rule == "is_json":
             # noinspection PyBroadException
             try:
                 # 不能用ast，因为ast的处理能力太强，各种格式都不报错，无法触发tey
                 resource = json.loads(self.parameter)
                 return True if isinstance(resource, dict) else False
```

### Comparing `xToolkit-0.0.84/xToolkit/xstring/dispose/dispose.py` & `xToolkit-0.0.85/xToolkit/xstring/dispose/dispose.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.84/xToolkit/xstring/xstring.py` & `xToolkit-0.0.85/xToolkit/xstring/xstring.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.84/xToolkit/xthreading/xthread.py` & `xToolkit-0.0.85/xToolkit/xthreading/xthread.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.84/xToolkit/xtoolkit/judgement.py` & `xToolkit-0.0.85/xToolkit/xtoolkit/judgement.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.84/xToolkit.egg-info/PKG-INFO` & `xToolkit-0.0.85/xToolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xToolkit
-Version: 0.0.84
+Version: 0.0.85
 Summary: UNKNOWN
 Home-page: https://github.com/xionglihong/xToolkit
 Author: xionglihong
 Author-email: xionglihong@163.com
 License: GNU General Public License v3.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -596,14 +596,15 @@
         # 参数校验
         parameter = {
             "rests_license": ParameterVerify(request, "rests_license", rule="is_url_list"),
             "limit": ParameterVerify(request, "limit", rule="is_int"),
             "shopping_sign": ParameterVerify(request, "shopping_sign", rule="casual"),  # 商店标识
             "title": ParameterVerify(request, "title", rule="casual"),
             "distribution": ParameterVerify(request, "distribution", rule="is_choices", choices=["快递", "线下取货"]),
+            "phoenix": ParameterVerify(request, "cn123451", regular="cn\d{6}(?!\d)"),  # 微鳯号
         }
 
         for key, item in parameter.items():
             if item is False:
                 return GlobalReturn(code=10001, msg="{}为{}，格式错误".format(key, item))
 
         return GlobalReturn(**OperationOrderForm().select_order_list(request=request, **parameter))
@@ -641,14 +642,15 @@
 | is_casual_list          | 任意列表         | 列表里面的值不进行校验，只能确保整体是一个列表 |
 
 参数说明 xstring.formative(parameter, **kwargs)：
 
 - parameter 为需要校验的参数名称
 - is_blank 是否可以为空，如果可以为空，不进行规则校验，直接返回空字符串，如果用户传了，就进行规则校验
 - rule 为正则标识，如果rule为is_choices，必须传choices，choices为枚举值，choices的类型为列表
+- regular 为自定义正则表达式，如果传入自定义正则表达式就使用用户的正则表达式
 
 
 
 ## 3.3 多线程模块xthread
 
 ### 3.3.1 多线程模块
 
@@ -914,9 +916,10 @@
 
 2022年05月17日 V0.0.84
 
 - 复合参数校验添加自定义正则表达式校验
 
 开发计划：
 
-- 无
+- 加入微鳯号校验，经纬度格式校验，版本号，大陆联系号码正则表达式校验
+- 密码校验改为必须包含数字和字母，可以包含字符，6到18位
```

### Comparing `xToolkit-0.0.84/xToolkit.egg-info/SOURCES.txt` & `xToolkit-0.0.85/xToolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

