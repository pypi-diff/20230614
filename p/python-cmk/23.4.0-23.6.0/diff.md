# Comparing `tmp/python_cmk-23.4.0.tar.gz` & `tmp/python_cmk-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_cmk-23.4.0.tar", max compression
+gzip compressed data, was "python_cmk-23.6.0.tar", max compression
```

## Comparing `python_cmk-23.4.0.tar` & `python_cmk-23.6.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0    34672 2022-09-01 18:58:18.513934 python_cmk-23.4.0/LICENSE.md
--rw-r--r--   0        0        0      884 2023-03-19 00:16:02.972445 python_cmk-23.4.0/README.md
--rw-r--r--   0        0        0     3057 2023-04-03 20:49:55.037716 python_cmk-23.4.0/pyproject.toml
--rw-r--r--   0        0        0      510 2022-05-15 20:11:08.237914 python_cmk-23.4.0/src/cmk/__about__.py
--rw-r--r--   0        0        0      304 2022-07-07 00:00:59.174973 python_cmk-23.4.0/src/cmk/__init__.py
--rw-r--r--   0        0        0      247 2023-04-03 20:48:59.441946 python_cmk-23.4.0/src/cmk/_version.py
--rw-r--r--   0        0        0     1901 2023-03-18 20:27:55.570897 python_cmk-23.4.0/src/cmk/common.py
--rw-r--r--   0        0        0     3263 2022-09-01 22:55:16.927379 python_cmk-23.4.0/src/cmk/httpapi.py
--rw-r--r--   0        0        0     4304 2023-04-03 20:32:47.226142 python_cmk-23.4.0/src/cmk/objectapi.py
--rw-r--r--   0        0        0      738 2023-03-31 20:37:51.143158 python_cmk-23.4.0/src/cmk/objects/__init__.py
--rw-r--r--   0        0        0      450 2022-11-04 09:49:12.944068 python_cmk-23.4.0/src/cmk/objects/activation_run.py
--rw-r--r--   0        0        0     2126 2022-11-11 21:14:42.674456 python_cmk-23.4.0/src/cmk/objects/attributes.py
--rw-r--r--   0        0        0      722 2023-04-03 20:43:07.980108 python_cmk-23.4.0/src/cmk/objects/aux_tag.py
--rw-r--r--   0        0        0     7440 2023-03-18 21:50:34.579541 python_cmk-23.4.0/src/cmk/objects/base.py
--rw-r--r--   0        0        0      464 2023-04-03 20:42:23.604497 python_cmk-23.4.0/src/cmk/objects/bi_aggregation.py
--rw-r--r--   0        0        0      270 2023-04-03 20:43:07.968108 python_cmk-23.4.0/src/cmk/objects/bi_pack.py
--rw-r--r--   0        0        0      525 2022-10-28 21:48:36.246675 python_cmk-23.4.0/src/cmk/objects/contact_group_config.py
--rw-r--r--   0        0        0      423 2023-01-30 20:48:10.009967 python_cmk-23.4.0/src/cmk/objects/dictionary.py
--rw-r--r--   0        0        0     2931 2023-01-30 20:48:10.009967 python_cmk-23.4.0/src/cmk/objects/folder_config.py
--rw-r--r--   0        0        0     1181 2023-03-18 21:45:41.220147 python_cmk-23.4.0/src/cmk/objects/host.py
--rw-r--r--   0        0        0     1206 2023-01-23 20:57:28.083432 python_cmk-23.4.0/src/cmk/objects/host_config.py
--rw-r--r--   0        0        0      516 2023-01-25 22:34:11.430895 python_cmk-23.4.0/src/cmk/objects/host_group_config.py
--rw-r--r--   0        0        0       25 2023-04-03 20:32:44.978204 python_cmk-23.4.0/src/cmk/objects/interface/__init__.py
--rw-r--r--   0        0        0      545 2023-04-03 20:32:47.142144 python_cmk-23.4.0/src/cmk/objects/interface/title.py
--rw-r--r--   0        0        0      389 2023-03-10 22:23:39.513594 python_cmk-23.4.0/src/cmk/objects/internal.py
--rw-r--r--   0        0        0     1487 2023-03-18 21:23:55.894318 python_cmk-23.4.0/src/cmk/objects/rule.py
--rw-r--r--   0        0        0      429 2023-01-30 20:48:10.009967 python_cmk-23.4.0/src/cmk/objects/ruleset.py
--rw-r--r--   0        0        0      493 2023-03-18 21:44:11.188319 python_cmk-23.4.0/src/cmk/objects/service.py
--rw-r--r--   0        0        0      614 2023-03-18 20:26:38.359704 python_cmk-23.4.0/src/cmk/objects/service_discovery.py
--rw-r--r--   0        0        0      790 2023-03-18 20:26:53.655856 python_cmk-23.4.0/src/cmk/objects/service_discovery_run.py
--rw-r--r--   0        0        0      525 2023-01-22 00:41:20.794218 python_cmk-23.4.0/src/cmk/objects/service_group_config.py
--rw-r--r--   0        0        0      524 2022-10-28 21:50:00.850790 python_cmk-23.4.0/src/cmk/objects/user_config.py
--rw-r--r--   0        0        0      501 2022-10-29 22:18:29.348397 python_cmk-23.4.0/src/cmk/objects/user_role.py
--rw-r--r--   0        0        0     3817 2023-03-18 22:02:36.757901 python_cmk-23.4.0/src/cmk/restapi.py
--rw-r--r--   0        0        0     1676 1970-01-01 00:00:00.000000 python_cmk-23.4.0/setup.py
--rw-r--r--   0        0        0     2163 1970-01-01 00:00:00.000000 python_cmk-23.4.0/PKG-INFO
+-rw-r--r--   0        0        0    34672 2022-09-01 18:58:18.513934 python_cmk-23.6.0/LICENSE.md
+-rw-r--r--   0        0        0      884 2023-03-19 00:16:02.972445 python_cmk-23.6.0/README.md
+-rw-r--r--   0        0        0     3057 2023-06-14 20:31:32.182273 python_cmk-23.6.0/pyproject.toml
+-rw-r--r--   0        0        0      510 2022-05-15 20:11:08.237914 python_cmk-23.6.0/src/cmk/__about__.py
+-rw-r--r--   0        0        0      304 2022-07-07 00:00:59.174973 python_cmk-23.6.0/src/cmk/__init__.py
+-rw-r--r--   0        0        0      247 2023-06-14 20:30:43.370541 python_cmk-23.6.0/src/cmk/_version.py
+-rw-r--r--   0        0        0     1901 2023-03-18 20:27:55.570897 python_cmk-23.6.0/src/cmk/common.py
+-rw-r--r--   0        0        0     3263 2022-09-01 22:55:16.927379 python_cmk-23.6.0/src/cmk/httpapi.py
+-rw-r--r--   0        0        0     4337 2023-06-04 21:13:44.119207 python_cmk-23.6.0/src/cmk/objectapi.py
+-rw-r--r--   0        0        0      782 2023-06-14 20:26:55.972176 python_cmk-23.6.0/src/cmk/objects/__init__.py
+-rw-r--r--   0        0        0      450 2022-11-04 09:49:12.944068 python_cmk-23.6.0/src/cmk/objects/activation_run.py
+-rw-r--r--   0        0        0     2126 2022-11-11 21:14:42.674456 python_cmk-23.6.0/src/cmk/objects/attributes.py
+-rw-r--r--   0        0        0      722 2023-04-03 20:43:07.980108 python_cmk-23.6.0/src/cmk/objects/aux_tag.py
+-rw-r--r--   0        0        0     7440 2023-03-18 21:50:34.579541 python_cmk-23.6.0/src/cmk/objects/base.py
+-rw-r--r--   0        0        0      464 2023-04-03 20:42:23.604497 python_cmk-23.6.0/src/cmk/objects/bi_aggregation.py
+-rw-r--r--   0        0        0      270 2023-04-03 20:43:07.968108 python_cmk-23.6.0/src/cmk/objects/bi_pack.py
+-rw-r--r--   0        0        0      525 2022-10-28 21:48:36.246675 python_cmk-23.6.0/src/cmk/objects/contact_group_config.py
+-rw-r--r--   0        0        0      423 2023-01-30 20:48:10.009967 python_cmk-23.6.0/src/cmk/objects/dictionary.py
+-rw-r--r--   0        0        0     3017 2023-06-14 20:00:43.439257 python_cmk-23.6.0/src/cmk/objects/folder_config.py
+-rw-r--r--   0        0        0     1181 2023-03-18 21:45:41.220147 python_cmk-23.6.0/src/cmk/objects/host.py
+-rw-r--r--   0        0        0     1206 2023-01-23 20:57:28.083432 python_cmk-23.6.0/src/cmk/objects/host_config.py
+-rw-r--r--   0        0        0      516 2023-01-25 22:34:11.430895 python_cmk-23.6.0/src/cmk/objects/host_group_config.py
+-rw-r--r--   0        0        0       25 2023-04-03 20:32:44.978204 python_cmk-23.6.0/src/cmk/objects/interface/__init__.py
+-rw-r--r--   0        0        0      545 2023-04-03 20:32:47.142144 python_cmk-23.6.0/src/cmk/objects/interface/title.py
+-rw-r--r--   0        0        0      389 2023-03-10 22:23:39.513594 python_cmk-23.6.0/src/cmk/objects/internal.py
+-rw-r--r--   0        0        0     1487 2023-03-18 21:23:55.894318 python_cmk-23.6.0/src/cmk/objects/rule.py
+-rw-r--r--   0        0        0      429 2023-01-30 20:48:10.009967 python_cmk-23.6.0/src/cmk/objects/ruleset.py
+-rw-r--r--   0        0        0      493 2023-03-18 21:44:11.188319 python_cmk-23.6.0/src/cmk/objects/service.py
+-rw-r--r--   0        0        0      614 2023-03-18 20:26:38.359704 python_cmk-23.6.0/src/cmk/objects/service_discovery.py
+-rw-r--r--   0        0        0      790 2023-03-18 20:26:53.655856 python_cmk-23.6.0/src/cmk/objects/service_discovery_run.py
+-rw-r--r--   0        0        0      525 2023-01-22 00:41:20.794218 python_cmk-23.6.0/src/cmk/objects/service_group_config.py
+-rw-r--r--   0        0        0      497 2023-06-14 20:24:43.980440 python_cmk-23.6.0/src/cmk/objects/site_connection.py
+-rw-r--r--   0        0        0      524 2022-10-28 21:50:00.850790 python_cmk-23.6.0/src/cmk/objects/user_config.py
+-rw-r--r--   0        0        0      501 2022-10-29 22:18:29.348397 python_cmk-23.6.0/src/cmk/objects/user_role.py
+-rw-r--r--   0        0        0     3817 2023-03-18 22:02:36.757901 python_cmk-23.6.0/src/cmk/restapi.py
+-rw-r--r--   0        0        0     1676 1970-01-01 00:00:00.000000 python_cmk-23.6.0/setup.py
+-rw-r--r--   0        0        0     2163 1970-01-01 00:00:00.000000 python_cmk-23.6.0/PKG-INFO
```

### Comparing `python_cmk-23.4.0/LICENSE.md` & `python_cmk-23.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `python_cmk-23.4.0/README.md` & `python_cmk-23.6.0/README.md`

 * *Files identical despite different names*

### Comparing `python_cmk-23.4.0/pyproject.toml` & `python_cmk-23.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.masonry.api"
 
 [tool.black]
 line-length = 88
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "23.4.0"
+version = "23.6.0"
 version_files = [
   "pyproject.toml:version"
 ]
 tag_format = "v$version"
 
 [tool.flakeheaven]
 format = "grouped"
@@ -69,15 +69,15 @@
   "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 description = "API for CheckMK"
 license = "GPL-3.0-or-later"
 name = "python-cmk"
 readme = "README.md"
 repository = "https://github.com/NimVek/python-cmk"
-version = "23.4.0"
+version = "23.6.0"
 packages = [
   {include = "cmk", from = "src"}
 ]
 
 [tool.poetry.dependencies]
 incremental = "^22"
 python = "^3.8"
```

### Comparing `python_cmk-23.4.0/src/cmk/common.py` & `python_cmk-23.6.0/src/cmk/common.py`

 * *Files identical despite different names*

### Comparing `python_cmk-23.4.0/src/cmk/httpapi.py` & `python_cmk-23.6.0/src/cmk/httpapi.py`

 * *Files identical despite different names*

### Comparing `python_cmk-23.4.0/src/cmk/objectapi.py` & `python_cmk-23.6.0/src/cmk/objectapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,20 +22,22 @@
 
 
 class Edition(enum.Enum):
     FREE = "cfe"
     RAW = "cre"
     ENTERPRISE = "cee"
     CLOUD = "cce"
+    SAAS = "saas"
     MANAGED = "cme"
     PLUS = "cpe"
     CFE = FREE
     CRE = RAW
     CEE = ENTERPRISE
     CCE = CLOUD
+    CSE = SAAS
     CME = MANAGED
     CPE = PLUS
 
 
 class Version:
     def __init__(self, api):
         self._version = api._request("GET", "version")
```

### Comparing `python_cmk-23.4.0/src/cmk/objects/__init__.py` & `python_cmk-23.6.0/src/cmk/objects/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,9 +11,10 @@
 from .internal import Internal
 from .rule import Rule
 from .ruleset import Ruleset
 from .service import Service
 from .service_discovery import ServiceDiscovery
 from .service_discovery_run import ServiceDiscoveryRun
 from .service_group_config import ServiceGroupConfig
+from .site_connection import SiteConnection
 from .user_config import UserConfig
 from .user_role import UserRole
```

### Comparing `python_cmk-23.4.0/src/cmk/objects/attributes.py` & `python_cmk-23.6.0/src/cmk/objects/attributes.py`

 * *Files identical despite different names*

### Comparing `python_cmk-23.4.0/src/cmk/objects/aux_tag.py` & `python_cmk-23.6.0/src/cmk/objects/aux_tag.py`

 * *Files identical despite different names*

### Comparing `python_cmk-23.4.0/src/cmk/objects/base.py` & `python_cmk-23.6.0/src/cmk/objects/base.py`

 * *Files identical despite different names*

### Comparing `python_cmk-23.4.0/src/cmk/objects/contact_group_config.py` & `python_cmk-23.6.0/src/cmk/objects/contact_group_config.py`

 * *Files identical despite different names*

### Comparing `python_cmk-23.4.0/src/cmk/objects/folder_config.py` & `python_cmk-23.6.0/src/cmk/objects/folder_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,7 +90,11 @@
         return changed
 
     @property
     def folders(self):
         return self.api.FolderConfig.list(
             parent=self, recursive=False, show_hosts=False
         )
+
+    @property
+    def hosts(self):
+        return self.list(collection_name="hosts")
```

### Comparing `python_cmk-23.4.0/src/cmk/objects/host.py` & `python_cmk-23.6.0/src/cmk/objects/host.py`

 * *Files identical despite different names*

### Comparing `python_cmk-23.4.0/src/cmk/objects/host_config.py` & `python_cmk-23.6.0/src/cmk/objects/host_config.py`

 * *Files identical despite different names*

### Comparing `python_cmk-23.4.0/src/cmk/objects/host_group_config.py` & `python_cmk-23.6.0/src/cmk/objects/host_group_config.py`

 * *Files identical despite different names*

### Comparing `python_cmk-23.4.0/src/cmk/objects/interface/title.py` & `python_cmk-23.6.0/src/cmk/objects/interface/title.py`

 * *Files identical despite different names*

### Comparing `python_cmk-23.4.0/src/cmk/objects/rule.py` & `python_cmk-23.6.0/src/cmk/objects/rule.py`

 * *Files identical despite different names*

### Comparing `python_cmk-23.4.0/src/cmk/objects/service_discovery.py` & `python_cmk-23.6.0/src/cmk/objects/service_discovery.py`

 * *Files identical despite different names*

### Comparing `python_cmk-23.4.0/src/cmk/objects/service_discovery_run.py` & `python_cmk-23.6.0/src/cmk/objects/service_discovery_run.py`

 * *Files identical despite different names*

### Comparing `python_cmk-23.4.0/src/cmk/objects/service_group_config.py` & `python_cmk-23.6.0/src/cmk/objects/service_group_config.py`

 * *Files identical despite different names*

### Comparing `python_cmk-23.4.0/src/cmk/objects/user_config.py` & `python_cmk-23.6.0/src/cmk/objects/user_config.py`

 * *Files identical despite different names*

### Comparing `python_cmk-23.4.0/src/cmk/restapi.py` & `python_cmk-23.6.0/src/cmk/restapi.py`

 * *Files identical despite different names*

### Comparing `python_cmk-23.4.0/setup.py` & `python_cmk-23.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['furl>=2.1,<3.0', 'incremental>=22,<23', 'requests>=2.28,<3.0']
 
 setup_kwargs = {
     'name': 'python-cmk',
-    'version': '23.4.0',
+    'version': '23.6.0',
     'description': 'API for CheckMK',
     'long_description': '# python-cmk\n\n[![GitHub](https://img.shields.io/github/license/NimVek/python-cmk)](https://github.com/NimVek/python-cmk/blob/main/LICENSE)\n[![PyPI](https://img.shields.io/pypi/v/python-cmk)](https://pypi.org/project/python-cmk)\n[![GitHub last commit](https://img.shields.io/github/last-commit/NimVek/python-cmk)](https://github.com/NimVek/python-cmk/commits/main)\n[![Build Status](https://img.shields.io/github/actions/workflow/status/NimVek/python-cmk/ci.yml)](https://github.com/NimVek/python-cmk/actions/workflows/ci.yml)\n[![Coverage Status](https://img.shields.io/codecov/c/github/NimVek/python-cmk)](https://codecov.io/gh/NimVek/python-cmk/)\n[![Documentation](https://img.shields.io/badge/docs-passing-brightgreen)](https://nimvek.github.io/python-cmk/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)\n\nAPI for CheckMK\n',
     'author': 'NimVek',
     'author_email': 'NimVek@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/NimVek/python-cmk',
```

### Comparing `python_cmk-23.4.0/PKG-INFO` & `python_cmk-23.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-cmk
-Version: 23.4.0
+Version: 23.6.0
 Summary: API for CheckMK
 Home-page: https://github.com/NimVek/python-cmk
 License: GPL-3.0-or-later
 Author: NimVek
 Author-email: NimVek@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

