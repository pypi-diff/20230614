# Comparing `tmp/tencentcloud-sdk-python-gme-3.0.913.tar.gz` & `tmp/tencentcloud-sdk-python-gme-3.0.914.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-gme-3.0.913.tar", last modified: Tue Jun 13 02:11:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-gme-3.0.914.tar", last modified: Wed Jun 14 00:26:52 2023, max compression
```

## Comparing `tencentcloud-sdk-python-gme-3.0.913.tar` & `tencentcloud-sdk-python-gme-3.0.914.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:11:57.000000 tencentcloud-sdk-python-gme-3.0.913/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-13 02:11:57.000000 tencentcloud-sdk-python-gme-3.0.913/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:11:57.000000 tencentcloud-sdk-python-gme-3.0.913/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:11:57.000000 tencentcloud-sdk-python-gme-3.0.913/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:11:57.000000 tencentcloud-sdk-python-gme-3.0.913/tencentcloud/gme/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:11:57.000000 tencentcloud-sdk-python-gme-3.0.913/tencentcloud/gme/v20180711/
--rw-r--r--   0 root         (0) root         (0)    33250 2023-06-13 02:11:57.000000 tencentcloud-sdk-python-gme-3.0.913/tencentcloud/gme/v20180711/gme_client.py
--rw-r--r--   0 root         (0) root         (0)     3906 2023-06-13 02:11:57.000000 tencentcloud-sdk-python-gme-3.0.913/tencentcloud/gme/v20180711/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:11:57.000000 tencentcloud-sdk-python-gme-3.0.913/tencentcloud/gme/v20180711/__init__.py
--rw-r--r--   0 root         (0) root         (0)   104897 2023-06-13 02:11:57.000000 tencentcloud-sdk-python-gme-3.0.913/tencentcloud/gme/v20180711/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:11:57.000000 tencentcloud-sdk-python-gme-3.0.913/tencentcloud/gme/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:11:57.000000 tencentcloud-sdk-python-gme-3.0.913/tencentcloud_sdk_python_gme.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:11:57.000000 tencentcloud-sdk-python-gme-3.0.913/tencentcloud_sdk_python_gme.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-13 02:11:57.000000 tencentcloud-sdk-python-gme-3.0.913/tencentcloud_sdk_python_gme.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-13 02:11:57.000000 tencentcloud-sdk-python-gme-3.0.913/tencentcloud_sdk_python_gme.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:11:57.000000 tencentcloud-sdk-python-gme-3.0.913/tencentcloud_sdk_python_gme.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-13 02:11:57.000000 tencentcloud-sdk-python-gme-3.0.913/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-13 02:11:57.000000 tencentcloud-sdk-python-gme-3.0.913/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:11:57.000000 tencentcloud-sdk-python-gme-3.0.913/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:26:52.000000 tencentcloud-sdk-python-gme-3.0.914/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-14 00:26:52.000000 tencentcloud-sdk-python-gme-3.0.914/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:26:52.000000 tencentcloud-sdk-python-gme-3.0.914/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:26:52.000000 tencentcloud-sdk-python-gme-3.0.914/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:26:52.000000 tencentcloud-sdk-python-gme-3.0.914/tencentcloud/gme/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:26:52.000000 tencentcloud-sdk-python-gme-3.0.914/tencentcloud/gme/v20180711/
+-rw-r--r--   0 root         (0) root         (0)    33250 2023-06-14 00:26:52.000000 tencentcloud-sdk-python-gme-3.0.914/tencentcloud/gme/v20180711/gme_client.py
+-rw-r--r--   0 root         (0) root         (0)     3906 2023-06-14 00:26:52.000000 tencentcloud-sdk-python-gme-3.0.914/tencentcloud/gme/v20180711/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:26:52.000000 tencentcloud-sdk-python-gme-3.0.914/tencentcloud/gme/v20180711/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   105312 2023-06-14 00:26:52.000000 tencentcloud-sdk-python-gme-3.0.914/tencentcloud/gme/v20180711/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:26:52.000000 tencentcloud-sdk-python-gme-3.0.914/tencentcloud/gme/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:26:52.000000 tencentcloud-sdk-python-gme-3.0.914/tencentcloud_sdk_python_gme.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:26:52.000000 tencentcloud-sdk-python-gme-3.0.914/tencentcloud_sdk_python_gme.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-14 00:26:52.000000 tencentcloud-sdk-python-gme-3.0.914/tencentcloud_sdk_python_gme.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-14 00:26:52.000000 tencentcloud-sdk-python-gme-3.0.914/tencentcloud_sdk_python_gme.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:26:52.000000 tencentcloud-sdk-python-gme-3.0.914/tencentcloud_sdk_python_gme.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-14 00:26:52.000000 tencentcloud-sdk-python-gme-3.0.914/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-14 00:26:52.000000 tencentcloud-sdk-python-gme-3.0.914/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:26:52.000000 tencentcloud-sdk-python-gme-3.0.914/setup.cfg
```

### Comparing `tencentcloud-sdk-python-gme-3.0.913/README.rst` & `tencentcloud-sdk-python-gme-3.0.914/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gme-3.0.913/tencentcloud/__init__.py` & `tencentcloud-sdk-python-gme-3.0.914/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.913'
+__version__ = '3.0.914'
```

### Comparing `tencentcloud-sdk-python-gme-3.0.913/tencentcloud/gme/v20180711/gme_client.py` & `tencentcloud-sdk-python-gme-3.0.914/tencentcloud/gme/v20180711/gme_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gme-3.0.913/tencentcloud/gme/v20180711/errorcodes.py` & `tencentcloud-sdk-python-gme-3.0.914/tencentcloud/gme/v20180711/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gme-3.0.913/tencentcloud/gme/v20180711/models.py` & `tencentcloud-sdk-python-gme-3.0.914/tencentcloud/gme/v20180711/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2539,20 +2539,24 @@
         :type Porn: :class:`tencentcloud.gme.v20180711.models.StatusInfo`
         :param Live: 语音录制服务开关状态
 注意：此字段可能返回 null，表示取不到有效值。
         :type Live: :class:`tencentcloud.gme.v20180711.models.StatusInfo`
         :param RealTimeAsr: 语音转文本服务开关状态
 注意：此字段可能返回 null，表示取不到有效值。
         :type RealTimeAsr: :class:`tencentcloud.gme.v20180711.models.StatusInfo`
+        :param TextTranslate: 文本翻译服务开关状态
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TextTranslate: :class:`tencentcloud.gme.v20180711.models.StatusInfo`
         """
         self.RealTimeSpeech = None
         self.VoiceMessage = None
         self.Porn = None
         self.Live = None
         self.RealTimeAsr = None
+        self.TextTranslate = None
 
 
     def _deserialize(self, params):
         if params.get("RealTimeSpeech") is not None:
             self.RealTimeSpeech = StatusInfo()
             self.RealTimeSpeech._deserialize(params.get("RealTimeSpeech"))
         if params.get("VoiceMessage") is not None:
@@ -2563,14 +2567,17 @@
             self.Porn._deserialize(params.get("Porn"))
         if params.get("Live") is not None:
             self.Live = StatusInfo()
             self.Live._deserialize(params.get("Live"))
         if params.get("RealTimeAsr") is not None:
             self.RealTimeAsr = StatusInfo()
             self.RealTimeAsr._deserialize(params.get("RealTimeAsr"))
+        if params.get("TextTranslate") is not None:
+            self.TextTranslate = StatusInfo()
+            self.TextTranslate._deserialize(params.get("TextTranslate"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-gme-3.0.913/tencentcloud_sdk_python_gme.egg-info/PKG-INFO` & `tencentcloud-sdk-python-gme-3.0.914/tencentcloud_sdk_python_gme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gme
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Gme SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-gme-3.0.913/PKG-INFO` & `tencentcloud-sdk-python-gme-3.0.914/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gme
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Gme SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-gme-3.0.913/setup.py` & `tencentcloud-sdk-python-gme-3.0.914/setup.py`

 * *Files identical despite different names*

