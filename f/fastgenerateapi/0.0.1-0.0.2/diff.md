# Comparing `tmp/fastgenerateapi-0.0.1.tar.gz` & `tmp/fastgenerateapi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastgenerateapi-0.0.1.tar", last modified: Mon Jun  5 11:31:46 2023, max compression
+gzip compressed data, was "fastgenerateapi-0.0.2.tar", last modified: Wed Jun 14 08:53:03 2023, max compression
```

## Comparing `fastgenerateapi-0.0.1.tar` & `fastgenerateapi-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 11:31:46.354431 fastgenerateapi-0.0.1/
--rw-rw-rw-   0        0        0    35821 2023-06-03 07:15:26.000000 fastgenerateapi-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      948 2023-06-05 11:31:46.354431 fastgenerateapi-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-03 09:02:13.000000 fastgenerateapi-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 11:31:46.351437 fastgenerateapi-0.0.1/fastgenerateapi/
--rw-rw-rw-   0        0        0      456 2023-06-05 11:30:53.000000 fastgenerateapi-0.0.1/fastgenerateapi/__init__.py
--rw-rw-rw-   0        0        0      496 2023-06-05 11:30:53.000000 fastgenerateapi-0.0.1/fastgenerateapi/__version__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 11:31:46.353432 fastgenerateapi-0.0.1/fastgenerateapi.egg-info/
--rw-rw-rw-   0        0        0      948 2023-06-05 11:31:46.000000 fastgenerateapi-0.0.1/fastgenerateapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-06-05 11:31:46.000000 fastgenerateapi-0.0.1/fastgenerateapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 11:31:46.000000 fastgenerateapi-0.0.1/fastgenerateapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-05 11:31:46.000000 fastgenerateapi-0.0.1/fastgenerateapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 11:31:46.354431 fastgenerateapi-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     3831 2023-06-05 11:27:14.000000 fastgenerateapi-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:53:03.579274 fastgenerateapi-0.0.2/
+-rw-rw-rw-   0        0        0    35821 2023-06-14 08:27:11.000000 fastgenerateapi-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      885 2023-06-14 08:53:03.579274 fastgenerateapi-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-06-14 08:27:11.000000 fastgenerateapi-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 08:53:03.375508 fastgenerateapi-0.0.2/fastgenerateapi/
+-rw-rw-rw-   0        0        0      756 2023-06-14 01:36:26.000000 fastgenerateapi-0.0.2/fastgenerateapi/__init__.py
+-rw-rw-rw-   0        0        0      496 2023-06-14 08:27:11.000000 fastgenerateapi-0.0.2/fastgenerateapi/__version__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:53:03.407435 fastgenerateapi-0.0.2/fastgenerateapi/api_view/
+-rw-rw-rw-   0        0        0       14 2023-06-09 00:54:08.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/__init__.py
+-rw-rw-rw-   0        0        0     1160 2023-06-09 00:54:08.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/api_view.py
+-rw-rw-rw-   0        0        0     9133 2023-06-14 01:34:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/base_view.py
+-rw-rw-rw-   0        0        0     4202 2023-06-13 14:48:03.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/create_view.py
+-rw-rw-rw-   0        0        0     3075 2023-06-14 01:34:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/delete_view.py
+-rw-rw-rw-   0        0        0     7585 2023-06-14 01:34:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/get_all_view.py
+-rw-rw-rw-   0        0        0     3077 2023-06-13 00:43:06.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/get_one_view.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:53:03.438713 fastgenerateapi-0.0.2/fastgenerateapi/api_view/mixin/
+-rw-rw-rw-   0        0        0        0 2023-06-09 00:54:08.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/mixin/__init__.py
+-rw-rw-rw-   0        0        0     6486 2023-06-12 00:42:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/mixin/base_mixin.py
+-rw-rw-rw-   0        0        0      266 2023-06-12 00:42:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/mixin/get_mixin.py
+-rw-rw-rw-   0        0        0     2221 2023-06-13 00:43:06.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/mixin/response_mixin.py
+-rw-rw-rw-   0        0        0      317 2023-06-13 14:43:14.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/mixin/save_mixin.py
+-rw-rw-rw-   0        0        0    13029 2023-06-12 00:42:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/mixin/tool_mixin.py
+-rw-rw-rw-   0        0        0     3279 2023-06-14 01:34:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/switch_view.py
+-rw-rw-rw-   0        0        0     4150 2023-06-14 01:34:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/update_view.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:53:03.469957 fastgenerateapi-0.0.2/fastgenerateapi/controller/
+-rw-rw-rw-   0        0        0      316 2023-06-09 00:54:08.000000 fastgenerateapi-0.0.2/fastgenerateapi/controller/__init__.py
+-rw-rw-rw-   0        0        0     3391 2023-06-13 10:04:30.000000 fastgenerateapi-0.0.2/fastgenerateapi/controller/filter_controller.py
+-rw-rw-rw-   0        0        0     2385 2023-06-09 00:54:08.000000 fastgenerateapi-0.0.2/fastgenerateapi/controller/router_controller.py
+-rw-rw-rw-   0        0        0     2298 2023-06-09 00:54:08.000000 fastgenerateapi-0.0.2/fastgenerateapi/controller/rpc_controller.py
+-rw-rw-rw-   0        0        0      873 2023-06-09 00:54:08.000000 fastgenerateapi-0.0.2/fastgenerateapi/controller/search_controller.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:53:03.469957 fastgenerateapi-0.0.2/fastgenerateapi/data_type/
+-rw-rw-rw-   0        0        0        0 2023-06-09 00:54:08.000000 fastgenerateapi-0.0.2/fastgenerateapi/data_type/__init__.py
+-rw-rw-rw-   0        0        0      727 2023-06-09 00:54:08.000000 fastgenerateapi-0.0.2/fastgenerateapi/data_type/data_type.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:53:03.501166 fastgenerateapi-0.0.2/fastgenerateapi/deps/
+-rw-rw-rw-   0        0        0      160 2023-06-09 00:54:08.000000 fastgenerateapi-0.0.2/fastgenerateapi/deps/__init__.py
+-rw-rw-rw-   0        0        0     1573 2023-06-13 01:42:38.000000 fastgenerateapi-0.0.2/fastgenerateapi/deps/filter_params_deps.py
+-rw-rw-rw-   0        0        0     3171 2023-06-13 01:42:38.000000 fastgenerateapi-0.0.2/fastgenerateapi/deps/paginator_deps.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:53:03.501166 fastgenerateapi-0.0.2/fastgenerateapi/pydantic_utils/
+-rw-rw-rw-   0        0        0        0 2023-06-09 00:54:09.000000 fastgenerateapi-0.0.2/fastgenerateapi/pydantic_utils/__init__.py
+-rw-rw-rw-   0        0        0      648 2023-06-14 01:34:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/pydantic_utils/base_model.py
+-rw-rw-rw-   0        0        0     2814 2023-06-12 00:42:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/pydantic_utils/json_encoders.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:53:03.548030 fastgenerateapi-0.0.2/fastgenerateapi/schemas_factory/
+-rw-rw-rw-   0        0        0      472 2023-06-12 00:42:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/schemas_factory/__init__.py
+-rw-rw-rw-   0        0        0     4296 2023-06-14 01:34:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/schemas_factory/common_function.py
+-rw-rw-rw-   0        0        0     1856 2023-06-14 01:34:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/schemas_factory/create_schema_factory.py
+-rw-rw-rw-   0        0        0     3102 2023-06-14 01:34:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/schemas_factory/get_all_schema_factory.py
+-rw-rw-rw-   0        0        0     1763 2023-06-14 01:34:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/schemas_factory/get_one_schema_factory.py
+-rw-rw-rw-   0        0        0     1251 2023-06-12 00:42:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/schemas_factory/response_factory.py
+-rw-rw-rw-   0        0        0     1856 2023-06-14 01:34:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/schemas_factory/update_schema_factory.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:53:03.563683 fastgenerateapi-0.0.2/fastgenerateapi/settings/
+-rw-rw-rw-   0        0        0        6 2023-06-09 00:54:09.000000 fastgenerateapi-0.0.2/fastgenerateapi/settings/__init__.py
+-rw-rw-rw-   0        0        0      232 2023-06-09 00:54:09.000000 fastgenerateapi-0.0.2/fastgenerateapi/settings/register_settings.py
+-rw-rw-rw-   0        0        0     2955 2023-06-14 01:34:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/settings/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:53:03.563683 fastgenerateapi-0.0.2/fastgenerateapi/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-09 00:54:09.000000 fastgenerateapi-0.0.2/fastgenerateapi/utils/__init__.py
+-rw-rw-rw-   0        0        0      121 2023-06-09 00:54:09.000000 fastgenerateapi-0.0.2/fastgenerateapi/utils/exception.py
+-rw-rw-rw-   0        0        0      670 2023-06-09 00:54:09.000000 fastgenerateapi-0.0.2/fastgenerateapi/utils/parse_str.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:53:03.391129 fastgenerateapi-0.0.2/fastgenerateapi.egg-info/
+-rw-rw-rw-   0        0        0      885 2023-06-14 08:53:03.000000 fastgenerateapi-0.0.2/fastgenerateapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2023 2023-06-14 08:53:03.000000 fastgenerateapi-0.0.2/fastgenerateapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 08:53:03.000000 fastgenerateapi-0.0.2/fastgenerateapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-14 08:53:03.000000 fastgenerateapi-0.0.2/fastgenerateapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 08:53:03.579274 fastgenerateapi-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     3832 2023-06-14 08:51:43.000000 fastgenerateapi-0.0.2/setup.py
```

### Comparing `fastgenerateapi-0.0.1/LICENSE` & `fastgenerateapi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.1/PKG-INFO` & `fastgenerateapi-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: fastgenerateapi
-Version: 0.0.1
+Version: 0.0.2
 Summary: FastAPIView Class View
-Home-page: https://github.com/ShiLiangAPI/FastGenerateAPI.git
 Author: ShiLiang
 Author-email: 2509144896@qq.com
 License: GPL-3.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `fastgenerateapi-0.0.1/fastgenerateapi.egg-info/PKG-INFO` & `fastgenerateapi-0.0.2/fastgenerateapi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: fastgenerateapi
-Version: 0.0.1
+Version: 0.0.2
 Summary: FastAPIView Class View
-Home-page: https://github.com/ShiLiangAPI/FastGenerateAPI.git
 Author: ShiLiang
 Author-email: 2509144896@qq.com
 License: GPL-3.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `fastgenerateapi-0.0.1/setup.py` & `fastgenerateapi-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 import setuptools
 
 
 # Package meta-data.
 NAME = 'fastgenerateapi'
 DESCRIPTION = 'FastAPIView Class View'
-URL = 'https://github.com/ShiLiangAPI/FastGenerateAPI.git'
+# URL = 'https://github.com/ShiLiangAPI/FastGenerateAPI.git'
 EMAIL = '2509144896@qq.com'
 AUTHOR = 'ShiLiang'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.1'
+VERSION = None
 
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
@@ -97,15 +97,15 @@
     version=about['__version__'],
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
-    url=URL,
+    # url=URL,
     packages=setuptools.find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
     # If your package is a single module, use this instead of 'packages':
     # py_modules=['mypackage'],
 
     # entry_points={
     #     'console_scripts': ['mycli=mymodule:cli'],
     # },
```

