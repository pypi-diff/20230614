# Comparing `tmp/cloudpss-3.2.0a2.tar.gz` & `tmp/cloudpss-3.5.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cloudpss-3.2.0a2.tar", last modified: Mon Aug  1 08:13:49 2022, max compression
+gzip compressed data, was "dist\cloudpss-3.5.0a1.tar", last modified: Mon May 15 02:52:40 2023, max compression
```

## Comparing `cloudpss-3.2.0a2.tar` & `cloudpss-3.5.0a1.tar`

### file list

```diff
@@ -1,47 +1,63 @@
-drwxrwxrwx   0        0        0        0 2022-08-01 08:13:49.000000 cloudpss-3.2.0a2/
--rw-rw-rw-   0        0        0     2364 2022-08-01 08:13:49.000000 cloudpss-3.2.0a2/PKG-INFO
--rw-rw-rw-   0        0        0     1760 2022-08-01 03:22:41.000000 cloudpss-3.2.0a2/README.md
-drwxrwxrwx   0        0        0        0 2022-08-01 08:13:49.000000 cloudpss-3.2.0a2/cloudpss/
--rw-rw-rw-   0        0        0      669 2022-08-01 08:13:05.000000 cloudpss-3.2.0a2/cloudpss/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-01 08:13:49.000000 cloudpss-3.2.0a2/cloudpss/function/
--rw-rw-rw-   0        0        0     1629 2022-08-01 08:12:21.000000 cloudpss-3.2.0a2/cloudpss/function/__init__.py
--rw-rw-rw-   0        0        0       29 2022-01-20 05:13:06.000000 cloudpss-3.2.0a2/cloudpss/function/function.py
--rw-rw-rw-   0        0        0    14737 2022-08-01 04:53:29.000000 cloudpss-3.2.0a2/cloudpss/function/functionExecution.py
--rw-rw-rw-   0        0        0    13162 2022-07-31 12:40:10.000000 cloudpss-3.2.0a2/cloudpss/function/job.py
-drwxrwxrwx   0        0        0        0 2022-08-01 08:13:49.000000 cloudpss-3.2.0a2/cloudpss/model/
--rw-rw-rw-   0        0        0      151 2021-12-29 02:28:37.000000 cloudpss-3.2.0a2/cloudpss/model/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-01 08:13:49.000000 cloudpss-3.2.0a2/cloudpss/model/implements/
--rw-rw-rw-   0        0        0       67 2021-12-29 06:40:28.000000 cloudpss-3.2.0a2/cloudpss/model/implements/__init__.py
--rw-rw-rw-   0        0        0      734 2021-12-24 02:31:09.000000 cloudpss-3.2.0a2/cloudpss/model/implements/component.py
--rw-rw-rw-   0        0        0     1063 2021-12-24 02:31:09.000000 cloudpss-3.2.0a2/cloudpss/model/implements/diagram.py
--rw-rw-rw-   0        0        0      954 2021-12-29 06:40:28.000000 cloudpss-3.2.0a2/cloudpss/model/implements/implement.py
--rw-rw-rw-   0        0        0     2755 2021-12-29 06:40:28.000000 cloudpss-3.2.0a2/cloudpss/model/jobDefinitions.py
--rw-rw-rw-   0        0        0    16144 2022-01-19 08:08:22.000000 cloudpss-3.2.0a2/cloudpss/model/model.py
--rw-rw-rw-   0        0        0     3682 2021-12-29 11:23:01.000000 cloudpss-3.2.0a2/cloudpss/model/revision.py
--rw-rw-rw-   0        0        0     2234 2021-12-29 11:22:22.000000 cloudpss-3.2.0a2/cloudpss/model/topology.py
-drwxrwxrwx   0        0        0        0 2022-08-01 08:13:49.000000 cloudpss-3.2.0a2/cloudpss/project/
--rw-rw-rw-   0        0        0       51 2022-01-06 03:40:26.000000 cloudpss-3.2.0a2/cloudpss/project/__init__.py
--rw-rw-rw-   0        0        0    17721 2022-01-19 08:08:20.000000 cloudpss-3.2.0a2/cloudpss/project/project.py
-drwxrwxrwx   0        0        0        0 2022-08-01 08:13:49.000000 cloudpss-3.2.0a2/cloudpss/runner/
--rw-rw-rw-   0        0        0      241 2021-08-18 04:07:17.000000 cloudpss-3.2.0a2/cloudpss/runner/__init__.py
--rw-rw-rw-   0        0        0     4073 2022-04-07 06:45:11.000000 cloudpss-3.2.0a2/cloudpss/runner/receiver.py
--rw-rw-rw-   0        0        0    11495 2022-01-05 08:46:05.000000 cloudpss-3.2.0a2/cloudpss/runner/result.py
--rw-rw-rw-   0        0        0     3434 2022-08-01 04:58:40.000000 cloudpss-3.2.0a2/cloudpss/runner/runner.py
--rw-rw-rw-   0        0        0     4162 2021-12-29 06:40:28.000000 cloudpss-3.2.0a2/cloudpss/runner/storage.py
--rw-rw-rw-   0        0        0    11613 2021-08-16 11:17:24.000000 cloudpss-3.2.0a2/cloudpss/runner/transform.py
-drwxrwxrwx   0        0        0        0 2022-08-01 08:13:49.000000 cloudpss-3.2.0a2/cloudpss/utils/
--rw-rw-rw-   0        0        0      291 2021-12-24 02:31:13.000000 cloudpss-3.2.0a2/cloudpss/utils/__init__.py
--rw-rw-rw-   0        0        0      885 2021-12-24 03:16:00.000000 cloudpss-3.2.0a2/cloudpss/utils/dataEncoder.py
--rw-rw-rw-   0        0        0      255 2022-01-06 03:40:44.000000 cloudpss-3.2.0a2/cloudpss/utils/graphqlUtil.py
--rw-rw-rw-   0        0        0     1321 2022-01-06 04:32:27.000000 cloudpss-3.2.0a2/cloudpss/utils/httprequests.py
--rw-rw-rw-   0        0        0      795 2021-08-13 08:49:11.000000 cloudpss-3.2.0a2/cloudpss/utils/matlab.py
--rw-rw-rw-   0        0        0     2885 2021-12-24 03:16:00.000000 cloudpss-3.2.0a2/cloudpss/utils/yamlLoader.py
--rw-rw-rw-   0        0        0      810 2021-12-24 03:16:24.000000 cloudpss-3.2.0a2/cloudpss/verify.py
-drwxrwxrwx   0        0        0        0 2022-08-01 08:13:49.000000 cloudpss-3.2.0a2/cloudpss.egg-info/
--rw-rw-rw-   0        0        0     2364 2022-08-01 08:13:47.000000 cloudpss-3.2.0a2/cloudpss.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1025 2022-08-01 08:13:47.000000 cloudpss-3.2.0a2/cloudpss.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-01 08:13:47.000000 cloudpss-3.2.0a2/cloudpss.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2022-08-01 08:13:47.000000 cloudpss-3.2.0a2/cloudpss.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-08-01 08:13:47.000000 cloudpss-3.2.0a2/cloudpss.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-01 08:13:49.000000 cloudpss-3.2.0a2/setup.cfg
--rw-rw-rw-   0        0        0      801 2022-01-06 04:37:02.000000 cloudpss-3.2.0a2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 02:52:40.000000 cloudpss-3.5.0a1/
+-rw-rw-rw-   0        0        0     2103 2023-05-15 02:52:40.000000 cloudpss-3.5.0a1/PKG-INFO
+-rw-rw-rw-   0        0        0     1760 2023-01-12 12:36:01.000000 cloudpss-3.5.0a1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 02:52:40.000000 cloudpss-3.5.0a1/cloudpss/
+-rw-rw-rw-   0        0        0      760 2023-05-15 02:14:40.000000 cloudpss-3.5.0a1/cloudpss/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 02:52:40.000000 cloudpss-3.5.0a1/cloudpss/function/
+-rw-rw-rw-   0        0        0     1629 2023-01-12 12:36:01.000000 cloudpss-3.5.0a1/cloudpss/function/__init__.py
+-rw-rw-rw-   0        0        0       29 2023-01-12 12:36:01.000000 cloudpss-3.5.0a1/cloudpss/function/function.py
+-rw-rw-rw-   0        0        0    14640 2023-01-12 12:36:01.000000 cloudpss-3.5.0a1/cloudpss/function/functionExecution.py
+-rw-rw-rw-   0        0        0    13162 2023-01-12 12:36:01.000000 cloudpss-3.5.0a1/cloudpss/function/job.py
+drwxrwxrwx   0        0        0        0 2023-05-15 02:52:40.000000 cloudpss-3.5.0a1/cloudpss/ieslab/
+-rw-rw-rw-   0        0        0    19493 2023-05-05 06:18:36.000000 cloudpss-3.5.0a1/cloudpss/ieslab/DataManageModel.py
+-rw-rw-rw-   0        0        0     6452 2023-01-12 13:58:16.000000 cloudpss-3.5.0a1/cloudpss/ieslab/EvaluationModel.py
+-rw-rw-rw-   0        0        0     4422 2023-03-31 06:23:52.000000 cloudpss-3.5.0a1/cloudpss/ieslab/IESLabPlan.py
+-rw-rw-rw-   0        0        0     1700 2023-01-12 13:58:16.000000 cloudpss-3.5.0a1/cloudpss/ieslab/IESLabSimulation.py
+-rw-rw-rw-   0        0        0     3012 2023-01-12 13:58:16.000000 cloudpss-3.5.0a1/cloudpss/ieslab/PlanModel.py
+-rw-rw-rw-   0        0        0      126 2023-01-12 12:36:01.000000 cloudpss-3.5.0a1/cloudpss/ieslab/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 02:52:40.000000 cloudpss-3.5.0a1/cloudpss/model/
+-rw-rw-rw-   0        0        0      151 2023-01-12 12:36:01.000000 cloudpss-3.5.0a1/cloudpss/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 02:52:40.000000 cloudpss-3.5.0a1/cloudpss/model/implements/
+-rw-rw-rw-   0        0        0       67 2023-01-12 12:36:01.000000 cloudpss-3.5.0a1/cloudpss/model/implements/__init__.py
+-rw-rw-rw-   0        0        0      734 2023-01-12 12:36:01.000000 cloudpss-3.5.0a1/cloudpss/model/implements/component.py
+-rw-rw-rw-   0        0        0     1063 2023-01-12 12:36:01.000000 cloudpss-3.5.0a1/cloudpss/model/implements/diagram.py
+-rw-rw-rw-   0        0        0      954 2023-01-12 12:36:01.000000 cloudpss-3.5.0a1/cloudpss/model/implements/implement.py
+-rw-rw-rw-   0        0        0     2755 2023-01-12 12:36:01.000000 cloudpss-3.5.0a1/cloudpss/model/jobDefinitions.py
+-rw-rw-rw-   0        0        0    21858 2023-05-15 02:14:40.000000 cloudpss-3.5.0a1/cloudpss/model/model.py
+-rw-rw-rw-   0        0        0     3758 2023-05-15 02:14:40.000000 cloudpss-3.5.0a1/cloudpss/model/revision.py
+-rw-rw-rw-   0        0        0     2234 2023-01-12 12:36:01.000000 cloudpss-3.5.0a1/cloudpss/model/topology.py
+drwxrwxrwx   0        0        0        0 2023-05-15 02:52:40.000000 cloudpss-3.5.0a1/cloudpss/project/
+-rw-rw-rw-   0        0        0       51 2023-01-12 12:36:01.000000 cloudpss-3.5.0a1/cloudpss/project/__init__.py
+-rw-rw-rw-   0        0        0    17700 2023-01-12 12:36:01.000000 cloudpss-3.5.0a1/cloudpss/project/project.py
+drwxrwxrwx   0        0        0        0 2023-05-15 02:52:40.000000 cloudpss-3.5.0a1/cloudpss/runner/
+-rw-rw-rw-   0        0        0     5232 2023-01-12 13:58:16.000000 cloudpss-3.5.0a1/cloudpss/runner/IESLabEvaluationResult.py
+-rw-rw-rw-   0        0        0     5226 2023-01-12 13:58:16.000000 cloudpss-3.5.0a1/cloudpss/runner/IESLabPlanResult.py
+-rw-rw-rw-   0        0        0     7499 2023-01-12 12:36:01.000000 cloudpss-3.5.0a1/cloudpss/runner/IESLabTypicalDayResult.py
+-rw-rw-rw-   0        0        0     5883 2023-05-15 02:14:40.000000 cloudpss-3.5.0a1/cloudpss/runner/MessageStreamReceiver.py
+-rw-rw-rw-   0        0        0      341 2023-05-15 02:14:40.000000 cloudpss-3.5.0a1/cloudpss/runner/__init__.py
+-rw-rw-rw-   0        0        0     4162 2023-05-15 02:14:40.000000 cloudpss-3.5.0a1/cloudpss/runner/receiver.py
+-rw-rw-rw-   0        0        0    13125 2023-01-12 13:58:16.000000 cloudpss-3.5.0a1/cloudpss/runner/result.py
+-rw-rw-rw-   0        0        0     7146 2023-05-15 02:14:40.000000 cloudpss-3.5.0a1/cloudpss/runner/runner.py
+-rw-rw-rw-   0        0        0     4162 2023-01-12 12:36:01.000000 cloudpss-3.5.0a1/cloudpss/runner/storage.py
+-rw-rw-rw-   0        0        0    11613 2023-01-12 12:36:01.000000 cloudpss-3.5.0a1/cloudpss/runner/transform.py
+drwxrwxrwx   0        0        0        0 2023-05-15 02:52:40.000000 cloudpss-3.5.0a1/cloudpss/utils/
+-rw-rw-rw-   0        0        0     4796 2023-05-15 02:14:40.000000 cloudpss-3.5.0a1/cloudpss/utils/IO.py
+-rw-rw-rw-   0        0        0      326 2023-05-15 02:14:40.000000 cloudpss-3.5.0a1/cloudpss/utils/__init__.py
+-rw-rw-rw-   0        0        0      885 2023-01-12 12:36:01.000000 cloudpss-3.5.0a1/cloudpss/utils/dataEncoder.py
+-rw-rw-rw-   0        0        0      260 2023-05-15 02:14:40.000000 cloudpss-3.5.0a1/cloudpss/utils/graphqlUtil.py
+-rw-rw-rw-   0        0        0     1508 2023-05-15 02:14:40.000000 cloudpss-3.5.0a1/cloudpss/utils/httprequests.py
+-rw-rw-rw-   0        0        0      795 2023-01-12 12:36:01.000000 cloudpss-3.5.0a1/cloudpss/utils/matlab.py
+-rw-rw-rw-   0        0        0     2677 2023-05-15 02:14:40.000000 cloudpss-3.5.0a1/cloudpss/utils/yamlLoader.py
+-rw-rw-rw-   0        0        0      993 2023-03-31 06:18:19.000000 cloudpss-3.5.0a1/cloudpss/verify.py
+drwxrwxrwx   0        0        0        0 2023-05-15 02:52:40.000000 cloudpss-3.5.0a1/cloudpss.egg-info/
+-rw-rw-rw-   0        0        0     2103 2023-05-15 02:52:40.000000 cloudpss-3.5.0a1/cloudpss.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1452 2023-05-15 02:52:40.000000 cloudpss-3.5.0a1/cloudpss.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 02:52:40.000000 cloudpss-3.5.0a1/cloudpss.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2023-05-15 02:52:40.000000 cloudpss-3.5.0a1/cloudpss.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-15 02:52:40.000000 cloudpss-3.5.0a1/cloudpss.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 02:52:40.000000 cloudpss-3.5.0a1/setup.cfg
+-rw-rw-rw-   0        0        0      858 2023-05-15 02:14:40.000000 cloudpss-3.5.0a1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 02:52:40.000000 cloudpss-3.5.0a1/test/
+-rw-rw-rw-   0        0        0     1097 2023-05-05 06:18:36.000000 cloudpss-3.5.0a1/test/test-sdk.py
+-rw-rw-rw-   0        0        0     3091 2023-05-05 06:18:36.000000 cloudpss-3.5.0a1/test/test-snapshot.py
+-rw-rw-rw-   0        0        0     3325 2023-05-05 06:18:36.000000 cloudpss-3.5.0a1/test/test.py
```

### Comparing `cloudpss-3.2.0a2/PKG-INFO` & `cloudpss-3.5.0a1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: cloudpss
-Version: 3.2.0a2
+Version: 3.5.0a1
 Summary: cloudpss sdk
 Home-page: https://www.cloudpss.net
 Author: cloudpss
 Author-email: zhangdaming@cloudpss.net
 License: MIT Licence
-Description: 
-        CloudPSS SDK
-        ----------------------------------------------------------------
-        CloudPSS SDK是基于CloudPSS-API封装的模型及软件开发套件。用户可通过编写Python、Matlab等脚本构建自定义模型，或是调用CloudPSS平台中的模型修改、仿真计算功能，实现诸如自动修改模型、批量仿真计算、自动化生成报告等复杂且繁琐的功能。用户也可在其自己的应用程序中调用CloudPSS仿真引擎，实现仿真驱动的高级分析应用。
-        
-        CloudPSS SDK包含模型层、算法层和应用层三种开发套件，其中：
-        
-        1. `模型层开发套件`帮助用户在CloudPSS SimStudio官方潮流计算、电磁暂态仿真、移频电磁暂态仿真、综合能源能量流计算等内核中开发第三方模型或用户自定义模型。目前，模型层SDK已开放基于Matlab函数的自定义控制元件接入，后续将进一步开放Python、C/C++的标准元件开发套件。
-        2. `算法层开发套件`帮助用户在CloudPSS FuncStudio中集成自己的算法内核，从而借助CloudPSS XStudio平台快速开发并部署自己的计算应用。该部分内容将在年内发布，敬请期待。
-        3. `应用层开发套件`帮助用户在利用脚本的形式快速调用CloudPSS官方计算内核和第三方接入的计算内核，从而方便用户开发高级计算分析应用。其中，SimStudio-SDK现已支持SimStudio中的模型修改和`潮流计算`和`电磁暂态仿真`两种计算内核。
-        
-        
-        ---
-        ### 下载与安装
-        
-        ```[pyhton]
-        pip install cloudpss
-        ```
-        需要`升级`的话，执行下面的命令:
-        ```[pyhton]
-        pip install --upgrade cloudpss
-        ```
-        ### 完全卸载
-        
-        执行下面的命令进行`完全卸载`:
-        ```[pyhton]
-        pip uninstall cloudpss
-        ```
-        
-                  
-        
-        
 Keywords: cloudpss,cloudpss-sdk
 Platform: any
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+
+
+CloudPSS SDK
+----------------------------------------------------------------
+CloudPSS SDK是基于CloudPSS-API封装的模型及软件开发套件。用户可通过编写Python、Matlab等脚本构建自定义模型，或是调用CloudPSS平台中的模型修改、仿真计算功能，实现诸如自动修改模型、批量仿真计算、自动化生成报告等复杂且繁琐的功能。用户也可在其自己的应用程序中调用CloudPSS仿真引擎，实现仿真驱动的高级分析应用。
+
+CloudPSS SDK包含模型层、算法层和应用层三种开发套件，其中：
+
+1. `模型层开发套件`帮助用户在CloudPSS SimStudio官方潮流计算、电磁暂态仿真、移频电磁暂态仿真、综合能源能量流计算等内核中开发第三方模型或用户自定义模型。目前，模型层SDK已开放基于Matlab函数的自定义控制元件接入，后续将进一步开放Python、C/C++的标准元件开发套件。
+2. `算法层开发套件`帮助用户在CloudPSS FuncStudio中集成自己的算法内核，从而借助CloudPSS XStudio平台快速开发并部署自己的计算应用。该部分内容将在年内发布，敬请期待。
+3. `应用层开发套件`帮助用户在利用脚本的形式快速调用CloudPSS官方计算内核和第三方接入的计算内核，从而方便用户开发高级计算分析应用。其中，SimStudio-SDK现已支持SimStudio中的模型修改和`潮流计算`和`电磁暂态仿真`两种计算内核。
+
+
+---
+### 下载与安装
+
+```[pyhton]
+pip install cloudpss
+```
+需要`升级`的话，执行下面的命令:
+```[pyhton]
+pip install --upgrade cloudpss
+```
+### 完全卸载
+
+执行下面的命令进行`完全卸载`:
+```[pyhton]
+pip uninstall cloudpss
+```
+
+          
+
```

### Comparing `cloudpss-3.2.0a2/README.md` & `cloudpss-3.5.0a1/README.md`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a2/cloudpss/function/__init__.py` & `cloudpss-3.5.0a1/cloudpss/function/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a2/cloudpss/function/functionExecution.py` & `cloudpss-3.5.0a1/cloudpss/function/functionExecution.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,14 @@
             self.__abortedEvents()
 
     @staticmethod
     def current():
         """
         获取表示当前执行的 FunctionExecution 单例
         """
-        if FunctionExecution._current is not None:
-            return FunctionExecution._current
         jobId = os.environ.get('CLOUDPSS_JOB_ID', None)
         functionId = os.environ.get('CLOUDPSS_FUNCTION_ID', None)
         executorId = os.environ.get('CLOUDPSS_EXECUTOR_ID', None)
         executorName = os.environ.get('CLOUDPSS_EXECUTOR_NAME', None)
         executorVersion = os.environ.get('CLOUDPSS_EXECUTOR_VERSION', None)
         apiUrl = os.environ.get('CLOUDPSS_API_URL', None)
         gqlUrl = os.environ.get('CLOUDPSS_GQL_URL', None)
```

### Comparing `cloudpss-3.2.0a2/cloudpss/function/job.py` & `cloudpss-3.5.0a1/cloudpss/function/job.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a2/cloudpss/model/implements/component.py` & `cloudpss-3.5.0a1/cloudpss/model/implements/component.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a2/cloudpss/model/implements/diagram.py` & `cloudpss-3.5.0a1/cloudpss/model/implements/diagram.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a2/cloudpss/model/implements/implement.py` & `cloudpss-3.5.0a1/cloudpss/model/implements/implement.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a2/cloudpss/model/jobDefinitions.py` & `cloudpss-3.5.0a1/cloudpss/model/jobDefinitions.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a2/cloudpss/model/model.py` & `cloudpss-3.5.0a1/cloudpss/project/project.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import os
 import re
 import io
 import json
 import yaml
 import gzip
 from copy import deepcopy
-from .revision import ModelRevision
-from .jobDefinitions import JOB_DEFINITIONS
+from ..model.revision import ModelRevision
+from ..model.jobDefinitions import JOB_DEFINITIONS
 from ..utils import request, fileLoad, graphql_request
+from ..model import Model
+from deprecated import deprecated
+from ..verify import userName
 
 
-class Model(object):
+@deprecated(version='3.0', reason="该类将在 5.0 版本移除，请使用 Model 类代替")
+class Project(Model):
     """
         CloudPSS工程类，用于处理加载后的工程数据
 
         实例变量说明：
 
         rid         项目的 rid
 
@@ -27,48 +31,42 @@
         configs     当前项目的所有参数方案
 
         jobs        当前项目的所有计算方案
 
         context     当前项目的上下文相关信息
 
     """
-    def __init__(self, model: dict = {}):
+    def __init__(self, project: dict = {}):
         """
             项目初始化
         """
-        for k, v in model.items():
+        for k, v in project.items():
             if k == 'revision':
-                if 'version' in v and v['version'] == 3:
-                    self.__dict__[k] = ModelRevision(v)
-                else:
-                    raise Exception(
-                        '当前SDK版本（ver 3.X.X）不兼容该项目文件，请先升级项目文件。具体方法：将该项目文件导入至XStudio 3.X.X平台后重新保存至本地后即可。'
-                    )
-
+                self.__dict__[k] = ModelRevision(v)
             else:
                 self.__dict__[k] = v
 
     def __getitem__(self, attr):
-        return super(Model, self).__getattribute__(attr)
+        return super(Project, self).__getattribute__(attr)
 
     def toJSON(self):
         """
             类对象序列化为 dict
             :return: dict
         """
-        model = {**self.__dict__, 'revision': self.revision.toJSON()}
-        return model
+        project = {**self.__dict__, 'revision': self.revision.toJSON()}
+        return project
 
     def getAllComponents(self):
         """
             获取实现
 
             :return: 所有元件信息
 
-            >>> model.getAllComponents()
+            >>> project.getAllComponents()
             {
                 'canvas_0_2': Component 实例
             }
         """
         diagramImplement = self.revision.getImplements().getDiagram()
         if diagramImplement is None:
             raise ValueError('不存在拓扑实现')
@@ -80,21 +78,22 @@
 
             :params str: 元件类型
 
             :type rid: str
 
             :return: 按照元件的 rid 过滤后的 dict<>
 
-            >>> model.getComponentsByRid('model/CloudPSS/newInductorRouter')
+            >>> project.getComponentsByRid('model/CloudPSS/newInductorRouter')
             {
                 'canvas_0_2': Component 实例
             }
 
         """
-
+        if rid.startswith('project/'):
+            rid = rid.replace('project/', 'model/')
         v = self.getAllComponents()
 
         cells = {}
         for key, val in v.items():
 
             if val.shape.endswith('edge'):
                 continue
@@ -108,30 +107,30 @@
         """
             通过元件的 key 获取对应的元件
 
             :params key: key 元件的key
 
             :Return: Component 实例
 
-            >>> model.getComponentByKey('canvas_0_757')
+            >>> project.getComponentByKey('canvas_0_757')
             Component 实例
         """
 
         v = self.getAllComponents()
         return v[componentKey]
 
-    def getModelJob(self, name):
+    def getProjectJob(self, name):
         """
             获取指定名称的计算方案
 
             :params Name: Name 参数名称
 
             :return: 同名计算方案数组
 
-            >>> model.getModelJob('电磁暂态方案 1')
+            >>> project.getProjectJob('电磁暂态方案 1')
         """
         jobs = []
 
         for val in self.jobs:
             if val['name'] == name:
                 jobs.append(val)
 
@@ -145,42 +144,42 @@
             :params jobType:  方案类型 
                 电磁暂态仿真方案 emtp
                 移频电磁暂态仿真方案 sfemt
                 潮流计算方案 powerFlow
 
             :return: 返回一个指定类型的计算方案
 
-            >>> model.createJob('emtp','emtp job')
+            >>> project.createJob('emtp','emtp job')
             计算方案
         """
         job = deepcopy(JOB_DEFINITIONS[jobType])
         job['name'] = name
         return job
 
     def addJob(self, job: dict):
         """
             将计算方案添加到工程中
 
             :params job:  计算方案 dict
 
-            >>> job = model.createJob('emtp','emtp job')
-                model.addJob(job)
+            >>> job = project.createJob('emtp','emtp job')
+                project.addJob(job)
         """
 
         self.jobs.append(job)
 
-    def getModelConfig(self, name):
+    def getProjectConfig(self, name):
         """
             获取指定名称的参数方案
 
             :params name:  参数方案名称
 
             :return: 同名的方案数组
 
-            >>> model.getModelConfig('参数方案 1')
+            >>> project.getProjectConfig('参数方案 1')
         """
         configs = []
 
         for val in self.configs:
             if val['name'] == name:
                 configs.append(val)
 
@@ -191,80 +190,85 @@
             创建一个参数方案
             根据项目的第一个参数方案生成一个方案
             创建出的方案默认不加入到项目中，需要加入请调用 addConfig
             :params name:  参数方案名称
 
             :return: 返回一个参数方案 dict
 
-            >>> job = model.createConfig('my config')
+            >>> job = project.createConfig('my config')
                 参数方案
         """
 
         config = deepcopy(self.configs[0])
         config['name'] = name
         return config
 
     def addConfig(self, config):
         """
             将参数方案添加到工程中
 
             :params config:  参数方案 dict
 
-            >>> config = model.createConfig('my config')
-                model.addConfig(config)
+            >>> config = project.createConfig('my config')
+                project.addConfig(config)
         """
 
         self.configs.append(config)
         return config
 
     @staticmethod
+    @deprecated(version='3.0',
+                reason="该方法将在 5.0 版本移除，请使用 Model.fetchMany 方法代替")
     def fetchMany(name=None, pageSize=10, pageOffset=0):
         """
             获取用户可以运行的项目列表
 
             :params name:  查询名称，模糊查询
             :params pageSize:  分页大小
             :params pageOffset:  分页开始位置
 
             :return: 按分页信息返回项目列表
 
-            >>> data=Model.fetchMany()
+            >>> data=Project.fetchMany()
             [
-                {'rid': 'model/admin/share-test', 'name': '1234', 'description': '1234'}
+                {'rid': 'project/Demo/share-test', 'name': '1234', 'description': '1234'}
                 ...
             ]
         """
 
         r = request('GET',
-                    'api/resources/type/model/permission/write',
+                    'api/resources/type/project/permission/write',
                     params={
                         'page_offset': pageOffset,
                         'page_size': pageSize,
                         'search': name
                     })
-        modelList = json.loads(r.text)
+        projectList = json.loads(r.text)
 
         return [{
             'rid': '/'.join([val['type'], val['owner'], val['key']]),
             'name': val['name'],
             'description': val['description']
-        } for val in modelList]
+        } for val in projectList]
 
     @staticmethod
+    @deprecated(version='3.0', reason="该方法将在 5.0 版本移除，请使用 Model.fetch 方法代替")
     def fetch(rid):
         """
             获取项目
 
             :params rid:  项目 rid 
 
             :return: 返回一个项目实例
 
-            >>> model=Model.fetch('model/Demo/test')
+            >>> project=Project.fetch('project/Demo/test')
 
         """
+        if rid.startswith('project/'):
+            rid = rid.replace('project/', 'model/')
         query = """
             query  t($rid:ResourceId!){
                 model(input:{rid: $rid}) {
                     configs
                     context
                     description
                     jobs
@@ -282,140 +286,157 @@
                         pins
                         version
                     }
                 }
             }
         """
         data = graphql_request(query, {'rid': rid})
-        if 'errors' in data:
+        if "errors" in data:
             raise Exception(data['errors'][0]['message'])
-        return Model(data['data']['model'])
+        return Project(data['data']['model'])
 
     def run(self, job=None, config=None, name=None, **kwargs):
         """
 
             调用仿真 
 
             :params job:  调用仿真时使用的计算方案，不指定将使用算例保存时选中的计算方案
             :params config:  调用仿真时使用的参数方案，不指定将使用算例保存时选中的参数方案
             :params name:  任务名称，为空时使用项目的参数方案名称和计算方案名称
 
             :return: 返回一个运行实例
 
-            >>> runner=model.run(job,config,'')
+            >>> runner=project.run(job,config,'')
             runner
 
         """
         if job is None:
             currentJob = self.context['currentJob']
             job = self.jobs[currentJob]
         if config is None:
             currentConfig = self.context['currentConfig']
             config = self.configs[currentConfig]
-
+        # output_channels= job['args']['output_channels']
+        output_channels = []
+        if 'output_channels' in job['args']:
+            for output in job['args']['output_channels']:
+                if type(output) is list and len(output) > 0:
+                    output_channels.append({
+                        '0': output[0],
+                        '1': output[1],
+                        '2': output[2],
+                        '3': output[3],
+                        '4': output[4].split(','),
+                    })
+                    continue
+                output_channels.append(output)
+        job['args']['output_channels'] = output_channels
         return self.revision.run(job, config, name, self.rid, **kwargs)
 
     @staticmethod
+    @deprecated(version='3.0', reason="该方法将在 5.0 版本移除，请使用 Model.load 方法代替")
     def load(filePath):
         """
             加载本地项目文件
 
             :params file:  文件目录
 
             :return: 返回一个项目实例
 
-            >>> model = Model.load('filePath')
+            >>> project = Project.load('filePath')
 
         """
 
         if not os.path.exists(filePath):
             raise FileNotFoundError('未找到文件')
         data = fileLoad(filePath)
-        return Model(data)
+        return Project(data)
 
     @staticmethod
-    def dump(model, file):
+    @deprecated(version='3.0', reason="该方法将在 5.0 版本移除，请使用 Model.dump 方法代替")
+    def dump(project, file):
         """
             下载项目文件
 
-            :params model:  项目
+            :params project:  项目
             :params file:  文件路径
 
             :return: 无
 
-            >>> Model.dump(model,file)
+            >>> Project.dump(project,file)
         """
 
-        data = model.toJSON()
+        data = project.toJSON()
 
         yamlData = yaml.dump(data)
         with gzip.open(file, 'w') as output:
             with io.TextIOWrapper(output, encoding='utf-8') as enc:
                 enc.write(yamlData)
 
     def save(self, key=None):
         """
             保存/创建项目 
 
             key 不为空时如果远程存在相同的资源名称时将覆盖远程项目。
             key 为空时如果项目 rid 不存在则抛异常，需要重新设置 key。
             如果保存时，当前用户不是该项目的拥有者时，将重新创建项目，重建项目时如果参数的 key 为空将使用当前当前项目的 key 作为资源的 key ，当资源的 key 和远程冲突时保存失败
 
-            :params: model 项目
+            :params: project 项目
             :params: key 资源 id 的唯一标识符，
             
             :return: 保存成功/保存失败
             
-            >>> model.save(model)
-                model.save(model,'newKey') # 另存为新的项目
+            >>> project.save(project)
+                project.save(project,'newKey') # 另存为新的项目
 
         """
-        username = os.environ.get('USER_NAME')
+        username = userName()
 
         if key is not None:
             matchObj = re.match(r'^[-_A-Za-z0-9]+$', key, re.I | re.S)
             if matchObj:
                 self.rid = 'model/' + username + '/' + key
                 try:
                     r = request('GET', 'api/resources/' + self.rid)
-                    return Model.update(self)
+                    return Project.update(self)
                 except:
-                    return Model.create(self)
+                    return Project.create(self)
             else:
                 raise Exception('key 能包含字母数子和下划线')
         else:
             t = '(?<=/)\\S+(?=/)'
             owner = re.search(t, self.rid)
             if owner is None:
                 raise Exception('rid 错误，请传入 key')
             elif owner[0] != username:
                 rid = re.sub(t, username, self.rid)
                 try:
                     r = request('GET', 'api/resources/' + self.rid)
-                    return Model.create(self)
+                    return Project.create(self)
                 except:
                     raise Exception(rid + ' 该资源已存在，无法重复创建,请修改 key')
 
-        return Model.update(self)
+        return Project.update(self)
 
     @staticmethod
-    def create(model):
+    @deprecated(version='3.0', reason="该方法将在 5.0 版本移除，请使用 Model.create 方法代替")
+    def create(project):
         """
             新建项目 
 
-            :params: model 项目
+            :params: project 项目
 
             :return: 保存成功/保存失败
 
-            >>> Model.create(model)
+            >>> Project.create(project)
             保存成功
         """
-        # Model.update(model)
+        # Project.update(project)
         t = '(?<=/)\\S+(?=/)'
-        username = os.environ.get('USER_NAME')
+        username = userName()
         owner = re.search(t, model.rid)
 
         if owner is None:
             raise Exception('rid 错误，无法保存')
         elif owner[0] != username:
             raise Exception('rid 错误，无法保存')
 
@@ -446,56 +467,60 @@
                         "member": 1,
                         "everyone": auth,
                     },
                 }
             })
 
     @staticmethod
-    def update(model):
+    @deprecated(version='3.0', reason="该方法将在 5.0 版本移除，请使用 Model.update 方法代替")
+    def update(project):
         """
             更新项目 
 
-            :params: model 项目
+            :params: project 项目
 
             :return: 保存成功/保存失败
 
-            >>> Model.update(model)
+            >>> Project.update(project)
         """
 
         t = '(?<=/)\\S+(?=/)'
-        username = os.environ.get('USER_NAME')
-        owner = re.search(t, model.rid)
+        username = userName()
+        owner = re.search(t, project.rid)
 
         if owner is None:
             raise Exception('rid 错误，无法保存')
         elif owner[0] != username:
             raise Exception('rid 错误，无法保存')
 
         modelQuery = """
                     mutation($a:UpdateModelInput!){updateModel(input:$a){
                                          rid
                                 }}
                 """
-        isPublic = model.context.get('auth', '') != 'private'
-        isComponent = model.context.get('category', '') == 'component'
-        publicRead = model.context.get('publicRead', '') != False
+        isPublic = project.context.get('auth', '') != 'private'
+        isComponent = project.context.get('category', '') == 'component'
+        publicRead = project.context.get('publicRead', '') != False
+
         auth = (65539 if publicRead else 65537) if isPublic else 0
-        revision = ModelRevision.create(model.revision, model.revision.hash)
+        project.revision.author = username
+        revision = ModelRevision.create(project.revision,
+                                        project.revision.hash)
 
         return graphql_request(
             modelQuery, {
                 'a': {
-                    'rid': model.rid,
+                    'rid': project.rid,
                     'revision': revision['hash'],
-                    'context': model.context,
-                    'configs': model.configs,
-                    'jobs': model.jobs,
-                    'name': model.name,
-                    'description': model.description,
-                    'tags': model.tags,
+                    'context': project.context,
+                    'configs': project.configs,
+                    'jobs': project.jobs,
+                    'name': project.name,
+                    'description': project.description,
+                    'tags': project.tags,
                     "permissions": {
                         "moderator": 1,
                         "member": 1,
                         "everyone": auth,
                     },
                 }
             })
@@ -511,17 +536,17 @@
 
             :params implementType:  实现类型
             :params config: config 项目参数, 不指定将使用算例保存时选中的参数方案
             :params maximumDepth:  最大递归深度，用于自定义项目中使用 diagram 实现元件展开情况
 
             :return:  一个拓扑实例
 
-            >>> topology=model.fetchTopology()
-                topology=model.fetchTopology(implementType='powerFlow',config=config) # 获取潮流实现的拓扑数据
-                topology=model.fetchTopology(maximumDepth=2) # 获取仅展开 2 层的拓扑数据
+            >>> topology=project.fetchTopology()
+                topology=project.fetchTopology(implementType='powerFlow',config=config) # 获取潮流实现的拓扑数据
+                topology=project.fetchTopology(maximumDepth=2) # 获取仅展开 2 层的拓扑数据
         """
 
         if self.revision is not None:
             if implementType is None:
                 implementType = 'emtp'
             if config is None:
                 currentConfig = self.context['currentConfig']
```

### Comparing `cloudpss-3.2.0a2/cloudpss/model/revision.py` & `cloudpss-3.5.0a1/cloudpss/model/revision.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 from .topology import ModelTopology
 from .implements import ModelImplement
 from ..utils import request, graphql_request
 from ..runner import Runner
 
 
 class ModelRevision(object):
@@ -18,14 +17,15 @@
         pins                项目当前版本的引脚信息
 
         documentation       项目当前版本的文档信息
 
 
 
     """
+
     def __init__(self, revision: dict = {}):
         """
             初始化
         """
         for k, v in revision.items():
             if k == 'implements':
                 self.__dict__[k] = ModelImplement(v)
@@ -51,30 +51,29 @@
             :return: 实现实例
 
             >>> revision.getImplements()
         """
 
         return self.implements
 
-    def run(self, job, config, name=None, rid='', **kwargs):
+    def run(self, job, config, name=None, rid='', policy=None, **kwargs):
         """
             运行某个指定版本的项目
 
             :params job:  调用仿真时使用的计算方案，为空时使用项目的第一个计算方案
             :params config:  调用仿真时使用的参数方案，为空时使用项目的第一个参数方案
             :params name:  任务名称，为空时使用项目的参数方案名称和计算方案名称
             :params rid:  项目rid，可为空
 
             :return: 返回一个运行实例
 
             >>> revision.run(revision,job,config,'')
         """
-
         revision = ModelRevision.create(self)
-        return Runner.create(revision['hash'], job, config, name, rid,
+        return Runner.create(revision['hash'], job, config, name, rid, policy,
                              **kwargs)
 
     @staticmethod
     def create(revision, parentHash=None):
         """
             创建一个新版本
 
@@ -92,14 +91,16 @@
                     }}
                 """
         r = revision.toJSON()
         del r['hash']
         variables = {'a': {**r, 'parent': parentHash}}
 
         r = graphql_request(query, variables)
+        if 'errors' in r:
+            raise Exception(r['errors'])
         return r['data']['createModelRevision']
 
     def fetchTopology(self, implementType, config, maximumDepth):
         """
             获取当前项目版本的拓扑数据
 
             :params implementType:  实现类型
```

### Comparing `cloudpss-3.2.0a2/cloudpss/model/topology.py` & `cloudpss-3.5.0a1/cloudpss/model/topology.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a2/cloudpss/runner/receiver.py` & `cloudpss-3.5.0a1/cloudpss/runner/receiver.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 import os
 import traceback
 from urllib.parse import urlparse, urlunparse
 from .transform import Transformer
 import datetime
 import pytz
 import ssl
+import time
 
 utc_tz = pytz.timezone('UTC')
 
 
 class Receiver(object):
     '''
         socket 接收服务
     '''
-    def __init__(self, taskId, db, url: str = None, **kwargs):
+    def __init__(self, taskId, db, url = None, **kwargs):
         '''
             连接远程服务器接收结果数据
 
             :params: taskId 邮箱
             :params: result 结果实例
             :params: url 地址
 
@@ -58,14 +59,15 @@
             heartbeat ws心跳服务
             __testData__
         '''
         if message == b'--heartbeat--' or message == b'__testData__' or message == '__testData__' or message == '--heartbeat--':
             return
         try:
             payload = json.loads(message)
+            payload['when'] = datetime.datetime.now()
             msg = payload
             try:
                 if ('version' in payload and payload['version'] == 1):
                     self.db.storeMessage(payload)
                 else:
                     msg = self.transformer.transform(payload)
                     if msg == None:
@@ -109,15 +111,15 @@
                 'level': 'error',
                 'content': "websocket error",
             },
         }
         self.db.storeMessage(msg)
         self.error = error
 
-    def on_close(self, ws):
+    def on_close(self, *args,**kwargs):
         msg = {
             'type': 'log',
             'verb': 'create',
             'version': 1,
             'data': {
                 'level': 'error',
                 'content': "websocket closed",
@@ -126,14 +128,14 @@
         self.db.storeMessage(msg)
 
     def on_open(self, ws):
         self.isOpen = True
 
     def connect(self):
         self._status = 0
-        url = requests.compat.urljoin(self.url, self.taskId)
+        url = requests.compat.urljoin(self.url, self.taskId)  # type: ignore
         self.ws = websocket.WebSocketApp(url + '?subscribe-broadcast',
                                          on_open=self.on_open,
                                          on_message=self.on_message,
                                          on_error=self.on_error,
                                          on_close=self.on_close)
         self.ws.run_forever()
```

### Comparing `cloudpss-3.2.0a2/cloudpss/runner/result.py` & `cloudpss-3.5.0a1/cloudpss/runner/result.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import copy
 import re
 import collections
-from .storage import Storage
 
+from cloudpss.utils.httprequests import request
+from .storage import Storage
 
 class Result(object):
     """
         结果处理类，从消息存储库中获取数据，并进行简单的整理
 
         可迭代器，迭代时按接收顺序返回数据
 
@@ -329,16 +330,20 @@
                                     'y'].extend(v['y'])
             self.__plotIndex = length
 
     def getPlotData(self, compID, labelName, traceName='all', index=-1):
         '''
             获取元件ID为compID的元件，对应标签为labelName、图例名称为traceName的plot 数据的第index项
 
-            >>> result.getPlots(compID, labelName, traceName, index)
-            {...}
+            :params: compID string类型，代表元件的标识符
+            :params: lableName string类型，代表plot曲线的分组标签
+            :params: traceName string类型，代表Plot曲线对应分组下的图例名称，当为'all'时，返回所有图例的数据
+            :params: index int类型，代表对应图例时序数据中的第index项，当小于0时，返回该图例所有的时序数据
+            
+            :return: dict类型
         '''
         self.__readPlotResult()
         key = compID + '_' + labelName
         if key not in self.result.keys():
             raise Exception('未找到元件标志为{0},对应label为{1}的plot数据'.format(
                 compID, labelName))
 
@@ -385,8 +390,37 @@
     def getSankeyNum(self):
         '''
             获取桑基图数据序列的长度
 
             >>> result.getSankeyNum()
         '''
         self.__readPlotResult()
-        return len(self.result['Sankey'])
+        return len(self.result['Sankey'])
+
+class IESLabSimulationResult(IESResult):
+    pass
+
+class IESLabTypicalDayResult(IESResult):
+    def GetTypicalDayNum():
+        '''
+            获取当前result的典型日数量
+            
+            :return: int类型，代表典型日数量
+        '''
+    def GetTypicalDayInfo(dayID):
+        '''
+            获取dayID对应典型日的基础信息
+            
+            :params: dayID int类型，表示典型日的ID，数值位于 0~典型日数量 之间
+            
+            :return: dict类型，代表典型日的基础信息，包括典型日所代表的日期范围、典型日的名称等
+        '''
+    def GetTypicalDayCurve(dayID, dataType):
+        '''
+            获取dayID对应典型日下dataType参数的时序曲线
+            
+            :params: dayID int类型，表示典型日的ID，数值位于 0~典型日数量 之间
+            :params: dataType enum类型，标识辐照强度、环境温度、土壤温度、建筑物高度风速、风机高度风速、电负荷、热负荷、冷负荷的参数类型
+            
+            :return: list<float>类型，代表以1h为时间间隔的该参数的日内时序曲线
+        '''
+    pass
```

### Comparing `cloudpss-3.2.0a2/cloudpss/runner/storage.py` & `cloudpss-3.5.0a1/cloudpss/runner/storage.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a2/cloudpss/runner/transform.py` & `cloudpss-3.5.0a1/cloudpss/runner/transform.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a2/cloudpss/utils/dataEncoder.py` & `cloudpss-3.5.0a1/cloudpss/utils/dataEncoder.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a2/cloudpss/utils/matlab.py` & `cloudpss-3.5.0a1/cloudpss/utils/matlab.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a2/cloudpss/utils/yamlLoader.py` & `cloudpss-3.5.0a1/cloudpss/utils/yamlLoader.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,80 @@
 import yaml
 import io
 import gzip
 import struct
 import base64
 
 
-class JavascriptSchema():
-    def float32Array(self, node):
-        data = base64.b64decode(node.value)
-        return list(struct.unpack('f' * (len(data) // 4), data))
-
-    def float64Array(self, node):
-        data = base64.b64decode(node.value)
-        return list(struct.unpack('d' * (len(data) // 8), data))
-
-    def uint8Array(self, node):
-        data = base64.b64decode(node.value)
-        return list(struct.unpack('B' * (len(data) // 1), data))
-
-    def uint8ClampedArray(self, node):
-        data = base64.b64decode(node.value)
-        return list(struct.unpack('B' * (len(data) // 1), data))
-
-    def uint16Array(self, node):
-        data = base64.b64decode(node.value)
-        return list(struct.unpack('H' * (len(data) // 2), data))
-
-    def uint32Array(self, node):
-        data = base64.b64decode(node.value)
-        return list(struct.unpack('I' * (len(data) // 4), data))
-
-    def int8Array(self, node):
-        data = base64.b64decode(node.value)
-        return list(struct.unpack('b' * (len(data) // 1), data))
-
-    def int16Array(self, node):
-        data = base64.b64decode(node.value)
-        return list(struct.unpack('h' * (len(data) // 2), data))
-
-    def int32Array(self, node):
-
-        data = base64.b64decode(node.value)
-        return list(struct.unpack('i' * (len(data) // 4), data)).toList()
 
+def float32Array(_loader, node):
+    data = base64.b64decode(node.value)
+    return list(struct.unpack('f' * (len(data) // 4), data))
+
+def float64Array(_loader, node):
+    data = base64.b64decode(node.value)
+    return list(struct.unpack('d' * (len(data) // 8), data))
+
+def uint8Array(_loader, node):
+    data = base64.b64decode(node.value)
+    return list(struct.unpack('B' * (len(data) // 1), data))
+
+def uint8ClampedArray(_loader, node):
+    data = base64.b64decode(node.value)
+    return list(struct.unpack('B' * (len(data) // 1), data))
+
+def uint16Array(_loader, node):
+    data = base64.b64decode(node.value)
+    return list(struct.unpack('H' * (len(data) // 2), data))
+
+def uint32Array(_loader, node):
+    data = base64.b64decode(node.value)
+    return list(struct.unpack('I' * (len(data) // 4), data))
+
+def int8Array(_loader, node):
+    data = base64.b64decode(node.value)
+    return list(struct.unpack('b' * (len(data) // 1), data))
+
+def int16Array(_loader, node):
+    data = base64.b64decode(node.value)
+    return list(struct.unpack('h' * (len(data) // 2), data))
+
+def int32Array(_loader, node):
+    data = base64.b64decode(node.value)
+    return list(struct.unpack('i' * (len(data) // 4), data))
 
+#type:ignore
 yaml.add_constructor('tag:yaml.org,2002:js/Float32Array',
-                     JavascriptSchema.float32Array)
+                     float32Array)
 yaml.add_constructor('tag:yaml.org,2002:js/Float64Array',
-                     JavascriptSchema.float64Array)
+                     float64Array)
 yaml.add_constructor('tag:yaml.org,2002:js/Uint8Array',
-                     JavascriptSchema.uint8Array)
+                     uint8Array)
 yaml.add_constructor('tag:yaml.org,2002:js/Uint8ClampedArray',
-                     JavascriptSchema.uint8ClampedArray)
+                     uint8ClampedArray)
 yaml.add_constructor('tag:yaml.org,2002:js/Uint16Array',
-                     JavascriptSchema.uint16Array)
+                     uint16Array)
 yaml.add_constructor('tag:yaml.org,2002:js/Uint32Array',
-                     JavascriptSchema.uint32Array)
+                     uint32Array)
 yaml.add_constructor('tag:yaml.org,2002:js/Int8Array',
-                     JavascriptSchema.int8Array)
+                     int8Array)
 yaml.add_constructor('tag:yaml.org,2002:js/Int16Array',
-                     JavascriptSchema.int16Array)
+                     int16Array)
 yaml.add_constructor('tag:yaml.org,2002:js/Int32Array',
-                     JavascriptSchema.int32Array)
+                     int32Array)
 
 
 def fileLoad(fileName):
     f = open(fileName, 'r+', encoding='utf-8')
     t = f.buffer.read(2)
     f.close()
     data = None
     if t == b'\x1f\x8b':
         with gzip.open(fileName, 'rb') as input_file:
-            with io.TextIOWrapper(input_file, encoding='utf-8') as dec:
+            with io.TextIOWrapper(input_file, encoding='utf-8') as dec: # type: ignore
                 r = dec.read()
-                data = yaml.load(r, Loader=yaml.FullLoader)
+                data = yaml.load(r, _loader=yaml.Full_loader) # type: ignore
     else:
         f = open(fileName, 'r+', encoding='utf-8')
-        data = yaml.load(f, Loader=yaml.FullLoader)
+        data = yaml.load(f, _loader=yaml.Full_loader) # type: ignore
         f.close()
     return data
```

### Comparing `cloudpss-3.2.0a2/cloudpss.egg-info/PKG-INFO` & `cloudpss-3.5.0a1/cloudpss.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: cloudpss
-Version: 3.2.0a2
+Version: 3.5.0a1
 Summary: cloudpss sdk
 Home-page: https://www.cloudpss.net
 Author: cloudpss
 Author-email: zhangdaming@cloudpss.net
 License: MIT Licence
-Description: 
-        CloudPSS SDK
-        ----------------------------------------------------------------
-        CloudPSS SDK是基于CloudPSS-API封装的模型及软件开发套件。用户可通过编写Python、Matlab等脚本构建自定义模型，或是调用CloudPSS平台中的模型修改、仿真计算功能，实现诸如自动修改模型、批量仿真计算、自动化生成报告等复杂且繁琐的功能。用户也可在其自己的应用程序中调用CloudPSS仿真引擎，实现仿真驱动的高级分析应用。
-        
-        CloudPSS SDK包含模型层、算法层和应用层三种开发套件，其中：
-        
-        1. `模型层开发套件`帮助用户在CloudPSS SimStudio官方潮流计算、电磁暂态仿真、移频电磁暂态仿真、综合能源能量流计算等内核中开发第三方模型或用户自定义模型。目前，模型层SDK已开放基于Matlab函数的自定义控制元件接入，后续将进一步开放Python、C/C++的标准元件开发套件。
-        2. `算法层开发套件`帮助用户在CloudPSS FuncStudio中集成自己的算法内核，从而借助CloudPSS XStudio平台快速开发并部署自己的计算应用。该部分内容将在年内发布，敬请期待。
-        3. `应用层开发套件`帮助用户在利用脚本的形式快速调用CloudPSS官方计算内核和第三方接入的计算内核，从而方便用户开发高级计算分析应用。其中，SimStudio-SDK现已支持SimStudio中的模型修改和`潮流计算`和`电磁暂态仿真`两种计算内核。
-        
-        
-        ---
-        ### 下载与安装
-        
-        ```[pyhton]
-        pip install cloudpss
-        ```
-        需要`升级`的话，执行下面的命令:
-        ```[pyhton]
-        pip install --upgrade cloudpss
-        ```
-        ### 完全卸载
-        
-        执行下面的命令进行`完全卸载`:
-        ```[pyhton]
-        pip uninstall cloudpss
-        ```
-        
-                  
-        
-        
 Keywords: cloudpss,cloudpss-sdk
 Platform: any
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+
+
+CloudPSS SDK
+----------------------------------------------------------------
+CloudPSS SDK是基于CloudPSS-API封装的模型及软件开发套件。用户可通过编写Python、Matlab等脚本构建自定义模型，或是调用CloudPSS平台中的模型修改、仿真计算功能，实现诸如自动修改模型、批量仿真计算、自动化生成报告等复杂且繁琐的功能。用户也可在其自己的应用程序中调用CloudPSS仿真引擎，实现仿真驱动的高级分析应用。
+
+CloudPSS SDK包含模型层、算法层和应用层三种开发套件，其中：
+
+1. `模型层开发套件`帮助用户在CloudPSS SimStudio官方潮流计算、电磁暂态仿真、移频电磁暂态仿真、综合能源能量流计算等内核中开发第三方模型或用户自定义模型。目前，模型层SDK已开放基于Matlab函数的自定义控制元件接入，后续将进一步开放Python、C/C++的标准元件开发套件。
+2. `算法层开发套件`帮助用户在CloudPSS FuncStudio中集成自己的算法内核，从而借助CloudPSS XStudio平台快速开发并部署自己的计算应用。该部分内容将在年内发布，敬请期待。
+3. `应用层开发套件`帮助用户在利用脚本的形式快速调用CloudPSS官方计算内核和第三方接入的计算内核，从而方便用户开发高级计算分析应用。其中，SimStudio-SDK现已支持SimStudio中的模型修改和`潮流计算`和`电磁暂态仿真`两种计算内核。
+
+
+---
+### 下载与安装
+
+```[pyhton]
+pip install cloudpss
+```
+需要`升级`的话，执行下面的命令:
+```[pyhton]
+pip install --upgrade cloudpss
+```
+### 完全卸载
+
+执行下面的命令进行`完全卸载`:
+```[pyhton]
+pip uninstall cloudpss
+```
+
+          
+
```

### Comparing `cloudpss-3.2.0a2/setup.py` & `cloudpss-3.5.0a1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 from cloudpss import __version__
+import os
+
+os.system('git tag '+__version__)
 
 setup(
     name='cloudpss',
     version=__version__,
-    keywords=("cloudpss", "cloudpss-sdk"),
+    keywords=["cloudpss", "cloudpss-sdk"],
     description='cloudpss sdk',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT Licence",
     url='https://www.cloudpss.net',
     author='cloudpss',
     author_email='zhangdaming@cloudpss.net',
     packages=find_packages(),
     include_package_data=True,
     platforms="any",
     python_requires='>=3.7',
     install_requires=[
         'cffi', 'cryptography', 'cycler', 'pycparser', 'PyJWT', 'numpy',
-        'PyYAML', 'requests', 'websocket-client', 'pytz', 'deprecated'
+        'PyYAML', 'requests', 'websocket-client', 'pytz', 'deprecated','py-ubjson'
     ],
 )
```

