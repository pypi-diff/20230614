# Comparing `tmp/igz_mgmt-0.0.5.tar.gz` & `tmp/igz_mgmt-0.0.6.tar.gz`

## Comparing `igz_mgmt-0.0.5.tar` & `igz_mgmt-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 igz_mgmt-0.0.5/igz_mgmt/__init__.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 igz_mgmt-0.0.5/igz_mgmt/__version__.py
--rw-r--r--   0        0        0    11746 2020-02-02 00:00:00.000000 igz_mgmt-0.0.5/igz_mgmt/app_services.py
--rw-r--r--   0        0        0    13485 2020-02-02 00:00:00.000000 igz_mgmt-0.0.5/igz_mgmt/client.py
--rw-r--r--   0        0        0     4705 2020-02-02 00:00:00.000000 igz_mgmt-0.0.5/igz_mgmt/constants.py
--rw-r--r--   0        0        0     5151 2020-02-02 00:00:00.000000 igz_mgmt-0.0.5/igz_mgmt/cruds.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 igz_mgmt-0.0.5/igz_mgmt/exceptions.py
--rw-r--r--   0        0        0     8407 2020-02-02 00:00:00.000000 igz_mgmt-0.0.5/igz_mgmt/operations.py
--rw-r--r--   0        0        0    36079 2020-02-02 00:00:00.000000 igz_mgmt-0.0.5/igz_mgmt/resources.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 igz_mgmt-0.0.5/igz_mgmt/common/__init__.py
--rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 igz_mgmt-0.0.5/igz_mgmt/common/helpers.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 igz_mgmt-0.0.5/igz_mgmt/logger/__init__.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 igz_mgmt-0.0.5/igz_mgmt/logger/logger.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 igz_mgmt-0.0.5/LICENSE
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 igz_mgmt-0.0.5/README.md
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 igz_mgmt-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 igz_mgmt-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/__init__.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/__version__.py
+-rw-r--r--   0        0        0    15533 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/client.py
+-rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/constants.py
+-rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/cruds.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/exceptions.py
+-rw-r--r--   0        0        0     9734 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/operations.py
+-rw-r--r--   0        0        0    47741 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/resources.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/common/__init__.py
+-rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/common/helpers.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/logger/__init__.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/logger/logger.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/schemas/__init__.py
+-rw-r--r--   0        0        0    11993 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/schemas/app_services.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/schemas/manual_events.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/LICENSE
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/README.md
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/PKG-INFO
```

### Comparing `igz_mgmt-0.0.5/igz_mgmt/__init__.py` & `igz_mgmt-0.0.6/igz_mgmt/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,39 +8,45 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from .app_services import (
+from igz_mgmt.schemas.app_services import (
     AppServiceBase,
     AppServiceSpec,
     AppServiceStatus,
     CustomAppServiceSpec,
     JupyterSpec,
     ScaleResource,
     ScaleToZeroSpec,
 )
-from .app_services import ScaleToZeroSpecPresets as AppServiceScaleToZeroSpecPresets
+from igz_mgmt.schemas.app_services import (
+    ScaleToZeroSpecPresets as AppServiceScaleToZeroSpecPresets,
+)
+from igz_mgmt.schemas.manual_events import ManualEventSchema
+
 from .client import APIClient as Client
 from .constants import (
-    AdminStatuses,
     ApplyServicesMode,
     AppServiceDesiredStates,
     AppServicePriorityClass,
     ForceApplyAllMode,
     JupyterAppServicePrebakedImage,
+    ProjectDeletionStrategies,
     ScaleToZeroMode,
     TenantManagementRoles,
+    UserAdminStatuses,
+    UserOperationalStatuses,
 )
 from .cruds import ResourceListPagingQueryParams
 from .logger import get_or_create_logger
-from .operations import AppServices, ClusterConfigurations
-from .resources import AccessKey, AppServicesManifest, Group, Job, User
+from .operations import AppServices, ClusterConfigurations, ManualEvents
+from .resources import AccessKey, AppServicesManifest, Group, Job, Project, User
 
 __all__ = [
     "Client",
     "User",
     "Group",
     "AccessKey",
     "Job",
@@ -57,12 +63,17 @@
     "TenantManagementRoles",
     "ScaleToZeroMode",
     "AppServiceDesiredStates",
     "ForceApplyAllMode",
     "ResourceListPagingQueryParams",
     "AppServiceScaleToZeroSpecPresets",
     "AppServicePriorityClass",
-    "AdminStatuses",
+    "UserAdminStatuses",
+    "UserOperationalStatuses",
     "JupyterAppServicePrebakedImage",
     "AppServices",
     "get_or_create_logger",
+    "ManualEvents",
+    "ManualEventSchema",
+    "ProjectDeletionStrategies",
+    "Project",
 ]
```

### Comparing `igz_mgmt-0.0.5/igz_mgmt/__version__.py` & `igz_mgmt-0.0.6/igz_mgmt/logger/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,12 +9,10 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-# version can be either one of the following:
-# x.y.z
-# x.y.z.rcN
+from .logger import Logger, get_or_create_logger
 
-__version__ = "0.0.5"
+__all__ = ["get_or_create_logger", "Logger"]
```

### Comparing `igz_mgmt-0.0.5/igz_mgmt/app_services.py` & `igz_mgmt-0.0.6/igz_mgmt/schemas/app_services.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,186 +12,174 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import typing
 
 import pydantic
 
-from igz_mgmt.constants import (
-    AppServiceDesiredStates,
-    AppServicesScaleToZeroMetrics,
-    JupyterAppServicePrebakedImage,
-    ScaleToZeroMode,
-)
+import igz_mgmt.constants
+import igz_mgmt.schemas
 
 
 # helper function
 def generate_scale_to_zero_spec(window_size: str) -> typing.List["ScaleResource"]:
     """Generates scale resource with metric name and window size.
 
     Args:
         window_size (str): Time to wait before scaling the service to zero.
 
     Returns:
         typing.List["ScaleResource"]: scale to zero spec.
     """
     return [
         ScaleResource(
-            metric_name=AppServicesScaleToZeroMetrics.num_of_requests,
+            metric_name=igz_mgmt.constants.AppServicesScaleToZeroMetrics.num_of_requests,
             window_size=window_size,
         ),
         ScaleResource(
-            metric_name=AppServicesScaleToZeroMetrics.jupyter_kernel_busyness,
+            metric_name=igz_mgmt.constants.AppServicesScaleToZeroMetrics.jupyter_kernel_busyness,
             window_size=window_size,
         ),
     ]
 
 
-class _Base(pydantic.BaseModel):
-    class Config:
-        # be forward compatible
-        extra = "allow"
-        orm_mode = True
-        use_enum_values = True
-
-
-class CredentialsSpec(_Base):
+class CredentialsSpec(igz_mgmt.schemas._Base):
     """Credentials spec.
 
     Spec for describing credentials with which the app service will preform its operations with in the Iguazio cluster.
     """
 
     username: str = pydantic.Field(description="Iguazio username")
 
 
-class SystemResources(_Base):
+class SystemResources(igz_mgmt.schemas._Base):
     """System resource description for use with limits and requests."""
 
     cpu: typing.Optional[str]
     memory: typing.Optional[str]
     nvidia_gpu: typing.Optional[str]
 
 
-class ResourcesSpec(_Base):
+class ResourcesSpec(igz_mgmt.schemas._Base):
     """Resource spec describing the limits and requests for each app service."""
 
     limits: typing.Optional[SystemResources]
     requests: typing.Optional[SystemResources]
 
 
-class ScaleResource(_Base):
+class ScaleResource(igz_mgmt.schemas._Base):
     """Threshold descriptor for scaling app services to zero."""
 
     metric_name: str = pydantic.Field(description="The threshold metric to watch")
     threshold: int = pydantic.Field(
         0,
         description="The value of the metric where if exceeded, the resource will be scaled",
     )
     window_size: str = pydantic.Field(
         description="The amount of time for which the threshold has to be exceeded for the resource to be scaled"
     )
 
 
-class ScaleToZeroSpec(_Base):
+class ScaleToZeroSpec(igz_mgmt.schemas._Base):
     """Spec describing the scale to zero resources/rules."""
 
-    mode: ScaleToZeroMode
+    mode: igz_mgmt.constants.ScaleToZeroMode
     scale_resources: typing.Optional[typing.List[ScaleResource]]
 
 
-class PvcSpec(_Base):
+class PvcSpec(igz_mgmt.schemas._Base):
     """Pvc - kubernetes persistent volume claim spec for app service pod."""
 
     # TODO: convert mounts entries to dictionary
     mounts: typing.Optional[
         typing.Dict[str, typing.List[typing.Dict[str, str]]]
     ] = pydantic.Field(
         description="Dictionary describing the pvc mounts where the key is a volume and the values \
         is the path inside the container"
     )
 
 
 class ScaleToZeroSpecPresets:
     """Scale to zero spec presets."""
 
-    disabled = ScaleToZeroSpec(mode=ScaleToZeroMode.disabled)
+    disabled = ScaleToZeroSpec(mode=igz_mgmt.constants.ScaleToZeroMode.disabled)
     one_minute = ScaleToZeroSpec(
-        mode=ScaleToZeroMode.enabled,
+        mode=igz_mgmt.constants.ScaleToZeroMode.enabled,
         scale_resources=generate_scale_to_zero_spec("1m"),
     )
     five_minutes = ScaleToZeroSpec(
-        mode=ScaleToZeroMode.enabled,
+        mode=igz_mgmt.constants.ScaleToZeroMode.enabled,
         scale_resources=generate_scale_to_zero_spec("5m"),
     )
     ten_minutes = ScaleToZeroSpec(
-        mode=ScaleToZeroMode.enabled,
+        mode=igz_mgmt.constants.ScaleToZeroMode.enabled,
         scale_resources=generate_scale_to_zero_spec("10m"),
     )
     one_hour = ScaleToZeroSpec(
-        mode=ScaleToZeroMode.enabled,
+        mode=igz_mgmt.constants.ScaleToZeroMode.enabled,
         scale_resources=generate_scale_to_zero_spec("1h"),
     )
     two_hours = ScaleToZeroSpec(
-        mode=ScaleToZeroMode.enabled,
+        mode=igz_mgmt.constants.ScaleToZeroMode.enabled,
         scale_resources=generate_scale_to_zero_spec("2h"),
     )
     four_hours = ScaleToZeroSpec(
-        mode=ScaleToZeroMode.enabled,
+        mode=igz_mgmt.constants.ScaleToZeroMode.enabled,
         scale_resources=generate_scale_to_zero_spec("4h"),
     )
 
 
-class SecurityContextSpec(_Base):
+class SecurityContextSpec(igz_mgmt.schemas._Base):
     """Kubernetes Security context spec for app service pods."""
 
     run_as_user: str
     run_as_group: str
     fs_group: str
     supplemental_groups: typing.List[str]
     run_as_non_root: bool
 
 
-class AdvancedSpec(_Base):
+class AdvancedSpec(igz_mgmt.schemas._Base):
     """Advanced app service spec."""
 
     # TODO: convert node_selector entries to dictionary
     # "entries" kind of list. e.g.: {"entries:[{"key":"", "value":""}, ...]}
     node_selector: typing.Optional[typing.Dict[str, typing.List[typing.Dict[str, str]]]]
     priority_class_name: typing.Optional[str] = pydantic.Field(
         description="Use `igz_mgmt.AppServicePriorityClass` enum for the value. \
         However, it is possible to pass any priority class name you want"
     )
 
 
-class Url(_Base):
+class Url(igz_mgmt.schemas._Base):
     """URL for accessing app services."""
 
     kind: str
     url: str
 
 
-class Meta(_Base):
+class Meta(igz_mgmt.schemas._Base):
     """App services metadata class."""
 
     labels: typing.Optional[typing.Dict[str, str]] = pydantic.Field(
         description="Labels for the app service. these will be propagated to all the app service resources"
     )
 
     # TODO: convert annotations entries to dictionary
     # annotations: typing.Optional[typing.Dict[str, str]]
 
 
-class StatusErrorInfo(_Base):
+class StatusErrorInfo(igz_mgmt.schemas._Base):
     """App service Status error info."""
 
     description: str
     timestamp: str
 
 
-class AppServiceStatus(_Base):
+class AppServiceStatus(igz_mgmt.schemas._Base):
     """App service status."""
 
     state: str
     urls: typing.Optional[typing.List[Url]]
     api_urls: typing.Optional[typing.List[Url]]
     internal_api_urls: typing.Optional[typing.List[Url]]
     version: typing.Optional[str]
@@ -209,39 +197,39 @@
         description="Shell specific app service status"
     )
     jupyter: typing.Optional[typing.Dict[str, typing.Any]] = pydantic.Field(
         description="jupyter specific app service status"
     )
 
 
-class HomeContainer(_Base):
+class HomeContainer(igz_mgmt.schemas._Base):
     """Home container."""
 
     container: str
     prefix: str
 
 
-class SSHServerSpec(_Base):
+class SSHServerSpec(igz_mgmt.schemas._Base):
     """SSH configuration for accessing interactive shell app services (e.g. jupyter, shell)."""
 
     force_key_regeneration: bool
     port: int
 
 
-class CustomAppServiceSpec(_Base):
+class CustomAppServiceSpec(igz_mgmt.schemas._Base):
     """Base class for custom app service spec."""
 
     pass
 
 
 class JupyterSpec(CustomAppServiceSpec):
     """Jupyter app service spec."""
 
     image_name: str = (
-        JupyterAppServicePrebakedImage.full_stack
+        igz_mgmt.constants.JupyterAppServicePrebakedImage.full_stack
     )  # TODO: change to optional when backend changed
 
     # optional fields
     spark_name: typing.Optional[str]
     presto_name: typing.Optional[str]
     framesd: typing.Optional[str]
     home_spec: typing.Optional[HomeContainer]
@@ -253,15 +241,15 @@
     ]
     demos_datasets_archive_address: typing.Optional[str]
     docker_registry_name: typing.Optional[str]
     ssh_enabled: typing.Optional[bool]
     ssh_server: typing.Optional[SSHServerSpec]
 
 
-class AppServiceSpec(_Base):
+class AppServiceSpec(igz_mgmt.schemas._Base):
     """App service spec."""
 
     name: str = pydantic.Field(description="The name of the app service")
     kind: str = pydantic.Field(description="The app service kind (jupyter / shell .. )")
 
     # optional fields
     owner: typing.Optional[str] = pydantic.Field(
@@ -297,15 +285,15 @@
         app service and redeploy it according to those changes",
     )
     visible_to_all: typing.Optional[bool] = pydantic.Field(
         description="Whether the app service is visible to all users or only the owner"
     )
     scale_to_zero: typing.Optional[ScaleToZeroSpec]
     pvc: typing.Optional[PvcSpec]
-    desired_state: typing.Optional[AppServiceDesiredStates]
+    desired_state: typing.Optional[igz_mgmt.constants.AppServiceDesiredStates]
     authentication_mode: typing.Optional[str]
     security_context: typing.Optional[SecurityContextSpec]
     persistency_mode: typing.Optional[str]
     advanced: typing.Optional[AdvancedSpec]
 
     # app services
     jupyter: typing.Optional[JupyterSpec]
@@ -346,13 +334,13 @@
                     self.__fields__[field_name].type_, CustomAppServiceSpec
                 ) and kwargs.get(field_name):
                     kwargs["kind"] = field_name
                     break
         super().__init__(**kwargs)
 
 
-class AppServiceBase(_Base):
+class AppServiceBase(igz_mgmt.schemas._Base):
     """App service base class."""
 
     spec: AppServiceSpec
     meta: typing.Optional[Meta]
     status: typing.Optional[AppServiceStatus]
```

### Comparing `igz_mgmt-0.0.5/igz_mgmt/client.py` & `igz_mgmt-0.0.6/igz_mgmt/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 from http import HTTPStatus
 
 import httpx
 import inflection
 import semver
 
 import igz_mgmt.common
+import igz_mgmt.constants
 import igz_mgmt.logger
-from igz_mgmt.constants import SessionPlanes
 
 
 class _BaseHTTPClient:
     def __init__(
         self,
         parent_logger: igz_mgmt.logger.Logger,
         api_url: str,
@@ -36,15 +36,17 @@
         timeout: int = 60,
         retries: int = 3,
     ) -> None:
         super().__init__()
         self._logger = parent_logger.get_child("httpc")
         self._transport = httpx.HTTPTransport(verify=False, retries=retries)
         self._cookies = httpx.Cookies()
-        self._headers = {"Content-Type": "application/json"}
+        self._headers = {
+            igz_mgmt.constants._RequestHeaders.content_type_header: "application/json"
+        }
         self._session = httpx.Client(
             base_url=api_url,
             timeout=timeout,
             mounts={
                 "http://": self._transport,
                 "https://": self._transport,
             },
@@ -147,14 +149,16 @@
         timeout (int, optional): protocol timeout.
         retries (int, optional): number of retries for a request before failing.
         username (str, optional): username to log in the system.
         password (str, optional): password to log in the system.
         access_key (str, optional): control plane access key for the Iguazio system.
     """
 
+    __DEFAULT_EXTERNAL_VERSION_NUMBER = "3.4.2"
+
     def __init__(
         self,
         *,
         endpoint: str = "",
         timeout: int = 60,
         retries: int = 3,
         username: str = "",
@@ -275,14 +279,33 @@
         """
         return self._client.delete(
             f"{inflection.pluralize(resource_name)}/{resource_id}",
             f"Failed to delete {resource_name} {resource_id}".strip(),
             **kwargs,
         )
 
+    def delete_by_attribute(
+        self, resource_name: str, attribute_name: str, attribute_value: str, **kwargs
+    ):
+        """Deletes an existing resource by resource attribute.
+
+        Args:
+            resource_name (str): The resource name.
+            attribute_name (str): The identifying attribute in the resource to be deleted.
+            attribute_value (str): The value of the resource attribute to delete by.
+            **kwargs: additional arguments to pass to the request.
+        """
+        attributes = {attribute_name: attribute_value}
+        return self._client.delete(
+            f"{inflection.pluralize(resource_name)}",
+            f"Failed to delete {resource_name} by {attribute_name}:{attribute_value}".strip(),
+            json=self._compile_api_request(resource_name, attributes),
+            **kwargs,
+        )
+
     def detail(self, resource_name: str, resource_id, **kwargs):
         """Gets an existing single resource.
 
         Args:
             resource_name (str): The resource name.
             resource_id: The resource ID to delete
             **kwargs: additional arguments to pass to the request.
@@ -337,15 +360,15 @@
             "/sessions",
             "Authentication failed",
             json=self._compile_api_request(
                 data_type="session",
                 attributes={
                     "username": username,
                     "password": password,
-                    "plane": SessionPlanes.control.value,
+                    "plane": igz_mgmt.constants.SessionPlanes.control.value,
                 },
             ),
         )
         self._set_auth(username=username, session=response.cookies.get("session"))
 
     def _set_auth(self, username: str, access_key: str = "", session: str = ""):
         if access_key and session:
@@ -356,31 +379,60 @@
         )
 
         if access_key:
             encoded_auth = f"{username}:{access_key}"
             base64_encoded_auth = base64.b64encode(encoded_auth.encode("utf-8")).decode(
                 "utf-8"
             )
-            self._client._headers["Authorization"] = f"Basic {base64_encoded_auth}"
+            self._client._headers[
+                igz_mgmt.constants._RequestHeaders.authorization_header
+            ] = f"Basic {base64_encoded_auth}"
         self._version = self._get_external_versions()
 
-    def _get_external_versions(self):
-        response = self._client.get(
-            "/external_versions",
-            "Failed to get external versions",
-        )
+    def _try_resolve_external_version(self, node):
         try:
+            # get external version via tunnel
+            response = self._client.get(
+                "/tunnel/{0}.version.0/external_versions/{0}".format(node),
+                "Failed to get external version from node {0}".format(node),
+                timeout=10,
+            )
             version = (
-                response.json().get("data", {})[0].get("attributes", {}).get("external")
+                response.json().get("data", {}).get("attributes", {}).get("external")
             )
             return semver.VersionInfo.parse(version).finalize_version()
-        except Exception:
+        except Exception as exc:
+            self._logger.debug_with(str(exc) or repr(exc))
             return None
 
+    def _get_external_versions(self):
+        # try to iterate over 3 nodes
+        for node in ["igz0", "igz1", "igz2"]:
+            external_version = self._try_resolve_external_version(node)
+            if external_version:
+                return external_version
+
+        # if got here, something is off
+        self._logger.info(
+            "Failed to resolve auto detect iguazio external version, use `client.version = x.y.z` for explicitness"
+        )
+
+        # oldest supported GA version
+        return self.__DEFAULT_EXTERNAL_VERSION_NUMBER
+
     @property
     def version(self) -> semver.VersionInfo:
         """Iguazio system version info.
 
         Returns:
             semver.VersionInfo: Iguazio version
         """
         return self._version
+
+    @version.setter
+    def version(self, value: semver.VersionInfo):
+        """Change Iguazio system version info.
+
+        Args:
+            value (semver.VersionInfo): Iguazio version
+        """
+        self._version = value
```

### Comparing `igz_mgmt-0.0.5/igz_mgmt/constants.py` & `igz_mgmt-0.0.6/igz_mgmt/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -156,22 +156,104 @@
     workload_medium = "igz-workload-medium"
     workload_high = "igz-workload-high"
     system_medium = "igz-system-medium"
     system_high = "igz-system-high"
     system_critical = "igz-system-critical"
 
 
-class AdminStatuses(_BaseEnumStr):
+class UserAdminStatuses(_BaseEnumStr):
     """Admin status types to disable/enable user."""
 
     up = "up"
     down = "down"
 
 
+class UserOperationalStatuses(_BaseEnumStr):
+    """User operational status types."""
+
+    up = "up"
+    deleting = "deleting"
+    down = "down"
+
+
 class JupyterAppServicePrebakedImage:
     """Jupyter app service images types."""
 
     gpu_cuda = "jupyter-gpu-cuda"
     """Full stack with GPU."""
 
     full_stack = "jupyter-all"
     """Full stack without GPU"""
+
+
+class EventSeverity(_BaseEnumStr):
+    """Severity types."""
+
+    unknown = "unknown"
+    debug = "debug"
+    info = "info"
+    warning = "warning"
+    major = "major"
+    critical = "critical"
+
+
+class EventClassification(_BaseEnumStr):
+    """Classification types.
+
+    mapping to zebo event classification.
+    """
+
+    unknown = "unknown"
+    hardware = "hw"
+    user_action = "ua"
+    background = "bg"
+    software = "sw"
+    sla = "sla"
+    capacity = "cap"
+    security = "sec"
+    audit = "audit"
+    system = "system"
+
+
+class EventVisibility(_BaseEnumStr):
+    """Visibility types."""
+
+    unknown = "unknown"
+    internal = "internal"
+    external = "external"
+    customer_only = "customerOnly"
+
+
+class ProjectAdminStatuses(_BaseEnumStr):
+    """Project admin status types."""
+
+    online = "online"
+    offline = "offline"
+    archived = "archived"
+
+
+class ProjectOperationalStatuses(_BaseEnumStr):
+    """Project operational status types."""
+
+    unknown = "unknown"
+    creating = "creating"
+    deleting = "deleting"
+    online = "online"
+    offline = "offline"
+    archived = "archived"
+
+
+class _RequestHeaders(_BaseEnumStr):
+    content_type_header = "Content-Type"
+    authorization_header = "Authorization"
+    projects_role_header = "x-projects-role"
+    deletion_strategy_header = "igz-project-deletion-strategy"
+
+
+class ProjectDeletionStrategies(_BaseEnumStr):
+    """Project deletion strategies types."""
+
+    restricted = "restricted"
+    """Restrict deletion if project has resources such as functions, runs, etc."""
+
+    cascading = "cascading"
+    """Delete the project with all resources"""
```

### Comparing `igz_mgmt-0.0.5/igz_mgmt/cruds.py` & `igz_mgmt-0.0.6/igz_mgmt/cruds.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 import http
 import typing
 
 import httpx
 import inflection
 import pydantic
 
-from igz_mgmt.client import APIClient
-from igz_mgmt.exceptions import ResourceNotFoundException
+import igz_mgmt.client
+import igz_mgmt.exceptions
 
 
 class ResourceListPagingQueryParams(pydantic.BaseModel):
     """List paging query params."""
 
     number: int = pydantic.Field(0, ge=0)
     size: int = pydantic.Field(50, ge=0)
@@ -46,45 +46,55 @@
             return _UserGroupCrud
         elif crud_type == "access_key":
             return _AccessKeyCrud
         elif crud_type == "job":
             return _JobCrud
         elif crud_type == "app_services_manifest":
             return _AppServicesManifestCrud
+        elif crud_type == "project":
+            return _ProjectCrud
         else:
             raise Exception("Unknown type")
 
 
 class _BaseCrud(abc.ABC):
     __ALLOW_GET_DETAIL__ = True
 
     @classmethod
-    def create(cls, http_client: APIClient, attributes, relationships=None):
-        return http_client.create(cls.type(), attributes, relationships)
+    def create(
+        cls,
+        http_client: igz_mgmt.client.APIClient,
+        attributes,
+        relationships=None,
+        **kwargs,
+    ):
+        return http_client.create(cls.type(), attributes, relationships, **kwargs)
 
     @classmethod
-    def get(cls, http_client: APIClient, resource_id, **kwargs):
+    def get(cls, http_client: igz_mgmt.client.APIClient, resource_id, **kwargs):
         # we do it for endpoints that don't really support get detail thought
         # they behave like they do (e.g. app services manifests)
         if not cls.__ALLOW_GET_DETAIL__:
             response_list = cls.list(http_client)
             return response_list[0]
 
         # get detail
         try:
             return http_client.detail(cls.type(), resource_id, **kwargs)
         except httpx.HTTPStatusError as exc:
             if exc.response.status_code == http.HTTPStatus.NOT_FOUND:
-                raise ResourceNotFoundException(cls.type(), resource_id) from exc
+                raise igz_mgmt.exceptions.ResourceNotFoundException(
+                    cls.type(), resource_id
+                ) from exc
             raise exc
 
     @classmethod
     def list(
         cls,
-        http_client: APIClient,
+        http_client: igz_mgmt.client.APIClient,
         filter_by: typing.Optional[typing.Mapping[str, str]] = None,
         sort_by: typing.Optional[typing.List[str]] = None,
         paging: typing.Optional[ResourceListPagingQueryParams] = None,
         include: typing.Optional[typing.List[str]] = None,
     ):
         params = {}
         if filter_by:
@@ -101,21 +111,31 @@
             # currently not needed. it simply returns the total number of items.
             # might be needed when we will add a dedicated pagination function
             # params["count"] = "records"
         return http_client.list(cls.type(), params=params)
 
     @classmethod
     def update(
-        cls, http_client: APIClient, resource_id, attributes, relationships=None
+        cls,
+        http_client: igz_mgmt.client.APIClient,
+        resource_id,
+        attributes,
+        relationships=None,
+        **kwargs,
     ):
-        return http_client.update(cls.type(), resource_id, attributes, relationships)
+        return http_client.update(
+            cls.type(), resource_id, attributes, relationships, **kwargs
+        )
 
     @classmethod
     def delete(
-        cls, http_client: APIClient, resource_id, ignore_missing: bool = False
+        cls,
+        http_client: igz_mgmt.client.APIClient,
+        resource_id,
+        ignore_missing: bool = False,
     ) -> typing.Optional[str]:
         response = http_client.delete(
             cls.type(), resource_id, ignore_missing=ignore_missing
         )
 
         # check if response is a job of "deletion_response" type
         if response.status_code == http.HTTPStatus.ACCEPTED:
@@ -128,15 +148,15 @@
                     .get("jobs", {})
                     .get("data", [])
                 )
                 if jobs_data:
                     return jobs_data[0].get("id", None)
 
     @classmethod
-    def get_custom(cls, http_client: APIClient, path, **kwargs):
+    def get_custom(cls, http_client: igz_mgmt.client.APIClient, path, **kwargs):
         return http_client.request("GET", path, **kwargs)
 
     @classmethod
     def type(cls):
         return inflection.underscore(cls.__name__.strip("_")).replace("_crud", "")
 
 
@@ -154,7 +174,11 @@
 
 class _JobCrud(_BaseCrud):
     pass
 
 
 class _AppServicesManifestCrud(_BaseCrud):
     __ALLOW_GET_DETAIL__ = False
+
+
+class _ProjectCrud(_BaseCrud):
+    pass
```

### Comparing `igz_mgmt-0.0.5/igz_mgmt/exceptions.py` & `igz_mgmt-0.0.6/igz_mgmt/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from http import HTTPStatus
+import http
 
 import inflection
 
 
 class ResourceDeleteException(Exception):
     """The resource is not delete-able."""
 
@@ -51,9 +51,9 @@
 
 
 class ResourceNotFoundException(Exception):
     """The resource is not found."""
 
     def __init__(self, resource, name_or_id):
         self.message = f"{inflection.humanize(resource)} {name_or_id} not found"
-        self.status_code = HTTPStatus.NOT_FOUND
+        self.status_code = http.HTTPStatus.NOT_FOUND
         super().__init__(self.message)
```

### Comparing `igz_mgmt-0.0.5/igz_mgmt/operations.py` & `igz_mgmt-0.0.6/igz_mgmt/operations.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,202 +17,237 @@
 Some endpoints within the management API are considered “operations”,
 which means that the response may not represent a resource.
 Some operations are long-living, which means a background job is created whereas the response will hold its id.
 """
 
 import typing
 
-from igz_mgmt.app_services import AppServiceBase, AppServiceSpec
-from igz_mgmt.client import APIClient
-from igz_mgmt.constants import AppServiceDesiredStates, ConfigTypes
-from igz_mgmt.exceptions import AppServiceNotExistsException
-from igz_mgmt.resources import AppServicesManifest, Job
+import igz_mgmt.client
+import igz_mgmt.constants
+import igz_mgmt.exceptions
+import igz_mgmt.resources
+import igz_mgmt.schemas.app_services
+import igz_mgmt.schemas.manual_events
 
 
 class ClusterConfigurations(object):
     """Cluster configuration operations."""
 
     @classmethod
-    def reload(cls, http_client: APIClient, config_type: ConfigTypes):
+    def reload(
+        cls,
+        http_client: igz_mgmt.client.APIClient,
+        config_type: igz_mgmt.constants.ConfigTypes,
+    ):
         """Cluster configuration reload.
 
         Args:
             http_client (APIClient): The client to use.
             config_type (ConfigTypes): The configuration type.
         """
         response = http_client.request(
             "POST", f"configurations/{config_type.value}/reloads"
         )
         job_id = response["data"]["id"]
-        Job.wait_for_completion(http_client, job_id, timeout=360)
+        igz_mgmt.Job.wait_for_completion(http_client, job_id, timeout=360)
+
+
+class ManualEvents(object):
+    """Manual event operations."""
+
+    @classmethod
+    def emit(
+        cls,
+        http_client: igz_mgmt.client.APIClient,
+        event: igz_mgmt.schemas.manual_events.ManualEventSchema,
+    ):
+        """Emits a manual event.
+
+        This operation requires system-admin role permissions.
+
+        Args:
+            http_client (APIClient): The client to use.
+            event (ManualEventSchema): The event to emit.
+        """
+        manual_event_request = {
+            "data": {
+                **igz_mgmt.schemas.manual_events.ManualEventRequest(
+                    attributes=event
+                ).dict(exclude_none=True)
+            }
+        }
+        http_client.request("POST", "manual_events", json=manual_event_request)
 
 
 class AppServices(object):
     """Syntactic sugar to AppServicesManifest class."""
 
     @classmethod
     def get(
         cls,
-        http_client: APIClient,
+        http_client: igz_mgmt.client.APIClient,
         app_service_spec_name: str,
-    ) -> typing.Optional[AppServiceBase]:
+    ) -> typing.Optional[igz_mgmt.schemas.app_services.AppServiceBase]:
         """Gets the app service that matches the given spec name.
 
         Args:
             http_client (APIClient): The client to use.
             app_service_spec_name (str): The name of the app service spec.
 
         Returns:
             AppServiceBase, optional: The app service instance that matches the given spec name.
         """
-        app_services_manifest = AppServicesManifest.get(http_client)
+        app_services_manifest = igz_mgmt.resources.AppServicesManifest.get(http_client)
         return app_services_manifest.resolve_service(app_service_spec_name)
 
     @classmethod
     def create_or_update(
         cls,
-        http_client: APIClient,
-        app_service: typing.Union[AppServiceSpec, AppServiceBase],
+        http_client: igz_mgmt.client.APIClient,
+        app_service: typing.Union[
+            igz_mgmt.schemas.app_services.AppServiceSpec,
+            igz_mgmt.schemas.app_services.AppServiceBase,
+        ],
         wait_for_completion=True,
-    ) -> typing.Optional[Job]:
+    ) -> typing.Optional[igz_mgmt.resources.Job]:
         """Creates or updates an app service.
 
         Args:
             http_client (APIClient): The client to use.
             app_service (AppServiceSpec or AppServiceBase): app service to create or update.
             wait_for_completion (bool): Whether to wait for the job to complete.
 
         Returns:
             Job, optional: The job that was created or None if wait_for_completion is False
         """
-        app_services_manifest = AppServicesManifest.get(http_client)
+        app_services_manifest = igz_mgmt.resources.AppServicesManifest.get(http_client)
         return app_services_manifest.create_or_update(
             http_client, app_service, wait_for_completion
         )
 
     @classmethod
     def restart(
         cls,
-        http_client: APIClient,
+        http_client: igz_mgmt.client.APIClient,
         app_service_spec_name: str,
         wait_for_completion=True,
-    ) -> typing.Optional[Job]:
+    ) -> typing.Optional[igz_mgmt.resources.Job]:
         """Restarts an app service.
 
         Args:
             http_client (APIClient): The client to use.
             app_service_spec_name (str): Name of the app service to restart.
             wait_for_completion (bool): Whether to wait for the job to complete.
 
         Returns:
             Job, optional: The job that was created or None if wait_for_completion is False
         """
-        app_services_manifest = AppServicesManifest.get(http_client)
+        app_services_manifest = igz_mgmt.resources.AppServicesManifest.get(http_client)
         return app_services_manifest.restart(
             http_client, app_service_spec_name, wait_for_completion
         )
 
     @classmethod
     def remove(
         cls,
-        http_client: APIClient,
+        http_client: igz_mgmt.client.APIClient,
         app_service_spec_name: str,
         wait_for_completion=True,
-    ) -> typing.Optional[Job]:
+    ) -> typing.Optional[igz_mgmt.resources.Job]:
         """Removes an app service.
 
         Args:
             http_client (APIClient): The client to use.
             app_service_spec_name (str): Name of the app service to remove.
             wait_for_completion (bool): Whether to wait for the job to complete.
 
         Returns:
             Job, optional: The job that was created or None if wait_for_completion is False
         """
-        app_services_manifest = AppServicesManifest.get(http_client)
+        app_services_manifest = igz_mgmt.resources.AppServicesManifest.get(http_client)
         return app_services_manifest.remove_service(
             http_client, app_service_spec_name, wait_for_completion
         )
 
     @classmethod
     def enable(
         cls,
-        http_client: APIClient,
+        http_client: igz_mgmt.client.APIClient,
         app_service_spec_name: str,
         wait_for_completion=True,
-    ) -> typing.Optional[Job]:
+    ) -> typing.Optional[igz_mgmt.resources.Job]:
         """Enables an app service.
 
         Args:
             http_client (APIClient): The client to use.
             app_service_spec_name (str): Name of the app service to enable.
             wait_for_completion (bool): Whether to wait for the job to complete.
 
         Returns:
             Job, optional: The job that was created or None if wait_for_completion is False
         """
         return cls._change_service_state(
             http_client,
             app_service_spec_name,
-            AppServiceDesiredStates.ready,
+            igz_mgmt.constants.AppServiceDesiredStates.ready,
             wait_for_completion,
         )
 
     @classmethod
     def disable(
         cls,
-        http_client: APIClient,
+        http_client: igz_mgmt.client.APIClient,
         app_service_spec_name: str,
         wait_for_completion=True,
-    ) -> typing.Optional[Job]:
+    ) -> typing.Optional[igz_mgmt.resources.Job]:
         """Disables an app service.
 
         Args:
             http_client (APIClient): The client to use.
             app_service_spec_name (str): Name of the app service to disable.
             wait_for_completion (bool): Whether to wait for the job to complete.
 
         Returns:
             Job, optional: The job that was created or None if wait_for_completion is False
         """
         return cls._change_service_state(
             http_client,
             app_service_spec_name,
-            AppServiceDesiredStates.disabled,
+            igz_mgmt.constants.AppServiceDesiredStates.disabled,
             wait_for_completion,
         )
 
     @classmethod
     def scale_from_zero(
         cls,
-        http_client: APIClient,
+        http_client: igz_mgmt.client.APIClient,
         app_service_spec_name: str,
         wait_for_completion=True,
-    ) -> typing.Optional[Job]:
+    ) -> typing.Optional[igz_mgmt.resources.Job]:
         """Scales an app service from zero.
 
         Args:
             http_client (APIClient): The client to use.
             app_service_spec_name (str): Name of the app service to scale from zero.
             wait_for_completion (bool): Whether to wait for the job to complete.
 
         Returns:
             Job, optional: The job that was created or None if wait_for_completion is False
         """
-        app_services_manifest = AppServicesManifest.get(http_client)
+        app_services_manifest = igz_mgmt.resources.AppServicesManifest.get(http_client)
         return app_services_manifest.scale_from_zero(
             http_client, app_service_spec_name, wait_for_completion
         )
 
     @classmethod
     def _change_service_state(
         cls,
-        http_client: APIClient,
+        http_client: igz_mgmt.client.APIClient,
         app_service_spec_name: str,
-        service_state: AppServiceDesiredStates,
+        service_state: igz_mgmt.constants.AppServiceDesiredStates,
         wait_for_completion=True,
     ):
         """Changes an app service desired state.
 
         Args:
             http_client (APIClient): The client to use.
             app_service_spec_name (str): Name of the app service.
@@ -221,15 +256,17 @@
 
         Returns:
             Job, optional: The job that was created or None if wait_for_completion is False
 
         Raises:
             AppServiceNotExistsException: If app service not exists
         """
-        app_services_manifest = AppServicesManifest.get(http_client)
+        app_services_manifest = igz_mgmt.resources.AppServicesManifest.get(http_client)
         app_service_base = app_services_manifest.resolve_service(app_service_spec_name)
         if not app_service_base:
-            raise AppServiceNotExistsException(name=app_service_spec_name)
+            raise igz_mgmt.exceptions.AppServiceNotExistsException(
+                name=app_service_spec_name
+            )
         app_service_base.spec.desired_state = service_state
         return app_services_manifest.create_or_update(
             http_client, app_service_base, wait_for_completion
         )
```

### Comparing `igz_mgmt-0.0.5/igz_mgmt/resources.py` & `igz_mgmt-0.0.6/igz_mgmt/resources.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,61 +13,41 @@
 # limitations under the License.
 #
 """This module represents resources.
 
 Most of the resources support all CRUD methods.
 """
 import collections
+import contextlib
+import http
 import json
 import time
 import typing
-from contextlib import contextmanager
 
 import inflection
-import pydantic
+import pydantic.utils
 import semver
-from pydantic import SecretStr
-from pydantic.utils import GetterDict
 
-from igz_mgmt.app_services import AppServiceBase, AppServiceSpec
-from igz_mgmt.client import APIClient
-from igz_mgmt.common.helpers import (
-    RetryUntilSuccessfulFatalError,
-    RetryUntilSuccessfulInProgressErrorMessage,
-    retry_until_successful,
-)
-from igz_mgmt.constants import (
-    AdminStatuses,
-    ApplyServicesMode,
-    AppServiceDesiredStates,
-    AppServicesManifestStates,
-    ForceApplyAllMode,
-    JobStates,
-    SessionPlanes,
-    TenantManagementRoles,
-)
-from igz_mgmt.cruds import ResourceListPagingQueryParams, _BaseCrud, _CrudFactory
-from igz_mgmt.exceptions import (
-    AppServiceNotExistsException,
-    ResourceDeleteException,
-    ResourceListException,
-    ResourceNotFoundException,
-    ResourceUpdateException,
-)
+import igz_mgmt.client
+import igz_mgmt.common.helpers
+import igz_mgmt.constants
+import igz_mgmt.cruds
+import igz_mgmt.exceptions
+import igz_mgmt.schemas.app_services
 
 
 class BaseResource(pydantic.BaseModel):
     """Base resource contains common attributes and methods for resources in the system."""
 
     type: str
     id: typing.Optional[typing.Union[int, str]]
     relationships: typing.Optional[dict]
 
     class Config:
-        class _BaseGetter(GetterDict):
+        class _BaseGetter(pydantic.utils.GetterDict):
             def get(self, key: typing.Any, default: typing.Any = None) -> typing.Any:
                 if key in ["id", "type"]:
                     return self._obj["data"][key]
                 elif key == "relationships":
                     return self._obj["data"].get("relationships", {})
                 elif key in self._obj["data"]["attributes"]:
                     return self._obj["data"]["attributes"][key]
@@ -80,15 +60,15 @@
 
         # be forward compatible
         extra = "allow"
 
     @classmethod
     def get(
         cls,
-        http_client: APIClient,
+        http_client: igz_mgmt.client.APIClient,
         resource_id: typing.Union[int, str],
         include: typing.Optional[typing.List[str]] = None,
     ) -> "BaseResource":
         """Gets the resource record.
 
         Args:
             http_client (APIClient): The client to use.
@@ -103,18 +83,18 @@
             params["include"] = ",".join(include)
         resource = cls._get_crud().get(http_client, resource_id, params=params)
         return cls.from_orm(resource)
 
     @classmethod
     def list(
         cls,
-        http_client: APIClient,
+        http_client: igz_mgmt.client.APIClient,
         filter_by: typing.Optional[typing.Mapping[str, str]] = None,
         sort_by: typing.Optional[typing.List[str]] = None,
-        paging: typing.Optional[ResourceListPagingQueryParams] = None,
+        paging: typing.Optional[igz_mgmt.cruds.ResourceListPagingQueryParams] = None,
         include: typing.Optional[typing.List[str]] = None,
     ) -> typing.List["BaseResource"]:
         """Lists resource records.
 
         Args:
             http_client (APIClient): The client to use.
             filter_by (typing.Mapping[str, str], optional): Filter by field values. None by default.
@@ -130,76 +110,87 @@
             http_client, filter_by, sort_by, paging, include
         )
         return [
             cls.from_orm({"data": item, "included": item.get("included", [])})
             for item in list_resource["data"]
         ]
 
-    def update(self, http_client: APIClient, relationships=None) -> "BaseResource":
+    def update(
+        self, http_client: igz_mgmt.client.APIClient, relationships=None, **kwargs
+    ) -> "BaseResource":
         """Updates resource record.
 
         Args:
             http_client (APIClient): The client to use.
             relationships (optional): The resource relationships. None by default.
+            **kwargs: additional arguments to pass to the request.
 
         Returns:
             BaseResource: The updated record.
         """
         self._get_crud().update(
             http_client,
             self.id,
             attributes=self._fields_to_attributes(),
             relationships=relationships,
+            **kwargs,
         )
 
         # TODO: build cls from response when BE will return the updated resource within the response body
         updated_resource = self.get(http_client, self.id)
         self.__dict__.update(updated_resource)
         return self
 
     def delete(
         self,
-        http_client: APIClient,
+        http_client: igz_mgmt.client.APIClient,
         ignore_missing: bool = False,
         wait_for_job_deletion: bool = True,
-    ):
+    ) -> typing.Optional["Job"]:
         """Deletes resource record.
 
         Args:
             http_client (APIClient): The client to use.
             ignore_missing (bool, optional): When True, don't raise an exception in case the record does not exist.
             False by default.
             wait_for_job_deletion (bool, optional): Whether to wait for the job to complete. True by default.
+
+        Returns:
+            Job, optional: the job that was created or None.
         """
         job_id = self._get_crud().delete(http_client, self.id, ignore_missing)
-        if job_id and wait_for_job_deletion:
-            Job.wait_for_completion(
-                http_client, job_id, job_completion_retry_interval=10
-            )
+        if job_id:
+            if wait_for_job_deletion:
+                Job.wait_for_completion(
+                    http_client, job_id, job_completion_retry_interval=10
+                )
+            return Job.get(http_client, job_id)
 
     @classmethod
-    def _get_crud(cls) -> _BaseCrud:
-        return _CrudFactory.create(
+    def _get_crud(cls) -> igz_mgmt.cruds._BaseCrud:
+        return igz_mgmt.cruds._CrudFactory.create(
             inflection.underscore(cls.__fields__["type"].default)
         )
 
     @classmethod
     def _get_resource_by_name(
-        cls, http_client: APIClient, filter_key, name, include=None
+        cls, http_client: igz_mgmt.client.APIClient, filter_key, name, include=None
     ) -> "BaseResource":
         """Gets a resource by name, by listing all resource instances and filtering by name.
 
         If resource is not found, ResourceNotFoundException is raised
         """
         resources = cls.list(http_client, filter_by={filter_key: name})
         if not resources:
-            raise ResourceNotFoundException(cls.__fields__["type"].default, name)
+            raise igz_mgmt.exceptions.ResourceNotFoundException(
+                cls.__fields__["type"].default, name
+            )
         resource_id = resources[0].id
 
-        # although we already have the user, we need to get it again to get the relationships
+        # although we already have the resource, we need to get it again to get the relationships
         # passed in the include parameter
         return cls.get(http_client, resource_id, include=include)
 
     def _fields_to_attributes(self, exclude_unset=True):
         return self.dict(
             exclude={"type", "relationships", "id"},
             exclude_none=True,
@@ -217,61 +208,82 @@
     last_name: str = ""
     email: str = ""
     uid: int = 0
     created_at: str = ""
     data_access_mode: str = ""
     authentication_scheme: str = ""
     send_password_on_creation: bool = False
-    assigned_policies: typing.List[TenantManagementRoles] = []
-    operational_status: str = ""
-    admin_status: str = AdminStatuses.up
-    password: SecretStr = None
+    assigned_policies: typing.List[igz_mgmt.constants.TenantManagementRoles] = []
+    operational_status: str = igz_mgmt.constants.UserOperationalStatuses.up
+    admin_status: str = igz_mgmt.constants.UserAdminStatuses.up
+    password: pydantic.SecretStr = None
+    phone_number: str = ""
+    job_title: str = ""
+    department: str = ""
+    last_activity: str = ""
 
     @classmethod
     def create(
         cls,
-        http_client: APIClient,
+        http_client: igz_mgmt.client.APIClient,
         username: str,
-        password: str,
         email: str,
         first_name: str,
         last_name: str,
+        password: str = None,
         uid: int = None,
-        assigned_policies: typing.List[TenantManagementRoles] = None,
+        assigned_policies: typing.List[igz_mgmt.constants.TenantManagementRoles] = None,
         primary_group: typing.Union[str, "Group", None] = None,
         groups: typing.Union[typing.List[str], typing.List["Group"], None] = None,
+        timeout: int = 30,
+        wait_for_completion=True,
+        phone_number: str = "",
+        job_title: str = "",
+        department: str = "",
     ) -> "User":
         """Creates a new User.
 
         Args:
             http_client (APIClient): The client to use.
             username (str): The user username.
+            password (str, optional): The user password. None by default. (if not provided, an email is automatically
+            sent to the user to set his password)
             assigned_policies (typing.List[TenantManagementRoles], optional): The assigned policies of the group.
             None by default.
             primary_group (str or Group or None): None by default.
             groups (typing.Union[typing.List[str], typing.List["Group"], None], optional): A list of group objects
             or group ids to add user to the groups. None by default.
+            timeout (int, optional): The default is 30.
+            wait_for_completion (bool): Whether to wait for the job to complete
+            phone_number (str, optional): The user phone number.
+            job_title (str, optional): The user job title.
+            department (str, optional): The user department.
 
         Returns:
             User
         """
         assigned_policies = assigned_policies or [
-            TenantManagementRoles.developer.value,
-            TenantManagementRoles.application_read_only.value,
+            igz_mgmt.constants.TenantManagementRoles.developer.value,
+            igz_mgmt.constants.TenantManagementRoles.application_read_only.value,
         ]
         attributes = {
             "username": username,
             "first_name": first_name,
             "last_name": last_name,
             "email": email,
-            "password": password,
             "assigned_policies": assigned_policies,
+            "phone_number": phone_number,
+            "job_title": job_title,
+            "department": department,
         }
-        if uid:
+        if uid is not None:
             attributes["uid"] = uid
+        if password is not None:
+            attributes["password"] = password
+
         relationships = collections.defaultdict(dict)
         if primary_group:
             primary_group_id = (
                 primary_group.id if isinstance(primary_group, Group) else primary_group
             )
             relationships["primary_group"] = {
                 "data": {
@@ -303,19 +315,74 @@
                 )
 
         created_resource = cls._get_crud().create(
             http_client,
             attributes=attributes,
             relationships=relationships,
         )
-        return cls.from_orm(created_resource)
+
+        # there might be jobs handling the creating
+        jobs_data = (
+            created_resource.get("data", {})
+            .get("relationships", {})
+            .get("jobs", {})
+            .get("data", [])
+        )
+        if jobs_data and wait_for_completion:
+            job_id = jobs_data[0].get("id", None)
+            Job.wait_for_completion(
+                http_client, job_id, job_completion_retry_interval=10
+            )
+
+        def _verify_user_is_operational(user_id):
+            user_obj = User.get(http_client, user_id, include=["user_groups"])
+            if not user_obj.is_operational(http_client):
+                http_client._logger.warn_with("User is not yet operational, retrying")
+
+                raise igz_mgmt.common.helpers.RetryUntilSuccessfulInProgressErrorMessage(
+                    "Waiting for the user to be operational",
+                )
+            return user_obj
+
+        user = cls.from_orm(created_resource)
+
+        user = igz_mgmt.common.helpers.retry_until_successful(
+            1,
+            timeout,
+            http_client._logger,
+            True,
+            _verify_user_is_operational,
+            user_id=user.id,
+        )
+        return user
+
+    def is_operational(self, http_client: igz_mgmt.client.APIClient):
+        """Verify user is operational.
+
+        Verifying that the user operational status is up and that the all_users group
+        exists in the user_groups relationships.
+
+        Args:
+            http_client (APIClient): The client to use.
+
+        Returns:
+            bool: True if user is operational, False otherwise.
+        """
+        if self.operational_status == igz_mgmt.constants.UserOperationalStatuses.up:
+            # check that all_users group exists in the user_groups relationships
+            if "user_groups" in self.relationships:
+                all_users_group = Group.get_by_name(http_client, "all_users")
+                for relationship_group in self.relationships["user_groups"]["data"]:
+                    if relationship_group["id"] == all_users_group.id:
+                        return True
+        return False
 
     @classmethod
     def get_by_username(
-        cls, http_client: APIClient, username: str, include=None
+        cls, http_client: igz_mgmt.client.APIClient, username: str, include=None
     ) -> "User":
         """A convenience method to get a user by username.
 
         Args:
             http_client (APIClient): The client to use.
             username (str): The user username.
             include (optional): Include related resources. None by default.
@@ -327,27 +394,29 @@
             ResourceNotFoundException: If user is not found
         """
         return cls._get_resource_by_name(
             http_client, "username", username, include=include
         )
 
     @classmethod
-    def self(cls, http_client: APIClient) -> "User":
+    def self(cls, http_client: igz_mgmt.client.APIClient) -> "User":
         """Gets the current user.
 
         Args:
             http_client (APIClient): The client to use.
 
         Returns:
             User: The current user instance.
         """
         user = cls._get_crud().get_custom(http_client, "self")
         return cls.from_orm(user)
 
-    def add_to_group(self, http_client: APIClient, group: typing.Union[str, "Group"]):
+    def add_to_group(
+        self, http_client: igz_mgmt.client.APIClient, group: typing.Union[str, "Group"]
+    ):
         """Adds a user to a group.
 
         1. get the user
         2. add the group to the user
         3. update the user
 
         Args:
@@ -359,15 +428,15 @@
             user.relationships["user_groups"] = {"data": []}
 
         group_id = group.id if isinstance(group, Group) else group
         if User._ensure_user_in_group(user, group_id):
             user.update(http_client, relationships=user.relationships)
 
     def remove_from_group(
-        self, http_client: APIClient, group: typing.Union[str, "Group"]
+        self, http_client: igz_mgmt.client.APIClient, group: typing.Union[str, "Group"]
     ):
         """Removes a user from a group.
 
         Args:
             http_client (APIClient): The client to use.
             group (str or Group): The group id or group instance to remove user from it.
         """
@@ -378,15 +447,15 @@
                 group
                 for group in user.relationships["user_groups"]["data"]
                 if group["id"] != group_id
             ]
             user.update(http_client, relationships=user.relationships)
 
     def set_primary_group(
-        self, http_client: APIClient, group: typing.Union[str, "Group"]
+        self, http_client: igz_mgmt.client.APIClient, group: typing.Union[str, "Group"]
     ):
         """Sets the primary group of a user.
 
         Args:
             http_client (APIClient): The client to use.
             group (str or Group): The primary group id or group instance.
         """
@@ -402,67 +471,67 @@
         User._ensure_user_in_group(user, group_id)
         user.relationships["primary_group"]["data"] = {
             "id": group_id,
             "type": "user_group",
         }
         user.update(http_client, relationships=user.relationships)
 
-    def disable(self, http_client: APIClient):
+    def disable(self, http_client: igz_mgmt.client.APIClient):
         """Disables the user instance.
 
         Args:
             http_client (APIClient): The client to use.
         """
-        self.admin_status = AdminStatuses.down
+        self.admin_status = igz_mgmt.constants.UserAdminStatuses.down
         return self.update(http_client)
 
     @classmethod
-    def disable_by_username(cls, http_client: APIClient, username: str):
+    def disable_by_username(cls, http_client: igz_mgmt.client.APIClient, username: str):
         """Disables the user by username.
 
         Args:
             http_client (APIClient): The client to use.
             username (str): The user username.
         """
         user = cls.get_by_username(http_client, username)
         return user.disable(http_client)
 
     @classmethod
-    def disable_by_id(cls, http_client: APIClient, user_id: str):
+    def disable_by_id(cls, http_client: igz_mgmt.client.APIClient, user_id: str):
         """Disables the user by user id.
 
         Args:
             http_client (APIClient): The client to use.
             user_id (str): The user id.
         """
         user = cls.get(http_client, user_id)
         return user.disable(http_client)
 
-    def enable(self, http_client: APIClient):
+    def enable(self, http_client: igz_mgmt.client.APIClient):
         """Enables the user instance.
 
         Args:
             http_client (APIClient): The client to use.
         """
-        self.admin_status = AdminStatuses.up
+        self.admin_status = igz_mgmt.constants.UserAdminStatuses.up
         return self.update(http_client)
 
     @classmethod
-    def enable_by_username(cls, http_client: APIClient, username: str):
+    def enable_by_username(cls, http_client: igz_mgmt.client.APIClient, username: str):
         """Enables the user by username.
 
         Args:
             http_client (APIClient): The client to use.
             username (str): The user username.
         """
         user = cls.get_by_username(http_client, username)
         return user.enable(http_client)
 
     @classmethod
-    def enable_by_id(cls, http_client: APIClient, user_id: str):
+    def enable_by_id(cls, http_client: igz_mgmt.client.APIClient, user_id: str):
         """Enables the user by user id.
 
         Args:
             http_client (APIClient): The client to use.
             user_id (str): The user id.
         """
         user = cls.get(http_client, user_id)
@@ -495,23 +564,25 @@
 
     type: str = "user_group"
     name: str = ""
     description: str = None
     data_access_mode: str = "enabled"
     gid: int = 0
     kind: str = "local"
-    assigned_policies: typing.List[TenantManagementRoles] = []
+    assigned_policies: typing.List[igz_mgmt.constants.TenantManagementRoles] = []
     system_provided: bool = False
 
     @classmethod
     def create(
         cls,
-        http_client: APIClient,
+        http_client: igz_mgmt.client.APIClient,
         name: typing.Optional[str],
-        assigned_policies: typing.Optional[typing.List[TenantManagementRoles]] = None,
+        assigned_policies: typing.Optional[
+            typing.List[igz_mgmt.constants.TenantManagementRoles]
+        ] = None,
         description: typing.Optional[str] = None,
         gid: typing.Optional[int] = None,
         users: typing.Optional[typing.List[typing.Union[int, str, User]]] = None,
     ) -> "Group":
         """Creates a new group.
 
         Args:
@@ -525,16 +596,16 @@
             to add to the group. None by default.
 
         Returns:
             Group
         """
         if not assigned_policies:
             assigned_policies = [
-                TenantManagementRoles.data.value,
-                TenantManagementRoles.application_admin.value,
+                igz_mgmt.constants.TenantManagementRoles.data.value,
+                igz_mgmt.constants.TenantManagementRoles.application_admin.value,
             ]
         relationships = {}
         if users:
             relationships["users"] = {
                 "data": [
                     {"id": user.id if isinstance(user, User) else user, "type": "user"}
                     for user in users
@@ -549,15 +620,17 @@
                 "assigned_policies": assigned_policies,
             },
             relationships=relationships,
         )
         return cls.from_orm(created_resource)
 
     @classmethod
-    def get_by_name(cls, http_client: APIClient, name: str, include=None) -> "Group":
+    def get_by_name(
+        cls, http_client: igz_mgmt.client.APIClient, name: str, include=None
+    ) -> "Group":
         """A convenience method to get a group by name.
 
         Args:
             http_client (APIClient): The client to use.
             name (str): Group name.
             include (optional): Include related resources. None by default.
 
@@ -565,15 +638,19 @@
             Group: The group instance by group name.
 
         Raises:
             ResourceNotFoundException: If group is not found
         """
         return cls._get_resource_by_name(http_client, "name", name, include=include)
 
-    def add_user(self, http_client: APIClient, user: typing.Union[str, int, "User"]):
+    def add_user(
+        self,
+        http_client: igz_mgmt.client.APIClient,
+        user: typing.Union[str, int, "User"],
+    ):
         """Adds a user to group.
 
         1. get the user
         2. add the group to the user
         3. update the group
 
         Args:
@@ -581,15 +658,19 @@
             user (str or int or User): The user id or user instance to add.
         """
         if not isinstance(user, User):
             user = User.get(http_client, user)
         user.add_to_group(http_client, self)
         self.__dict__.update(Group.get(http_client, self.id))
 
-    def remove_user(self, http_client: APIClient, user: typing.Union[str, int, "User"]):
+    def remove_user(
+        self,
+        http_client: igz_mgmt.client.APIClient,
+        user: typing.Union[str, int, "User"],
+    ):
         """Removes a user from group.
 
         Args:
             http_client (APIClient): The client to use.
             user (str ot int or User): The user id or user instance to remove.
         """
         if not isinstance(user, User):
@@ -609,21 +690,25 @@
     group_ids: typing.List[str] = []
     uid: int = 0
     gids: typing.List[int] = []
     expires_at: int = 0  # EPOCH
     interface_kind: str = "web"
     label: str = ""
     kind: str = "accessKey"
-    planes: typing.List[SessionPlanes] = SessionPlanes.all()
+    planes: typing.List[
+        igz_mgmt.constants.SessionPlanes
+    ] = igz_mgmt.constants.SessionPlanes.all()
 
     @classmethod
     def create(
         cls,
-        http_client: APIClient,
-        planes: typing.List[SessionPlanes] = SessionPlanes.all(),
+        http_client: igz_mgmt.client.APIClient,
+        planes: typing.List[
+            igz_mgmt.constants.SessionPlanes
+        ] = igz_mgmt.constants.SessionPlanes.all(),
         label: str = None,
     ):
         """Creates a new access key.
 
         Args:
             http_client (APIClient): The client to use.
             planes (typing.List[SessionPlanes], optional): The planes of the access key.
@@ -648,34 +733,36 @@
 
     type: str = "job"
     kind: str = ""
     params: str = ""
     max_total_execution_time: int = 3 * 60 * 60  # in seconds
     max_worker_execution_time: typing.Optional[int] = None  # in seconds
     delay: float = 0  # in seconds
-    state: JobStates = JobStates.created
+    state: igz_mgmt.constants.JobStates = igz_mgmt.constants.JobStates.created
     result: str = ""
     created_at: str = ""
     on_success: typing.List[dict] = None
     on_failure: typing.List[dict] = None
     updated_at: str = ""
     handler: str = ""
     ctx_id: str = ""
 
-    def delete(self, http_client: APIClient, **kwargs):
+    def delete(
+        self, http_client: igz_mgmt.client.APIClient, **kwargs
+    ) -> typing.Optional["Job"]:
         """This method is forbidden."""
-        raise ResourceDeleteException
+        raise igz_mgmt.exceptions.ResourceDeleteException
 
-    def update(self, http_client: APIClient, **kwargs):
+    def update(self, http_client: igz_mgmt.client.APIClient, **kwargs):
         """This method is forbidden."""
-        raise ResourceUpdateException
+        raise igz_mgmt.exceptions.ResourceUpdateException
 
     @staticmethod
     def wait_for_completion(
-        http_client: APIClient,
+        http_client: igz_mgmt.client.APIClient,
         job_id: str,
         job_completion_retry_interval: float = 30,
         timeout: int = 3600,
     ):
         """Wait for a job to be finished.
 
         Args:
@@ -684,46 +771,46 @@
             job_completion_retry_interval (float, optional): The default is 30.
             timeout (int, optional): The default is 3600.
         """
 
         def _verify_job_in_terminal_state():
             try:
                 job_obj = Job.get(http_client, job_id)
-            except ResourceNotFoundException as exc:
+            except igz_mgmt.exceptions.ResourceNotFoundException as exc:
                 http_client._logger.warn_with(
                     "Job not found, bail out",
                     job_id=job_id,
                 )
-                raise RetryUntilSuccessfulFatalError(
+                raise igz_mgmt.common.helpers.RetryUntilSuccessfulFatalError(
                     "Resource was not found", caused_by_exc=exc
                 )
-            if job_obj.state not in JobStates.terminal_states():
+            if job_obj.state not in igz_mgmt.constants.JobStates.terminal_states():
                 http_client._logger.info_with(
                     "Job is not in a terminal state yet, retrying",
                     current_state=job_obj.state,
                     job_id=job_id,
                 )
-                raise RetryUntilSuccessfulInProgressErrorMessage(
+                raise igz_mgmt.common.helpers.RetryUntilSuccessfulInProgressErrorMessage(
                     "Waiting for job completion",
                     variables={
                         "job_id": job_id,
                         "job_state": job_obj.state,
                     },
                 )
             return job_obj
 
         http_client._logger.info_with("Waiting for job completion", job_id=job_id)
-        job = retry_until_successful(
+        job = igz_mgmt.common.helpers.retry_until_successful(
             job_completion_retry_interval,
             timeout,
             http_client._logger,
             True,
             _verify_job_in_terminal_state,
         )
-        if job.state != JobStates.completed:
+        if job.state != igz_mgmt.constants.JobStates.completed:
             error_message = f"Job {job_id} failed with state: {job.state}"
             try:
                 parsed_result = json.loads(job.result)
                 error_message += f", message: {parsed_result['message']}"
                 # status is optional
                 if "status" in parsed_result:
                     status_code = int(parsed_result["status"])
@@ -739,29 +826,29 @@
 class AppServicesManifest(BaseResource):
     """AppServicesManifest resource."""
 
     type: str = "app_services_manifest"
     cluster_name: str = ""
     tenant_name: str = ""
     tenant_id: str = ""
-    app_services: typing.List[AppServiceBase] = []
-    state: typing.Optional[AppServicesManifestStates]
+    app_services: typing.List[igz_mgmt.schemas.app_services.AppServiceBase] = []
+    state: typing.Optional[igz_mgmt.constants.AppServicesManifestStates]
     last_error: typing.Optional[str]
     last_modification_job: str = ""
-    apply_services_mode: typing.Optional[ApplyServicesMode]
+    apply_services_mode: typing.Optional[igz_mgmt.constants.ApplyServicesMode]
     running_modification_job: str = ""
-    force_apply_all_mode: typing.Optional[ForceApplyAllMode]
+    force_apply_all_mode: typing.Optional[igz_mgmt.constants.ForceApplyAllMode]
 
     _skip_apply: bool = False
 
     @staticmethod
-    @contextmanager
+    @contextlib.contextmanager
     def apply_services(
-        http_client: APIClient,
-        force_apply_all_mode: ForceApplyAllMode = ForceApplyAllMode.disabled,
+        http_client: igz_mgmt.client.APIClient,
+        force_apply_all_mode: igz_mgmt.constants.ForceApplyAllMode = igz_mgmt.constants.ForceApplyAllMode.disabled,
     ):
         """A context manager to apply services with multiple changes at once.
 
         Args:
             http_client (APIClient): The client to use.
             force_apply_all_mode (ForceApplyAllMode, optional): Disabled by default.
 
@@ -777,52 +864,56 @@
                 http_client,
                 # writing it down here for explicitness
                 wait_for_completion=True,
                 force_apply_all_mode=force_apply_all_mode,
             )
             app_services_manifest._skip_apply = False
 
-    def delete(self, http_client: APIClient, **kwargs):
+    def delete(
+        self, http_client: igz_mgmt.client.APIClient, **kwargs
+    ) -> typing.Optional[Job]:
         """This method is forbidden."""
-        raise ResourceDeleteException
+        raise igz_mgmt.exceptions.ResourceDeleteException
 
-    def update(self, http_client: APIClient, **kwargs):
+    def update(self, http_client: igz_mgmt.client.APIClient, **kwargs):
         """This method is forbidden."""
-        raise ResourceUpdateException
+        raise igz_mgmt.exceptions.ResourceUpdateException
 
-    def list(self, http_client: APIClient, **kwargs):
+    def list(self, http_client: igz_mgmt.client.APIClient, **kwargs):
         """This method is forbidden."""
-        raise ResourceListException
+        raise igz_mgmt.exceptions.ResourceListException
 
     @classmethod
-    def get(cls, http_client: APIClient, **kwargs) -> "AppServicesManifest":
+    def get(
+        cls, http_client: igz_mgmt.client.APIClient, **kwargs
+    ) -> "AppServicesManifest":
         """Gets the app services manifest from the API.
 
         Args:
             http_client (APIClient): The client to use.
             **kwargs: Arbitrary keyword arguments (not in used).
 
         Returns:
             AppServicesManifest: The app service manifest instance.
         """
         resource = cls._get_crud().list(http_client)
         return [cls.from_orm({"data": item}) for item in resource["data"]][0]
 
-    def set_apply_mode(self, apply_mode: ApplyServicesMode):
+    def set_apply_mode(self, apply_mode: igz_mgmt.constants.ApplyServicesMode):
         """Sets the apply mode of the app services manifest.
 
         Args:
             apply_mode (ApplyServicesMode): apply services mode value.
         """
         self.apply_services_mode = apply_mode
 
     def resolve_service(
         self,
         app_service_spec_name: str,
-    ) -> typing.Optional[AppServiceBase]:
+    ) -> typing.Optional[igz_mgmt.schemas.app_services.AppServiceBase]:
         """Gets the app service that matches the given spec name.
 
         Args:
             app_service_spec_name (str): The name of the app service spec.
 
         Returns:
             AppServiceBase, optional: The app service instance that matches the given spec name.
@@ -830,46 +921,53 @@
         for app_service in self.app_services:
             if app_service.spec.name == app_service_spec_name:
                 return app_service
         return None
 
     def create_or_update(
         self,
-        http_client: APIClient,
-        app_service: typing.Union[AppServiceSpec, AppServiceBase],
+        http_client: igz_mgmt.client.APIClient,
+        app_service: typing.Union[
+            igz_mgmt.schemas.app_services.AppServiceSpec,
+            igz_mgmt.schemas.app_services.AppServiceBase,
+        ],
         wait_for_completion=True,
     ) -> typing.Optional[Job]:
         """Creates or updates an app service.
 
         Args:
             http_client (APIClient): The client to use.
             app_service (AppServiceSpec or AppServiceBase): The app service to create or update
             wait_for_completion (bool): Whether to wait for the job to complete
 
         Returns:
             Job, optional: the job that was created or None if wait_for_completion is False.
         """
         app_service_spec = (
-            app_service.spec if isinstance(app_service, AppServiceBase) else app_service
+            app_service.spec
+            if isinstance(app_service, igz_mgmt.schemas.app_services.AppServiceBase)
+            else app_service
         )
         app_service_spec.mark_as_changed = True
         app_service_spec_obj = self.resolve_service(app_service_spec.name)
         if app_service_spec_obj:
             for position, service in enumerate(self.app_services):
                 if service.spec.name == app_service_spec_obj.spec.name:
                     self.app_services[position].spec = app_service_spec
                     break
         else:
-            self.app_services.append(AppServiceBase(spec=app_service_spec))
+            self.app_services.append(
+                igz_mgmt.schemas.app_services.AppServiceBase(spec=app_service_spec)
+            )
         if not self._skip_apply:
             return self._apply(http_client, wait_for_completion)
 
     def restart(
         self,
-        http_client: APIClient,
+        http_client: igz_mgmt.client.APIClient,
         app_service_spec_name: str,
         wait_for_completion=True,
     ) -> typing.Optional[Job]:
         """Restarts an app service.
 
         Args:
             http_client (APIClient): The client to use.
@@ -877,25 +975,27 @@
             wait_for_completion (bool): Whether to wait for the job to complete
 
         Returns:
             Job, optional: the job that was created or None if wait_for_completion is False.
         """
         app_service_obj = self.resolve_service(app_service_spec_name)
         if not app_service_obj:
-            raise AppServiceNotExistsException(name=app_service_spec_name)
+            raise igz_mgmt.exceptions.AppServiceNotExistsException(
+                name=app_service_spec_name
+            )
         for position, app_service in enumerate(self.app_services):
             if app_service.spec.name == app_service_obj.spec.name:
                 self.app_services[position].spec.mark_for_restart = True
                 break
         if not self._skip_apply:
             return self._apply(http_client, wait_for_completion)
 
     def remove_service(
         self,
-        http_client: APIClient,
+        http_client: igz_mgmt.client.APIClient,
         app_service_spec_name: str,
         wait_for_completion=True,
     ) -> typing.Optional[Job]:
         """Removes an app service.
 
         Args:
             http_client (APIClient): The client to use.
@@ -903,25 +1003,27 @@
             wait_for_completion (bool): Whether to wait for the job to complete
 
         Returns:
             Job, optional: the job that was created or None if wait_for_completion is False.
         """
         app_service_obj = self.resolve_service(app_service_spec_name)
         if not app_service_obj:
-            raise AppServiceNotExistsException(name=app_service_spec_name)
+            raise igz_mgmt.exceptions.AppServiceNotExistsException(
+                name=app_service_spec_name
+            )
         for position, app_service in enumerate(self.app_services):
             if app_service.spec.name == app_service_obj.spec.name:
                 del self.app_services[position]
                 break
         if not self._skip_apply:
             return self._apply(http_client, wait_for_completion)
 
     def scale_from_zero(
         self,
-        http_client: APIClient,
+        http_client: igz_mgmt.client.APIClient,
         app_service_spec_name: str,
         wait_for_completion=True,
     ) -> typing.Optional[Job]:
         """Scales an app service from zero.
 
         Args:
             http_client (APIClient): The client to use.
@@ -929,41 +1031,49 @@
             wait_for_completion (bool): Whether to wait for the job to complete
 
         Returns:
             Job, optional: the job that was created or None if wait_for_completion is False.
         """
         app_service_obj = self.resolve_service(app_service_spec_name)
         if not app_service_obj:
-            raise AppServiceNotExistsException(name=app_service_spec_name)
+            raise igz_mgmt.exceptions.AppServiceNotExistsException(
+                name=app_service_spec_name
+            )
         app_service_obj.spec.mark_as_changed = True
-        app_service_obj.spec.desired_state = AppServiceDesiredStates.ready
+        app_service_obj.spec.desired_state = (
+            igz_mgmt.constants.AppServiceDesiredStates.ready
+        )
         for position, app_service in enumerate(self.app_services):
             if app_service.spec.name == app_service_obj.spec.name:
                 self.app_services[position].spec = app_service_obj.spec
                 break
         if not self._skip_apply:
             current_apply_mode = self.apply_services_mode
 
             # In 3.5.3, the ApplyServicesMode.scale_from_zero_only mode is deprecated.
             # because we can scale services from zero by using the mark_as_changed and desired_state fields
             if http_client.version >= semver.VersionInfo.parse("3.5.3"):
-                self.set_apply_mode(ApplyServicesMode.service_owner_edit)
+                self.set_apply_mode(
+                    igz_mgmt.constants.ApplyServicesMode.service_owner_edit
+                )
             else:
-                self.set_apply_mode(ApplyServicesMode.scale_from_zero_only)
+                self.set_apply_mode(
+                    igz_mgmt.constants.ApplyServicesMode.scale_from_zero_only
+                )
             apply_result = self._apply(http_client, wait_for_completion)
 
             # set to the previous apply mode
             self.set_apply_mode(current_apply_mode)
             return apply_result
 
     def _apply(
         self,
-        http_client: APIClient,
+        http_client: igz_mgmt.client.APIClient,
         wait_for_completion=True,
-        force_apply_all_mode=ForceApplyAllMode.disabled,
+        force_apply_all_mode=igz_mgmt.constants.ForceApplyAllMode.disabled,
     ) -> Job:
         """Apply the current state of the manifest to the API.
 
         Args:
             http_client (APIClient): The client to use.
             wait_for_completion (bool, optional): Whether to wait for the job to complete. True by default.
             force_apply_all_mode (ForceApplyAllMode, optional): Disabled by default.
@@ -1005,7 +1115,202 @@
                         f"Service {service.spec.name} failed due to {service.status.error_info.description}"
                     )
             if errors:
                 raise RuntimeError(", ".join(errors)) from apply_exc
             else:
                 raise apply_exc
         return Job.get(http_client, job_id)
+
+
+class Project(BaseResource):
+    """Project resource represents project in the system."""
+
+    type: str = "project"
+    name: str = ""
+    description: str = ""
+    created_at: str = ""
+    updated_at: str = ""
+    admin_status: str = igz_mgmt.constants.ProjectAdminStatuses.online
+    operational_status: str = igz_mgmt.constants.ProjectOperationalStatuses.creating
+
+    # e.g.: [{"name":"", "value":""}, ...]
+    labels: typing.List[typing.Dict[str, str]] = []
+    annotations: typing.List[typing.Dict[str, str]] = []
+
+    mlrun_project: str = ""
+    nuclio_project: str = ""
+
+    @classmethod
+    def create(
+        cls,
+        http_client: igz_mgmt.client.APIClient,
+        name: str,
+        description: str = "",
+        labels: typing.List[typing.Dict[str, str]] = None,
+        annotations: typing.List[typing.Dict[str, str]] = None,
+        owner: typing.Union[str, "User", None] = None,
+        wait_for_completion=True,
+    ) -> "Project":
+        """Creates a new project.
+
+        Args:
+            http_client (APIClient): The client to use.
+            name (str): The project name.
+            description (str, optional): The project description.
+            labels (typing.List[typing.Dict[str, str]], optional): The project labels.
+            annotations (typing.List[typing.Dict[str, str]], optional): The project annotations.
+            owner (str or User or None): The project owner. None by default
+            wait_for_completion (bool): Whether to wait for the job to complete
+
+        Returns:
+            Project: The project instance.
+        """
+        attributes = {
+            "name": name,
+            "description": description,
+            "labels": labels,
+            "annotations": annotations,
+        }
+
+        relationships = cls._fill_relationships(owner=owner)
+
+        created_resource = cls._get_crud().create(
+            http_client,
+            attributes=attributes,
+            relationships=relationships,
+            headers=cls._resolve_project_header(),
+        )
+
+        # there might be jobs handling the creating
+        job_id = (
+            created_resource.get("data", {})
+            .get("relationships", {})
+            .get("last_job", {})
+            .get("data", {})
+            .get("id", None)
+        )
+        if job_id and wait_for_completion:
+            Job.wait_for_completion(
+                http_client, job_id, job_completion_retry_interval=10
+            )
+        return cls.from_orm(created_resource)
+
+    def update(
+        self, http_client: igz_mgmt.client.APIClient, relationships=None, **kwargs
+    ) -> "BaseResource":
+        """Updates project.
+
+        Args:
+            http_client (APIClient): The client to use.
+            relationships (optional): The project relationships. None by default.
+            **kwargs: additional arguments to pass to the request.
+
+        Returns:
+            BaseResource: The updated record.
+        """
+        return super().update(
+            http_client,
+            relationships=relationships,
+            headers=self._resolve_project_header(),
+            **kwargs,
+        )
+
+    def delete(
+        self,
+        http_client: igz_mgmt.client.APIClient,
+        ignore_missing: bool = False,
+        wait_for_job_deletion: bool = True,
+        deletion_strategy: igz_mgmt.constants.ProjectDeletionStrategies = None,
+    ) -> typing.Optional[Job]:
+        """Deletes resource record.
+
+        Args:
+            http_client (APIClient): The client to use.
+            ignore_missing (bool, optional): When True, don't raise an exception in case the record does not exist.
+            False by default.
+            wait_for_job_deletion (bool, optional): Whether to wait for the job to complete. True by default.
+            deletion_strategy (ProjectDeletionStrategies, optional): The project deletion type. None by default
+
+        Returns:
+            Job, optional: the job that was created or None.
+        """
+        response = http_client.delete_by_attribute(
+            self.type,
+            "name",
+            self.name,
+            ignore_missing=ignore_missing,
+            headers=self._resolve_project_header(deletion_strategy),
+        )
+
+        if response.status_code == http.HTTPStatus.ACCEPTED:
+            response_body = response.json()
+            job_id = response_body.get("data", {}).get("id", None)
+            if job_id:
+                if wait_for_job_deletion:
+                    Job.wait_for_completion(
+                        http_client, job_id, job_completion_retry_interval=10
+                    )
+                return Job.get(http_client, job_id)
+
+    @classmethod
+    def get_by_name(
+        cls,
+        http_client: igz_mgmt.client.APIClient,
+        name: str,
+        include: typing.Optional[typing.List[str]] = None,
+    ) -> "Project":
+        """A convenience method to get a project by name.
+
+        Args:
+            http_client (APIClient): The client to use.
+            name (str): The project name.
+            include (typing.List[str], optional): Include related resources (e.g. include=["tenant", "owner"]).
+                None by default.
+
+        Returns:
+            Project: The project instance by name.
+
+        Raises:
+            ResourceNotFoundException: If project is not found
+        """
+        return cls._get_resource_by_name(http_client, "name", name, include=include)
+
+    def set_owner(
+        self, http_client: igz_mgmt.client.APIClient, owner: typing.Union[str, "User"]
+    ):
+        """Sets the owner of the project.
+
+        Args:
+            http_client (APIClient): The client to use.
+            owner (str or User): The user id or user instance.
+
+        Returns:
+            Project: The project instance.
+        """
+        relationships = self._fill_relationships(owner=owner)
+        return self.update(http_client, relationships=relationships)
+
+    @staticmethod
+    def _resolve_project_header(
+        deletion_strategy: igz_mgmt.constants.ProjectDeletionStrategies = None,
+    ):
+        headers = {
+            igz_mgmt.constants._RequestHeaders.projects_role_header: "igz-mgmt-sdk"
+        }
+        if deletion_strategy:
+            headers[
+                igz_mgmt.constants._RequestHeaders.deletion_strategy_header
+            ] = deletion_strategy
+        return headers
+
+    @staticmethod
+    def _fill_relationships(owner: typing.Union[str, "User", None]):
+        relationships = collections.defaultdict(dict)
+        if owner:
+            user_id = owner.id if isinstance(owner, User) else owner
+            relationships["owner"] = {
+                "data": {
+                    "type": "user",
+                    "id": user_id,
+                },
+            }
+        return relationships
```

### Comparing `igz_mgmt-0.0.5/igz_mgmt/common/__init__.py` & `igz_mgmt-0.0.6/igz_mgmt/common/__init__.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.5/igz_mgmt/common/helpers.py` & `igz_mgmt-0.0.6/igz_mgmt/common/helpers.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.5/igz_mgmt/logger/__init__.py` & `igz_mgmt-0.0.6/igz_mgmt/schemas/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,11 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+import pydantic
 
-from .logger import Logger, get_or_create_logger
 
-__all__ = ["get_or_create_logger", "Logger"]
+class _Base(pydantic.BaseModel):
+    class Config:
+        # be forward compatible
+        extra = "allow"
+        orm_mode = True
+        use_enum_values = True
```

### Comparing `igz_mgmt-0.0.5/igz_mgmt/logger/logger.py` & `igz_mgmt-0.0.6/igz_mgmt/logger/logger.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.5/LICENSE` & `igz_mgmt-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.5/pyproject.toml` & `igz_mgmt-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.5/PKG-INFO` & `igz_mgmt-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igz-mgmt
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python SDK For Iguazio Management API
 Project-URL: Homepage, https://github.com/iguazio/igz-mgmt-sdk
 Author-email: Iguazio Platform Team <liranb@iguazio.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

