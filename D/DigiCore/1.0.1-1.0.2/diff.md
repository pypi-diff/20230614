# Comparing `tmp/DigiCore-1.0.1.tar.gz` & `tmp/DigiCore-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\DigiCore-1.0.1.tar", last modified: Wed Jun 14 03:49:49 2023, max compression
+gzip compressed data, was "dist\DigiCore-1.0.2.tar", last modified: Wed Jun 14 06:15:31 2023, max compression
```

## Comparing `DigiCore-1.0.1.tar` & `DigiCore-1.0.2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 03:49:49.158271 DigiCore-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-14 03:49:49.133606 DigiCore-1.0.1/DigiCore.egg-info/
--rw-rw-rw-   0        0        0     3976 2023-06-14 03:49:49.000000 DigiCore-1.0.1/DigiCore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      622 2023-06-14 03:49:49.000000 DigiCore-1.0.1/DigiCore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 03:49:49.000000 DigiCore-1.0.1/DigiCore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 03:49:49.000000 DigiCore-1.0.1/DigiCore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-06-14 03:49:49.000000 DigiCore-1.0.1/DigiCore.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1104 2023-05-20 03:41:32.000000 DigiCore-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     3976 2023-06-14 03:49:49.157271 DigiCore-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2670 2023-05-20 03:41:32.000000 DigiCore-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 03:49:49.141757 DigiCore-1.0.1/digiCore/
--rw-rw-rw-   0        0        0     1382 2023-05-20 06:50:26.000000 DigiCore-1.0.1/digiCore/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:49:49.144759 DigiCore-1.0.1/digiCore/dingding/
--rw-rw-rw-   0        0        0      130 2023-05-20 03:41:32.000000 DigiCore-1.0.1/digiCore/dingding/__init__.py
--rw-rw-rw-   0        0        0     1015 2023-05-23 01:25:52.000000 DigiCore-1.0.1/digiCore/dingding/dingding_model.py
--rw-rw-rw-   0        0        0     3747 2023-06-07 01:34:09.000000 DigiCore-1.0.1/digiCore/dingding/send_to_group.py
--rw-rw-rw-   0        0        0     4901 2023-06-14 02:12:46.000000 DigiCore-1.0.1/digiCore/dsd_kafka.py
--rw-rw-rw-   0        0        0     3673 2023-06-14 02:12:46.000000 DigiCore-1.0.1/digiCore/dsd_mongodb.py
--rw-rw-rw-   0        0        0     6853 2023-06-14 02:12:46.000000 DigiCore-1.0.1/digiCore/dsd_mysql.py
--rw-rw-rw-   0        0        0     3919 2023-05-20 07:33:42.000000 DigiCore-1.0.1/digiCore/dsd_redis.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:49:49.147758 DigiCore-1.0.1/digiCore/kingdee/
--rw-rw-rw-   0        0        0      571 2023-06-14 02:12:46.000000 DigiCore-1.0.1/digiCore/kingdee/__init__.py
--rw-rw-rw-   0        0        0     9953 2023-06-14 02:12:46.000000 DigiCore-1.0.1/digiCore/kingdee/kingdee_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:49:49.151271 DigiCore-1.0.1/digiCore/lingxing/
--rw-rw-rw-   0        0        0      130 2023-05-20 03:41:32.000000 DigiCore-1.0.1/digiCore/lingxing/__init__.py
--rw-rw-rw-   0        0        0     4167 2023-06-14 02:12:46.000000 DigiCore-1.0.1/digiCore/lingxing/api_scheduler.py
--rw-rw-rw-   0        0        0      786 2023-05-20 03:41:55.000000 DigiCore-1.0.1/digiCore/status_code.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:49:49.152272 DigiCore-1.0.1/digiCore/test/
--rw-rw-rw-   0        0        0      130 2023-05-20 03:41:32.000000 DigiCore-1.0.1/digiCore/test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:49:49.156271 DigiCore-1.0.1/digiCore/utils/
--rw-rw-rw-   0        0        0       25 2023-06-07 01:34:09.000000 DigiCore-1.0.1/digiCore/utils/__init__.py
--rw-rw-rw-   0        0        0     5351 2023-06-14 02:12:46.000000 DigiCore-1.0.1/digiCore/utils/utils.py
--rw-rw-rw-   0        0        0       42 2023-06-14 03:49:49.158271 DigiCore-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2202 2023-06-14 03:31:19.000000 DigiCore-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:15:31.241558 DigiCore-1.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-14 06:15:31.212948 DigiCore-1.0.2/DigiCore.egg-info/
+-rw-rw-rw-   0        0        0     4014 2023-06-14 06:15:31.000000 DigiCore-1.0.2/DigiCore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      653 2023-06-14 06:15:31.000000 DigiCore-1.0.2/DigiCore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 06:15:31.000000 DigiCore-1.0.2/DigiCore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      720 2023-06-14 06:15:31.000000 DigiCore-1.0.2/DigiCore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-14 06:15:31.000000 DigiCore-1.0.2/DigiCore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-06-14 06:15:31.000000 DigiCore-1.0.2/DigiCore.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1104 2023-05-20 03:41:32.000000 DigiCore-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4014 2023-06-14 06:15:31.240443 DigiCore-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2670 2023-05-20 03:41:32.000000 DigiCore-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 06:15:31.222850 DigiCore-1.0.2/digiCore/
+-rw-rw-rw-   0        0        0     1382 2023-05-20 06:50:26.000000 DigiCore-1.0.2/digiCore/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:15:31.227849 DigiCore-1.0.2/digiCore/dingding/
+-rw-rw-rw-   0        0        0      130 2023-05-20 03:41:32.000000 DigiCore-1.0.2/digiCore/dingding/__init__.py
+-rw-rw-rw-   0        0        0     1015 2023-05-23 01:25:52.000000 DigiCore-1.0.2/digiCore/dingding/dingding_model.py
+-rw-rw-rw-   0        0        0     3747 2023-06-07 01:34:09.000000 DigiCore-1.0.2/digiCore/dingding/send_to_group.py
+-rw-rw-rw-   0        0        0     4901 2023-06-14 02:12:46.000000 DigiCore-1.0.2/digiCore/dsd_kafka.py
+-rw-rw-rw-   0        0        0     3673 2023-06-14 02:12:46.000000 DigiCore-1.0.2/digiCore/dsd_mongodb.py
+-rw-rw-rw-   0        0        0     6853 2023-06-14 02:12:46.000000 DigiCore-1.0.2/digiCore/dsd_mysql.py
+-rw-rw-rw-   0        0        0     3919 2023-05-20 07:33:42.000000 DigiCore-1.0.2/digiCore/dsd_redis.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:15:31.230849 DigiCore-1.0.2/digiCore/kingdee/
+-rw-rw-rw-   0        0        0      571 2023-06-14 02:12:46.000000 DigiCore-1.0.2/digiCore/kingdee/__init__.py
+-rw-rw-rw-   0        0        0     9953 2023-06-14 02:12:46.000000 DigiCore-1.0.2/digiCore/kingdee/kingdee_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:15:31.233852 DigiCore-1.0.2/digiCore/lingxing/
+-rw-rw-rw-   0        0        0      130 2023-05-20 03:41:32.000000 DigiCore-1.0.2/digiCore/lingxing/__init__.py
+-rw-rw-rw-   0        0        0     4167 2023-06-14 02:12:46.000000 DigiCore-1.0.2/digiCore/lingxing/api_scheduler.py
+-rw-rw-rw-   0        0        0      786 2023-05-20 03:41:55.000000 DigiCore-1.0.2/digiCore/status_code.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:15:31.235642 DigiCore-1.0.2/digiCore/test/
+-rw-rw-rw-   0        0        0      130 2023-05-20 03:41:32.000000 DigiCore-1.0.2/digiCore/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:15:31.238647 DigiCore-1.0.2/digiCore/utils/
+-rw-rw-rw-   0        0        0       25 2023-06-07 01:34:09.000000 DigiCore-1.0.2/digiCore/utils/__init__.py
+-rw-rw-rw-   0        0        0     5351 2023-06-14 02:12:46.000000 DigiCore-1.0.2/digiCore/utils/utils.py
+-rw-rw-rw-   0        0        0       42 2023-06-14 06:15:31.241558 DigiCore-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2506 2023-06-14 06:15:28.000000 DigiCore-1.0.2/setup.py
```

### Comparing `DigiCore-1.0.1/DigiCore.egg-info/PKG-INFO` & `DigiCore-1.0.2/DigiCore.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: DigiCore
-Version: 1.0.1
+Version: 1.0.2
 Summary: DigiCore是一个基于Python的数字化支持部第三方库，旨在为数据处理和开发提供完备的工具集和服务。
 Home-page: UNKNOWN
 Author: yarm
 Author-email: yangyang@doocn.com
 License: MIT License
-Keywords: faker fixtures data test mock generator
+Keywords: digicore是服务于道诚集团数字化支持部的自建第三方库项目
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `DigiCore-1.0.1/DigiCore.egg-info/SOURCES.txt` & `DigiCore-1.0.2/DigiCore.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.py
 DigiCore.egg-info/PKG-INFO
 DigiCore.egg-info/SOURCES.txt
 DigiCore.egg-info/dependency_links.txt
+DigiCore.egg-info/requires.txt
 DigiCore.egg-info/top_level.txt
 DigiCore.egg-info/zip-safe
 digiCore/__init__.py
 digiCore/dsd_kafka.py
 digiCore/dsd_mongodb.py
 digiCore/dsd_mysql.py
 digiCore/dsd_redis.py
```

### Comparing `DigiCore-1.0.1/LICENSE` & `DigiCore-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.1/PKG-INFO` & `DigiCore-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: DigiCore
-Version: 1.0.1
+Version: 1.0.2
 Summary: DigiCore是一个基于Python的数字化支持部第三方库，旨在为数据处理和开发提供完备的工具集和服务。
 Home-page: UNKNOWN
 Author: yarm
 Author-email: yangyang@doocn.com
 License: MIT License
-Keywords: faker fixtures data test mock generator
+Keywords: digicore是服务于道诚集团数字化支持部的自建第三方库项目
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `DigiCore-1.0.1/README.md` & `DigiCore-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.1/digiCore/__init__.py` & `DigiCore-1.0.2/digiCore/__init__.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.1/digiCore/dingding/dingding_model.py` & `DigiCore-1.0.2/digiCore/dingding/dingding_model.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.1/digiCore/dingding/send_to_group.py` & `DigiCore-1.0.2/digiCore/dingding/send_to_group.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.1/digiCore/dsd_kafka.py` & `DigiCore-1.0.2/digiCore/dsd_kafka.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.1/digiCore/dsd_mongodb.py` & `DigiCore-1.0.2/digiCore/dsd_mongodb.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.1/digiCore/dsd_mysql.py` & `DigiCore-1.0.2/digiCore/dsd_mysql.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.1/digiCore/dsd_redis.py` & `DigiCore-1.0.2/digiCore/dsd_redis.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.1/digiCore/kingdee/__init__.py` & `DigiCore-1.0.2/digiCore/kingdee/__init__.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.1/digiCore/kingdee/kingdee_tools.py` & `DigiCore-1.0.2/digiCore/kingdee/kingdee_tools.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.1/digiCore/lingxing/api_scheduler.py` & `DigiCore-1.0.2/digiCore/lingxing/api_scheduler.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.1/digiCore/status_code.py` & `DigiCore-1.0.2/digiCore/status_code.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.1/digiCore/utils/utils.py` & `DigiCore-1.0.2/digiCore/utils/utils.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.1/setup.py` & `DigiCore-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # @Author : 杨洋
 # @Email ： yangyang@doocn.com
 # @File : DigiCore
 # @Desc :
 
 from pathlib import Path
 
+import chardet
 from setuptools import find_packages, setup
 
 here = Path(__file__).resolve().parent
 README = (here / "README.md").read_text(encoding="utf-8")
 
 excluded_packages = ["tests", "tests.*"]
 
@@ -24,17 +25,24 @@
     zip_safe = (
         hasattr(zipimport.zipimporter, "iter_modules")
         or zipimport.zipimporter in pkgutil.iter_importer_modules.registry.keys()
     )
 except AttributeError:
     zip_safe = False
 
+with open('requirements.txt', 'rb') as f:
+    data = chardet.detect(f.read())
+    encoding = data['encoding']
+
+with open('requirements.txt',encoding=encoding) as f:
+    requirements = f.read().splitlines()
+
 setup(
     name="DigiCore",
-    version="1.0.1",
+    version="1.0.2",
     description="DigiCore是一个基于Python的数字化支持部第三方库，旨在为数据处理和开发提供完备的工具集和服务。",
     long_description=README,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
@@ -48,16 +56,17 @@
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: Testing",
         "Topic :: Utilities",
         "License :: OSI Approved :: MIT License",
     ],
-    keywords="faker fixtures data test mock generator",
+    keywords="digicore是服务于道诚集团数字化支持部的自建第三方库项目",
     author="yarm",
     author_email="yangyang@doocn.com",
     license="MIT License",
     packages=find_packages(exclude=excluded_packages),
+    install_requires=requirements,
     platforms=["any"],
     zip_safe=zip_safe,
     python_requires=">=3.7",
 )
```

