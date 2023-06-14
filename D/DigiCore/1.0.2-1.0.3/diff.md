# Comparing `tmp/DigiCore-1.0.2.tar.gz` & `tmp/DigiCore-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\DigiCore-1.0.2.tar", last modified: Wed Jun 14 06:15:31 2023, max compression
+gzip compressed data, was "dist\DigiCore-1.0.3.tar", last modified: Wed Jun 14 06:39:15 2023, max compression
```

## Comparing `DigiCore-1.0.2.tar` & `DigiCore-1.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 06:15:31.241558 DigiCore-1.0.2/
-drwxrwxrwx   0        0        0        0 2023-06-14 06:15:31.212948 DigiCore-1.0.2/DigiCore.egg-info/
--rw-rw-rw-   0        0        0     4014 2023-06-14 06:15:31.000000 DigiCore-1.0.2/DigiCore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      653 2023-06-14 06:15:31.000000 DigiCore-1.0.2/DigiCore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 06:15:31.000000 DigiCore-1.0.2/DigiCore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      720 2023-06-14 06:15:31.000000 DigiCore-1.0.2/DigiCore.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 06:15:31.000000 DigiCore-1.0.2/DigiCore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-06-14 06:15:31.000000 DigiCore-1.0.2/DigiCore.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1104 2023-05-20 03:41:32.000000 DigiCore-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     4014 2023-06-14 06:15:31.240443 DigiCore-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2670 2023-05-20 03:41:32.000000 DigiCore-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 06:15:31.222850 DigiCore-1.0.2/digiCore/
--rw-rw-rw-   0        0        0     1382 2023-05-20 06:50:26.000000 DigiCore-1.0.2/digiCore/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:15:31.227849 DigiCore-1.0.2/digiCore/dingding/
--rw-rw-rw-   0        0        0      130 2023-05-20 03:41:32.000000 DigiCore-1.0.2/digiCore/dingding/__init__.py
--rw-rw-rw-   0        0        0     1015 2023-05-23 01:25:52.000000 DigiCore-1.0.2/digiCore/dingding/dingding_model.py
--rw-rw-rw-   0        0        0     3747 2023-06-07 01:34:09.000000 DigiCore-1.0.2/digiCore/dingding/send_to_group.py
--rw-rw-rw-   0        0        0     4901 2023-06-14 02:12:46.000000 DigiCore-1.0.2/digiCore/dsd_kafka.py
--rw-rw-rw-   0        0        0     3673 2023-06-14 02:12:46.000000 DigiCore-1.0.2/digiCore/dsd_mongodb.py
--rw-rw-rw-   0        0        0     6853 2023-06-14 02:12:46.000000 DigiCore-1.0.2/digiCore/dsd_mysql.py
--rw-rw-rw-   0        0        0     3919 2023-05-20 07:33:42.000000 DigiCore-1.0.2/digiCore/dsd_redis.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:15:31.230849 DigiCore-1.0.2/digiCore/kingdee/
--rw-rw-rw-   0        0        0      571 2023-06-14 02:12:46.000000 DigiCore-1.0.2/digiCore/kingdee/__init__.py
--rw-rw-rw-   0        0        0     9953 2023-06-14 02:12:46.000000 DigiCore-1.0.2/digiCore/kingdee/kingdee_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:15:31.233852 DigiCore-1.0.2/digiCore/lingxing/
--rw-rw-rw-   0        0        0      130 2023-05-20 03:41:32.000000 DigiCore-1.0.2/digiCore/lingxing/__init__.py
--rw-rw-rw-   0        0        0     4167 2023-06-14 02:12:46.000000 DigiCore-1.0.2/digiCore/lingxing/api_scheduler.py
--rw-rw-rw-   0        0        0      786 2023-05-20 03:41:55.000000 DigiCore-1.0.2/digiCore/status_code.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:15:31.235642 DigiCore-1.0.2/digiCore/test/
--rw-rw-rw-   0        0        0      130 2023-05-20 03:41:32.000000 DigiCore-1.0.2/digiCore/test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:15:31.238647 DigiCore-1.0.2/digiCore/utils/
--rw-rw-rw-   0        0        0       25 2023-06-07 01:34:09.000000 DigiCore-1.0.2/digiCore/utils/__init__.py
--rw-rw-rw-   0        0        0     5351 2023-06-14 02:12:46.000000 DigiCore-1.0.2/digiCore/utils/utils.py
--rw-rw-rw-   0        0        0       42 2023-06-14 06:15:31.241558 DigiCore-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2506 2023-06-14 06:15:28.000000 DigiCore-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:39:15.140298 DigiCore-1.0.3/
+drwxrwxrwx   0        0        0        0 2023-06-14 06:39:15.124551 DigiCore-1.0.3/DigiCore.egg-info/
+-rw-rw-rw-   0        0        0     4014 2023-06-14 06:39:15.000000 DigiCore-1.0.3/DigiCore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      653 2023-06-14 06:39:15.000000 DigiCore-1.0.3/DigiCore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 06:39:15.000000 DigiCore-1.0.3/DigiCore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      663 2023-06-14 06:39:15.000000 DigiCore-1.0.3/DigiCore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-14 06:39:15.000000 DigiCore-1.0.3/DigiCore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-06-14 06:39:15.000000 DigiCore-1.0.3/DigiCore.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1104 2023-05-20 03:41:32.000000 DigiCore-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4014 2023-06-14 06:39:15.140298 DigiCore-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2670 2023-05-20 03:41:32.000000 DigiCore-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 06:39:15.126779 DigiCore-1.0.3/digiCore/
+-rw-rw-rw-   0        0        0     1382 2023-05-20 06:50:26.000000 DigiCore-1.0.3/digiCore/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:39:15.126779 DigiCore-1.0.3/digiCore/dingding/
+-rw-rw-rw-   0        0        0      130 2023-05-20 03:41:32.000000 DigiCore-1.0.3/digiCore/dingding/__init__.py
+-rw-rw-rw-   0        0        0     1015 2023-05-23 01:25:52.000000 DigiCore-1.0.3/digiCore/dingding/dingding_model.py
+-rw-rw-rw-   0        0        0     3747 2023-06-07 01:34:09.000000 DigiCore-1.0.3/digiCore/dingding/send_to_group.py
+-rw-rw-rw-   0        0        0     4901 2023-06-14 02:12:46.000000 DigiCore-1.0.3/digiCore/dsd_kafka.py
+-rw-rw-rw-   0        0        0     3673 2023-06-14 02:12:46.000000 DigiCore-1.0.3/digiCore/dsd_mongodb.py
+-rw-rw-rw-   0        0        0     6853 2023-06-14 02:12:46.000000 DigiCore-1.0.3/digiCore/dsd_mysql.py
+-rw-rw-rw-   0        0        0     3919 2023-05-20 07:33:42.000000 DigiCore-1.0.3/digiCore/dsd_redis.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:39:15.140298 DigiCore-1.0.3/digiCore/kingdee/
+-rw-rw-rw-   0        0        0      553 2023-06-14 06:38:53.000000 DigiCore-1.0.3/digiCore/kingdee/__init__.py
+-rw-rw-rw-   0        0        0     9953 2023-06-14 02:12:46.000000 DigiCore-1.0.3/digiCore/kingdee/kingdee_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:39:15.140298 DigiCore-1.0.3/digiCore/lingxing/
+-rw-rw-rw-   0        0        0      130 2023-05-20 03:41:32.000000 DigiCore-1.0.3/digiCore/lingxing/__init__.py
+-rw-rw-rw-   0        0        0     4167 2023-06-14 02:12:46.000000 DigiCore-1.0.3/digiCore/lingxing/api_scheduler.py
+-rw-rw-rw-   0        0        0      786 2023-05-20 03:41:55.000000 DigiCore-1.0.3/digiCore/status_code.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:39:15.140298 DigiCore-1.0.3/digiCore/test/
+-rw-rw-rw-   0        0        0      130 2023-05-20 03:41:32.000000 DigiCore-1.0.3/digiCore/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:39:15.140298 DigiCore-1.0.3/digiCore/utils/
+-rw-rw-rw-   0        0        0       25 2023-06-07 01:34:09.000000 DigiCore-1.0.3/digiCore/utils/__init__.py
+-rw-rw-rw-   0        0        0     5351 2023-06-14 02:12:46.000000 DigiCore-1.0.3/digiCore/utils/utils.py
+-rw-rw-rw-   0        0        0       42 2023-06-14 06:39:15.140298 DigiCore-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     3118 2023-06-14 06:38:53.000000 DigiCore-1.0.3/setup.py
```

### Comparing `DigiCore-1.0.2/DigiCore.egg-info/PKG-INFO` & `DigiCore-1.0.3/DigiCore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DigiCore
-Version: 1.0.2
+Version: 1.0.3
 Summary: DigiCore是一个基于Python的数字化支持部第三方库，旨在为数据处理和开发提供完备的工具集和服务。
 Home-page: UNKNOWN
 Author: yarm
 Author-email: yangyang@doocn.com
 License: MIT License
 Keywords: digicore是服务于道诚集团数字化支持部的自建第三方库项目
 Platform: any
```

### Comparing `DigiCore-1.0.2/DigiCore.egg-info/SOURCES.txt` & `DigiCore-1.0.3/DigiCore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.2/LICENSE` & `DigiCore-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.2/PKG-INFO` & `DigiCore-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DigiCore
-Version: 1.0.2
+Version: 1.0.3
 Summary: DigiCore是一个基于Python的数字化支持部第三方库，旨在为数据处理和开发提供完备的工具集和服务。
 Home-page: UNKNOWN
 Author: yarm
 Author-email: yangyang@doocn.com
 License: MIT License
 Keywords: digicore是服务于道诚集团数字化支持部的自建第三方库项目
 Platform: any
```

### Comparing `DigiCore-1.0.2/README.md` & `DigiCore-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.2/digiCore/__init__.py` & `DigiCore-1.0.3/digiCore/__init__.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.2/digiCore/dingding/dingding_model.py` & `DigiCore-1.0.3/digiCore/dingding/dingding_model.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.2/digiCore/dingding/send_to_group.py` & `DigiCore-1.0.3/digiCore/dingding/send_to_group.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.2/digiCore/dsd_kafka.py` & `DigiCore-1.0.3/digiCore/dsd_kafka.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.2/digiCore/dsd_mongodb.py` & `DigiCore-1.0.3/digiCore/dsd_mongodb.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.2/digiCore/dsd_mysql.py` & `DigiCore-1.0.3/digiCore/dsd_mysql.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.2/digiCore/dsd_redis.py` & `DigiCore-1.0.3/digiCore/dsd_redis.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.2/digiCore/kingdee/__init__.py` & `DigiCore-1.0.3/digiCore/kingdee/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,17 @@
 # @Email ： yangyang@doocn.com
 # @File : DigiCore
 # @Desc :
 import subprocess
 
 from loguru import logger
 
-import package_name
 # 查看已安装的包列表
 import pkg_resources
 
 installed_packages = [pkg.key for pkg in pkg_resources.working_set]
 
 if 'kingdee.cdp.webapi.sdk' not in installed_packages:
     try:
-        subprocess.call(['pip', 'install', 'kingdee.cdp.webapi.sdk-8.0.3-py3-none-any.whl'])
+        subprocess.call(['pip', 'install', '../kingdee.cdp.webapi.sdk-8.0.3-py3-none-any.whl'])
     except Exception as e:
         logger.error('金蝶安装包安装失败！')
```

### Comparing `DigiCore-1.0.2/digiCore/kingdee/kingdee_tools.py` & `DigiCore-1.0.3/digiCore/kingdee/kingdee_tools.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.2/digiCore/lingxing/api_scheduler.py` & `DigiCore-1.0.3/digiCore/lingxing/api_scheduler.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.2/digiCore/status_code.py` & `DigiCore-1.0.3/digiCore/status_code.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.2/digiCore/utils/utils.py` & `DigiCore-1.0.3/digiCore/utils/utils.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.2/setup.py` & `DigiCore-1.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,24 +25,58 @@
     zip_safe = (
         hasattr(zipimport.zipimporter, "iter_modules")
         or zipimport.zipimporter in pkgutil.iter_importer_modules.registry.keys()
     )
 except AttributeError:
     zip_safe = False
 
-with open('requirements.txt', 'rb') as f:
-    data = chardet.detect(f.read())
-    encoding = data['encoding']
+requires = [
+"async-timeout==4.0.2",
+"certifi==2023.5.7",
+"chardet==5.1.0",
+"charset-normalizer==3.1.0",
+"colorama==0.4.6",
+"confluent-kafka==2.1.1",
+"crypto==1.4.1",
+"DBUtils==3.0.3",
+"dnspython==2.3.0",
+"et-xmlfile==1.1.0",
+"idna==3.4",
+"kingdee.cdp.webapi.sdk @ file:///kingdee.cdp.webapi.sdk-8.0.3-py3-none-any.whl",
+"loguru==0.7.0",
+"lz4==4.3.2",
+"Naked==0.1.32",
+"numpy==1.24.3",
+"openpyxl==3.1.2",
+"orjson==3.8.12",
+"package-name==0.1",
+"pandas==2.0.1",
+"pycryptodome==3.18.0",
+"pycryptodomex==3.18.0",
+"pydantic==1.10.7",
+"pymongo==4.3.3",
+"PyMySQL==1.0.3",
+"python-dateutil==2.8.2",
+"pytz==2023.3",
+"PyYAML==6.0",
+"redis==4.5.5",
+"requests==2.30.0",
+"shellescape==3.8.1",
+"six==1.16.0",
+"typing_extensions==4.5.0",
+"tzdata==2023.3",
+"urllib3==2.0.2",
+"win32-setctime==1.1.0"
 
-with open('requirements.txt',encoding=encoding) as f:
-    requirements = f.read().splitlines()
+
+]
 
 setup(
     name="DigiCore",
-    version="1.0.2",
+    version="1.0.3",
     description="DigiCore是一个基于Python的数字化支持部第三方库，旨在为数据处理和开发提供完备的工具集和服务。",
     long_description=README,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
@@ -61,12 +95,12 @@
         "License :: OSI Approved :: MIT License",
     ],
     keywords="digicore是服务于道诚集团数字化支持部的自建第三方库项目",
     author="yarm",
     author_email="yangyang@doocn.com",
     license="MIT License",
     packages=find_packages(exclude=excluded_packages),
-    install_requires=requirements,
+    install_requires=requires,
     platforms=["any"],
     zip_safe=zip_safe,
     python_requires=">=3.7",
 )
```

