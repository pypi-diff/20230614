# Comparing `tmp/mathtranslate-2.4.1.tar.gz` & `tmp/mathtranslate-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathtranslate-2.4.1.tar", last modified: Mon Jun 12 18:36:23 2023, max compression
+gzip compressed data, was "mathtranslate-2.4.2.tar", last modified: Wed Jun 14 20:30:52 2023, max compression
```

## Comparing `mathtranslate-2.4.1.tar` & `mathtranslate-2.4.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:36:23.496516 mathtranslate-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-06-12 18:36:23.496516 mathtranslate-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:36:23.492516 mathtranslate-2.4.1/mathtranslate/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/process_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/process_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/process_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/tencent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:36:23.492516 mathtranslate-2.4.1/mathtranslate/tencentcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/tencentcloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:36:23.496516 mathtranslate-2.4.1/mathtranslate/tencentcloud/common/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/tencentcloud/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/tencentcloud/common/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/tencentcloud/common/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/tencentcloud/common/common_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/tencentcloud/common/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:36:23.496516 mathtranslate-2.4.1/mathtranslate/tencentcloud/common/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/tencentcloud/common/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:36:23.496516 mathtranslate-2.4.1/mathtranslate/tencentcloud/common/http/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/tencentcloud/common/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/tencentcloud/common/http/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:36:23.496516 mathtranslate-2.4.1/mathtranslate/tencentcloud/common/profile/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/tencentcloud/common/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/tencentcloud/common/profile/client_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/tencentcloud/common/profile/http_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/tencentcloud/common/sign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:36:23.496516 mathtranslate-2.4.1/mathtranslate/tencentcloud/tmt/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/tencentcloud/tmt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:36:23.496516 mathtranslate-2.4.1/mathtranslate/tencentcloud/tmt/v20180321/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/tencentcloud/tmt/v20180321/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    33836 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/tencentcloud/tmt/v20180321/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/translate_arxiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/translate_tex.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/upload_overleaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/mathtranslate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:36:23.492516 mathtranslate-2.4.1/mathtranslate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-06-12 18:36:23.000000 mathtranslate-2.4.1/mathtranslate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-12 18:36:23.000000 mathtranslate-2.4.1/mathtranslate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 18:36:23.000000 mathtranslate-2.4.1/mathtranslate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-12 18:36:23.000000 mathtranslate-2.4.1/mathtranslate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-12 18:36:23.000000 mathtranslate-2.4.1/mathtranslate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 18:36:23.000000 mathtranslate-2.4.1/mathtranslate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 18:36:23.496516 mathtranslate-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-12 18:36:08.000000 mathtranslate-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:30:52.730088 mathtranslate-2.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-06-14 20:30:52.726087 mathtranslate-2.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:30:52.726087 mathtranslate-2.4.2/mathtranslate/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/process_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17250 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/process_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:30:52.726087 mathtranslate-2.4.2/mathtranslate/tencentcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:30:52.726087 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/common_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:30:52.726087 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:30:52.726087 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/http/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:30:52.726087 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/profile/client_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/profile/http_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/sign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:30:52.726087 mathtranslate-2.4.2/mathtranslate/tencentcloud/tmt/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/tmt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:30:52.726087 mathtranslate-2.4.2/mathtranslate/tencentcloud/tmt/v20180321/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/tmt/v20180321/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33836 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/tmt/v20180321/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/translate_arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/translate_tex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/upload_overleaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:30:52.726087 mathtranslate-2.4.2/mathtranslate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-06-14 20:30:52.000000 mathtranslate-2.4.2/mathtranslate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-14 20:30:52.000000 mathtranslate-2.4.2/mathtranslate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 20:30:52.000000 mathtranslate-2.4.2/mathtranslate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-14 20:30:52.000000 mathtranslate-2.4.2/mathtranslate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-14 20:30:52.000000 mathtranslate-2.4.2/mathtranslate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-14 20:30:52.000000 mathtranslate-2.4.2/mathtranslate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 20:30:52.730088 mathtranslate-2.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/setup.py
```

### Comparing `mathtranslate-2.4.1/LICENSE` & `mathtranslate-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/PKG-INFO` & `mathtranslate-2.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathtranslate
-Version: 2.4.1
+Version: 2.4.2
 Summary: Translate math-heavy papers
 Home-page: https://github.com/SUSYUSTC/MathTranslate
 Author: MathTranslate developers
 Author-email: susyustc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mathtranslate Version: 2.4.1 Summary: Translate
+Metadata-Version: 2.1 Name: mathtranslate Version: 2.4.2 Summary: Translate
 math-heavy papers Home-page: https://github.com/SUSYUSTC/MathTranslate Author:
 MathTranslate developers Author-email: susyustc@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE #
 MathTranslate
      [https://img.shields.io/pypi/v/mathtranslate.svg?logo=pypi]  [https://
        img.shields.io/badge/license-Apache%202.0-yellow.svg?logo=apache]
```

### Comparing `mathtranslate-2.4.1/README.md` & `mathtranslate-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/cache.py` & `mathtranslate-2.4.2/mathtranslate/cache.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/config.py` & `mathtranslate-2.4.2/mathtranslate/config.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/encoding.py` & `mathtranslate-2.4.2/mathtranslate/encoding.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/process_file.py` & `mathtranslate-2.4.2/mathtranslate/process_file.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/process_latex.py` & `mathtranslate-2.4.2/mathtranslate/process_latex.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     '.': 'DT',
     '*': 'ST',
     '@': 'AT',
 }
 special_character_backward = {special_character_forward[key]: key for key in special_character_forward}
 assert len(set(special_character_forward.values())) == len(special_character_forward)
 
-environment_list = ['abstract', 'acknowledgments', 'itemize', 'enumerate', 'description', 'list', 'proof', 'quote']
+environment_list = ['abstract', 'acknowledgments', 'itemize', 'enumerate', 'description', 'list', 'proof', 'quote', 'spacing']
 command_list = ['section', 'subsection', 'subsubsection', 'caption', 'subcaption', 'footnote', 'paragraph']
 mularg_command_list = [('textcolor', 2, (1, ))]
 format_list = ['textbf', 'textit', 'emph']
 replace_newcommand_list = ['equation', 'array', 'displaymath', 'align', 'multiple', 'gather', 'theorem', 'textcolor'] + environment_list + command_list
 
 patterns_mularg_command = [get_pattern_command_full(name, n) for name, n, index in mularg_command_list]
```

### Comparing `mathtranslate-2.4.1/mathtranslate/process_text.py` & `mathtranslate-2.4.2/mathtranslate/process_text.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/tencent.py` & `mathtranslate-2.4.2/mathtranslate/tencent.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/tencentcloud/__init__.py` & `mathtranslate-2.4.2/mathtranslate/tencentcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/tencentcloud/common/__init__.py` & `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/tencentcloud/common/abstract_client.py` & `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/tencentcloud/common/abstract_model.py` & `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/tencentcloud/common/common_client.py` & `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/common_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/tencentcloud/common/credential.py` & `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/credential.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/tencentcloud/common/exception/__init__.py` & `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py` & `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/tencentcloud/common/http/__init__.py` & `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/http/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/tencentcloud/common/http/request.py` & `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/http/request.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/tencentcloud/common/profile/__init__.py` & `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/tencentcloud/common/profile/client_profile.py` & `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/tencentcloud/common/profile/http_profile.py` & `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/tencentcloud/common/sign.py` & `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/sign.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/tencentcloud/tmt/__init__.py` & `mathtranslate-2.4.2/mathtranslate/tencentcloud/tmt/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/tencentcloud/tmt/v20180321/__init__.py` & `mathtranslate-2.4.2/mathtranslate/tencentcloud/tmt/v20180321/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py` & `mathtranslate-2.4.2/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/tencentcloud/tmt/v20180321/models.py` & `mathtranslate-2.4.2/mathtranslate/tencentcloud/tmt/v20180321/models.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py` & `mathtranslate-2.4.2/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/translate.py` & `mathtranslate-2.4.2/mathtranslate/translate.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/translate_arxiv.py` & `mathtranslate-2.4.2/mathtranslate/translate_arxiv.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/translate_tex.py` & `mathtranslate-2.4.2/mathtranslate/translate_tex.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/upload_overleaf.py` & `mathtranslate-2.4.2/mathtranslate/upload_overleaf.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate/utils.py` & `mathtranslate-2.4.2/mathtranslate/utils.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/mathtranslate.egg-info/PKG-INFO` & `mathtranslate-2.4.2/mathtranslate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathtranslate
-Version: 2.4.1
+Version: 2.4.2
 Summary: Translate math-heavy papers
 Home-page: https://github.com/SUSYUSTC/MathTranslate
 Author: MathTranslate developers
 Author-email: susyustc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mathtranslate Version: 2.4.1 Summary: Translate
+Metadata-Version: 2.1 Name: mathtranslate Version: 2.4.2 Summary: Translate
 math-heavy papers Home-page: https://github.com/SUSYUSTC/MathTranslate Author:
 MathTranslate developers Author-email: susyustc@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE #
 MathTranslate
      [https://img.shields.io/pypi/v/mathtranslate.svg?logo=pypi]  [https://
        img.shields.io/badge/license-Apache%202.0-yellow.svg?logo=apache]
```

### Comparing `mathtranslate-2.4.1/mathtranslate.egg-info/SOURCES.txt` & `mathtranslate-2.4.2/mathtranslate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.1/setup.py` & `mathtranslate-2.4.2/setup.py`

 * *Files identical despite different names*

