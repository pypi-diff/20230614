# Comparing `tmp/rolling-in-the-deep-0.1.2.tar.gz` & `tmp/rolling-in-the-deep-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rolling-in-the-deep-0.1.2.tar", last modified: Mon May  8 09:35:39 2023, max compression
+gzip compressed data, was "rolling-in-the-deep-0.1.3.tar", last modified: Wed Jun 14 02:15:17 2023, max compression
```

## Comparing `rolling-in-the-deep-0.1.2.tar` & `rolling-in-the-deep-0.1.3.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.641059 rolling-in-the-deep-0.1.2/
--rw-rw-rw-   0        0        0     1073 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1805 2023-05-08 09:35:39.640058 rolling-in-the-deep-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1280 2022-01-26 04:12:06.000000 rolling-in-the-deep-0.1.2/README.md
--rw-rw-rw-   0        0        0      104 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 09:35:39.641059 rolling-in-the-deep-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1905 2023-05-08 09:31:51.000000 rolling-in-the-deep-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.456506 rolling-in-the-deep-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.478509 rolling-in-the-deep-0.1.2/src/example_package/
--rw-rw-rw-   0        0        0      494 2023-05-08 08:41:06.000000 rolling-in-the-deep-0.1.2/src/example_package/RichTest.py
--rw-rw-rw-   0        0        0      159 2023-05-08 08:41:06.000000 rolling-in-the-deep-0.1.2/src/example_package/__init__.py
--rw-rw-rw-   0        0        0      202 2023-05-08 08:41:06.000000 rolling-in-the-deep-0.1.2/src/example_package/example.py
--rw-rw-rw-   0        0        0     6602 2023-05-08 09:15:00.000000 rolling-in-the-deep-0.1.2/src/example_package/pyecharts_test.py
--rw-rw-rw-   0        0        0     7022 2023-05-08 09:15:00.000000 rolling-in-the-deep-0.1.2/src/example_package/reportlab_pdf.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.486509 rolling-in-the-deep-0.1.2/src/rolling_in_the_deep.egg-info/
--rw-rw-rw-   0        0        0     1805 2023-05-08 09:35:39.000000 rolling-in-the-deep-0.1.2/src/rolling_in_the_deep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3923 2023-05-08 09:35:39.000000 rolling-in-the-deep-0.1.2/src/rolling_in_the_deep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 09:35:39.000000 rolling-in-the-deep-0.1.2/src/rolling_in_the_deep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-05-08 09:35:39.000000 rolling-in-the-deep-0.1.2/src/rolling_in_the_deep.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.488510 rolling-in-the-deep-0.1.2/src/rolling_king/
--rw-rw-rw-   0        0        0        0 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.489510 rolling-in-the-deep-0.1.2/src/rolling_king/jason/
--rw-rw-rw-   0        0        0        0 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.492510 rolling-in-the-deep-0.1.2/src/rolling_king/jason/autogen/
--rw-rw-rw-   0        0        0      153 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/autogen/__init__.py
--rw-rw-rw-   0        0        0     1171 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/autogen/auto_generate.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.495510 rolling-in-the-deep-0.1.2/src/rolling_king/jason/chatgpt/
--rw-rw-rw-   0        0        0        0 2023-05-08 09:20:22.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/chatgpt/__init__.py
--rw-rw-rw-   0        0        0     1885 2023-05-08 09:20:22.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/chatgpt/openai.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.499512 rolling-in-the-deep-0.1.2/src/rolling_king/jason/newcore/
--rw-rw-rw-   0        0        0        0 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/newcore/__init__.py
--rw-rw-rw-   0        0        0     1041 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/newcore/test_ccc.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.503512 rolling-in-the-deep-0.1.2/src/rolling_king/jason/openpyxl/
--rw-rw-rw-   0        0        0        0 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/openpyxl/__init__.py
--rw-rw-rw-   0        0        0     2576 2023-05-08 09:15:00.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/openpyxl/excel_util.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.509513 rolling-in-the-deep-0.1.2/src/rolling_king/jason/playwright/
--rw-rw-rw-   0        0        0        0 2023-05-08 09:20:22.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/playwright/__init__.py
--rw-rw-rw-   0        0        0    15090 2023-05-08 09:20:22.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/playwright/playwright_common.py
--rw-rw-rw-   0        0        0     2861 2023-05-08 09:20:22.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/playwright/test_generate.py
--rw-rw-rw-   0        0        0     1247 2023-05-08 09:20:22.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/playwright/test_playwright.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.517514 rolling-in-the-deep-0.1.2/src/rolling_king/jason/pypac/
--rw-rw-rw-   0        0        0      206 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/pypac/__init__.py
--rw-rw-rw-   0        0        0       82 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/pypac/pyfile1.py
--rw-rw-rw-   0        0        0       81 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/pypac/pyfile2.py
--rw-rw-rw-   0        0        0      142 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/pypac/test.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.525323 rolling-in-the-deep-0.1.2/src/rolling_king/jason/pytest/
--rw-rw-rw-   0        0        0      154 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/pytest/__init__.py
--rw-rw-rw-   0        0        0      634 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/pytest/conftest.py
--rw-rw-rw-   0        0        0     1618 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/pytest/test_class.py
--rw-rw-rw-   0        0        0      455 2023-05-08 08:41:06.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/pytest/test_sample.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.544046 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/
--rw-rw-rw-   0        0        0    13268 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/ClassTest.py
--rw-rw-rw-   0        0        0     1639 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/DbTest.py
--rw-rw-rw-   0        0        0     1146 2022-03-29 13:07:08.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/MailTest.py
--rw-rw-rw-   0        0        0    15111 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/MyPyTest.py
--rw-rw-rw-   0        0        0    14302 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/PythonTest.py
--rw-rw-rw-   0        0        0     1557 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/QueueTest.py
--rw-rw-rw-   0        0        0    11731 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/SeniorTest.py
--rw-rw-rw-   0        0        0        0 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.550047 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/socket/
--rw-rw-rw-   0        0        0      424 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/socket/SocketClient.py
--rw-rw-rw-   0        0        0      670 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/socket/SocketServer.py
--rw-rw-rw-   0        0        0      154 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/socket/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.556048 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/thread/
--rw-rw-rw-   0        0        0     2483 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/thread/ThreadingTest.py
--rw-rw-rw-   0        0        0      910 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/thread/_ThreadTest.py
--rw-rw-rw-   0        0        0      154 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/thread/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.569050 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/tools/
--rw-rw-rw-   0        0        0     1985 2022-03-29 13:07:08.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/tools/ExcelTest.py
--rw-rw-rw-   0        0        0        0 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/tools/__init__.py
--rw-rw-rw-   0        0        0     1044 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/tools/xmind_excel_converter.py
--rw-rw-rw-   0        0        0     4991 2023-05-08 08:41:06.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/tools/zy_schedule.py
--rw-rw-rw-   0        0        0     1161 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/tools/zy_shell.py
--rw-rw-rw-   0        0        0     1340 2023-05-08 09:15:00.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/tools/zy_stamp_tool.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.579051 rolling-in-the-deep-0.1.2/src/rolling_king/jason/requests/
--rw-rw-rw-   0        0        0        0 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/requests/__init__.py
--rw-rw-rw-   0        0        0     3102 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/requests/http_sender_module.py
--rw-rw-rw-   0        0        0      763 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/requests/test_ccc.py
--rw-rw-rw-   0        0        0     6463 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/requests/test_http.py
--rw-rw-rw-   0        0        0     2442 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/requests/test_m_project.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.583051 rolling-in-the-deep-0.1.2/src/rolling_king/jason/webdriver/
--rw-rw-rw-   0        0        0      155 2023-05-08 09:01:41.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/webdriver/__init__.py
--rw-rw-rw-   0        0        0    11714 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/webdriver/webdriver_common.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.585051 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/
--rw-rw-rw-   0        0        0        0 2023-05-08 08:41:07.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.591052 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/db/
--rw-rw-rw-   0        0        0        0 2023-05-08 08:41:07.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/db/__init__.py
--rw-rw-rw-   0        0        0    15845 2023-05-08 08:41:07.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/db/db_models.py
--rw-rw-rw-   0        0        0     3204 2023-05-08 08:41:07.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/db/db_util.py
--rw-rw-rw-   0        0        0    11495 2023-05-08 08:41:07.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/db/sqlalchemy_util.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.595053 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/requests/
--rw-rw-rw-   0        0        0        0 2023-05-08 08:41:07.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/requests/__init__.py
--rw-rw-rw-   0        0        0     3414 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/requests/http_sender_module.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.604054 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/rpc_thrift/
--rw-rw-rw-   0        0        0        0 2023-05-08 08:41:07.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/rpc_thrift/__init__.py
--rw-rw-rw-   0        0        0    17075 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/rpc_thrift/eventcollect.py
--rw-rw-rw-   0        0        0     2127 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/rpc_thrift/get_service_info.py
--rw-rw-rw-   0        0        0     1411 2023-05-08 08:41:07.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/rpc_thrift/thrift_rpc_util.py
--rw-rw-rw-   0        0        0    11163 2023-05-08 09:01:42.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/rpc_thrift/update_idl.py
--rw-rw-rw-   0        0        0      458 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/rpc_thrift/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.606055 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/tests/
--rw-rw-rw-   0        0        0      160 2023-05-08 08:41:07.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.612055 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/tests/base/
--rw-rw-rw-   0        0        0        0 2023-05-08 08:41:07.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/tests/base/__init__.py
--rw-rw-rw-   0        0        0    16165 2023-05-08 09:01:42.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/tests/base/autotest_generator.py
--rw-rw-rw-   0        0        0    14266 2023-05-08 09:01:42.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/tests/base/base_compare.py
--rw-rw-rw-   0        0        0    12560 2023-05-08 09:01:42.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/tests/base/base_test.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.621056 rolling-in-the-deep-0.1.2/src/tests/
--rw-rw-rw-   0        0        0      155 2023-05-08 09:01:42.000000 rolling-in-the-deep-0.1.2/src/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.626057 rolling-in-the-deep-0.1.2/src/tests/apscheduler/
--rw-rw-rw-   0        0        0      155 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/tests/apscheduler/__init__.py
--rw-rw-rw-   0        0        0     2080 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/tests/apscheduler/backgroud_scheduler.py
--rw-rw-rw-   0        0        0     7664 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/tests/apscheduler/sample_apscheduler.py
--rw-rw-rw-   0        0        0      881 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.629057 rolling-in-the-deep-0.1.2/src/tests/excel/
--rw-rw-rw-   0        0        0      159 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/tests/excel/__init__.py
--rw-rw-rw-   0        0        0     1634 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/tests/excel/excel_test.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.633057 rolling-in-the-deep-0.1.2/src/tests/hive/
--rw-rw-rw-   0        0        0      155 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/tests/hive/__init__.py
--rw-rw-rw-   0        0        0      555 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/tests/hive/pyhive_test.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.638058 rolling-in-the-deep-0.1.2/src/tests/refresh_page/
--rw-rw-rw-   0        0        0      159 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/tests/refresh_page/__init__.py
--rw-rw-rw-   0        0        0      903 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/tests/refresh_page/data_analysis.py
--rw-rw-rw-   0        0        0     2473 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/tests/refresh_page/temp_refresh.py
--rw-rw-rw-   0        0        0      788 2023-05-08 09:01:42.000000 rolling-in-the-deep-0.1.2/src/tests/test_options.py
--rw-rw-rw-   0        0        0     1644 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/tests/upload_file_test.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.803057 rolling-in-the-deep-0.1.3/
+-rw-rw-rw-   0        0        0     1073 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1805 2023-06-14 02:15:17.803057 rolling-in-the-deep-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1280 2022-01-26 04:12:06.000000 rolling-in-the-deep-0.1.3/README.md
+-rw-rw-rw-   0        0        0      104 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 02:15:17.803057 rolling-in-the-deep-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1905 2023-06-14 02:09:38.000000 rolling-in-the-deep-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.704596 rolling-in-the-deep-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.714595 rolling-in-the-deep-0.1.3/src/example_package/
+-rw-rw-rw-   0        0        0      494 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/example_package/RichTest.py
+-rw-rw-rw-   0        0        0      159 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/example_package/__init__.py
+-rw-rw-rw-   0        0        0      202 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/example_package/example.py
+-rw-rw-rw-   0        0        0     6602 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/example_package/pyecharts_test.py
+-rw-rw-rw-   0        0        0     7022 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/example_package/reportlab_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.722597 rolling-in-the-deep-0.1.3/src/rolling_in_the_deep.egg-info/
+-rw-rw-rw-   0        0        0     1805 2023-06-14 02:15:17.000000 rolling-in-the-deep-0.1.3/src/rolling_in_the_deep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3923 2023-06-14 02:15:17.000000 rolling-in-the-deep-0.1.3/src/rolling_in_the_deep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 02:15:17.000000 rolling-in-the-deep-0.1.3/src/rolling_in_the_deep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-14 02:15:17.000000 rolling-in-the-deep-0.1.3/src/rolling_in_the_deep.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.723596 rolling-in-the-deep-0.1.3/src/rolling_king/
+-rw-rw-rw-   0        0        0        0 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.724597 rolling-in-the-deep-0.1.3/src/rolling_king/jason/
+-rw-rw-rw-   0        0        0        0 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.725597 rolling-in-the-deep-0.1.3/src/rolling_king/jason/autogen/
+-rw-rw-rw-   0        0        0      153 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/autogen/__init__.py
+-rw-rw-rw-   0        0        0     1171 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/autogen/auto_generate.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.727595 rolling-in-the-deep-0.1.3/src/rolling_king/jason/chatgpt/
+-rw-rw-rw-   0        0        0        0 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/chatgpt/__init__.py
+-rw-rw-rw-   0        0        0     1948 2023-06-14 02:04:00.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/chatgpt/openai.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.728596 rolling-in-the-deep-0.1.3/src/rolling_king/jason/newcore/
+-rw-rw-rw-   0        0        0        0 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/newcore/__init__.py
+-rw-rw-rw-   0        0        0     1041 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/newcore/test_ccc.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.731266 rolling-in-the-deep-0.1.3/src/rolling_king/jason/openpyxl/
+-rw-rw-rw-   0        0        0        0 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/openpyxl/__init__.py
+-rw-rw-rw-   0        0        0     2576 2023-05-08 09:44:46.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/openpyxl/excel_util.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.737726 rolling-in-the-deep-0.1.3/src/rolling_king/jason/playwright/
+-rw-rw-rw-   0        0        0        0 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/playwright/__init__.py
+-rw-rw-rw-   0        0        0    15090 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/playwright/playwright_common.py
+-rw-rw-rw-   0        0        0     2861 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/playwright/test_generate.py
+-rw-rw-rw-   0        0        0     1247 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/playwright/test_playwright.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.741934 rolling-in-the-deep-0.1.3/src/rolling_king/jason/pypac/
+-rw-rw-rw-   0        0        0      206 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/pypac/__init__.py
+-rw-rw-rw-   0        0        0       82 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/pypac/pyfile1.py
+-rw-rw-rw-   0        0        0       81 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/pypac/pyfile2.py
+-rw-rw-rw-   0        0        0      142 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/pypac/test.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.745053 rolling-in-the-deep-0.1.3/src/rolling_king/jason/pytest/
+-rw-rw-rw-   0        0        0      154 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/pytest/__init__.py
+-rw-rw-rw-   0        0        0      634 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/pytest/conftest.py
+-rw-rw-rw-   0        0        0     1618 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/pytest/test_class.py
+-rw-rw-rw-   0        0        0      455 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/pytest/test_sample.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.755052 rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/
+-rw-rw-rw-   0        0        0    13268 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/ClassTest.py
+-rw-rw-rw-   0        0        0     1639 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/DbTest.py
+-rw-rw-rw-   0        0        0     1146 2022-03-29 13:07:08.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/MailTest.py
+-rw-rw-rw-   0        0        0    15111 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/MyPyTest.py
+-rw-rw-rw-   0        0        0    14302 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/PythonTest.py
+-rw-rw-rw-   0        0        0     1557 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/QueueTest.py
+-rw-rw-rw-   0        0        0    11731 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/SeniorTest.py
+-rw-rw-rw-   0        0        0        0 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.757052 rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/socket/
+-rw-rw-rw-   0        0        0      424 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/socket/SocketClient.py
+-rw-rw-rw-   0        0        0      670 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/socket/SocketServer.py
+-rw-rw-rw-   0        0        0      154 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/socket/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.760050 rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/thread/
+-rw-rw-rw-   0        0        0     2483 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/thread/ThreadingTest.py
+-rw-rw-rw-   0        0        0      910 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/thread/_ThreadTest.py
+-rw-rw-rw-   0        0        0      154 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/thread/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.766054 rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/tools/
+-rw-rw-rw-   0        0        0     1985 2022-03-29 13:07:08.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/tools/ExcelTest.py
+-rw-rw-rw-   0        0        0        0 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/tools/__init__.py
+-rw-rw-rw-   0        0        0     1044 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/tools/xmind_excel_converter.py
+-rw-rw-rw-   0        0        0     4991 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/tools/zy_schedule.py
+-rw-rw-rw-   0        0        0     1161 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/tools/zy_shell.py
+-rw-rw-rw-   0        0        0     1340 2023-05-08 09:44:46.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/tools/zy_stamp_tool.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.772050 rolling-in-the-deep-0.1.3/src/rolling_king/jason/requests/
+-rw-rw-rw-   0        0        0        0 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/requests/__init__.py
+-rw-rw-rw-   0        0        0     3663 2023-06-14 02:08:36.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/requests/http_sender_module.py
+-rw-rw-rw-   0        0        0      763 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/requests/test_ccc.py
+-rw-rw-rw-   0        0        0     6463 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/requests/test_http.py
+-rw-rw-rw-   0        0        0     2442 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/requests/test_m_project.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.774052 rolling-in-the-deep-0.1.3/src/rolling_king/jason/webdriver/
+-rw-rw-rw-   0        0        0      155 2023-05-08 09:44:46.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/webdriver/__init__.py
+-rw-rw-rw-   0        0        0    11714 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/rolling_king/jason/webdriver/webdriver_common.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.775051 rolling-in-the-deep-0.1.3/src/rolling_king/zijie/
+-rw-rw-rw-   0        0        0        0 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/rolling_king/zijie/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.778051 rolling-in-the-deep-0.1.3/src/rolling_king/zijie/db/
+-rw-rw-rw-   0        0        0        0 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/rolling_king/zijie/db/__init__.py
+-rw-rw-rw-   0        0        0    15845 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/rolling_king/zijie/db/db_models.py
+-rw-rw-rw-   0        0        0     3204 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/rolling_king/zijie/db/db_util.py
+-rw-rw-rw-   0        0        0    11495 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/rolling_king/zijie/db/sqlalchemy_util.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.780052 rolling-in-the-deep-0.1.3/src/rolling_king/zijie/requests/
+-rw-rw-rw-   0        0        0        0 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/rolling_king/zijie/requests/__init__.py
+-rw-rw-rw-   0        0        0     3916 2023-06-14 02:06:41.000000 rolling-in-the-deep-0.1.3/src/rolling_king/zijie/requests/http_sender_module.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.784054 rolling-in-the-deep-0.1.3/src/rolling_king/zijie/rpc_thrift/
+-rw-rw-rw-   0        0        0        0 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/rolling_king/zijie/rpc_thrift/__init__.py
+-rw-rw-rw-   0        0        0    17075 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/rolling_king/zijie/rpc_thrift/eventcollect.py
+-rw-rw-rw-   0        0        0     2127 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/rolling_king/zijie/rpc_thrift/get_service_info.py
+-rw-rw-rw-   0        0        0     1411 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/rolling_king/zijie/rpc_thrift/thrift_rpc_util.py
+-rw-rw-rw-   0        0        0    11163 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/rolling_king/zijie/rpc_thrift/update_idl.py
+-rw-rw-rw-   0        0        0      458 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/rolling_king/zijie/rpc_thrift/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.785057 rolling-in-the-deep-0.1.3/src/rolling_king/zijie/tests/
+-rw-rw-rw-   0        0        0      160 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/rolling_king/zijie/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.788051 rolling-in-the-deep-0.1.3/src/rolling_king/zijie/tests/base/
+-rw-rw-rw-   0        0        0        0 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/rolling_king/zijie/tests/base/__init__.py
+-rw-rw-rw-   0        0        0    16165 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/rolling_king/zijie/tests/base/autotest_generator.py
+-rw-rw-rw-   0        0        0    14266 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/rolling_king/zijie/tests/base/base_compare.py
+-rw-rw-rw-   0        0        0    12560 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/rolling_king/zijie/tests/base/base_test.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.791052 rolling-in-the-deep-0.1.3/src/tests/
+-rw-rw-rw-   0        0        0      155 2023-05-08 09:44:46.000000 rolling-in-the-deep-0.1.3/src/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.794051 rolling-in-the-deep-0.1.3/src/tests/apscheduler/
+-rw-rw-rw-   0        0        0      155 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/tests/apscheduler/__init__.py
+-rw-rw-rw-   0        0        0     2080 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/tests/apscheduler/backgroud_scheduler.py
+-rw-rw-rw-   0        0        0     7664 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/tests/apscheduler/sample_apscheduler.py
+-rw-rw-rw-   0        0        0      881 2023-05-08 09:44:46.000000 rolling-in-the-deep-0.1.3/src/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.795053 rolling-in-the-deep-0.1.3/src/tests/excel/
+-rw-rw-rw-   0        0        0      159 2023-05-08 09:44:46.000000 rolling-in-the-deep-0.1.3/src/tests/excel/__init__.py
+-rw-rw-rw-   0        0        0     1634 2023-05-08 09:44:46.000000 rolling-in-the-deep-0.1.3/src/tests/excel/excel_test.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.798053 rolling-in-the-deep-0.1.3/src/tests/hive/
+-rw-rw-rw-   0        0        0      155 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/tests/hive/__init__.py
+-rw-rw-rw-   0        0        0      555 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/tests/hive/pyhive_test.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:15:17.802060 rolling-in-the-deep-0.1.3/src/tests/refresh_page/
+-rw-rw-rw-   0        0        0      159 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/tests/refresh_page/__init__.py
+-rw-rw-rw-   0        0        0      903 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/tests/refresh_page/data_analysis.py
+-rw-rw-rw-   0        0        0     2473 2023-06-14 01:19:16.000000 rolling-in-the-deep-0.1.3/src/tests/refresh_page/temp_refresh.py
+-rw-rw-rw-   0        0        0      788 2023-05-08 09:44:46.000000 rolling-in-the-deep-0.1.3/src/tests/test_options.py
+-rw-rw-rw-   0        0        0     1644 2023-05-08 09:44:46.000000 rolling-in-the-deep-0.1.3/src/tests/upload_file_test.py
```

### Comparing `rolling-in-the-deep-0.1.2/LICENSE` & `rolling-in-the-deep-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/PKG-INFO` & `rolling-in-the-deep-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rolling-in-the-deep
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python Project For QA Test
 Home-page: https://gitee.com/jason024/python_project
 Author: RollingKing
 Author-email: 386773780@qq.com
 Project-URL: Bug Tracker, https://gitee.com/jason024/python_project/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rolling-in-the-deep-0.1.2/README.md` & `rolling-in-the-deep-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/setup.py` & `rolling-in-the-deep-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 ]
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rolling-in-the-deep",
-    version="0.1.2",
+    version="0.1.3",
     author="RollingKing",
     author_email="386773780@qq.com",
     description="Python Project For QA Test",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/jason024/python_project",
     project_urls={
```

### Comparing `rolling-in-the-deep-0.1.2/src/example_package/pyecharts_test.py` & `rolling-in-the-deep-0.1.3/src/example_package/pyecharts_test.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/example_package/reportlab_pdf.py` & `rolling-in-the-deep-0.1.3/src/example_package/reportlab_pdf.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_in_the_deep.egg-info/PKG-INFO` & `rolling-in-the-deep-0.1.3/src/rolling_in_the_deep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rolling-in-the-deep
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python Project For QA Test
 Home-page: https://gitee.com/jason024/python_project
 Author: RollingKing
 Author-email: 386773780@qq.com
 Project-URL: Bug Tracker, https://gitee.com/jason024/python_project/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_in_the_deep.egg-info/SOURCES.txt` & `rolling-in-the-deep-0.1.3/src/rolling_in_the_deep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/autogen/auto_generate.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/autogen/auto_generate.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/chatgpt/openai.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/chatgpt/openai.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import openai
 import json
-from src.rolling_king.zijie.requests.http_sender_module import HttpSender
+from rolling_king.zijie.requests.http_sender_module import HttpSender
 
 key_seg_1: str = "sk"
 key_seg_2: str = "-"
 key_seg_3: str = "wPe4VZsysqVYpOt4nIByT3BlbkFJf1Rx0O9HXr9znv5lzBG4"
 openai.api_key = key_seg_1+key_seg_2+key_seg_3
 
 
@@ -35,17 +35,18 @@
         for choice in choice_list:
             result_list.append(choice['message']['content'])
         return result_list
 
 
 if __name__ == "__main__":
     chatgpt: OpenAi = OpenAi()
-    print(chatgpt.get_specific_model())
-    print(chatgpt.chat_with_gpt(question="请介绍一下字节跳动", model="gpt-3.5-turbo-0301"))
-    print(chatgpt.chat_with_gpt(question="请介绍一下字节跳动", model="gpt-3.5-turbo"))
+    # print(chatgpt.get_models())
+    # print(chatgpt.get_specific_model(model="gpt-3.5-turbo-0613"))
+    # print(chatgpt.chat_with_gpt(question="请介绍一下字节跳动", model="gpt-3.5-turbo-0613"))
+    # print(chatgpt.chat_with_gpt(question="请介绍一下字节跳动", model="gpt-3.5-turbo"))
```

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/newcore/test_ccc.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/newcore/test_ccc.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/openpyxl/excel_util.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/openpyxl/excel_util.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/playwright/playwright_common.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/playwright/playwright_common.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/playwright/test_generate.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/playwright/test_generate.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/playwright/test_playwright.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/playwright/test_playwright.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/pytest/conftest.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/pytest/conftest.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/pytest/test_class.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/pytest/test_class.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/ClassTest.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/ClassTest.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/DbTest.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/DbTest.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/MailTest.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/MailTest.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/MyPyTest.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/MyPyTest.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/PythonTest.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/PythonTest.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/QueueTest.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/QueueTest.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/SeniorTest.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/SeniorTest.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/socket/SocketServer.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/socket/SocketServer.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/thread/ThreadingTest.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/thread/ThreadingTest.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/thread/_ThreadTest.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/thread/_ThreadTest.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/tools/ExcelTest.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/tools/ExcelTest.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/tools/xmind_excel_converter.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/tools/xmind_excel_converter.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/tools/zy_schedule.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/tools/zy_schedule.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/tools/zy_shell.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/tools/zy_shell.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/tools/zy_stamp_tool.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/python/tools/zy_stamp_tool.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/requests/test_ccc.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/requests/test_ccc.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/requests/test_http.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/requests/test_http.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/requests/test_m_project.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/requests/test_m_project.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/jason/webdriver/webdriver_common.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/jason/webdriver/webdriver_common.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/zijie/db/db_models.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/zijie/db/db_models.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/zijie/db/db_util.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/zijie/db/db_util.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/zijie/db/sqlalchemy_util.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/zijie/db/sqlalchemy_util.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/zijie/rpc_thrift/eventcollect.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/zijie/rpc_thrift/eventcollect.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/zijie/rpc_thrift/get_service_info.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/zijie/rpc_thrift/get_service_info.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/zijie/rpc_thrift/thrift_rpc_util.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/zijie/rpc_thrift/thrift_rpc_util.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/zijie/rpc_thrift/update_idl.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/zijie/rpc_thrift/update_idl.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/zijie/tests/base/autotest_generator.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/zijie/tests/base/autotest_generator.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/zijie/tests/base/base_compare.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/zijie/tests/base/base_compare.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/rolling_king/zijie/tests/base/base_test.py` & `rolling-in-the-deep-0.1.3/src/rolling_king/zijie/tests/base/base_test.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/tests/apscheduler/backgroud_scheduler.py` & `rolling-in-the-deep-0.1.3/src/tests/apscheduler/backgroud_scheduler.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/tests/apscheduler/sample_apscheduler.py` & `rolling-in-the-deep-0.1.3/src/tests/apscheduler/sample_apscheduler.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/tests/conftest.py` & `rolling-in-the-deep-0.1.3/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/tests/excel/excel_test.py` & `rolling-in-the-deep-0.1.3/src/tests/excel/excel_test.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/tests/hive/pyhive_test.py` & `rolling-in-the-deep-0.1.3/src/tests/hive/pyhive_test.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/tests/refresh_page/data_analysis.py` & `rolling-in-the-deep-0.1.3/src/tests/refresh_page/data_analysis.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/tests/refresh_page/temp_refresh.py` & `rolling-in-the-deep-0.1.3/src/tests/refresh_page/temp_refresh.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/tests/test_options.py` & `rolling-in-the-deep-0.1.3/src/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.2/src/tests/upload_file_test.py` & `rolling-in-the-deep-0.1.3/src/tests/upload_file_test.py`

 * *Files identical despite different names*

