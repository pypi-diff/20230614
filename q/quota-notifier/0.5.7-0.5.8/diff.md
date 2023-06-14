# Comparing `tmp/quota_notifier-0.5.7.tar.gz` & `tmp/quota_notifier-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quota_notifier-0.5.7.tar", max compression
+gzip compressed data, was "quota_notifier-0.5.8.tar", max compression
```

## Comparing `quota_notifier-0.5.7.tar` & `quota_notifier-0.5.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    34906 2023-05-08 14:17:22.913718 quota_notifier-0.5.7/LICENSE.md
--rw-r--r--   0        0        0      653 2023-05-08 14:17:22.913718 quota_notifier-0.5.7/README.md
--rw-r--r--   0        0        0     1415 2023-05-08 14:17:45.889735 quota_notifier-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     1506 2023-05-08 14:17:22.917719 quota_notifier-0.5.7/quota_notifier/__init__.py
--rw-r--r--   0        0        0      202 2023-05-08 14:17:22.917719 quota_notifier-0.5.7/quota_notifier/__main__.py
--rw-r--r--   0        0        0     6662 2023-05-08 14:17:22.917719 quota_notifier-0.5.7/quota_notifier/cli.py
--rw-r--r--   0        0        0      298 2023-05-08 14:17:22.917719 quota_notifier-0.5.7/quota_notifier/data/template.html
--rw-r--r--   0        0        0    10990 2023-05-08 14:17:22.917719 quota_notifier-0.5.7/quota_notifier/disk_utils.py
--rw-r--r--   0        0        0    11137 2023-05-08 14:17:22.917719 quota_notifier-0.5.7/quota_notifier/notify.py
--rw-r--r--   0        0        0     3220 2023-05-08 14:17:22.917719 quota_notifier-0.5.7/quota_notifier/orm.py
--rw-r--r--   0        0        0     9157 2023-05-08 14:17:22.917719 quota_notifier-0.5.7/quota_notifier/settings.py
--rw-r--r--   0        0        0     2874 2023-05-08 14:17:22.917719 quota_notifier-0.5.7/quota_notifier/shell.py
--rw-r--r--   0        0        0     1821 1970-01-01 00:00:00.000000 quota_notifier-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0    34906 2023-06-13 13:10:52.748133 quota_notifier-0.5.8/LICENSE.md
+-rw-r--r--   0        0        0      653 2023-06-13 13:10:52.748133 quota_notifier-0.5.8/README.md
+-rw-r--r--   0        0        0     1415 2023-06-13 13:11:12.004049 quota_notifier-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0     1506 2023-06-13 13:10:52.748133 quota_notifier-0.5.8/quota_notifier/__init__.py
+-rw-r--r--   0        0        0      202 2023-06-13 13:10:52.748133 quota_notifier-0.5.8/quota_notifier/__main__.py
+-rw-r--r--   0        0        0     6662 2023-06-13 13:10:52.748133 quota_notifier-0.5.8/quota_notifier/cli.py
+-rw-r--r--   0        0        0      298 2023-06-13 13:10:52.748133 quota_notifier-0.5.8/quota_notifier/data/template.html
+-rw-r--r--   0        0        0    10990 2023-06-13 13:10:52.748133 quota_notifier-0.5.8/quota_notifier/disk_utils.py
+-rw-r--r--   0        0        0    11137 2023-06-13 13:10:52.748133 quota_notifier-0.5.8/quota_notifier/notify.py
+-rw-r--r--   0        0        0     3220 2023-06-13 13:10:52.748133 quota_notifier-0.5.8/quota_notifier/orm.py
+-rw-r--r--   0        0        0     9157 2023-06-13 13:10:52.748133 quota_notifier-0.5.8/quota_notifier/settings.py
+-rw-r--r--   0        0        0     2874 2023-06-13 13:10:52.748133 quota_notifier-0.5.8/quota_notifier/shell.py
+-rw-r--r--   0        0        0     1773 1970-01-01 00:00:00.000000 quota_notifier-0.5.8/PKG-INFO
```

### Comparing `quota_notifier-0.5.7/LICENSE.md` & `quota_notifier-0.5.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.7/README.md` & `quota_notifier-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.7/pyproject.toml` & `quota_notifier-0.5.8/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "quota-notifier"
-version = "0.5.7"  # Version is set dynamically by the CI tool on publication
+version = "0.5.8"  # Version is set dynamically by the CI tool on publication
 authors = ["Pitt Center for Research Computing", ]
 readme = "README.md"
 description = "Automatic email notification tool for disk quota usage."
 homepage = "https://github.com/pitt-crc/quota_notifier"
 repository = "https://github.com/pitt-crc/quota_notifier"
 documentation = "https://crc-pages.pitt.edu/quota_notifier/"
 keywords = ["disk", "usage", "quota", "notify", "email", ]
@@ -24,17 +24,17 @@
 ]
 
 [tool.poetry.scripts]
 notifier = "quota_notifier.cli:Application.execute"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-pydantic = "1.10.7"
-sqlalchemy = "2.0.12"
-prometheus_client = "0.16.0"
+pydantic = "1.10.9"
+sqlalchemy = "2.0.15"
+prometheus_client = "0.17.0"
 
 [tool.poetry.group.tests]
 optional = true
 
 [tool.poetry.group.tests.dependencies]
 coverage = "*"
 
@@ -42,9 +42,9 @@
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "6.2.1"
 sphinx-argparse = "0.4.0"
 sphinx-copybutton = "0.5.2"
 sphinx-pydantic = "0.1.1"
-sphinx-rtd-theme = "1.2.0"
+sphinx-rtd-theme = "1.2.1"
 sphinx-jsonschema = "1.15"
```

### Comparing `quota_notifier-0.5.7/quota_notifier/__init__.py` & `quota_notifier-0.5.8/quota_notifier/__init__.py`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.7/quota_notifier/cli.py` & `quota_notifier-0.5.8/quota_notifier/cli.py`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.7/quota_notifier/disk_utils.py` & `quota_notifier-0.5.8/quota_notifier/disk_utils.py`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.7/quota_notifier/notify.py` & `quota_notifier-0.5.8/quota_notifier/notify.py`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.7/quota_notifier/orm.py` & `quota_notifier-0.5.8/quota_notifier/orm.py`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.7/quota_notifier/settings.py` & `quota_notifier-0.5.8/quota_notifier/settings.py`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.7/quota_notifier/shell.py` & `quota_notifier-0.5.8/quota_notifier/shell.py`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.7/PKG-INFO` & `quota_notifier-0.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: quota-notifier
-Version: 0.5.7
+Version: 0.5.8
 Summary: Automatic email notification tool for disk quota usage.
 Home-page: https://github.com/pitt-crc/quota_notifier
 Keywords: disk,usage,quota,notify,email
 Author: Pitt Center for Research Computing
 Requires-Python: >=3.8
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: System :: Monitoring
 Classifier: Typing :: Typed
-Requires-Dist: prometheus_client (==0.16.0)
-Requires-Dist: pydantic (==1.10.7)
-Requires-Dist: sqlalchemy (==2.0.12)
+Requires-Dist: prometheus_client (==0.17.0)
+Requires-Dist: pydantic (==1.10.9)
+Requires-Dist: sqlalchemy (==2.0.15)
 Project-URL: Documentation, https://crc-pages.pitt.edu/quota_notifier/
 Project-URL: Repository, https://github.com/pitt-crc/quota_notifier
 Description-Content-Type: text/markdown
 
 # Storage Quota Notifier
 
 [![](https://app.codacy.com/project/badge/Grade/583c607400c2429ebbc1554d777d26b4)](https://app.codacy.com/gh/pitt-crc/quota_notifier/dashboard)
```

