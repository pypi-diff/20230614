# Comparing `tmp/langchainplus_sdk-0.0.8.tar.gz` & `tmp/langchainplus_sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchainplus_sdk-0.0.8.tar", max compression
+gzip compressed data, was "langchainplus_sdk-0.0.9.tar", max compression
```

## Comparing `langchainplus_sdk-0.0.8.tar` & `langchainplus_sdk-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     8124 2023-06-09 16:47:13.876598 langchainplus_sdk-0.0.8/README.md
--rw-r--r--   0        0        0      529 2023-06-09 16:47:13.876598 langchainplus_sdk-0.0.8/langchainplus_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 16:47:13.876598 langchainplus_sdk-0.0.8/langchainplus_sdk/cli/__init__.py
--rw-r--r--   0        0        0      363 2023-06-09 16:47:13.876598 langchainplus_sdk-0.0.8/langchainplus_sdk/cli/conf/nginx.conf
--rw-r--r--   0        0        0      315 2023-06-09 16:47:13.876598 langchainplus_sdk-0.0.8/langchainplus_sdk/cli/docker-compose.ngrok.yaml
--rw-r--r--   0        0        0     1198 2023-06-09 16:47:13.876598 langchainplus_sdk-0.0.8/langchainplus_sdk/cli/docker-compose.yaml
--rw-r--r--   0        0        0    12934 2023-06-09 16:47:13.876598 langchainplus_sdk-0.0.8/langchainplus_sdk/cli/main.py
--rw-r--r--   0        0        0       95 2023-06-09 16:47:13.876598 langchainplus_sdk-0.0.8/langchainplus_sdk/cli/ngrok_config.yaml
--rw-r--r--   0        0        0    21360 2023-06-09 16:47:13.876598 langchainplus_sdk-0.0.8/langchainplus_sdk/client.py
--rw-r--r--   0        0        0      250 2023-06-09 16:47:13.876598 langchainplus_sdk-0.0.8/langchainplus_sdk/evaluation/__init__.py
--rw-r--r--   0        0        0     1419 2023-06-09 16:47:13.876598 langchainplus_sdk-0.0.8/langchainplus_sdk/evaluation/evaluator.py
--rw-r--r--   0        0        0     1545 2023-06-09 16:47:13.876598 langchainplus_sdk-0.0.8/langchainplus_sdk/evaluation/string_evaluator.py
--rw-r--r--   0        0        0     4850 2023-06-09 16:47:13.876598 langchainplus_sdk-0.0.8/langchainplus_sdk/run_trees.py
--rw-r--r--   0        0        0     8657 2023-06-09 16:47:13.876598 langchainplus_sdk-0.0.8/langchainplus_sdk/schemas.py
--rw-r--r--   0        0        0     3271 2023-06-09 16:47:13.876598 langchainplus_sdk-0.0.8/langchainplus_sdk/utils.py
--rw-r--r--   0        0        0      879 2023-06-09 16:47:13.876598 langchainplus_sdk-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     8739 1970-01-01 00:00:00.000000 langchainplus_sdk-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     8124 2023-06-13 06:25:44.012021 langchainplus_sdk-0.0.9/README.md
+-rw-r--r--   0        0        0      529 2023-06-13 06:25:44.012021 langchainplus_sdk-0.0.9/langchainplus_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:25:44.012021 langchainplus_sdk-0.0.9/langchainplus_sdk/cli/__init__.py
+-rw-r--r--   0        0        0      363 2023-06-13 06:25:44.012021 langchainplus_sdk-0.0.9/langchainplus_sdk/cli/conf/nginx.conf
+-rw-r--r--   0        0        0      315 2023-06-13 06:25:44.012021 langchainplus_sdk-0.0.9/langchainplus_sdk/cli/docker-compose.ngrok.yaml
+-rw-r--r--   0        0        0     1061 2023-06-13 06:25:44.012021 langchainplus_sdk-0.0.9/langchainplus_sdk/cli/docker-compose.yaml
+-rw-r--r--   0        0        0    13476 2023-06-13 06:25:44.012021 langchainplus_sdk-0.0.9/langchainplus_sdk/cli/main.py
+-rw-r--r--   0        0        0    22810 2023-06-13 06:25:44.016021 langchainplus_sdk-0.0.9/langchainplus_sdk/client.py
+-rw-r--r--   0        0        0      250 2023-06-13 06:25:44.016021 langchainplus_sdk-0.0.9/langchainplus_sdk/evaluation/__init__.py
+-rw-r--r--   0        0        0     1419 2023-06-13 06:25:44.016021 langchainplus_sdk-0.0.9/langchainplus_sdk/evaluation/evaluator.py
+-rw-r--r--   0        0        0     1545 2023-06-13 06:25:44.016021 langchainplus_sdk-0.0.9/langchainplus_sdk/evaluation/string_evaluator.py
+-rw-r--r--   0        0        0     5437 2023-06-13 06:25:44.016021 langchainplus_sdk-0.0.9/langchainplus_sdk/run_trees.py
+-rw-r--r--   0        0        0     4897 2023-06-13 06:25:44.016021 langchainplus_sdk-0.0.9/langchainplus_sdk/schemas.py
+-rw-r--r--   0        0        0     3704 2023-06-13 06:25:44.016021 langchainplus_sdk-0.0.9/langchainplus_sdk/utils.py
+-rw-r--r--   0        0        0      879 2023-06-13 06:25:44.016021 langchainplus_sdk-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     8739 1970-01-01 00:00:00.000000 langchainplus_sdk-0.0.9/PKG-INFO
```

### Comparing `langchainplus_sdk-0.0.8/README.md` & `langchainplus_sdk-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.8/langchainplus_sdk/__init__.py` & `langchainplus_sdk-0.0.9/langchainplus_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.8/langchainplus_sdk/cli/main.py` & `langchainplus_sdk-0.0.9/langchainplus_sdk/cli/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import subprocess
 from contextlib import contextmanager
 from pathlib import Path
 from subprocess import CalledProcessError
 from typing import Dict, Generator, List, Mapping, Optional, Union, cast
 
 import requests
-import yaml
 
 from langchainplus_sdk.utils import get_runtime_environment
 
 logging.basicConfig(level=logging.INFO, format="%(message)s")
 logger = logging.getLogger(__name__)
 
 _DIR = Path(__file__).parent
@@ -103,14 +102,30 @@
         message = "ngrok failed to start correctly. "
         if auth_token is not None:
             message += "Please check that your authtoken is correct."
         raise ValueError(message)
     return exposed_url
 
 
+def _dumps_yaml(config: dict, depth: int = 0) -> str:
+    """Dump a dictionary to a YAML string without using any imports.
+
+    We can assume it's all strings, ints, or dictionaries, up to 3 layers deep
+    """
+    lines = []
+    prefix = "  " * depth
+    for key, value in config.items():
+        if isinstance(value, dict):
+            lines.append(f"{prefix}{key}:")
+            lines.append(_dumps_yaml(value, depth + 1))
+        else:
+            lines.append(f"{prefix}{key}: {value}")
+    return "\n".join(lines)
+
+
 @contextmanager
 def create_ngrok_config(
     auth_token: Optional[str] = None,
 ) -> Generator[Path, None, None]:
     """Create the ngrok configuration file."""
     config_path = _DIR / "ngrok_config.yaml"
     if config_path.exists():
@@ -120,25 +135,26 @@
             shutil.rmtree(config_path)
         else:
             config_path.unlink()
     ngrok_config = {
         "tunnels": {
             "langchain": {
                 "proto": "http",
-                "addr": "langchain-backend:8000",
+                "addr": "langchain-backend:1984",
             }
         },
         "version": "2",
         "region": "us",
     }
     if auth_token is not None:
         ngrok_config["authtoken"] = auth_token
     config_path = _DIR / "ngrok_config.yaml"
     with config_path.open("w") as f:
-        yaml.dump(ngrok_config, f)
+        s = _dumps_yaml(ngrok_config)
+        f.write(s)
     yield config_path
     # Delete the config file after use
     config_path.unlink(missing_ok=True)
 
 
 class PlusCommand:
     """Manage the LangChainPlus Tracing server."""
@@ -168,15 +184,15 @@
                 "up",
                 "--pull=always",
                 "--quiet-pull",
                 "--wait",
             ]
         )
         logger.info(
-            "langchain plus server is running at http://localhost.  To connect"
+            "langchain plus server is running at http://localhost:1984.  To connect"
             " locally, set the following environment variable"
             " when running your LangChain application."
         )
 
         logger.info("\tLANGCHAIN_TRACING_V2=true")
         self._open_browser("http://localhost")
 
@@ -199,15 +215,15 @@
                 ]
             )
         logger.info(
             "ngrok is running. You can view the dashboard at http://0.0.0.0:4040"
         )
         ngrok_url = get_ngrok_url(auth_token)
         logger.info(
-            "langchain plus server is running at http://localhost."
+            "langchain plus server is running at http://localhost:1984."
             " To connect remotely, set the following environment"
             " variable when running your LangChain application."
         )
         logger.info("\tLANGCHAIN_TRACING_V2=true")
         logger.info(f"\tLANGCHAIN_ENDPOINT={ngrok_url}")
         self._open_browser("http://0.0.0.0:4040")
         self._open_browser("http://localhost")
```

### Comparing `langchainplus_sdk-0.0.8/langchainplus_sdk/client.py` & `langchainplus_sdk-0.0.9/langchainplus_sdk/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from __future__ import annotations
 
+import json
 import logging
+import os
 import socket
 from datetime import datetime
 from io import BytesIO
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     Iterator,
     Mapping,
     Optional,
     Sequence,
     Tuple,
     Union,
+    cast,
 )
 from urllib.parse import urlsplit
 from uuid import UUID
 
 import requests
 from pydantic import BaseSettings, Field, root_validator
 from requests import Response
@@ -36,27 +39,25 @@
     Example,
     ExampleCreate,
     ExampleUpdate,
     Feedback,
     FeedbackCreate,
     FeedbackSourceBase,
     FeedbackSourceType,
-    ListFeedbackQueryParams,
-    ListRunsQueryParams,
     ModelFeedbackSource,
     Run,
-    RunCreate,
     RunTypeEnum,
     RunUpdate,
     TracerSession,
 )
 from langchainplus_sdk.utils import (
     LangChainPlusAPIError,
     LangChainPlusError,
     LangChainPlusUserError,
+    get_runtime_environment,
     raise_for_status_with_text,
     request_with_retries,
     xor_args,
 )
 
 if TYPE_CHECKING:
     import pandas as pd
@@ -82,22 +83,31 @@
         stop=stop_after_attempt(3),
         wait=wait_exponential(multiplier=1, min=4, max=10),
         retry=retry_if_exception_type(LangChainPlusAPIError),
         before_sleep=before_sleep_log(logger, logging.WARNING),
     )
 
 
+def _serialize_json(obj: Any) -> str:
+    if isinstance(obj, datetime):
+        return obj.isoformat()
+    elif isinstance(obj, UUID):
+        return str(obj)
+    raise TypeError("Type %s not serializable" % type(obj))
+
+
 class LangChainPlusClient(BaseSettings):
     """Client for interacting with the LangChain+ API."""
 
     api_key: Optional[str] = Field(default=None, env="LANGCHAIN_API_KEY")
     api_url: str = Field(default="http://localhost:1984", env="LANGCHAIN_ENDPOINT")
     retry_config: Mapping[str, Any] = Field(
         default_factory=_default_retry_config, exclude=True
     )
+    timeout_ms: int = Field(default=4000)
 
     @root_validator(pre=True)
     def validate_api_key_if_hosted(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """Verify API key is provided if url not localhost."""
         api_url: str = values.get("api_url", "http://localhost:1984")
         api_key: Optional[str] = values.get("api_key")
         if not _is_localhost(api_url):
@@ -131,15 +141,19 @@
 
     def _get_with_retries(
         self, path: str, params: Optional[Dict[str, Any]] = None
     ) -> Response:
         return request_with_retries(
             "get",
             f"{self.api_url}{path}",
-            request_kwargs={"params": params, "headers": self._headers},
+            request_kwargs={
+                "params": params,
+                "headers": self._headers,
+                "timeout": self.timeout_ms / 1000,
+            },
             retry_config=self.retry_config,
         )
 
     def upload_dataframe(
         self,
         df: pd.DataFrame,
         name: str,
@@ -185,76 +199,102 @@
         return Dataset(**result)
 
     def create_run(
         self,
         name: str,
         inputs: Dict[str, Any],
         run_type: Union[str, RunTypeEnum],
+        *,
+        execution_order: Optional[int] = None,
         **kwargs: Any,
-    ) -> Run:
+    ) -> None:
         """Persist a run to the LangChain+ API."""
-        run_create = RunCreate(
-            **kwargs,
-            name=name,
-            inputs=inputs,
-            run_type=run_type,
+        session_name = kwargs.pop(
+            "session_name", os.environ.get("LANGCHAIN_SESSION", "default")
         )
+        run_create = {
+            "session_name": session_name,
+            **kwargs,
+            "name": name,
+            "inputs": inputs,
+            "run_type": run_type,
+            "execution_order": execution_order,
+        }
+        run_extra = cast(dict, run_create.setdefault("extra", {}))
+        runtime = run_extra.setdefault("runtime", {})
+        runtime_env = get_runtime_environment()
+        run_extra["runtime"] = {**runtime_env, **runtime}
         headers = {**self._headers, "Accept": "application/json"}
         request_with_retries(
             "post",
             f"{self.api_url}/runs",
             request_kwargs={
-                "data": run_create.json(exclude_none=True),
+                "data": json.dumps(run_create, default=_serialize_json),
                 "headers": headers,
+                "timeout": self.timeout_ms / 1000,
             },
             retry_config=self.retry_config,
         )
-        return Run(**run_create.dict(exclude_none=True))
 
     def update_run(
         self,
         run_id: ID_TYPE,
         **kwargs: Any,
     ) -> None:
         """Update a run to the LangChain+ API."""
         run_update = RunUpdate(
             **kwargs,
         )
         headers = {**self._headers, "Accept": "application/json"}
         request_with_retries(
             "patch",
             f"{self.api_url}/runs/{run_id}",
-            request_kwargs={"data": run_update.json(), "headers": headers},
+            request_kwargs={
+                "data": run_update.json(),
+                "headers": headers,
+                "timeout": self.timeout_ms / 1000,
+            },
             retry_config=self.retry_config,
         )
 
     def read_run(self, run_id: ID_TYPE) -> Run:
         """Read a run from the LangChain+ API."""
         response = self._get_with_retries(f"/runs/{run_id}")
         return Run(**response.json())
 
     def list_runs(
         self,
         *,
         session_id: Optional[ID_TYPE] = None,
         session_name: Optional[str] = None,
         run_type: Optional[str] = None,
+        dataset_name: Optional[str] = None,
+        dataset_id: Optional[ID_TYPE] = None,
+        reference_example_id: Optional[ID_TYPE] = None,
         **kwargs: Any,
     ) -> Iterator[Run]:
         """List runs from the LangChain+ API."""
         if session_name is not None:
             if session_id is not None:
                 raise ValueError("Only one of session_id or session_name may be given")
             session_id = self.read_session(session_name=session_name).id
-        query_params = ListRunsQueryParams(
-            session_id=session_id, run_type=run_type, **kwargs
-        )
-        response = self._get_with_retries(
-            "/runs", params=query_params.dict(exclude_none=True)
-        )
+        if dataset_name is not None:
+            if dataset_id is not None:
+                raise ValueError("Only one of dataset_id or dataset_name may be given")
+            dataset_id = self.read_dataset(dataset_name=dataset_name).id
+        query_params = {
+            "session": session_id,
+            "run_type": run_type,
+            **kwargs,
+        }
+        if reference_example_id is not None:
+            query_params["reference_example"] = reference_example_id
+        if dataset_id is not None:
+            query_params["dataset"] = dataset_id
+        response = self._get_with_retries("/runs", params=query_params)
         yield from [Run(**run) for run in response.json()]
 
     def delete_run(self, run_id: ID_TYPE) -> None:
         """Delete a run from the LangChain+ API."""
         response = requests.delete(
             f"{self.api_url}/runs/{run_id}",
             headers=self._headers,
@@ -580,38 +620,37 @@
             correction=correction,
             comment=comment,
             feedback_source=feedback_source,
         )
         response = requests.post(
             self.api_url + "/feedback",
             headers={**self._headers, "Content-Type": "application/json"},
-            data=feedback.json(),
+            data=feedback.json(exclude_none=True),
         )
         raise_for_status_with_text(response)
-        return Feedback(**feedback.dict())
+        return Feedback(**response.json())
 
     def read_feedback(self, feedback_id: ID_TYPE) -> Feedback:
         """Read a feedback from the LangChain+ API."""
         response = self._get_with_retries(f"/feedback/{feedback_id}")
         return Feedback(**response.json())
 
     def list_feedback(
         self,
         *,
         run_ids: Optional[Sequence[ID_TYPE]] = None,
         **kwargs: Any,
     ) -> Iterator[Feedback]:
         """List the feedback objects on the LangChain+ API."""
-        params = ListFeedbackQueryParams(
-            run=run_ids,
+        params = {
+            "run": run_ids,
             **kwargs,
-        )
-        response = self._get_with_retries(
-            "/feedback", params=params.dict(exclude_none=True)
-        )
+        }
+
+        response = self._get_with_retries("/feedback", params=params)
         yield from [Feedback(**feedback) for feedback in response.json()]
 
     def delete_feedback(self, feedback_id: ID_TYPE) -> None:
         """Delete a feedback by ID."""
         response = requests.delete(
             f"{self.api_url}/feedback/{feedback_id}",
             headers=self._headers,
```

### Comparing `langchainplus_sdk-0.0.8/langchainplus_sdk/evaluation/evaluator.py` & `langchainplus_sdk-0.0.9/langchainplus_sdk/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.8/langchainplus_sdk/evaluation/string_evaluator.py` & `langchainplus_sdk-0.0.9/langchainplus_sdk/evaluation/string_evaluator.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.8/langchainplus_sdk/run_trees.py` & `langchainplus_sdk-0.0.9/langchainplus_sdk/run_trees.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 """Schemas for the langchainplus API."""
 from __future__ import annotations
 
 import logging
 import os
 from concurrent.futures import Future, ThreadPoolExecutor
 from datetime import datetime
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Optional, Union, cast
 from uuid import UUID, uuid4
 
 from pydantic import Field, root_validator, validator
 
 from langchainplus_sdk.client import LangChainPlusClient
-from langchainplus_sdk.schemas import RunBase, RunTypeEnum, infer_default_run_values
+from langchainplus_sdk.schemas import RunBase, RunTypeEnum
+from langchainplus_sdk.utils import get_runtime_environment
 
 logger = logging.getLogger(__name__)
 
 
 def _make_thread_pool() -> ThreadPoolExecutor:
     """Ensure a thread pool exists in the current context."""
     return ThreadPoolExecutor(max_workers=1)
 
 
 class RunTree(RunBase):
     """Run Schema with back-references for posting runs."""
 
     name: str
     id: UUID = Field(default_factory=uuid4)
+    start_time: datetime = Field(default_factory=datetime.utcnow)
     parent_run: Optional[RunTree] = Field(default=None, exclude=True)
     child_runs: List[RunTree] = Field(
         default_factory=list,
         exclude={"__all__": {"parent_run_id"}},
     )
     session_name: str = Field(
         default_factory=lambda: os.environ.get("LANGCHAIN_SESSION", "default")
     )
     session_id: Optional[UUID] = Field(default=None)
     execution_order: int = 1
     child_execution_order: int = Field(default=1, exclude=True)
+    extra: Dict = Field(default_factory=dict)
     client: LangChainPlusClient = Field(
         default_factory=LangChainPlusClient, exclude=True
     )
     executor: ThreadPoolExecutor = Field(
         default_factory=_make_thread_pool, exclude=True
     )
 
@@ -53,17 +56,25 @@
         if v._shutdown:
             raise ValueError("Executor has been shutdown.")
         return v
 
     @root_validator(pre=True)
     def infer_defaults(cls, values: dict) -> dict:
         """Assign name to the run."""
-        values = infer_default_run_values(values)
-        if values.get("child_runs") is None:
-            values["child_runs"] = []
+        if "serialized" not in values:
+            values["serialized"] = {"name": values["name"]}
+        if "execution_order" not in values:
+            values["execution_order"] = 1
+        if "child_execution_order" not in values:
+            values["child_execution_order"] = values["execution_order"]
+        if values.get("parent_run") is not None:
+            values["parent_run_id"] = values["parent_run"].id
+        extra = cast(dict, values.setdefault("extra", {}))
+        runtime = cast(dict, extra.setdefault("runtime", {}))
+        runtime.update(get_runtime_environment())
         return values
 
     def end(
         self,
         *,
         outputs: Optional[Dict] = None,
         error: Optional[str] = None,
@@ -105,15 +116,15 @@
             serialized=serialized_,
             inputs=inputs or {},
             outputs=outputs or {},
             error=error,
             run_type=run_type,
             reference_example_id=reference_example_id,
             start_time=start_time or datetime.utcnow(),
-            end_time=end_time or datetime.utcnow(),
+            end_time=end_time,
             execution_order=execution_order,
             child_execution_order=execution_order,
             extra=extra or {},
             parent_run=self,
             session_name=self.session_name,
             client=self.client,
             executor=self.executor,
```

### Comparing `langchainplus_sdk-0.0.8/langchainplus_sdk/utils.py` & `langchainplus_sdk-0.0.9/langchainplus_sdk/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Generic utility functions."""
 import platform
 from functools import lru_cache
 from typing import Any, Callable, Mapping, Tuple
 
 import requests
-from requests import HTTPError, Response
+from requests import ConnectionError, HTTPError, Response
 from tenacity import Retrying
 
 
 class LangChainPlusAPIError(Exception):
     """An error occurred while communicating with the LangChain API."""
 
 
@@ -16,37 +16,47 @@
     """An error occurred while communicating with the LangChain API."""
 
 
 class LangChainPlusError(Exception):
     """An error occurred while communicating with the LangChain API."""
 
 
+class LangChainPlusConnectionError(Exception):
+    """Couldn't connect to the LC+ API."""
+
+
 def request_with_retries(
     request_method: str, url: str, request_kwargs: Mapping, retry_config: Mapping
 ) -> Response:
     for attempt in Retrying(**retry_config):
         with attempt:
             try:
                 response = requests.request(request_method, url, **request_kwargs)
                 raise_for_status_with_text(response)
                 return response
             except HTTPError as e:
                 if response is not None and response.status_code == 500:
                     raise LangChainPlusAPIError(
-                        f"Failed to {request_method} {url} from LangChain+ API. {e}"
+                        f"Server error caused failure to {request_method} {url} in"
+                        f" LangChain+ API. {e}"
                     )
                 else:
                     raise LangChainPlusUserError(
-                        f"Failed to {request_method} {url} from LangChain+ API. {e}"
+                        f"Failed to {request_method} {url} in LangChain+ API. {e}"
                     )
+            except ConnectionError as e:
+                raise LangChainPlusConnectionError(
+                    f"Connection error caused failure to {request_method} {url}"
+                    "  in LangChain+ API. Please confirm your LANGCHAIN_ENDPOINT."
+                ) from e
             except Exception as e:
                 raise LangChainPlusError(
-                    f"Failed to {request_method} {url} from LangChain+ API. {e}"
+                    f"Failed to {request_method} {url} in LangChain+ API. {e}"
                 ) from e
-    raise LangChainPlusError(f"Failed to {request_method}  {url} from LangChain+ API.")
+    raise LangChainPlusError(f"Failed to {request_method}  {url} in LangChain+ API. ")
 
 
 def xor_args(*arg_groups: Tuple[str, ...]) -> Callable:
     """Validate specified keyword args are mutually exclusive."""
 
     def decorator(func: Callable) -> Callable:
         def wrapper(*args: Any, **kwargs: Any) -> Callable:
```

### Comparing `langchainplus_sdk-0.0.8/pyproject.toml` & `langchainplus_sdk-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchainplus-sdk"
-version = "0.0.8"
+version = "0.0.9"
 description = "Client library to connect to the LangChainPlus LLM Tracing and Evaluation Platform."
 authors = ["LangChain"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "langchainplus_sdk"}]
 
 [tool.poetry.scripts]
```

### Comparing `langchainplus_sdk-0.0.8/PKG-INFO` & `langchainplus_sdk-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchainplus-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Client library to connect to the LangChainPlus LLM Tracing and Evaluation Platform.
 License: MIT
 Author: LangChain
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

