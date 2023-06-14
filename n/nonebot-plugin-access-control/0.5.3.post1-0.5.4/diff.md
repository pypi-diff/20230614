# Comparing `tmp/nonebot_plugin_access_control-0.5.3.post1.tar.gz` & `tmp/nonebot_plugin_access_control-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_access_control-0.5.3.post1.tar", max compression
+gzip compressed data, was "nonebot_plugin_access_control-0.5.4.tar", max compression
```

## Comparing `nonebot_plugin_access_control-0.5.3.post1.tar` & `nonebot_plugin_access_control-0.5.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1085 2022-07-09 13:18:24.594000 nonebot_plugin_access_control-0.5.3.post1/LICENSE
--rw-r--r--   0        0        0      912 2023-06-07 03:20:22.691172 nonebot_plugin_access_control-0.5.3.post1/pyproject.toml
--rw-r--r--   0        0        0    19070 2023-06-02 01:51:58.407828 nonebot_plugin_access_control-0.5.3.post1/README.MD
--rw-r--r--   0        0        0     3470 2023-06-04 14:34:31.319994 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/__init__.py
--rw-r--r--   0        0        0      579 2023-05-30 02:34:22.187998 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/config.py
--rw-r--r--   0        0        0      248 2023-02-14 09:17:25.623083 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/errors.py
--rw-r--r--   0        0        0     2363 2023-02-14 08:19:30.714606 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/event_bus.py
--rw-r--r--   0        0        0    10794 2023-06-01 01:16:36.463425 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/matchers/__init__.py
--rw-r--r--   0        0        0     1005 2023-02-13 06:25:49.446680 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/matchers/handle_error.py
--rw-r--r--   0        0        0     3352 2023-06-01 01:13:05.751049 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/matchers/parser.py
--rw-r--r--   0        0        0     3693 2023-03-13 03:28:05.306313 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/migrations/875c4dd8c271_.py
--rw-r--r--   0        0        0      172 2023-03-13 03:19:06.944840 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/models/__init__.py
--rw-r--r--   0        0        0      461 2023-03-13 03:19:06.944840 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/models/permission.py
--rw-r--r--   0        0        0     1754 2023-03-13 03:19:06.945840 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/models/rate_limit.py
--rw-r--r--   0        0        0      119 2023-03-13 03:19:06.946840 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/plugin_data.py
--rw-r--r--   0        0        0      159 2023-02-13 07:58:33.466319 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/__init__.py
--rw-r--r--   0        0        0     8872 2023-05-30 03:15:13.076049 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/base.py
--rw-r--r--   0        0        0        0 2023-02-13 08:30:50.046295 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/impl/__init__.py
--rw-r--r--   0        0        0     8257 2023-03-13 03:19:06.946840 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/impl/permission.py
--rw-r--r--   0        0        0    11920 2023-05-27 05:28:53.341561 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/impl/rate_limit.py
--rw-r--r--   0        0        0       31 2023-02-13 07:07:23.516417 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/interface/__init__.py
--rw-r--r--   0        0        0     2089 2023-05-30 02:47:39.681782 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/interface/base.py
--rw-r--r--   0        0        0     1630 2023-02-14 07:23:00.750461 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/interface/permission.py
--rw-r--r--   0        0        0     1948 2023-05-27 05:06:59.272662 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/interface/rate_limit.py
--rw-r--r--   0        0        0      680 2023-02-13 08:40:31.774931 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/interface/service.py
--rw-r--r--   0        0        0      334 2023-02-13 07:59:53.174308 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/interface/subservice_owner.py
--rw-r--r--   0        0        0      882 2023-02-14 07:23:39.399678 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/methods.py
--rw-r--r--   0        0        0     2392 2023-02-14 07:30:48.027513 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/nonebot.py
--rw-r--r--   0        0        0       36 2023-02-14 06:34:31.631671 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/permission/__init__.py
--rw-r--r--   0        0        0      224 2023-02-14 07:59:38.644831 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/permission/permission.py
--rw-r--r--   0        0        0      907 2023-02-13 07:53:46.438693 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/plugin.py
--rw-r--r--   0        0        0       74 2023-05-27 05:06:59.273662 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/rate_limit/__init__.py
--rw-r--r--   0        0        0      318 2023-02-14 09:29:28.023174 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/rate_limit/rule.py
--rw-r--r--   0        0        0      181 2023-05-27 05:06:59.273662 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/rate_limit/token.py
--rw-r--r--   0        0        0      840 2023-02-13 07:54:44.558096 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/subservice.py
--rw-r--r--   0        0        0     1645 2023-02-14 06:59:06.539473 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/subservice_owner.py
--rw-r--r--   0        0        0       26 2023-02-20 02:15:08.129834 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/subject/__init__.py
--rw-r--r--   0        0        0      855 2023-06-02 02:16:32.433342 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/subject/extractor/__init__.py
--rw-r--r--   0        0        0      508 2023-06-02 02:16:32.442340 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/subject/extractor/base.py
--rw-r--r--   0        0        0     1826 2023-06-04 14:29:01.177719 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/subject/extractor/onebot_v11.py
--rw-r--r--   0        0        0      590 2023-06-02 02:16:32.446339 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/subject/extractor/onebot_v12.py
--rw-r--r--   0        0        0     2093 2023-06-02 02:16:32.413738 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/subject/extractor/session.py
--rw-r--r--   0        0        0      938 2023-06-02 02:16:32.471866 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/subject/extractor/union.py
--rw-r--r--   0        0        0        0 2022-12-10 06:08:59.849075 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/utils/__init__.py
--rw-r--r--   0        0        0      531 2023-03-13 03:19:06.948840 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/utils/session.py
--rw-r--r--   0        0        0      425 2023-02-20 04:34:52.815055 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/utils/superuser.py
--rw-r--r--   0        0        0     1015 2022-12-10 06:23:22.420137 nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/utils/tree.py
--rw-r--r--   0        0        0    19516 1970-01-01 00:00:00.000000 nonebot_plugin_access_control-0.5.3.post1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2022-07-09 13:18:24.594000 nonebot_plugin_access_control-0.5.4/LICENSE
+-rw-r--r--   0        0        0      907 2023-06-14 12:05:19.259680 nonebot_plugin_access_control-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0    19070 2023-06-02 01:51:58.407828 nonebot_plugin_access_control-0.5.4/README.MD
+-rw-r--r--   0        0        0     3470 2023-06-04 14:34:31.319994 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/__init__.py
+-rw-r--r--   0        0        0      579 2023-05-30 02:34:22.187998 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/config.py
+-rw-r--r--   0        0        0      248 2023-02-14 09:17:25.623083 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/errors.py
+-rw-r--r--   0        0        0     2363 2023-02-14 08:19:30.714606 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/event_bus.py
+-rw-r--r--   0        0        0    10794 2023-06-01 01:16:36.463425 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/matchers/__init__.py
+-rw-r--r--   0        0        0     1005 2023-02-13 06:25:49.446680 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/matchers/handle_error.py
+-rw-r--r--   0        0        0     3352 2023-06-01 01:13:05.751049 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/matchers/parser.py
+-rw-r--r--   0        0        0     3693 2023-03-13 03:28:05.306313 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/migrations/875c4dd8c271_.py
+-rw-r--r--   0        0        0      172 2023-03-13 03:19:06.944840 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/models/__init__.py
+-rw-r--r--   0        0        0      461 2023-03-13 03:19:06.944840 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/models/permission.py
+-rw-r--r--   0        0        0     1754 2023-03-13 03:19:06.945840 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/models/rate_limit.py
+-rw-r--r--   0        0        0      119 2023-03-13 03:19:06.946840 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/plugin_data.py
+-rw-r--r--   0        0        0      159 2023-02-13 07:58:33.466319 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/__init__.py
+-rw-r--r--   0        0        0     8872 2023-05-30 03:15:13.076049 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/base.py
+-rw-r--r--   0        0        0        0 2023-02-13 08:30:50.046295 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/impl/__init__.py
+-rw-r--r--   0        0        0     8257 2023-03-13 03:19:06.946840 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/impl/permission.py
+-rw-r--r--   0        0        0    11920 2023-05-27 05:28:53.341561 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/impl/rate_limit.py
+-rw-r--r--   0        0        0       31 2023-02-13 07:07:23.516417 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/interface/__init__.py
+-rw-r--r--   0        0        0     2089 2023-05-30 02:47:39.681782 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/interface/base.py
+-rw-r--r--   0        0        0     1630 2023-02-14 07:23:00.750461 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/interface/permission.py
+-rw-r--r--   0        0        0     1948 2023-05-27 05:06:59.272662 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/interface/rate_limit.py
+-rw-r--r--   0        0        0      680 2023-02-13 08:40:31.774931 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/interface/service.py
+-rw-r--r--   0        0        0      334 2023-02-13 07:59:53.174308 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/interface/subservice_owner.py
+-rw-r--r--   0        0        0      882 2023-02-14 07:23:39.399678 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/methods.py
+-rw-r--r--   0        0        0     2392 2023-02-14 07:30:48.027513 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/nonebot.py
+-rw-r--r--   0        0        0       36 2023-02-14 06:34:31.631671 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/permission/__init__.py
+-rw-r--r--   0        0        0      224 2023-02-14 07:59:38.644831 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/permission/permission.py
+-rw-r--r--   0        0        0      907 2023-02-13 07:53:46.438693 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/plugin.py
+-rw-r--r--   0        0        0       74 2023-05-27 05:06:59.273662 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/rate_limit/__init__.py
+-rw-r--r--   0        0        0      318 2023-02-14 09:29:28.023174 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/rate_limit/rule.py
+-rw-r--r--   0        0        0      181 2023-05-27 05:06:59.273662 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/rate_limit/token.py
+-rw-r--r--   0        0        0      840 2023-02-13 07:54:44.558096 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/subservice.py
+-rw-r--r--   0        0        0     1645 2023-02-14 06:59:06.539473 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/subservice_owner.py
+-rw-r--r--   0        0        0       26 2023-02-20 02:15:08.129834 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/subject/__init__.py
+-rw-r--r--   0        0        0      855 2023-06-02 02:16:32.433342 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/subject/extractor/__init__.py
+-rw-r--r--   0        0        0      508 2023-06-02 02:16:32.442340 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/subject/extractor/base.py
+-rw-r--r--   0        0        0     1826 2023-06-04 14:29:01.177719 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/subject/extractor/onebot_v11.py
+-rw-r--r--   0        0        0      590 2023-06-02 02:16:32.446339 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/subject/extractor/onebot_v12.py
+-rw-r--r--   0        0        0     2093 2023-06-02 02:16:32.413738 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/subject/extractor/session.py
+-rw-r--r--   0        0        0      938 2023-06-02 02:16:32.471866 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/subject/extractor/union.py
+-rw-r--r--   0        0        0        0 2022-12-10 06:08:59.849075 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/utils/__init__.py
+-rw-r--r--   0        0        0      531 2023-03-13 03:19:06.948840 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/utils/session.py
+-rw-r--r--   0        0        0      425 2023-02-20 04:34:52.815055 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/utils/superuser.py
+-rw-r--r--   0        0        0     1015 2022-12-10 06:23:22.420137 nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/utils/tree.py
+-rw-r--r--   0        0        0    19503 1970-01-01 00:00:00.000000 nonebot_plugin_access_control-0.5.4/PKG-INFO
```

### Comparing `nonebot_plugin_access_control-0.5.3.post1/LICENSE` & `nonebot_plugin_access_control-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/pyproject.toml` & `nonebot_plugin_access_control-0.5.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "nonebot-plugin-access-control"
-version = "0.5.3.post1"
+version = "0.5.4"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 license = "MIT"
 readme = "README.MD"
 repository = "https://github.com/ssttkkl/nonebot-plugin-access-control"
 packages = [
     { include = "nonebot_plugin_access_control", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 nonebot2 = "^2.0.0"
-nonebot-plugin-datastore = "^0.6.0"
+nonebot-plugin-datastore = "^1.0.0"
 nonebot-plugin-apscheduler = "^0.2.0"
-nonebot-plugin-session = "^0.0.4"
+nonebot-plugin-session = ">=0.0.4"
 shortuuid = "^1.0.11"
 
 
 [tool.poetry.group.dev.dependencies]
 nonebot-adapter-onebot = "^2.1.5"
 nonebot-adapter-kaiheila = "^0.1.0"
 nonebot-adapter-qqguild = "^0.2.2"
```

### Comparing `nonebot_plugin_access_control-0.5.3.post1/README.MD` & `nonebot_plugin_access_control-0.5.4/README.MD`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/__init__.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/config.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/event_bus.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/event_bus.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/matchers/__init__.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/matchers/handle_error.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/matchers/handle_error.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/matchers/parser.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/matchers/parser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/migrations/875c4dd8c271_.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/migrations/875c4dd8c271_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/models/rate_limit.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/models/rate_limit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/base.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/impl/permission.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/impl/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/impl/rate_limit.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/impl/rate_limit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/interface/base.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/interface/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/interface/permission.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/interface/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/interface/rate_limit.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/interface/rate_limit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/interface/service.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/interface/service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/methods.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/methods.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/nonebot.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/nonebot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/plugin.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/plugin.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/subservice.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/subservice.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/service/subservice_owner.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/service/subservice_owner.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/subject/extractor/__init__.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/subject/extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/subject/extractor/onebot_v11.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/subject/extractor/onebot_v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/subject/extractor/onebot_v12.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/subject/extractor/onebot_v12.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/subject/extractor/session.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/subject/extractor/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/subject/extractor/union.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/subject/extractor/union.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/utils/session.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/utils/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/src/nonebot_plugin_access_control/utils/tree.py` & `nonebot_plugin_access_control-0.5.4/src/nonebot_plugin_access_control/utils/tree.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.3.post1/PKG-INFO` & `nonebot_plugin_access_control-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-access-control
-Version: 0.5.3.post1
+Version: 0.5.4
 Summary: 
 Home-page: https://github.com/ssttkkl/nonebot-plugin-access-control
 License: MIT
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
-Requires-Dist: nonebot-plugin-datastore (>=0.6.0,<0.7.0)
-Requires-Dist: nonebot-plugin-session (>=0.0.4,<0.0.5)
+Requires-Dist: nonebot-plugin-datastore (>=1.0.0,<2.0.0)
+Requires-Dist: nonebot-plugin-session (>=0.0.4)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Requires-Dist: shortuuid (>=1.0.11,<2.0.0)
 Project-URL: Repository, https://github.com/ssttkkl/nonebot-plugin-access-control
 Description-Content-Type: text/plain
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-access-control Version: 0.5.3.post1
+Metadata-Version: 2.1 Name: nonebot-plugin-access-control Version: 0.5.4
 Summary: Home-page: https://github.com/ssttkkl/nonebot-plugin-access-control
 License: MIT Author: ssttkkl Author-email: huang.wen.long@hotmail.com Requires-
 Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: nonebot-
 plugin-apscheduler (>=0.2.0,<0.3.0) Requires-Dist: nonebot-plugin-datastore
-(>=0.6.0,<0.7.0) Requires-Dist: nonebot-plugin-session (>=0.0.4,<0.0.5)
-Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Requires-Dist: shortuuid
-(>=1.0.11,<2.0.0) Project-URL: Repository, https://github.com/ssttkkl/nonebot-
-plugin-access-control Description-Content-Type: text/plain
+(>=1.0.0,<2.0.0) Requires-Dist: nonebot-plugin-session (>=0.0.4) Requires-Dist:
+nonebot2 (>=2.0.0,<3.0.0) Requires-Dist: shortuuid (>=1.0.11,<2.0.0) Project-
+URL: Repository, https://github.com/ssttkkl/nonebot-plugin-access-control
+Description-Content-Type: text/plain
                                    [nonebot]
    nonebot-plugin-access-control ============ _â¨ Nonebot æéæ§å¶ â¨_
                            [license] [pypi] [python]
 ## ç¹ç¹ - åè½ - [x] æ¯æéå¯¹ç¨æ·/ç¾¤ç»çæéå¼å³ - [x]
 æ¯æéå¶åä¸ç¨æ·å¨ä¸å®æ¶é´åçæä»¤è°ç¨æ¬¡æ° - [x]
 å¯¹æªééæä»¶æä¾**æä»¶çº§å«**çæ§å¶æ¯æ - æä»¶éé - [x]
 æ¯æ**åè½çº§å«**çç»ç²åº¦æ§å¶ - [x]
```

