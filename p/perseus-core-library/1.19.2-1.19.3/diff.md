# Comparing `tmp/perseus_core_library-1.19.2.tar.gz` & `tmp/perseus_core_library-1.19.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perseus_core_library-1.19.2.tar", max compression
+gzip compressed data, was "perseus_core_library-1.19.3.tar", max compression
```

## Comparing `perseus_core_library-1.19.2.tar` & `perseus_core_library-1.19.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     4465 2023-04-04 02:18:53.000358 perseus_core_library-1.19.2/CHANGELOG.md
--rw-r--r--   0        0        0     1089 2020-11-13 04:28:53.612751 perseus_core_library-1.19.2/LICENSE
--rwxr-xr-x   0        0        0      611 2023-03-31 11:33:19.503540 perseus_core_library-1.19.2/README.md
--rw-r--r--   0        0        0      991 2023-04-04 02:18:41.363679 perseus_core_library-1.19.2/pyproject.toml
--rwxr-xr-x   0        0        0     1189 2022-11-23 14:11:27.806929 perseus_core_library-1.19.2/src/majormode/__init__.py
--rwxr-xr-x   0        0        0     1189 2022-11-23 14:11:27.807149 perseus_core_library-1.19.2/src/majormode/perseus/__init__.py
--rwxr-xr-x   0        0        0     1189 2022-11-23 14:11:27.807322 perseus_core_library-1.19.2/src/majormode/perseus/constant/__init__.py
--rw-r--r--   0        0        0     1304 2022-11-23 14:11:27.807886 perseus_core_library-1.19.2/src/majormode/perseus/constant/account.py
--rw-r--r--   0        0        0     2681 2022-11-23 14:11:27.808081 perseus_core_library-1.19.2/src/majormode/perseus/constant/application.py
--rw-r--r--   0        0        0     1451 2022-11-23 14:11:27.808916 perseus_core_library-1.19.2/src/majormode/perseus/constant/area.py
--rw-r--r--   0        0        0     1225 2022-11-23 14:11:27.809504 perseus_core_library-1.19.2/src/majormode/perseus/constant/contact.py
--rw-r--r--   0        0        0     1287 2022-11-23 14:11:27.809738 perseus_core_library-1.19.2/src/majormode/perseus/constant/date.py
--rw-r--r--   0        0        0     1967 2022-11-23 14:11:27.810232 perseus_core_library-1.19.2/src/majormode/perseus/constant/http.py
--rw-r--r--   0        0        0    67093 2022-11-23 14:11:27.811739 perseus_core_library-1.19.2/src/majormode/perseus/constant/locale.py
--rw-r--r--   0        0        0     1660 2022-11-28 07:57:27.015219 perseus_core_library-1.19.2/src/majormode/perseus/constant/logging.py
--rw-r--r--   0        0        0     1507 2022-11-23 14:11:27.812751 perseus_core_library-1.19.2/src/majormode/perseus/constant/notification.py
--rw-r--r--   0        0        0     1487 2022-11-23 14:11:27.812967 perseus_core_library-1.19.2/src/majormode/perseus/constant/obj.py
--rw-r--r--   0        0        0     2148 2022-11-23 14:11:27.813172 perseus_core_library-1.19.2/src/majormode/perseus/constant/phone.py
--rw-r--r--   0        0        0     1495 2022-11-23 14:11:27.813400 perseus_core_library-1.19.2/src/majormode/perseus/constant/privacy.py
--rw-r--r--   0        0        0     5637 2023-02-08 23:35:16.851783 perseus_core_library-1.19.2/src/majormode/perseus/constant/regex.py
--rw-r--r--   0        0        0     1216 2022-11-23 14:11:27.814168 perseus_core_library-1.19.2/src/majormode/perseus/constant/sort_order.py
--rw-r--r--   0        0        0     2418 2022-11-23 14:11:27.814721 perseus_core_library-1.19.2/src/majormode/perseus/constant/stage.py
--rw-r--r--   0        0        0     1232 2022-11-23 14:11:27.815078 perseus_core_library-1.19.2/src/majormode/perseus/constant/team.py
--rw-r--r--   0        0        0     1327 2022-11-23 14:11:27.815626 perseus_core_library-1.19.2/src/majormode/perseus/constant/url.py
--rwxr-xr-x   0        0        0     1189 2022-11-23 14:11:27.816075 perseus_core_library-1.19.2/src/majormode/perseus/model/__init__.py
--rw-r--r--   0        0        0     2090 2023-02-08 23:34:13.342813 perseus_core_library-1.19.2/src/majormode/perseus/model/api_key.py
--rw-r--r--   0        0        0     3084 2023-02-08 23:34:13.317988 perseus_core_library-1.19.2/src/majormode/perseus/model/app.py
--rw-r--r--   0        0        0     2399 2023-02-08 23:34:13.342720 perseus_core_library-1.19.2/src/majormode/perseus/model/connection.py
--rw-r--r--   0        0        0    11488 2023-02-09 07:44:07.812315 perseus_core_library-1.19.2/src/majormode/perseus/model/contact.py
--rw-r--r--   0        0        0     5180 2023-02-08 23:35:01.771581 perseus_core_library-1.19.2/src/majormode/perseus/model/date.py
--rw-r--r--   0        0        0     8875 2022-11-23 14:11:27.818448 perseus_core_library-1.19.2/src/majormode/perseus/model/enum.py
--rwxr-xr-x   0        0        0    20872 2023-02-09 04:41:42.263143 perseus_core_library-1.19.2/src/majormode/perseus/model/geolocation.py
--rwxr-xr-x   0        0        0     2358 2023-02-08 23:34:41.390129 perseus_core_library-1.19.2/src/majormode/perseus/model/label.py
--rwxr-xr-x   0        0        0    14564 2023-02-08 23:35:01.747393 perseus_core_library-1.19.2/src/majormode/perseus/model/locale.py
--rwxr-xr-x   0        0        0    10597 2023-02-08 23:35:01.794562 perseus_core_library-1.19.2/src/majormode/perseus/model/obj.py
--rw-r--r--   0        0        0     2349 2023-02-08 14:09:26.884197 perseus_core_library-1.19.2/src/majormode/perseus/model/picture.py
--rw-r--r--   0        0        0     2704 2023-02-08 23:34:13.342895 perseus_core_library-1.19.2/src/majormode/perseus/model/smtp.py
--rwxr-xr-x   0        0        0     8584 2022-11-23 14:11:27.822916 perseus_core_library-1.19.2/src/majormode/perseus/model/version.py
--rwxr-xr-x   0        0        0     1189 2022-11-23 14:11:27.823305 perseus_core_library-1.19.2/src/majormode/perseus/utils/__init__.py
--rw-r--r--   0        0        0    19613 2023-02-08 23:35:01.817196 perseus_core_library-1.19.2/src/majormode/perseus/utils/cast.py
--rw-r--r--   0        0        0     5740 2023-02-08 23:35:01.816672 perseus_core_library-1.19.2/src/majormode/perseus/utils/date_util.py
--rw-r--r--   0        0        0     2009 2023-02-08 23:35:01.816582 perseus_core_library-1.19.2/src/majormode/perseus/utils/egg_util.py
--rw-r--r--   0        0        0     9876 2022-11-23 14:11:27.828666 perseus_core_library-1.19.2/src/majormode/perseus/utils/file_util.py
--rw-r--r--   0        0        0    17555 2022-11-23 14:11:27.829089 perseus_core_library-1.19.2/src/majormode/perseus/utils/image_util.py
--rw-r--r--   0        0        0     6208 2023-02-08 23:35:01.816626 perseus_core_library-1.19.2/src/majormode/perseus/utils/key_util.py
--rw-r--r--   0        0        0     3538 2023-04-04 02:18:22.869306 perseus_core_library-1.19.2/src/majormode/perseus/utils/logging.py
--rwxr-xr-x   0        0        0     6226 2022-11-23 14:11:27.829728 perseus_core_library-1.19.2/src/majormode/perseus/utils/logrotate.py
--rw-r--r--   0        0        0     2232 2022-11-23 14:11:27.830576 perseus_core_library-1.19.2/src/majormode/perseus/utils/module_util.py
--rw-r--r--   0        0        0    40681 2023-02-08 23:35:01.817460 perseus_core_library-1.19.2/src/majormode/perseus/utils/photo_util.py
--rw-r--r--   0        0        0     2748 2022-11-23 14:11:27.832666 perseus_core_library-1.19.2/src/majormode/perseus/utils/setup_util.py
--rw-r--r--   0        0        0     2325 2023-02-08 23:35:01.817123 perseus_core_library-1.19.2/src/majormode/perseus/utils/socket_util.py
--rw-r--r--   0        0        0     2659 2023-02-08 23:35:01.816384 perseus_core_library-1.19.2/src/majormode/perseus/utils/stage.py
--rw-r--r--   0        0        0     6330 2023-02-08 23:35:01.816554 perseus_core_library-1.19.2/src/majormode/perseus/utils/string_util.py
--rw-r--r--   0        0        0     4384 2023-02-08 23:35:01.816604 perseus_core_library-1.19.2/src/majormode/perseus/utils/zip_util.py
--rw-r--r--   0        0        0     1671 1970-01-01 00:00:00.000000 perseus_core_library-1.19.2/setup.py
--rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 perseus_core_library-1.19.2/PKG-INFO
+-rw-r--r--   0        0        0     4626 2023-06-14 07:57:54.260063 perseus_core_library-1.19.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1089 2020-11-13 04:28:53.612751 perseus_core_library-1.19.3/LICENSE
+-rwxr-xr-x   0        0        0      611 2023-03-31 11:33:19.503540 perseus_core_library-1.19.3/README.md
+-rw-r--r--   0        0        0      991 2023-06-14 07:57:54.256205 perseus_core_library-1.19.3/pyproject.toml
+-rwxr-xr-x   0        0        0     1189 2022-11-23 14:11:27.806929 perseus_core_library-1.19.3/src/majormode/__init__.py
+-rwxr-xr-x   0        0        0     1189 2022-11-23 14:11:27.807149 perseus_core_library-1.19.3/src/majormode/perseus/__init__.py
+-rwxr-xr-x   0        0        0     1189 2022-11-23 14:11:27.807322 perseus_core_library-1.19.3/src/majormode/perseus/constant/__init__.py
+-rw-r--r--   0        0        0     1304 2022-11-23 14:11:27.807886 perseus_core_library-1.19.3/src/majormode/perseus/constant/account.py
+-rw-r--r--   0        0        0     2681 2022-11-23 14:11:27.808081 perseus_core_library-1.19.3/src/majormode/perseus/constant/application.py
+-rw-r--r--   0        0        0     1451 2022-11-23 14:11:27.808916 perseus_core_library-1.19.3/src/majormode/perseus/constant/area.py
+-rw-r--r--   0        0        0     1225 2022-11-23 14:11:27.809504 perseus_core_library-1.19.3/src/majormode/perseus/constant/contact.py
+-rw-r--r--   0        0        0     1287 2022-11-23 14:11:27.809738 perseus_core_library-1.19.3/src/majormode/perseus/constant/date.py
+-rw-r--r--   0        0        0     1967 2022-11-23 14:11:27.810232 perseus_core_library-1.19.3/src/majormode/perseus/constant/http.py
+-rw-r--r--   0        0        0    67093 2022-11-23 14:11:27.811739 perseus_core_library-1.19.3/src/majormode/perseus/constant/locale.py
+-rw-r--r--   0        0        0     1660 2022-11-28 07:57:27.015219 perseus_core_library-1.19.3/src/majormode/perseus/constant/logging.py
+-rw-r--r--   0        0        0     1507 2022-11-23 14:11:27.812751 perseus_core_library-1.19.3/src/majormode/perseus/constant/notification.py
+-rw-r--r--   0        0        0     1487 2022-11-23 14:11:27.812967 perseus_core_library-1.19.3/src/majormode/perseus/constant/obj.py
+-rw-r--r--   0        0        0     2148 2022-11-23 14:11:27.813172 perseus_core_library-1.19.3/src/majormode/perseus/constant/phone.py
+-rw-r--r--   0        0        0     1495 2022-11-23 14:11:27.813400 perseus_core_library-1.19.3/src/majormode/perseus/constant/privacy.py
+-rw-r--r--   0        0        0     5637 2023-02-08 23:35:16.851783 perseus_core_library-1.19.3/src/majormode/perseus/constant/regex.py
+-rw-r--r--   0        0        0     1216 2022-11-23 14:11:27.814168 perseus_core_library-1.19.3/src/majormode/perseus/constant/sort_order.py
+-rw-r--r--   0        0        0     2418 2022-11-23 14:11:27.814721 perseus_core_library-1.19.3/src/majormode/perseus/constant/stage.py
+-rw-r--r--   0        0        0     1232 2022-11-23 14:11:27.815078 perseus_core_library-1.19.3/src/majormode/perseus/constant/team.py
+-rw-r--r--   0        0        0     1327 2022-11-23 14:11:27.815626 perseus_core_library-1.19.3/src/majormode/perseus/constant/url.py
+-rwxr-xr-x   0        0        0     1189 2022-11-23 14:11:27.816075 perseus_core_library-1.19.3/src/majormode/perseus/model/__init__.py
+-rw-r--r--   0        0        0     2090 2023-02-08 23:34:13.342813 perseus_core_library-1.19.3/src/majormode/perseus/model/api_key.py
+-rw-r--r--   0        0        0     3084 2023-02-08 23:34:13.317988 perseus_core_library-1.19.3/src/majormode/perseus/model/app.py
+-rw-r--r--   0        0        0     2399 2023-02-08 23:34:13.342720 perseus_core_library-1.19.3/src/majormode/perseus/model/connection.py
+-rw-r--r--   0        0        0    11488 2023-02-09 07:44:07.812315 perseus_core_library-1.19.3/src/majormode/perseus/model/contact.py
+-rw-r--r--   0        0        0     5180 2023-02-08 23:35:01.771581 perseus_core_library-1.19.3/src/majormode/perseus/model/date.py
+-rw-r--r--   0        0        0     8875 2022-11-23 14:11:27.818448 perseus_core_library-1.19.3/src/majormode/perseus/model/enum.py
+-rwxr-xr-x   0        0        0    20872 2023-02-09 04:41:42.263143 perseus_core_library-1.19.3/src/majormode/perseus/model/geolocation.py
+-rwxr-xr-x   0        0        0     2358 2023-02-08 23:34:41.390129 perseus_core_library-1.19.3/src/majormode/perseus/model/label.py
+-rwxr-xr-x   0        0        0    14564 2023-02-08 23:35:01.747393 perseus_core_library-1.19.3/src/majormode/perseus/model/locale.py
+-rwxr-xr-x   0        0        0    10597 2023-02-08 23:35:01.794562 perseus_core_library-1.19.3/src/majormode/perseus/model/obj.py
+-rw-r--r--   0        0        0     2349 2023-02-08 14:09:26.884197 perseus_core_library-1.19.3/src/majormode/perseus/model/picture.py
+-rw-r--r--   0        0        0     2704 2023-02-08 23:34:13.342895 perseus_core_library-1.19.3/src/majormode/perseus/model/smtp.py
+-rwxr-xr-x   0        0        0     8584 2022-11-23 14:11:27.822916 perseus_core_library-1.19.3/src/majormode/perseus/model/version.py
+-rwxr-xr-x   0        0        0     1189 2022-11-23 14:11:27.823305 perseus_core_library-1.19.3/src/majormode/perseus/utils/__init__.py
+-rw-r--r--   0        0        0    19613 2023-02-08 23:35:01.817196 perseus_core_library-1.19.3/src/majormode/perseus/utils/cast.py
+-rw-r--r--   0        0        0     5740 2023-02-08 23:35:01.816672 perseus_core_library-1.19.3/src/majormode/perseus/utils/date_util.py
+-rw-r--r--   0        0        0     2009 2023-02-08 23:35:01.816582 perseus_core_library-1.19.3/src/majormode/perseus/utils/egg_util.py
+-rw-r--r--   0        0        0     9876 2022-11-23 14:11:27.828666 perseus_core_library-1.19.3/src/majormode/perseus/utils/file_util.py
+-rw-r--r--   0        0        0    17555 2022-11-23 14:11:27.829089 perseus_core_library-1.19.3/src/majormode/perseus/utils/image_util.py
+-rw-r--r--   0        0        0     6208 2023-02-08 23:35:01.816626 perseus_core_library-1.19.3/src/majormode/perseus/utils/key_util.py
+-rw-r--r--   0        0        0     3538 2023-04-04 02:18:22.869306 perseus_core_library-1.19.3/src/majormode/perseus/utils/logging.py
+-rwxr-xr-x   0        0        0     6226 2022-11-23 14:11:27.829728 perseus_core_library-1.19.3/src/majormode/perseus/utils/logrotate.py
+-rw-r--r--   0        0        0     2232 2022-11-23 14:11:27.830576 perseus_core_library-1.19.3/src/majormode/perseus/utils/module_util.py
+-rw-r--r--   0        0        0    40681 2023-02-08 23:35:01.817460 perseus_core_library-1.19.3/src/majormode/perseus/utils/photo_util.py
+-rw-r--r--   0        0        0     2748 2022-11-23 14:11:27.832666 perseus_core_library-1.19.3/src/majormode/perseus/utils/setup_util.py
+-rw-r--r--   0        0        0     2325 2023-02-08 23:35:01.817123 perseus_core_library-1.19.3/src/majormode/perseus/utils/socket_util.py
+-rw-r--r--   0        0        0     2659 2023-02-08 23:35:01.816384 perseus_core_library-1.19.3/src/majormode/perseus/utils/stage.py
+-rw-r--r--   0        0        0     6352 2023-06-14 07:56:40.282483 perseus_core_library-1.19.3/src/majormode/perseus/utils/string_util.py
+-rw-r--r--   0        0        0     4384 2023-02-08 23:35:01.816604 perseus_core_library-1.19.3/src/majormode/perseus/utils/zip_util.py
+-rw-r--r--   0        0        0     1671 1970-01-01 00:00:00.000000 perseus_core_library-1.19.3/setup.py
+-rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 perseus_core_library-1.19.3/PKG-INFO
```

### Comparing `perseus_core_library-1.19.2/CHANGELOG.md` & `perseus_core_library-1.19.3/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
+## [1.19.3] - 2023-06-14
+## Fixed
+- Fix the function `string_to_keywords` to filter keywords that are not composed of the minimal required number of characters
+
 ## [1.19.2] - 2023-04-04
 ## Added
 - Add the functions `set_up_logger` and `get_console_handler` in the new module `majormode.perseus.utils.logging`
 
 ## [1.19.0] - 2023-02-08
 ## Added
 - Move the class `ISO8601DateTime` to the new module `majormode.perseus.model.date`
```

### Comparing `perseus_core_library-1.19.2/LICENSE` & `perseus_core_library-1.19.3/LICENSE`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/README.md` & `perseus_core_library-1.19.3/README.md`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/pyproject.toml` & `perseus_core_library-1.19.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 keywords = ["core", "library", "perseus"]
 license = "SEE LICENSE IN <LICENSE.md>"
 name = "perseus-core-library"
 packages = [{ include = "majormode", from = "src" }]
 readme = "README.md"
 repository = "https://github.com/majormode/perseus-core-python-library"
-version = "1.19.2"
+version = "1.19.3"
 
 [tool.poetry.dependencies]
 exifread = "^3.0.0"
 jsonpickle = "^3.0.1"
 pillow = "^9.5.0"
 python = "^3.9"
 python-dateutil = "^2.8.2"
```

### Comparing `perseus_core_library-1.19.2/src/majormode/__init__.py` & `perseus_core_library-1.19.3/src/majormode/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/__init__.py` & `perseus_core_library-1.19.3/src/majormode/perseus/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/constant/__init__.py` & `perseus_core_library-1.19.3/src/majormode/perseus/constant/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/constant/account.py` & `perseus_core_library-1.19.3/src/majormode/perseus/constant/account.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/constant/application.py` & `perseus_core_library-1.19.3/src/majormode/perseus/constant/application.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/constant/area.py` & `perseus_core_library-1.19.3/src/majormode/perseus/constant/area.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/constant/contact.py` & `perseus_core_library-1.19.3/src/majormode/perseus/constant/contact.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/constant/date.py` & `perseus_core_library-1.19.3/src/majormode/perseus/constant/date.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/constant/http.py` & `perseus_core_library-1.19.3/src/majormode/perseus/constant/http.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/constant/locale.py` & `perseus_core_library-1.19.3/src/majormode/perseus/constant/locale.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/constant/logging.py` & `perseus_core_library-1.19.3/src/majormode/perseus/constant/logging.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/constant/notification.py` & `perseus_core_library-1.19.3/src/majormode/perseus/constant/notification.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/constant/obj.py` & `perseus_core_library-1.19.3/src/majormode/perseus/constant/obj.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/constant/phone.py` & `perseus_core_library-1.19.3/src/majormode/perseus/constant/phone.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/constant/privacy.py` & `perseus_core_library-1.19.3/src/majormode/perseus/constant/privacy.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/constant/regex.py` & `perseus_core_library-1.19.3/src/majormode/perseus/constant/regex.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/constant/sort_order.py` & `perseus_core_library-1.19.3/src/majormode/perseus/constant/sort_order.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/constant/stage.py` & `perseus_core_library-1.19.3/src/majormode/perseus/constant/stage.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/constant/team.py` & `perseus_core_library-1.19.3/src/majormode/perseus/constant/team.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/constant/url.py` & `perseus_core_library-1.19.3/src/majormode/perseus/constant/url.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/model/__init__.py` & `perseus_core_library-1.19.3/src/majormode/perseus/model/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/model/api_key.py` & `perseus_core_library-1.19.3/src/majormode/perseus/model/api_key.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/model/app.py` & `perseus_core_library-1.19.3/src/majormode/perseus/model/app.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/model/connection.py` & `perseus_core_library-1.19.3/src/majormode/perseus/model/connection.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/model/contact.py` & `perseus_core_library-1.19.3/src/majormode/perseus/model/contact.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/model/date.py` & `perseus_core_library-1.19.3/src/majormode/perseus/model/date.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/model/enum.py` & `perseus_core_library-1.19.3/src/majormode/perseus/model/enum.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/model/geolocation.py` & `perseus_core_library-1.19.3/src/majormode/perseus/model/geolocation.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/model/label.py` & `perseus_core_library-1.19.3/src/majormode/perseus/model/label.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/model/locale.py` & `perseus_core_library-1.19.3/src/majormode/perseus/model/locale.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/model/obj.py` & `perseus_core_library-1.19.3/src/majormode/perseus/model/obj.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/model/picture.py` & `perseus_core_library-1.19.3/src/majormode/perseus/model/picture.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/model/smtp.py` & `perseus_core_library-1.19.3/src/majormode/perseus/model/smtp.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/model/version.py` & `perseus_core_library-1.19.3/src/majormode/perseus/model/version.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/utils/__init__.py` & `perseus_core_library-1.19.3/src/majormode/perseus/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/utils/cast.py` & `perseus_core_library-1.19.3/src/majormode/perseus/utils/cast.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/utils/date_util.py` & `perseus_core_library-1.19.3/src/majormode/perseus/utils/date_util.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/utils/egg_util.py` & `perseus_core_library-1.19.3/src/majormode/perseus/utils/egg_util.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/utils/file_util.py` & `perseus_core_library-1.19.3/src/majormode/perseus/utils/file_util.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/utils/image_util.py` & `perseus_core_library-1.19.3/src/majormode/perseus/utils/image_util.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/utils/key_util.py` & `perseus_core_library-1.19.3/src/majormode/perseus/utils/key_util.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/utils/logging.py` & `perseus_core_library-1.19.3/src/majormode/perseus/utils/logging.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/utils/logrotate.py` & `perseus_core_library-1.19.3/src/majormode/perseus/utils/logrotate.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/utils/module_util.py` & `perseus_core_library-1.19.3/src/majormode/perseus/utils/module_util.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/utils/photo_util.py` & `perseus_core_library-1.19.3/src/majormode/perseus/utils/photo_util.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/utils/setup_util.py` & `perseus_core_library-1.19.3/src/majormode/perseus/utils/setup_util.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/utils/socket_util.py` & `perseus_core_library-1.19.3/src/majormode/perseus/utils/socket_util.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/utils/stage.py` & `perseus_core_library-1.19.3/src/majormode/perseus/utils/stage.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/utils/string_util.py` & `perseus_core_library-1.19.3/src/majormode/perseus/utils/string_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,52 +34,52 @@
 
 
 def flatten_list(l):
     """
     Flatten the elements contained in the sub-lists of a list.
 
 
-    @param l: A list containing sub-lists of elements.
+    :param l: A list containing sub-lists of elements.
 
 
-    @return: A list with all the elements flattened from the sub-lists of
+    :return: A list with all the elements flattened from the sub-lists of
         the list `l`.
     """
     return [e for sublist in l for e in sublist]
 
 
 def inicap_string(s, cleanse=False):
     """
     Convert the first letter of each word to capital letter without
     touching the rest of the word.
 
 
-    @param s: a string.
+    :param s: a string.
 
-    @param cleanse: `True` to remove any separator character from the
+    :param cleanse: `True` to remove any separator character from the
         string, such as comma; `False` to keeps any character but space.
 
 
-    @return: a string for which the first letter of each word has been
+    :return: a string for which the first letter of each word has been
         capitalized without modifying the case of the rest of the word.
     """
     return s and ' '.join([
         word[0].upper() + word[1:]
         for word in (s.split() if cleanse else s.split(' '))])
 
 
 def is_email_address(s):
     """
     Indicate whether a string corresponds to an email address
 
 
-    @param s: A string that is expected to be an email address.
+    :param s: A string that is expected to be an email address.
 
 
-    @return: `True` if the string corresponds to an email address,
+    :return: `True` if the string corresponds to an email address,
         `False` otherwise.
     """
     return (s and REGEX_EMAIL_ADDRESS.match(s.strip().lower())) is not None
 
 
 def is_phone_number(s):
     """
@@ -91,87 +91,87 @@
 
     EPP-style phone numbers use the format `+CCC.NNNNNNNNNNxEEEE`, where
     `C` is the 1–3 digit country code, `N` is up to 14 digits, and `E` is
     the (optional) extension.  The leading plus sign and the dot following
     the country code are required.  The literal "x" character is required
     only if an extension is provided.
 
-    @param s: An EPP-style phone number.
+    :param s: An EPP-style phone number.
 
 
-    @return: `True` if the string represents an international phone number,
+    :return: `True` if the string represents an international phone number,
         `False` otherwise.
     """
     return (s and REGEX_PHONE_NUMBER.match(s.strip())) is not None
 
 
 def is_username(s):
     """
     Indicate whether a string corresponds to a username
 
 
-    @param s: A username
+    :param s: A username
 
 
-    @return: `True` if the string represents a username, `False` otherwise.
+    :return: `True` if the string represents a username, `False` otherwise.
     """
     return (s and REGEX_USERNAME.match(s.strip())) is not None
 
 
 def string_hash_code(s):
     """
     Calculate the hash code of a string.
 
 
-    @param s: a string.
+    :param s: a string.
 
 
-    @return: the hash code of the string.
+    :return: the hash code of the string.
     """
     string_length = len(s)
     return functools.reduce(
         lambda x, y: x + y,
         [ord(s[i]) * 31 ** (string_length - i - 1) for i in range(string_length)]) % sys.maxsize
 
 
 def strip_string_words(s):
     """
     Return the string with all its words stripped.
 
 
-    @param s: A string.
+    :param s: A string.
 
 
-    @return: The string with all its words stripped.
+    :return: The string with all its words stripped.
     """
     return s and ' '.join([word for word in s.split(' ')])
 
 
 def string_to_keywords(s, keyword_minimal_length=1):
     """
     Split the specified string(s) in a list of ASCII keywords
 
     Remove any punctuation character from the specified list of keywords,
     remove any double or more space character and represent Unicode
     characters in ASCII.
 
 
-    @param s: A word or a list of words to strip out any punctuation
+    :param s: A word or a list of words to strip out any punctuation
         characters and to convert to ASCII characters.
 
-    @param keyword_minimal_length: Minimal number of characters of the
+    :param keyword_minimal_length: Minimal number of characters of the
         keywords to be returned.
 
 
-    @return: A list of distinct keywords cleansed from any special Unicode
+    :return: A list of distinct keywords cleansed from any special Unicode
         accentuated character, punctuation character, and double space
         character.
 
 
-    @raise ValueError: If the argument is null, or if it is not a string
+    :raise ValueError: If the argument is null, or if it is not a string
         or a list of string.
     """
     if s is None:
         return None
 
     if isinstance(s, str):
         s = [s]
@@ -195,15 +195,15 @@
 
     # Decompose the string into distinct keywords.
     keywords = set(flatten_list([
         _.split()
         for _ in punctuationless_strings
     ]))
 
-    # Filter out sub-keywords of less than 2 characters.
+    # Filter out sub-keywords of less than the required number of characters.
     keywords = [
         keyword
         for keyword in keywords
-        if len(keyword) > keyword_minimal_length
+        if len(keyword) >= keyword_minimal_length
     ]
 
     return keywords
```

### Comparing `perseus_core_library-1.19.2/src/majormode/perseus/utils/zip_util.py` & `perseus_core_library-1.19.3/src/majormode/perseus/utils/zip_util.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.2/setup.py` & `perseus_core_library-1.19.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  'python-dateutil>=2.8.2,<3.0.0',
  'pytz>=2023.3,<2024.0',
  'six>=1.16.0,<2.0.0',
  'unidecode>=1.3.6,<2.0.0']
 
 setup_kwargs = {
     'name': 'perseus-core-library',
-    'version': '1.19.2',
+    'version': '1.19.3',
     'description': 'Perseus Core Python library',
     'long_description': '# Perseus: Core Python Library\n\nPerseus Core Python Library is a repository of reusable Python components to be shared with Python projects integrating Perseus RESTful API server framework.\n\nThese components have minimal dependencies on other libraries, so that they can be deployed easily.  In addition, these components will keep their interfaces as stable as possible, so that other Python projects can integrate these components without having to worry about changes in the future.\n\n\nTo install the Perseus Core Python Library, enter the follow command line:\n\n```bash\n$ pip install perseus-core-library\n```\n',
     'author': 'Daniel CAUNE',
     'author_email': 'daniel.caune@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/majormode/perseus-core-python-library',
```

### Comparing `perseus_core_library-1.19.2/PKG-INFO` & `perseus_core_library-1.19.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perseus-core-library
-Version: 1.19.2
+Version: 1.19.3
 Summary: Perseus Core Python library
 Home-page: https://github.com/majormode/perseus-core-python-library
 License: SEE LICENSE IN <LICENSE.md>
 Keywords: core,library,perseus
 Author: Daniel CAUNE
 Author-email: daniel.caune@gmail.com
 Requires-Python: >=3.9,<4.0
```

