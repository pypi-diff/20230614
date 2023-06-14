# Comparing `tmp/ignos-api-client-2023.5.22.5244.tar.gz` & `tmp/ignos-api-client-2023.6.14.5376.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ignos-api-client-2023.5.22.5244.tar", last modified: Mon May 22 06:17:08 2023, max compression
+gzip compressed data, was "ignos-api-client-2023.6.14.5376.tar", last modified: Wed Jun 14 13:11:17 2023, max compression
```

## Comparing `ignos-api-client-2023.5.22.5244.tar` & `ignos-api-client-2023.6.14.5376.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 06:17:08.062689 ignos-api-client-2023.5.22.5244/
--rw-r--r--   0 vsts      (1001) docker     (123)      171 2023-05-22 06:17:08.062689 ignos-api-client-2023.5.22.5244/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 06:17:08.054689 ignos-api-client-2023.5.22.5244/ignos/
--rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-05-22 06:16:53.000000 ignos-api-client-2023.5.22.5244/ignos/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 06:17:08.054689 ignos-api-client-2023.5.22.5244/ignos/api/
--rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-05-22 06:16:53.000000 ignos-api-client-2023.5.22.5244/ignos/api/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 06:17:08.054689 ignos-api-client-2023.5.22.5244/ignos/api/client/
--rw-r--r--   0 vsts      (1001) docker     (123)      866 2023-05-22 06:16:53.000000 ignos-api-client-2023.5.22.5244/ignos/api/client/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14050 2023-05-22 06:16:53.000000 ignos-api-client-2023.5.22.5244/ignos/api/client/_client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2942 2023-05-22 06:16:53.000000 ignos-api-client-2023.5.22.5244/ignos/api/client/_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-05-22 06:16:53.000000 ignos-api-client-2023.5.22.5244/ignos/api/client/_patch.py
--rw-r--r--   0 vsts      (1001) docker     (123)    78836 2023-05-22 06:16:53.000000 ignos-api-client-2023.5.22.5244/ignos/api/client/_serialization.py
--rw-r--r--   0 vsts      (1001) docker     (123)      976 2023-05-22 06:16:53.000000 ignos-api-client-2023.5.22.5244/ignos/api/client/_vendor.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-22 06:16:53.000000 ignos-api-client-2023.5.22.5244/ignos/api/client/_version.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 06:17:08.054689 ignos-api-client-2023.5.22.5244/ignos/api/client/aio/
--rw-r--r--   0 vsts      (1001) docker     (123)      813 2023-05-22 06:16:53.000000 ignos-api-client-2023.5.22.5244/ignos/api/client/aio/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14349 2023-05-22 06:16:53.000000 ignos-api-client-2023.5.22.5244/ignos/api/client/aio/_client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2985 2023-05-22 06:16:53.000000 ignos-api-client-2023.5.22.5244/ignos/api/client/aio/_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-05-22 06:16:53.000000 ignos-api-client-2023.5.22.5244/ignos/api/client/aio/_patch.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 06:17:08.058689 ignos-api-client-2023.5.22.5244/ignos/api/client/aio/operations/
--rw-r--r--   0 vsts      (1001) docker     (123)     3657 2023-05-22 06:16:53.000000 ignos-api-client-2023.5.22.5244/ignos/api/client/aio/operations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)   864238 2023-05-22 06:16:53.000000 ignos-api-client-2023.5.22.5244/ignos/api/client/aio/operations/_operations.py
--rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-05-22 06:16:53.000000 ignos-api-client-2023.5.22.5244/ignos/api/client/aio/operations/_patch.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 06:17:08.058689 ignos-api-client-2023.5.22.5244/ignos/api/client/models/
--rw-r--r--   0 vsts      (1001) docker     (123)    26028 2023-05-22 06:16:53.000000 ignos-api-client-2023.5.22.5244/ignos/api/client/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4978 2023-05-22 06:16:53.000000 ignos-api-client-2023.5.22.5244/ignos/api/client/models/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (123)   661240 2023-05-22 06:16:53.000000 ignos-api-client-2023.5.22.5244/ignos/api/client/models/_models.py
--rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-05-22 06:16:53.000000 ignos-api-client-2023.5.22.5244/ignos/api/client/models/_patch.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 06:17:08.058689 ignos-api-client-2023.5.22.5244/ignos/api/client/operations/
--rw-r--r--   0 vsts      (1001) docker     (123)     3657 2023-05-22 06:16:53.000000 ignos-api-client-2023.5.22.5244/ignos/api/client/operations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)  1056249 2023-05-22 06:16:53.000000 ignos-api-client-2023.5.22.5244/ignos/api/client/operations/_operations.py
--rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-05-22 06:16:53.000000 ignos-api-client-2023.5.22.5244/ignos/api/client/operations/_patch.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 06:17:08.058689 ignos-api-client-2023.5.22.5244/ignos_api_client.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      171 2023-05-22 06:17:08.000000 ignos-api-client-2023.5.22.5244/ignos_api_client.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      986 2023-05-22 06:17:08.000000 ignos-api-client-2023.5.22.5244/ignos_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-22 06:17:08.000000 ignos-api-client-2023.5.22.5244/ignos_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       48 2023-05-22 06:17:08.000000 ignos-api-client-2023.5.22.5244/ignos_api_client.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-05-22 06:17:08.000000 ignos-api-client-2023.5.22.5244/ignos_api_client.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-22 06:17:08.062689 ignos-api-client-2023.5.22.5244/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)      958 2023-05-22 06:16:53.000000 ignos-api-client-2023.5.22.5244/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-14 13:11:17.038585 ignos-api-client-2023.6.14.5376/
+-rw-r--r--   0 vsts      (1001) docker     (123)      171 2023-06-14 13:11:17.038585 ignos-api-client-2023.6.14.5376/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-14 13:11:17.022585 ignos-api-client-2023.6.14.5376/ignos/
+-rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-14 13:11:17.022585 ignos-api-client-2023.6.14.5376/ignos/api/
+-rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-14 13:11:17.026585 ignos-api-client-2023.6.14.5376/ignos/api/client/
+-rw-r--r--   0 vsts      (1001) docker     (123)      866 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14050 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/_client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2942 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/_patch.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    78836 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/_serialization.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      976 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/_vendor.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/_version.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-14 13:11:17.030585 ignos-api-client-2023.6.14.5376/ignos/api/client/aio/
+-rw-r--r--   0 vsts      (1001) docker     (123)      813 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/aio/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14349 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/aio/_client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2985 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/aio/_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/aio/_patch.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-14 13:11:17.030585 ignos-api-client-2023.6.14.5376/ignos/api/client/aio/operations/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3657 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/aio/operations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   863930 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/aio/operations/_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/aio/operations/_patch.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-14 13:11:17.034585 ignos-api-client-2023.6.14.5376/ignos/api/client/models/
+-rw-r--r--   0 vsts      (1001) docker     (123)    26096 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4978 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/models/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   669585 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/models/_models.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/models/_patch.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-14 13:11:17.038585 ignos-api-client-2023.6.14.5376/ignos/api/client/operations/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3657 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/operations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)  1055635 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/operations/_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/operations/_patch.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-14 13:11:17.038585 ignos-api-client-2023.6.14.5376/ignos_api_client.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      171 2023-06-14 13:11:17.000000 ignos-api-client-2023.6.14.5376/ignos_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      986 2023-06-14 13:11:17.000000 ignos-api-client-2023.6.14.5376/ignos_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-14 13:11:17.000000 ignos-api-client-2023.6.14.5376/ignos_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       48 2023-06-14 13:11:17.000000 ignos-api-client-2023.6.14.5376/ignos_api_client.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-14 13:11:17.000000 ignos-api-client-2023.6.14.5376/ignos_api_client.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-14 13:11:17.038585 ignos-api-client-2023.6.14.5376/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)      958 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/setup.py
```

### Comparing `ignos-api-client-2023.5.22.5244/ignos/api/client/__init__.py` & `ignos-api-client-2023.6.14.5376/ignos/api/client/__init__.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.5.22.5244/ignos/api/client/_client.py` & `ignos-api-client-2023.6.14.5376/ignos/api/client/_client.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.5.22.5244/ignos/api/client/_configuration.py` & `ignos-api-client-2023.6.14.5376/ignos/api/client/_configuration.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.5.22.5244/ignos/api/client/_patch.py` & `ignos-api-client-2023.6.14.5376/ignos/api/client/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.5.22.5244/ignos/api/client/_serialization.py` & `ignos-api-client-2023.6.14.5376/ignos/api/client/_serialization.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.5.22.5244/ignos/api/client/_vendor.py` & `ignos-api-client-2023.6.14.5376/ignos/api/client/_vendor.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.5.22.5244/ignos/api/client/aio/__init__.py` & `ignos-api-client-2023.6.14.5376/ignos/api/client/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.5.22.5244/ignos/api/client/aio/_client.py` & `ignos-api-client-2023.6.14.5376/ignos/api/client/aio/_client.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.5.22.5244/ignos/api/client/aio/_configuration.py` & `ignos-api-client-2023.6.14.5376/ignos/api/client/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.5.22.5244/ignos/api/client/aio/_patch.py` & `ignos-api-client-2023.6.14.5376/ignos/api/client/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.5.22.5244/ignos/api/client/aio/operations/__init__.py` & `ignos-api-client-2023.6.14.5376/ignos/api/client/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.5.22.5244/ignos/api/client/aio/operations/_operations.py` & `ignos-api-client-2023.6.14.5376/ignos/api/client/aio/operations/_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -9087,25 +9087,22 @@
 
     @distributed_trace_async
     async def list_alarms_per_machine(
         self,
         *,
         start_time: Optional[datetime.datetime] = None,
         end_time: Optional[datetime.datetime] = None,
-        asset_id: Optional[int] = None,
         **kwargs: Any
     ) -> List[_models.MachineAlarmSummaryDto]:
         """list_alarms_per_machine.
 
         :keyword start_time: Default value is None.
         :paramtype start_time: ~datetime.datetime
         :keyword end_time: Default value is None.
         :paramtype end_time: ~datetime.datetime
-        :keyword asset_id: Default value is None.
-        :paramtype asset_id: int
         :return: list of MachineAlarmSummaryDto
         :rtype: list[~ignos.api.client.models.MachineAlarmSummaryDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -9118,15 +9115,14 @@
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[List[_models.MachineAlarmSummaryDto]] = kwargs.pop("cls", None)
 
         request = build_machine_alarms_list_alarms_per_machine_request(
             start_time=start_time,
             end_time=end_time,
-            asset_id=asset_id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
@@ -9148,25 +9144,22 @@
 
     @distributed_trace_async
     async def list_alarm_severity_occurrences(
         self,
         *,
         start_time: Optional[datetime.datetime] = None,
         end_time: Optional[datetime.datetime] = None,
-        asset_id: Optional[int] = None,
         **kwargs: Any
     ) -> List[_models.MachineAlarmSeverityOccurenceDto]:
         """list_alarm_severity_occurrences.
 
         :keyword start_time: Default value is None.
         :paramtype start_time: ~datetime.datetime
         :keyword end_time: Default value is None.
         :paramtype end_time: ~datetime.datetime
-        :keyword asset_id: Default value is None.
-        :paramtype asset_id: int
         :return: list of MachineAlarmSeverityOccurenceDto
         :rtype: list[~ignos.api.client.models.MachineAlarmSeverityOccurenceDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -9179,15 +9172,14 @@
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[List[_models.MachineAlarmSeverityOccurenceDto]] = kwargs.pop("cls", None)
 
         request = build_machine_alarms_list_alarm_severity_occurrences_request(
             start_time=start_time,
             end_time=end_time,
-            asset_id=asset_id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
```

### Comparing `ignos-api-client-2023.5.22.5244/ignos/api/client/aio/operations/_patch.py` & `ignos-api-client-2023.6.14.5376/ignos/api/client/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.5.22.5244/ignos/api/client/models/__init__.py` & `ignos-api-client-2023.6.14.5376/ignos/api/client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,14 +294,15 @@
 from ._models import UtilizationDetailsDto
 from ._models import UtilizationDto
 from ._models import UtilizationListDto
 from ._models import UtilizationSummaryDto
 from ._models import UtilizationWorkorderDto
 from ._models import ValidationRuleDto
 from ._models import WhitelistMeasuringTool
+from ._models import WorkOrderProjectDto
 from ._models import WorkorderCustomerOrderReferenceDto
 from ._models import WorkorderDto
 from ._models import WorkorderHierarchyDto
 from ._models import WorkorderImportTraceItemDto
 from ._models import WorkorderListDto
 from ._models import WorkorderListDtoPagedResult
 from ._models import WorkorderMaterialDto
@@ -627,14 +628,15 @@
     "UtilizationDetailsDto",
     "UtilizationDto",
     "UtilizationListDto",
     "UtilizationSummaryDto",
     "UtilizationWorkorderDto",
     "ValidationRuleDto",
     "WhitelistMeasuringTool",
+    "WorkOrderProjectDto",
     "WorkorderCustomerOrderReferenceDto",
     "WorkorderDto",
     "WorkorderHierarchyDto",
     "WorkorderImportTraceItemDto",
     "WorkorderListDto",
     "WorkorderListDtoPagedResult",
     "WorkorderMaterialDto",
```

### Comparing `ignos-api-client-2023.5.22.5244/ignos/api/client/models/_enums.py` & `ignos-api-client-2023.6.14.5376/ignos/api/client/models/_enums.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.5.22.5244/ignos/api/client/models/_models.py` & `ignos-api-client-2023.6.14.5376/ignos/api/client/models/_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -12871,56 +12871,63 @@
     :vartype part_revision: str
     :ivar part_name:
     :vartype part_name: str
     :ivar drawing:
     :vartype drawing: str
     :ivar drawing_revision:
     :vartype drawing_revision: str
+    :ivar material:
+    :vartype material: str
     """
 
     _validation = {
         "part_number": {"required": True, "min_length": 1},
     }
 
     _attribute_map = {
         "part_number": {"key": "partNumber", "type": "str"},
         "part_revision": {"key": "partRevision", "type": "str"},
         "part_name": {"key": "partName", "type": "str"},
         "drawing": {"key": "drawing", "type": "str"},
         "drawing_revision": {"key": "drawingRevision", "type": "str"},
+        "material": {"key": "material", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         part_number: str,
         part_revision: Optional[str] = None,
         part_name: Optional[str] = None,
         drawing: Optional[str] = None,
         drawing_revision: Optional[str] = None,
+        material: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword part_number: Required.
         :paramtype part_number: str
         :keyword part_revision:
         :paramtype part_revision: str
         :keyword part_name:
         :paramtype part_name: str
         :keyword drawing:
         :paramtype drawing: str
         :keyword drawing_revision:
         :paramtype drawing_revision: str
+        :keyword material:
+        :paramtype material: str
         """
         super().__init__(**kwargs)
         self.part_number = part_number
         self.part_revision = part_revision
         self.part_name = part_name
         self.drawing = drawing
         self.drawing_revision = drawing_revision
+        self.material = material
 
 
 class PowerDto(_serialization.Model):
     """PowerDto.
 
     :ivar asset_name:
     :vartype asset_name: str
@@ -13270,145 +13277,300 @@
         super().__init__(**kwargs)
         self.id = id
         self.name = name
         self.employment_legal_entity_id = employment_legal_entity_id
         self.dimension_display_value = dimension_display_value
 
 
-class ProductionOrderDto(_serialization.Model):
+class ProductionOrderDto(_serialization.Model):  # pylint: disable=too-many-instance-attributes
     """ProductionOrderDto.
 
-    All required parameters must be populated in order to send to Azure.
-
-    :ivar data_area_id:
-    :vartype data_area_id: str
     :ivar id:
     :vartype id: str
+    :ivar company_id:
+    :vartype company_id: str
+    :ivar part:
+    :vartype part: ~ignos.api.client.models.PartDto
     :ivar quantity:
     :vartype quantity: float
+    :ivar unit:
+    :vartype unit: str
+    :ivar status: Known values are: "Draft", "Ready", "Ongoing", "Completed", and "Deleted".
+    :vartype status: str or ~ignos.api.client.models.WorkorderStatus
+    :ivar operations:
+    :vartype operations: list[~ignos.api.client.models.ProductionOrderOperationDto]
+    :ivar planned_start:
+    :vartype planned_start: ~datetime.datetime
+    :ivar planned_end:
+    :vartype planned_end: ~datetime.datetime
+    :ivar produced_quantity:
+    :vartype produced_quantity: float
+    :ivar scrapped_quantity:
+    :vartype scrapped_quantity: float
+    :ivar planner:
+    :vartype planner: ~ignos.api.client.models.UserDto
+    :ivar project_leader:
+    :vartype project_leader: ~ignos.api.client.models.UserDto
+    :ivar end_location:
+    :vartype end_location: str
+    :ivar project:
+    :vartype project: ~ignos.api.client.models.WorkOrderProjectDto
     :ivar start_date:
     :vartype start_date: ~datetime.datetime
     :ivar end_date:
     :vartype end_date: ~datetime.datetime
-    :ivar started_quantity:
-    :vartype started_quantity: float
-    :ivar item_number:
-    :vartype item_number: str
-    :ivar operations: Required.
-    :vartype operations: list[~ignos.api.client.models.ProductionOrderOperationDto]
+    :ivar bom_position:
+    :vartype bom_position: str
     """
 
-    _validation = {
-        "operations": {"required": True},
-    }
-
     _attribute_map = {
-        "data_area_id": {"key": "dataAreaId", "type": "str"},
         "id": {"key": "id", "type": "str"},
+        "company_id": {"key": "companyId", "type": "str"},
+        "part": {"key": "part", "type": "PartDto"},
         "quantity": {"key": "quantity", "type": "float"},
+        "unit": {"key": "unit", "type": "str"},
+        "status": {"key": "status", "type": "str"},
+        "operations": {"key": "operations", "type": "[ProductionOrderOperationDto]"},
+        "planned_start": {"key": "plannedStart", "type": "iso-8601"},
+        "planned_end": {"key": "plannedEnd", "type": "iso-8601"},
+        "produced_quantity": {"key": "producedQuantity", "type": "float"},
+        "scrapped_quantity": {"key": "scrappedQuantity", "type": "float"},
+        "planner": {"key": "planner", "type": "UserDto"},
+        "project_leader": {"key": "projectLeader", "type": "UserDto"},
+        "end_location": {"key": "endLocation", "type": "str"},
+        "project": {"key": "project", "type": "WorkOrderProjectDto"},
         "start_date": {"key": "startDate", "type": "iso-8601"},
         "end_date": {"key": "endDate", "type": "iso-8601"},
-        "started_quantity": {"key": "startedQuantity", "type": "float"},
-        "item_number": {"key": "itemNumber", "type": "str"},
-        "operations": {"key": "operations", "type": "[ProductionOrderOperationDto]"},
+        "bom_position": {"key": "bomPosition", "type": "str"},
     }
 
     def __init__(
         self,
         *,
-        operations: List["_models.ProductionOrderOperationDto"],
-        data_area_id: Optional[str] = None,
         id: Optional[str] = None,  # pylint: disable=redefined-builtin
+        company_id: Optional[str] = None,
+        part: Optional["_models.PartDto"] = None,
         quantity: Optional[float] = None,
+        unit: Optional[str] = None,
+        status: Optional[Union[str, "_models.WorkorderStatus"]] = None,
+        operations: Optional[List["_models.ProductionOrderOperationDto"]] = None,
+        planned_start: Optional[datetime.datetime] = None,
+        planned_end: Optional[datetime.datetime] = None,
+        produced_quantity: Optional[float] = None,
+        scrapped_quantity: Optional[float] = None,
+        planner: Optional["_models.UserDto"] = None,
+        project_leader: Optional["_models.UserDto"] = None,
+        end_location: Optional[str] = None,
+        project: Optional["_models.WorkOrderProjectDto"] = None,
         start_date: Optional[datetime.datetime] = None,
         end_date: Optional[datetime.datetime] = None,
-        started_quantity: Optional[float] = None,
-        item_number: Optional[str] = None,
+        bom_position: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """
-        :keyword data_area_id:
-        :paramtype data_area_id: str
         :keyword id:
         :paramtype id: str
+        :keyword company_id:
+        :paramtype company_id: str
+        :keyword part:
+        :paramtype part: ~ignos.api.client.models.PartDto
         :keyword quantity:
         :paramtype quantity: float
+        :keyword unit:
+        :paramtype unit: str
+        :keyword status: Known values are: "Draft", "Ready", "Ongoing", "Completed", and "Deleted".
+        :paramtype status: str or ~ignos.api.client.models.WorkorderStatus
+        :keyword operations:
+        :paramtype operations: list[~ignos.api.client.models.ProductionOrderOperationDto]
+        :keyword planned_start:
+        :paramtype planned_start: ~datetime.datetime
+        :keyword planned_end:
+        :paramtype planned_end: ~datetime.datetime
+        :keyword produced_quantity:
+        :paramtype produced_quantity: float
+        :keyword scrapped_quantity:
+        :paramtype scrapped_quantity: float
+        :keyword planner:
+        :paramtype planner: ~ignos.api.client.models.UserDto
+        :keyword project_leader:
+        :paramtype project_leader: ~ignos.api.client.models.UserDto
+        :keyword end_location:
+        :paramtype end_location: str
+        :keyword project:
+        :paramtype project: ~ignos.api.client.models.WorkOrderProjectDto
         :keyword start_date:
         :paramtype start_date: ~datetime.datetime
         :keyword end_date:
         :paramtype end_date: ~datetime.datetime
-        :keyword started_quantity:
-        :paramtype started_quantity: float
-        :keyword item_number:
-        :paramtype item_number: str
-        :keyword operations: Required.
-        :paramtype operations: list[~ignos.api.client.models.ProductionOrderOperationDto]
+        :keyword bom_position:
+        :paramtype bom_position: str
         """
         super().__init__(**kwargs)
-        self.data_area_id = data_area_id
         self.id = id
+        self.company_id = company_id
+        self.part = part
         self.quantity = quantity
+        self.unit = unit
+        self.status = status
+        self.operations = operations
+        self.planned_start = planned_start
+        self.planned_end = planned_end
+        self.produced_quantity = produced_quantity
+        self.scrapped_quantity = scrapped_quantity
+        self.planner = planner
+        self.project_leader = project_leader
+        self.end_location = end_location
+        self.project = project
         self.start_date = start_date
         self.end_date = end_date
-        self.started_quantity = started_quantity
-        self.item_number = item_number
-        self.operations = operations
+        self.bom_position = bom_position
 
 
-class ProductionOrderOperationDto(_serialization.Model):
+class ProductionOrderOperationDto(_serialization.Model):  # pylint: disable=too-many-instance-attributes
     """ProductionOrderOperationDto.
 
-    :ivar job_id:
-    :vartype job_id: str
     :ivar operation:
     :vartype operation: int
-    :ivar operation_resource_id:
-    :vartype operation_resource_id: str
-    :ivar job_processing_percentage:
-    :vartype job_processing_percentage: float
-    :ivar calculated_job_duration_hours:
-    :vartype calculated_job_duration_hours: float
+    :ivar operation_id:
+    :vartype operation_id: str
+    :ivar description:
+    :vartype description: str
+    :ivar planned_setup_time:
+    :vartype planned_setup_time: float
+    :ivar planned_production_time_per_part:
+    :vartype planned_production_time_per_part: float
+    :ivar fixed_time:
+    :vartype fixed_time: bool
+    :ivar resource:
+    :vartype resource: ~ignos.api.client.models.ResourceDto
+    :ivar planned_start:
+    :vartype planned_start: ~datetime.datetime
+    :ivar planned_end:
+    :vartype planned_end: ~datetime.datetime
+    :ivar status: Known values are: "NotReady", "Ready", "Ongoing", and "Completed".
+    :vartype status: str or ~ignos.api.client.models.OperationStatus
+    :ivar produced_quantity:
+    :vartype produced_quantity: float
+    :ivar scrapped_quantity:
+    :vartype scrapped_quantity: float
+    :ivar used_production_time:
+    :vartype used_production_time: float
+    :ivar used_setup_time:
+    :vartype used_setup_time: float
+    :ivar work_instructions:
+    :vartype work_instructions: str
+    :ivar fixture:
+    :vartype fixture: str
+    :ivar program:
+    :vartype program: str
+    :ivar tool_number:
+    :vartype tool_number: str
     """
 
     _attribute_map = {
-        "job_id": {"key": "jobId", "type": "str"},
         "operation": {"key": "operation", "type": "int"},
-        "operation_resource_id": {"key": "operationResourceId", "type": "str"},
-        "job_processing_percentage": {"key": "jobProcessingPercentage", "type": "float"},
-        "calculated_job_duration_hours": {"key": "calculatedJobDurationHours", "type": "float"},
+        "operation_id": {"key": "operationId", "type": "str"},
+        "description": {"key": "description", "type": "str"},
+        "planned_setup_time": {"key": "plannedSetupTime", "type": "float"},
+        "planned_production_time_per_part": {"key": "plannedProductionTimePerPart", "type": "float"},
+        "fixed_time": {"key": "fixedTime", "type": "bool"},
+        "resource": {"key": "resource", "type": "ResourceDto"},
+        "planned_start": {"key": "plannedStart", "type": "iso-8601"},
+        "planned_end": {"key": "plannedEnd", "type": "iso-8601"},
+        "status": {"key": "status", "type": "str"},
+        "produced_quantity": {"key": "producedQuantity", "type": "float"},
+        "scrapped_quantity": {"key": "scrappedQuantity", "type": "float"},
+        "used_production_time": {"key": "usedProductionTime", "type": "float"},
+        "used_setup_time": {"key": "usedSetupTime", "type": "float"},
+        "work_instructions": {"key": "workInstructions", "type": "str"},
+        "fixture": {"key": "fixture", "type": "str"},
+        "program": {"key": "program", "type": "str"},
+        "tool_number": {"key": "toolNumber", "type": "str"},
     }
 
     def __init__(
         self,
         *,
-        job_id: Optional[str] = None,
         operation: Optional[int] = None,
-        operation_resource_id: Optional[str] = None,
-        job_processing_percentage: Optional[float] = None,
-        calculated_job_duration_hours: Optional[float] = None,
+        operation_id: Optional[str] = None,
+        description: Optional[str] = None,
+        planned_setup_time: Optional[float] = None,
+        planned_production_time_per_part: Optional[float] = None,
+        fixed_time: Optional[bool] = None,
+        resource: Optional["_models.ResourceDto"] = None,
+        planned_start: Optional[datetime.datetime] = None,
+        planned_end: Optional[datetime.datetime] = None,
+        status: Optional[Union[str, "_models.OperationStatus"]] = None,
+        produced_quantity: Optional[float] = None,
+        scrapped_quantity: Optional[float] = None,
+        used_production_time: Optional[float] = None,
+        used_setup_time: Optional[float] = None,
+        work_instructions: Optional[str] = None,
+        fixture: Optional[str] = None,
+        program: Optional[str] = None,
+        tool_number: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """
-        :keyword job_id:
-        :paramtype job_id: str
         :keyword operation:
         :paramtype operation: int
-        :keyword operation_resource_id:
-        :paramtype operation_resource_id: str
-        :keyword job_processing_percentage:
-        :paramtype job_processing_percentage: float
-        :keyword calculated_job_duration_hours:
-        :paramtype calculated_job_duration_hours: float
+        :keyword operation_id:
+        :paramtype operation_id: str
+        :keyword description:
+        :paramtype description: str
+        :keyword planned_setup_time:
+        :paramtype planned_setup_time: float
+        :keyword planned_production_time_per_part:
+        :paramtype planned_production_time_per_part: float
+        :keyword fixed_time:
+        :paramtype fixed_time: bool
+        :keyword resource:
+        :paramtype resource: ~ignos.api.client.models.ResourceDto
+        :keyword planned_start:
+        :paramtype planned_start: ~datetime.datetime
+        :keyword planned_end:
+        :paramtype planned_end: ~datetime.datetime
+        :keyword status: Known values are: "NotReady", "Ready", "Ongoing", and "Completed".
+        :paramtype status: str or ~ignos.api.client.models.OperationStatus
+        :keyword produced_quantity:
+        :paramtype produced_quantity: float
+        :keyword scrapped_quantity:
+        :paramtype scrapped_quantity: float
+        :keyword used_production_time:
+        :paramtype used_production_time: float
+        :keyword used_setup_time:
+        :paramtype used_setup_time: float
+        :keyword work_instructions:
+        :paramtype work_instructions: str
+        :keyword fixture:
+        :paramtype fixture: str
+        :keyword program:
+        :paramtype program: str
+        :keyword tool_number:
+        :paramtype tool_number: str
         """
         super().__init__(**kwargs)
-        self.job_id = job_id
         self.operation = operation
-        self.operation_resource_id = operation_resource_id
-        self.job_processing_percentage = job_processing_percentage
-        self.calculated_job_duration_hours = calculated_job_duration_hours
+        self.operation_id = operation_id
+        self.description = description
+        self.planned_setup_time = planned_setup_time
+        self.planned_production_time_per_part = planned_production_time_per_part
+        self.fixed_time = fixed_time
+        self.resource = resource
+        self.planned_start = planned_start
+        self.planned_end = planned_end
+        self.status = status
+        self.produced_quantity = produced_quantity
+        self.scrapped_quantity = scrapped_quantity
+        self.used_production_time = used_production_time
+        self.used_setup_time = used_setup_time
+        self.work_instructions = work_instructions
+        self.fixture = fixture
+        self.program = program
+        self.tool_number = tool_number
 
 
 class ProductionResourceDto(_serialization.Model):
     """ProductionResourceDto.
 
     :ivar id:
     :vartype id: str
@@ -19039,14 +19201,53 @@
         self.resource_id = resource_id
         self.description = description
         self.part = part
         self.workorder_description = workorder_description
         self.operation_description = operation_description
 
 
+class WorkOrderProjectDto(_serialization.Model):
+    """WorkOrderProjectDto.
+
+    :ivar id:
+    :vartype id: str
+    :ivar name:
+    :vartype name: str
+    :ivar project_manager:
+    :vartype project_manager: str
+    """
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "project_manager": {"key": "projectManager", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        id: Optional[str] = None,  # pylint: disable=redefined-builtin
+        name: Optional[str] = None,
+        project_manager: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword id:
+        :paramtype id: str
+        :keyword name:
+        :paramtype name: str
+        :keyword project_manager:
+        :paramtype project_manager: str
+        """
+        super().__init__(**kwargs)
+        self.id = id
+        self.name = name
+        self.project_manager = project_manager
+
+
 class WorkorderTraceItemDto(_serialization.Model):
     """WorkorderTraceItemDto.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar sequence: Required.
     :vartype sequence: str
```

### Comparing `ignos-api-client-2023.5.22.5244/ignos/api/client/models/_patch.py` & `ignos-api-client-2023.6.14.5376/ignos/api/client/models/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.5.22.5244/ignos/api/client/operations/__init__.py` & `ignos-api-client-2023.6.14.5376/ignos/api/client/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.5.22.5244/ignos/api/client/operations/_operations.py` & `ignos-api-client-2023.6.14.5376/ignos/api/client/operations/_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -2185,64 +2185,52 @@
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_machine_alarms_list_alarms_per_machine_request(
-    *,
-    start_time: Optional[datetime.datetime] = None,
-    end_time: Optional[datetime.datetime] = None,
-    asset_id: Optional[int] = None,
-    **kwargs: Any
+    *, start_time: Optional[datetime.datetime] = None, end_time: Optional[datetime.datetime] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/machinealarms/alarmspermachine"
 
     # Construct parameters
     if start_time is not None:
         _params["startTime"] = _SERIALIZER.query("start_time", start_time, "iso-8601")
     if end_time is not None:
         _params["endTime"] = _SERIALIZER.query("end_time", end_time, "iso-8601")
-    if asset_id is not None:
-        _params["assetId"] = _SERIALIZER.query("asset_id", asset_id, "int")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_machine_alarms_list_alarm_severity_occurrences_request(
-    *,
-    start_time: Optional[datetime.datetime] = None,
-    end_time: Optional[datetime.datetime] = None,
-    asset_id: Optional[int] = None,
-    **kwargs: Any
+    *, start_time: Optional[datetime.datetime] = None, end_time: Optional[datetime.datetime] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/machinealarms/alarmtypeseverities"
 
     # Construct parameters
     if start_time is not None:
         _params["startTime"] = _SERIALIZER.query("start_time", start_time, "iso-8601")
     if end_time is not None:
         _params["endTime"] = _SERIALIZER.query("end_time", end_time, "iso-8601")
-    if asset_id is not None:
-        _params["assetId"] = _SERIALIZER.query("asset_id", asset_id, "int")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
@@ -14657,25 +14645,22 @@
 
     @distributed_trace
     def list_alarms_per_machine(
         self,
         *,
         start_time: Optional[datetime.datetime] = None,
         end_time: Optional[datetime.datetime] = None,
-        asset_id: Optional[int] = None,
         **kwargs: Any
     ) -> List[_models.MachineAlarmSummaryDto]:
         """list_alarms_per_machine.
 
         :keyword start_time: Default value is None.
         :paramtype start_time: ~datetime.datetime
         :keyword end_time: Default value is None.
         :paramtype end_time: ~datetime.datetime
-        :keyword asset_id: Default value is None.
-        :paramtype asset_id: int
         :return: list of MachineAlarmSummaryDto
         :rtype: list[~ignos.api.client.models.MachineAlarmSummaryDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -14688,15 +14673,14 @@
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[List[_models.MachineAlarmSummaryDto]] = kwargs.pop("cls", None)
 
         request = build_machine_alarms_list_alarms_per_machine_request(
             start_time=start_time,
             end_time=end_time,
-            asset_id=asset_id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
@@ -14718,25 +14702,22 @@
 
     @distributed_trace
     def list_alarm_severity_occurrences(
         self,
         *,
         start_time: Optional[datetime.datetime] = None,
         end_time: Optional[datetime.datetime] = None,
-        asset_id: Optional[int] = None,
         **kwargs: Any
     ) -> List[_models.MachineAlarmSeverityOccurenceDto]:
         """list_alarm_severity_occurrences.
 
         :keyword start_time: Default value is None.
         :paramtype start_time: ~datetime.datetime
         :keyword end_time: Default value is None.
         :paramtype end_time: ~datetime.datetime
-        :keyword asset_id: Default value is None.
-        :paramtype asset_id: int
         :return: list of MachineAlarmSeverityOccurenceDto
         :rtype: list[~ignos.api.client.models.MachineAlarmSeverityOccurenceDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -14749,15 +14730,14 @@
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[List[_models.MachineAlarmSeverityOccurenceDto]] = kwargs.pop("cls", None)
 
         request = build_machine_alarms_list_alarm_severity_occurrences_request(
             start_time=start_time,
             end_time=end_time,
-            asset_id=asset_id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
```

### Comparing `ignos-api-client-2023.5.22.5244/ignos/api/client/operations/_patch.py` & `ignos-api-client-2023.6.14.5376/ignos/api/client/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.5.22.5244/ignos_api_client.egg-info/SOURCES.txt` & `ignos-api-client-2023.6.14.5376/ignos_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.5.22.5244/setup.py` & `ignos-api-client-2023.6.14.5376/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 # coding: utf-8
 from setuptools import setup, find_packages
 
 
 PACKAGE_NAME = "ignos-api-client"
-version = "2023.5.22.5244"
+version = "2023.6.14.5376"
 setup(
     name=PACKAGE_NAME,
     version=version,
     description="ignos-api-client",
     author_email="",
     url="",
     keywords="azure, azure sdk",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "isodate<1.0.0,>=0.6.1",
-        "azure-core<2.0.0,>=1.24.0",
+        "azure-core<2.0.0,>=1.27.0",
     ],
     long_description="""\
     IgnosPortal.
     """,
 )
```

