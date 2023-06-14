# Comparing `tmp/pynocaptcha-1.5.2.tar.gz` & `tmp/pynocaptcha-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pynocaptcha-1.5.2.tar", last modified: Tue Jun 13 04:04:43 2023, max compression
+gzip compressed data, was "dist/pynocaptcha-1.5.3.tar", last modified: Wed Jun 14 09:34:50 2023, max compression
```

## Comparing `pynocaptcha-1.5.2.tar` & `pynocaptcha-1.5.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-13 04:04:43.000000 pynocaptcha-1.5.2/
--rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-06-13 04:04:43.000000 pynocaptcha-1.5.2/PKG-INFO
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-13 04:04:43.000000 pynocaptcha-1.5.2/pynocaptcha/
--rw-r--r--   0 esbiya     (501) staff       (20)      571 2023-05-15 07:30:18.000000 pynocaptcha-1.5.2/pynocaptcha/__init__.py
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-13 04:04:43.000000 pynocaptcha-1.5.2/pynocaptcha/crackers/
--rw-r--r--   0 esbiya     (501) staff       (20)     1016 2023-06-06 02:53:27.000000 pynocaptcha-1.5.2/pynocaptcha/crackers/akamai.py
--rw-r--r--   0 esbiya     (501) staff       (20)     4715 2023-06-06 02:54:14.000000 pynocaptcha-1.5.2/pynocaptcha/crackers/base.py
--rw-r--r--   0 esbiya     (501) staff       (20)     5186 2023-04-23 09:01:32.000000 pynocaptcha-1.5.2/pynocaptcha/crackers/cloudflare.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.5.2/pynocaptcha/crackers/hcaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)   222114 2023-06-13 04:02:11.000000 pynocaptcha-1.5.2/pynocaptcha/crackers/incapsula.py
--rw-r--r--   0 esbiya     (501) staff       (20)     2449 2023-04-23 08:59:52.000000 pynocaptcha-1.5.2/pynocaptcha/crackers/recaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-06-13 04:03:14.000000 pynocaptcha-1.5.2/setup.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-14 09:34:50.000000 pynocaptcha-1.5.3/
+-rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-06-14 09:34:50.000000 pynocaptcha-1.5.3/PKG-INFO
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-14 09:34:50.000000 pynocaptcha-1.5.3/pynocaptcha/
+-rw-r--r--   0 esbiya     (501) staff       (20)      630 2023-06-14 09:34:47.000000 pynocaptcha-1.5.3/pynocaptcha/__init__.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-14 09:34:50.000000 pynocaptcha-1.5.3/pynocaptcha/crackers/
+-rw-r--r--   0 esbiya     (501) staff       (20)     1006 2023-06-14 09:31:37.000000 pynocaptcha-1.5.3/pynocaptcha/crackers/akamai.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     4715 2023-06-06 02:54:14.000000 pynocaptcha-1.5.3/pynocaptcha/crackers/base.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     5186 2023-04-23 09:01:32.000000 pynocaptcha-1.5.3/pynocaptcha/crackers/cloudflare.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.5.3/pynocaptcha/crackers/hcaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)   222114 2023-06-13 04:02:11.000000 pynocaptcha-1.5.3/pynocaptcha/crackers/incapsula.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     2449 2023-04-23 08:59:52.000000 pynocaptcha-1.5.3/pynocaptcha/crackers/recaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)      890 2023-06-14 09:32:19.000000 pynocaptcha-1.5.3/pynocaptcha/crackers/tls.py
+-rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-06-14 09:33:44.000000 pynocaptcha-1.5.3/setup.py
```

### Comparing `pynocaptcha-1.5.2/PKG-INFO` & `pynocaptcha-1.5.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pynocaptcha
-Version: 1.5.2
+Version: 1.5.3
 Summary: nocaptcha.io api
 Home-page: UNKNOWN
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: MIT
 Description: nocaptcha.io python api
 Keywords: nocaptcha
```

### Comparing `pynocaptcha-1.5.2/pynocaptcha/__init__.py` & `pynocaptcha-1.5.3/pynocaptcha/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 
 
 from .crackers.cloudflare import CloudFlareCracker
 from .crackers.incapsula import IncapsulaReese84Cracker, IncapsulaUtmvcCracker
 from .crackers.hcaptcha import HcaptchaCracker
 from .crackers.akamai import AkamaiV2Cracker
 from .crackers.recaptcha import ReCaptchaUniversalCracker, ReCaptchaEnterpriseCracker, ReCaptchaSteamCracker
+from .crackers.tls import TlsV1Cracker
 
 __all__ = [
     'pynocaptcha', 
     'CloudFlareCracker', 'IncapsulaReese84Cracker', 'IncapsulaUtmvcCracker', 'HcaptchaCracker', 
-    'AkamaiV2Cracker', 'ReCaptchaUniversalCracker', 'ReCaptchaEnterpriseCracker', 'ReCaptchaSteamCracker'
+    'AkamaiV2Cracker', 'ReCaptchaUniversalCracker', 'ReCaptchaEnterpriseCracker', 'ReCaptchaSteamCracker',
+    'TlsV1Cracker'
 ]
```

### Comparing `pynocaptcha-1.5.2/pynocaptcha/crackers/akamai.py` & `pynocaptcha-1.5.3/pynocaptcha/crackers/akamai.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 class AkamaiV2Cracker(BaseCracker):
     
     cracker_name = "akamai"
     cracker_version = "v2"    
 
     """
-    recaptcha universal cracker
+    akamai v2 cracker
     :param href: 触发验证的页面地址
     :param api: akamai 提交 sensor_data 的地址
     :param telemetry: 是否 headers 中的 telemetry 参数验证形式, 默认 false
     :param cookies: 请求 href 首页返回的 cookie _abck, bm_sz 值, 传了 api 参数必须传该值, 示例: { "value": "_abck=xxx; bm_sz=xxx", "uri": "https://example.com" }
     :param device: 请求流程使用的设备类型, 可选 pc/mobile, 默认 mobile
     调用示例:
     cracker = AkamaiV2Cracker(
```

### Comparing `pynocaptcha-1.5.2/pynocaptcha/crackers/base.py` & `pynocaptcha-1.5.3/pynocaptcha/crackers/base.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.2/pynocaptcha/crackers/cloudflare.py` & `pynocaptcha-1.5.3/pynocaptcha/crackers/cloudflare.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.2/pynocaptcha/crackers/hcaptcha.py` & `pynocaptcha-1.5.3/pynocaptcha/crackers/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.2/pynocaptcha/crackers/incapsula.py` & `pynocaptcha-1.5.3/pynocaptcha/crackers/incapsula.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.2/pynocaptcha/crackers/recaptcha.py` & `pynocaptcha-1.5.3/pynocaptcha/crackers/recaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.2/setup.py` & `pynocaptcha-1.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 
 
 setup(
     name='pynocaptcha',
-    version='1.5.2',
+    version='1.5.3',
     description='nocaptcha.io api',
     long_description='nocaptcha.io python api',
     install_requires=["pyhttpx", "loguru"],
     license='MIT',
     packages=["pynocaptcha/crackers", "pynocaptcha"],
     package_dir={'pynocaptcha': 'pynocaptcha'},
     platforms=["all"],
```

