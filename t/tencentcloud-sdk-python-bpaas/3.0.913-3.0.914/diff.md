# Comparing `tmp/tencentcloud-sdk-python-bpaas-3.0.913.tar.gz` & `tmp/tencentcloud-sdk-python-bpaas-3.0.914.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-bpaas-3.0.913.tar", last modified: Tue Jun 13 02:05:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-bpaas-3.0.914.tar", last modified: Wed Jun 14 00:19:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-bpaas-3.0.913.tar` & `tencentcloud-sdk-python-bpaas-3.0.914.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:05:15.000000 tencentcloud-sdk-python-bpaas-3.0.913/
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-13 02:05:15.000000 tencentcloud-sdk-python-bpaas-3.0.913/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:05:15.000000 tencentcloud-sdk-python-bpaas-3.0.913/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:05:15.000000 tencentcloud-sdk-python-bpaas-3.0.913/tencentcloud/bpaas/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:05:15.000000 tencentcloud-sdk-python-bpaas-3.0.913/tencentcloud/bpaas/v20181217/
--rw-r--r--   0 root         (0) root         (0)     1297 2023-06-13 02:05:15.000000 tencentcloud-sdk-python-bpaas-3.0.913/tencentcloud/bpaas/v20181217/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:05:15.000000 tencentcloud-sdk-python-bpaas-3.0.913/tencentcloud/bpaas/v20181217/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16725 2023-06-13 02:05:15.000000 tencentcloud-sdk-python-bpaas-3.0.913/tencentcloud/bpaas/v20181217/models.py
--rw-r--r--   0 root         (0) root         (0)     2824 2023-06-13 02:05:15.000000 tencentcloud-sdk-python-bpaas-3.0.913/tencentcloud/bpaas/v20181217/bpaas_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:05:15.000000 tencentcloud-sdk-python-bpaas-3.0.913/tencentcloud/bpaas/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:05:15.000000 tencentcloud-sdk-python-bpaas-3.0.913/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:05:15.000000 tencentcloud-sdk-python-bpaas-3.0.913/tencentcloud_sdk_python_bpaas.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:05:15.000000 tencentcloud-sdk-python-bpaas-3.0.913/tencentcloud_sdk_python_bpaas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-06-13 02:05:15.000000 tencentcloud-sdk-python-bpaas-3.0.913/tencentcloud_sdk_python_bpaas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-13 02:05:15.000000 tencentcloud-sdk-python-bpaas-3.0.913/tencentcloud_sdk_python_bpaas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:05:15.000000 tencentcloud-sdk-python-bpaas-3.0.913/tencentcloud_sdk_python_bpaas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-13 02:05:15.000000 tencentcloud-sdk-python-bpaas-3.0.913/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-06-13 02:05:15.000000 tencentcloud-sdk-python-bpaas-3.0.913/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:05:15.000000 tencentcloud-sdk-python-bpaas-3.0.913/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:19:55.000000 tencentcloud-sdk-python-bpaas-3.0.914/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-14 00:19:55.000000 tencentcloud-sdk-python-bpaas-3.0.914/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:19:55.000000 tencentcloud-sdk-python-bpaas-3.0.914/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:19:55.000000 tencentcloud-sdk-python-bpaas-3.0.914/tencentcloud/bpaas/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:19:55.000000 tencentcloud-sdk-python-bpaas-3.0.914/tencentcloud/bpaas/v20181217/
+-rw-r--r--   0 root         (0) root         (0)     1297 2023-06-14 00:19:55.000000 tencentcloud-sdk-python-bpaas-3.0.914/tencentcloud/bpaas/v20181217/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:19:55.000000 tencentcloud-sdk-python-bpaas-3.0.914/tencentcloud/bpaas/v20181217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17492 2023-06-14 00:19:55.000000 tencentcloud-sdk-python-bpaas-3.0.914/tencentcloud/bpaas/v20181217/models.py
+-rw-r--r--   0 root         (0) root         (0)     2824 2023-06-14 00:19:55.000000 tencentcloud-sdk-python-bpaas-3.0.914/tencentcloud/bpaas/v20181217/bpaas_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:19:55.000000 tencentcloud-sdk-python-bpaas-3.0.914/tencentcloud/bpaas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:19:55.000000 tencentcloud-sdk-python-bpaas-3.0.914/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:19:55.000000 tencentcloud-sdk-python-bpaas-3.0.914/tencentcloud_sdk_python_bpaas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:19:55.000000 tencentcloud-sdk-python-bpaas-3.0.914/tencentcloud_sdk_python_bpaas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-06-14 00:19:55.000000 tencentcloud-sdk-python-bpaas-3.0.914/tencentcloud_sdk_python_bpaas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-14 00:19:55.000000 tencentcloud-sdk-python-bpaas-3.0.914/tencentcloud_sdk_python_bpaas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:19:55.000000 tencentcloud-sdk-python-bpaas-3.0.914/tencentcloud_sdk_python_bpaas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-14 00:19:55.000000 tencentcloud-sdk-python-bpaas-3.0.914/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-06-14 00:19:55.000000 tencentcloud-sdk-python-bpaas-3.0.914/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:19:55.000000 tencentcloud-sdk-python-bpaas-3.0.914/setup.cfg
```

### Comparing `tencentcloud-sdk-python-bpaas-3.0.913/README.rst` & `tencentcloud-sdk-python-bpaas-3.0.914/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bpaas-3.0.913/tencentcloud/bpaas/v20181217/errorcodes.py` & `tencentcloud-sdk-python-bpaas-3.0.914/tencentcloud/bpaas/v20181217/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bpaas-3.0.913/tencentcloud/bpaas/v20181217/models.py` & `tencentcloud-sdk-python-bpaas-3.0.914/tencentcloud/bpaas/v20181217/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -183,28 +183,32 @@
         :type Status: int
         :param Nodes: 节点信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type Nodes: list of StatusNode
         :param ApprovingNodeId: 正在审批的节点id
 注意：此字段可能返回 null，表示取不到有效值。
         :type ApprovingNodeId: str
+        :param ModifyTime: 更新时间，时间格式：2021-12-12 10:12:10	
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ModifyTime: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.ApplyUin = None
         self.ApplyOwnUin = None
         self.ApplyUinNick = None
         self.BpaasId = None
         self.BpaasName = None
         self.ApplicationParams = None
         self.Reason = None
         self.CreateTime = None
         self.Status = None
         self.Nodes = None
         self.ApprovingNodeId = None
+        self.ModifyTime = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.ApplyUin = params.get("ApplyUin")
         self.ApplyOwnUin = params.get("ApplyOwnUin")
         self.ApplyUinNick = params.get("ApplyUinNick")
@@ -222,14 +226,15 @@
         if params.get("Nodes") is not None:
             self.Nodes = []
             for item in params.get("Nodes"):
                 obj = StatusNode()
                 obj._deserialize(item)
                 self.Nodes.append(obj)
         self.ApprovingNodeId = params.get("ApprovingNodeId")
+        self.ModifyTime = params.get("ModifyTime")
         self.RequestId = params.get("RequestId")
 
 
 class OutApproveBpaasApplicationRequest(AbstractModel):
     """OutApproveBpaasApplication请求参数结构体
 
     """
@@ -420,14 +425,20 @@
         :type CKafkaRegion: str
         :param ExternalUrl: 外部审批Url
 注意：此字段可能返回 null，表示取不到有效值。
         :type ExternalUrl: str
         :param ParallelNodes: 并行节点 3-4
 注意：此字段可能返回 null，表示取不到有效值。
         :type ParallelNodes: str
+        :param RejectedCloudFunctionMsg: scf拒绝时返回信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RejectedCloudFunctionMsg: str
+        :param PrevNode: 上一个节点
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PrevNode: str
         """
         self.NodeId = None
         self.NodeName = None
         self.NodeType = None
         self.NextNode = None
         self.Opinion = None
         self.ScfName = None
@@ -442,14 +453,16 @@
         self.ApproveType = None
         self.CallMethod = None
         self.DataHubId = None
         self.TaskName = None
         self.CKafkaRegion = None
         self.ExternalUrl = None
         self.ParallelNodes = None
+        self.RejectedCloudFunctionMsg = None
+        self.PrevNode = None
 
 
     def _deserialize(self, params):
         self.NodeId = params.get("NodeId")
         self.NodeName = params.get("NodeName")
         self.NodeType = params.get("NodeType")
         self.NextNode = params.get("NextNode")
@@ -470,14 +483,16 @@
         self.ApproveType = params.get("ApproveType")
         self.CallMethod = params.get("CallMethod")
         self.DataHubId = params.get("DataHubId")
         self.TaskName = params.get("TaskName")
         self.CKafkaRegion = params.get("CKafkaRegion")
         self.ExternalUrl = params.get("ExternalUrl")
         self.ParallelNodes = params.get("ParallelNodes")
+        self.RejectedCloudFunctionMsg = params.get("RejectedCloudFunctionMsg")
+        self.PrevNode = params.get("PrevNode")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-bpaas-3.0.913/tencentcloud/bpaas/v20181217/bpaas_client.py` & `tencentcloud-sdk-python-bpaas-3.0.914/tencentcloud/bpaas/v20181217/bpaas_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bpaas-3.0.913/tencentcloud/__init__.py` & `tencentcloud-sdk-python-bpaas-3.0.914/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-bpaas-3.0.913/tencentcloud_sdk_python_bpaas.egg-info/PKG-INFO` & `tencentcloud-sdk-python-bpaas-3.0.914/tencentcloud_sdk_python_bpaas.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bpaas
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Bpaas SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bpaas-3.0.913/PKG-INFO` & `tencentcloud-sdk-python-bpaas-3.0.914/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bpaas
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Bpaas SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bpaas-3.0.913/setup.py` & `tencentcloud-sdk-python-bpaas-3.0.914/setup.py`

 * *Files identical despite different names*

