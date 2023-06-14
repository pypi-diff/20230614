# Comparing `tmp/tencentcloud-sdk-python-live-3.0.913.tar.gz` & `tmp/tencentcloud-sdk-python-live-3.0.914.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.913.tar", last modified: Tue Jun 13 02:14:23 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.914.tar", last modified: Wed Jun 14 00:29:24 2023, max compression
```

## Comparing `tencentcloud-sdk-python-live-3.0.913.tar` & `tencentcloud-sdk-python-live-3.0.914.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud_sdk_python_live.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud_sdk_python_live.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud_sdk_python_live.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud/live/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud/live/v20180801/
--rw-r--r--   0 root         (0) root         (0)   137300 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud/live/v20180801/live_client.py
--rw-r--r--   0 root         (0) root         (0)    18702 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud/live/v20180801/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud/live/v20180801/__init__.py
--rw-r--r--   0 root         (0) root         (0)   433875 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud/live/v20180801/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud/live/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud_sdk_python_live.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud_sdk_python_live.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud_sdk_python_live.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud/live/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud/live/v20180801/
+-rw-r--r--   0 root         (0) root         (0)   138415 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud/live/v20180801/live_client.py
+-rw-r--r--   0 root         (0) root         (0)    18702 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud/live/v20180801/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud/live/v20180801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   435096 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud/live/v20180801/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud/live/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/setup.cfg
```

### Comparing `tencentcloud-sdk-python-live-3.0.913/tencentcloud_sdk_python_live.egg-info/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.914/tencentcloud_sdk_python_live.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.913/README.rst` & `tencentcloud-sdk-python-live-3.0.914/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.913/tencentcloud/live/v20180801/live_client.py` & `tencentcloud-sdk-python-live-3.0.914/tencentcloud/live/v20180801/live_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2978,14 +2978,40 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def RestartLivePullStreamTask(self, request):
+        """将正在运行的拉流转推任务进行重启。
+        注意：
+        1. 重启任务会造成推流中断。
+        2. 点播源任务的重启，会根据VodRefreshType决定是续播还是从头开始播。
+
+        :param request: Request instance for RestartLivePullStreamTask.
+        :type request: :class:`tencentcloud.live.v20180801.models.RestartLivePullStreamTaskRequest`
+        :rtype: :class:`tencentcloud.live.v20180801.models.RestartLivePullStreamTaskResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("RestartLivePullStreamTask", params, headers=headers)
+            response = json.loads(body)
+            model = models.RestartLivePullStreamTaskResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ResumeDelayLiveStream(self, request):
         """取消直播流设置的延时配置，恢复实时直播画面。
 
         :param request: Request instance for ResumeDelayLiveStream.
         :type request: :class:`tencentcloud.live.v20180801.models.ResumeDelayLiveStreamRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.ResumeDelayLiveStreamResponse`
```

### Comparing `tencentcloud-sdk-python-live-3.0.913/tencentcloud/live/v20180801/errorcodes.py` & `tencentcloud-sdk-python-live-3.0.914/tencentcloud/live/v20180801/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.913/tencentcloud/live/v20180801/models.py` & `tencentcloud-sdk-python-live-3.0.914/tencentcloud/live/v20180801/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -11095,14 +11095,59 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class RestartLivePullStreamTaskRequest(AbstractModel):
+    """RestartLivePullStreamTask请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskId: 任务 Id。
+        :type TaskId: str
+        :param Operator: 操作人备注名称。
+        :type Operator: str
+        """
+        self.TaskId = None
+        self.Operator = None
+
+
+    def _deserialize(self, params):
+        self.TaskId = params.get("TaskId")
+        self.Operator = params.get("Operator")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class RestartLivePullStreamTaskResponse(AbstractModel):
+    """RestartLivePullStreamTask返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class ResumeDelayLiveStreamRequest(AbstractModel):
     """ResumeDelayLiveStream请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-live-3.0.913/tencentcloud/__init__.py` & `tencentcloud-sdk-python-live-3.0.914/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-live-3.0.913/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.914/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.913/setup.py` & `tencentcloud-sdk-python-live-3.0.914/setup.py`

 * *Files identical despite different names*

