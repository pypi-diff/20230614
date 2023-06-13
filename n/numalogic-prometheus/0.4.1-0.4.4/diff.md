# Comparing `tmp/numalogic_prometheus-0.4.1.tar.gz` & `tmp/numalogic_prometheus-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numalogic_prometheus-0.4.1.tar", max compression
+gzip compressed data, was "numalogic_prometheus-0.4.4.tar", max compression
```

## Comparing `numalogic_prometheus-0.4.1.tar` & `numalogic_prometheus-0.4.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-05-25 17:27:12.581593 numalogic_prometheus-0.4.1/LICENSE
--rw-r--r--   0        0        0      839 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/__init__.py
--rw-r--r--   0        0        0     1395 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/_config.py
--rw-r--r--   0        0        0      561 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/_constants.py
--rw-r--r--   0        0        0        0 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/clients/__init__.py
--rw-r--r--   0        0        0     3565 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/clients/prometheus.py
--rw-r--r--   0        0        0     1316 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/clients/redis.py
--rw-r--r--   0        0        0     2515 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/clients/sentinel.py
--rw-r--r--   0        0        0     2145 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/configs/config.yaml
--rw-r--r--   0        0        0     1841 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/default-configs/config.yaml
--rw-r--r--   0        0        0      337 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/default-configs/numalogic_config.yaml
--rw-r--r--   0        0        0      382 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/default-configs/pipeline_config.yaml
--rw-r--r--   0        0        0     4483 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/entities.py
--rw-r--r--   0        0        0      954 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/factory.py
--rw-r--r--   0        0        0     7002 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/tools.py
--rw-r--r--   0        0        0      366 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/udf/__init__.py
--rw-r--r--   0        0        0      747 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/udf/filter.py
--rw-r--r--   0        0        0     4339 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/udf/inference.py
--rw-r--r--   0        0        0     6836 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/udf/postprocess.py
--rw-r--r--   0        0        0     2768 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/udf/preprocess.py
--rw-r--r--   0        0        0     4193 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/udf/threshold.py
--rw-r--r--   0        0        0     4148 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/udf/window.py
--rw-r--r--   0        0        0      134 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/udsink/__init__.py
--rw-r--r--   0        0        0     6965 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/udsink/train.py
--rw-r--r--   0        0        0     8095 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/udsink/train_rollout.py
--rw-r--r--   0        0        0     5935 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/watcher.py
--rw-r--r--   0        0        0     1550 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 numalogic_prometheus-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-13 22:42:27.629992 numalogic_prometheus-0.4.4/LICENSE
+-rw-r--r--   0        0        0     1696 2023-06-13 22:42:27.633992 numalogic_prometheus-0.4.4/numaprom/__init__.py
+-rw-r--r--   0        0        0     1400 2023-06-13 22:42:27.633992 numalogic_prometheus-0.4.4/numaprom/_config.py
+-rw-r--r--   0        0        0      561 2023-06-13 22:42:27.633992 numalogic_prometheus-0.4.4/numaprom/_constants.py
+-rw-r--r--   0        0        0        0 2023-06-13 22:42:27.633992 numalogic_prometheus-0.4.4/numaprom/clients/__init__.py
+-rw-r--r--   0        0        0     3536 2023-06-13 22:42:27.633992 numalogic_prometheus-0.4.4/numaprom/clients/prometheus.py
+-rw-r--r--   0        0        0     1291 2023-06-13 22:42:27.633992 numalogic_prometheus-0.4.4/numaprom/clients/redis.py
+-rw-r--r--   0        0        0     2519 2023-06-13 22:42:27.633992 numalogic_prometheus-0.4.4/numaprom/clients/sentinel.py
+-rw-r--r--   0        0        0     2145 2023-06-13 22:42:27.633992 numalogic_prometheus-0.4.4/numaprom/configs/config.yaml
+-rw-r--r--   0        0        0     1841 2023-06-13 22:42:27.633992 numalogic_prometheus-0.4.4/numaprom/default-configs/config.yaml
+-rw-r--r--   0        0        0      337 2023-06-13 22:42:27.633992 numalogic_prometheus-0.4.4/numaprom/default-configs/numalogic_config.yaml
+-rw-r--r--   0        0        0      382 2023-06-13 22:42:27.633992 numalogic_prometheus-0.4.4/numaprom/default-configs/pipeline_config.yaml
+-rw-r--r--   0        0        0     4496 2023-06-13 22:42:27.633992 numalogic_prometheus-0.4.4/numaprom/entities.py
+-rw-r--r--   0        0        0      954 2023-06-13 22:42:27.633992 numalogic_prometheus-0.4.4/numaprom/factory.py
+-rw-r--r--   0        0        0     7169 2023-06-13 22:42:27.633992 numalogic_prometheus-0.4.4/numaprom/tools.py
+-rw-r--r--   0        0        0      366 2023-06-13 22:42:27.633992 numalogic_prometheus-0.4.4/numaprom/udf/__init__.py
+-rw-r--r--   0        0        0      720 2023-06-13 22:42:27.633992 numalogic_prometheus-0.4.4/numaprom/udf/filter.py
+-rw-r--r--   0        0        0     4687 2023-06-13 22:42:27.633992 numalogic_prometheus-0.4.4/numaprom/udf/inference.py
+-rw-r--r--   0        0        0     7309 2023-06-13 22:42:27.633992 numalogic_prometheus-0.4.4/numaprom/udf/postprocess.py
+-rw-r--r--   0        0        0     3012 2023-06-13 22:42:27.633992 numalogic_prometheus-0.4.4/numaprom/udf/preprocess.py
+-rw-r--r--   0        0        0     4484 2023-06-13 22:42:27.633992 numalogic_prometheus-0.4.4/numaprom/udf/threshold.py
+-rw-r--r--   0        0        0     4217 2023-06-13 22:42:27.633992 numalogic_prometheus-0.4.4/numaprom/udf/window.py
+-rw-r--r--   0        0        0      134 2023-06-13 22:42:27.633992 numalogic_prometheus-0.4.4/numaprom/udsink/__init__.py
+-rw-r--r--   0        0        0     7399 2023-06-13 22:42:27.633992 numalogic_prometheus-0.4.4/numaprom/udsink/train.py
+-rw-r--r--   0        0        0     8543 2023-06-13 22:42:27.633992 numalogic_prometheus-0.4.4/numaprom/udsink/train_rollout.py
+-rw-r--r--   0        0        0     6016 2023-06-13 22:42:27.633992 numalogic_prometheus-0.4.4/numaprom/watcher.py
+-rw-r--r--   0        0        0     1537 2023-06-13 22:42:27.637992 numalogic_prometheus-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     1065 1970-01-01 00:00:00.000000 numalogic_prometheus-0.4.4/PKG-INFO
```

### Comparing `numalogic_prometheus-0.4.1/LICENSE` & `numalogic_prometheus-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.1/numaprom/_config.py` & `numalogic_prometheus-0.4.4/numaprom/_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,46 @@
-from typing import List
 from omegaconf import MISSING
 from dataclasses import dataclass, field
 
 from numalogic.config import NumalogicConf
 
 
 @dataclass
 class UnifiedConf:
     unified_metric_name: str
-    unified_metrics: List[str]
+    unified_metrics: list[str]
     unified_strategy: str = "max"
-    unified_weights: List[float] = field(default_factory=list)
+    unified_weights: list[float] = field(default_factory=list)
 
 
 @dataclass
 class MetricConf:
     metric: str = "default"
-    composite_keys: List[str] = field(default_factory=lambda: ["namespace", "name"])
+    composite_keys: list[str] = field(default_factory=lambda: ["namespace", "name"])
     static_threshold: int = 3
     static_threshold_wt: float = 0.0
-    train_hours: int = 36
+    train_hours: int = 24 * 8  # 8 days worth of data
     min_train_size: int = 2000
-    retrain_freq_hr: int = 8
+    retrain_freq_hr: int = 24
     resume_training: bool = False
     scrape_interval: int = 30
     numalogic_conf: NumalogicConf = MISSING
 
 
 @dataclass
 class AppConf:
     app: str = "default"
     namespace: str = "default"
-    metric_configs: List[MetricConf] = field(default_factory=lambda: [MetricConf()])
-    unified_configs: List[UnifiedConf] = field(default_factory=list)
+    metric_configs: list[MetricConf] = field(default_factory=lambda: [MetricConf()])
+    unified_configs: list[UnifiedConf] = field(default_factory=list)
 
 
 @dataclass
 class DataConf:
-    configs: List[AppConf]
+    configs: list[AppConf]
 
 
 @dataclass
 class RedisConf:
     host: str
     port: int
     expiry: int = 300
```

### Comparing `numalogic_prometheus-0.4.1/numaprom/_constants.py` & `numalogic_prometheus-0.4.4/numaprom/_constants.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.1/numaprom/clients/prometheus.py` & `numalogic_prometheus-0.4.4/numaprom/clients/prometheus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 import requests
 import numpy as np
 import pandas as pd
-from typing import Dict, List, Optional
+from typing import Optional
 
-from numaprom import get_logger
-
-_LOGGER = get_logger(__name__)
+from numaprom import LOGGER
 
 
 class Prometheus:
     def __init__(self, prometheus_server: str):
         self.PROMETHEUS_SERVER = prometheus_server
 
     def query_metric(
         self,
         metric_name: str,
         start: float,
         end: float,
-        labels_map: Dict = None,
-        return_labels: List[str] = None,
+        labels_map: dict = None,
+        return_labels: list[str] = None,
         step: int = 30,
     ) -> pd.DataFrame:
         query = metric_name
         if labels_map:
             label_list = [str(key + "=" + "'" + labels_map[key] + "'") for key in labels_map]
             query = metric_name + "{" + ",".join(label_list) + "}"
 
-        _LOGGER.debug("Prometheus Query: %s", query)
+        LOGGER.debug("Prometheus Query: {query}", query=query)
 
         if end < start:
             raise ValueError("end_time must not be before start_time")
 
         result = self.query_range(query, start, end, step)
 
         arr = np.array(result["values"])
@@ -44,15 +42,15 @@
                     df[label] = data[label]
 
         if not df.empty:
             df.set_index("timestamp", inplace=True)
             df.index = pd.to_datetime(df.index.astype(int), unit="s")
         return df
 
-    def query_range(self, query: str, start: float, end: float, step: int = 30) -> Optional[Dict]:
+    def query_range(self, query: str, start: float, end: float, step: int = 30) -> Optional[dict]:
         results = {}
         data_points = (end - start) / step
         temp_start = start
         while data_points > 11000:
             temp_end = temp_start + 11000 * step
             response = self.query_range_limit(query, temp_start, temp_end, step)
             if results:
@@ -63,46 +61,46 @@
             data_points = (end - temp_start) / step
 
         if data_points > 0:
             response = self.query_range_limit(query, temp_start, end)
             if results:
                 results["values"] = results["values"] + response["values"]
             else:
-                _LOGGER.debug("Prometheus query has returned empty results.")
+                LOGGER.debug("Prometheus query has returned empty results.")
                 results = response
 
         return results
 
     def query_range_limit(
         self, query: str, start: float, end: float, step: int = 30
-    ) -> Optional[Dict]:
+    ) -> Optional[dict]:
         data_points = (end - start) / step
 
         if data_points > 11000:
-            _LOGGER.info("Limit query only supports 11,000 data points")
+            LOGGER.info("Limit query only supports 11,000 data points")
             return None
 
         results = None
         try:
             response = requests.get(
                 self.PROMETHEUS_SERVER + "/api/v1/query_range",
                 params={"query": query, "start": start, "end": end, "step": f"{step}s"},
             )
             results = response.json()["data"]["result"][0]
         except Exception as ex:
-            _LOGGER.exception("Prometheus error: %r", ex)
+            LOGGER.exception("Prometheus error: {err}", err=ex)
         return results
 
-    def query(self, query: str) -> Optional[Dict]:
+    def query(self, query: str) -> Optional[dict]:
         results = []
         try:
             response = requests.get(
                 self.PROMETHEUS_SERVER + "/api/v1/query", params={"query": query}
             )
             if response:
                 results = response.json()["data"]["result"]
             else:
-                _LOGGER.debug("Prometheus query has returned empty results.")
+                LOGGER.debug("Prometheus query has returned empty results.")
         except Exception as ex:
-            _LOGGER.exception("error: %r", ex)
+            LOGGER.exception("error: {err}", err=ex)
 
         return results
```

### Comparing `numalogic_prometheus-0.4.1/numaprom/clients/redis.py` & `numalogic_prometheus-0.4.4/numaprom/clients/redis.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from typing import Optional
 
 from redis.cluster import RedisCluster
 from redis.backoff import ExponentialBackoff
 from redis.exceptions import RedisClusterException, RedisError
 from redis.retry import Retry
 
-from numaprom import get_logger
+from numaprom import LOGGER
 from numaprom.tools import is_host_reachable
 
-_LOGGER = get_logger(__name__)
+
 redis_client: Optional[RedisCluster] = None
 
 
 def get_redis_client(
     host: str, port: str, password: str = None, decode_responses: bool = True, recreate=False
 ) -> RedisCluster:
     global redis_client
@@ -26,18 +26,18 @@
         "port": port,
         "password": password,
         "decode_responses": decode_responses,
         "skip_full_coverage_check": True,
         "dynamic_startup_nodes": False,
         "cluster_error_retry_attempts": 3,
     }
-    _LOGGER.info("Redis params: %s", json.dumps(redis_params, indent=4))
+    LOGGER.info("Redis params: {param}", param=json.dumps(redis_params, indent=4))
 
     if not is_host_reachable(host, port):
-        _LOGGER.error("Redis Cluster is unreachable after retries!")
+        LOGGER.error("Redis Cluster is unreachable after retries!")
 
     retry = Retry(
         ExponentialBackoff(cap=2, base=1),
         3,
         supported_errors=(ConnectionError, TimeoutError, RedisClusterException, RedisError),
     )
     redis_client = RedisCluster(**redis_params, retry=retry)
```

### Comparing `numalogic_prometheus-0.4.1/numaprom/clients/sentinel.py` & `numalogic_prometheus-0.4.4/numaprom/clients/sentinel.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,42 +3,43 @@
 
 from numalogic.tools.types import redis_client_t
 from redis.backoff import ExponentialBackoff
 from redis.exceptions import RedisClusterException, RedisError
 from redis.retry import Retry
 from redis.sentinel import Sentinel, MasterNotFoundError
 
-from numaprom import get_logger
+from numaprom import LOGGER
 from numaprom._config import RedisConf
 from numaprom.watcher import ConfigManager
 
-_LOGGER = get_logger(__name__)
+
 SENTINEL_MASTER_CLIENT: Optional[redis_client_t] = None
 
 
 def get_redis_client(
     host: str,
     port: int,
     password: str,
     mastername: str,
     decode_responses: bool = False,
     recreate: bool = False,
 ) -> redis_client_t:
-    """
-    Return a master redis client for sentinel connections, with retry.
+    """Return a master redis client for sentinel connections, with retry.
 
     Args:
+    ----
         host: Redis host
         port: Redis port
         password: Redis password
         mastername: Redis sentinel master name
         decode_responses: Whether to decode responses
         recreate: Whether to flush and recreate the client
 
-    Returns:
+    Returns
+    -------
         Redis client instance
     """
     global SENTINEL_MASTER_CLIENT
 
     if not recreate and SENTINEL_MASTER_CLIENT:
         return SENTINEL_MASTER_CLIENT
 
@@ -55,32 +56,33 @@
     )
     sentinel_args = {
         "sentinels": [(host, port)],
         "socket_timeout": 0.1,
         "decode_responses": decode_responses,
     }
 
-    _LOGGER.info("Sentinel redis params: %s", sentinel_args)
+    LOGGER.info("Sentinel redis params: {args}", args=sentinel_args)
 
     sentinel = Sentinel(
         **sentinel_args, sentinel_kwargs=dict(password=password), password=password, retry=retry
     )
     SENTINEL_MASTER_CLIENT = sentinel.master_for(mastername)
     return SENTINEL_MASTER_CLIENT
 
 
 def get_redis_client_from_conf(redis_conf: RedisConf = None, **kwargs) -> redis_client_t:
-    """
-    Return a master redis client from config for sentinel connections, with retry.
+    """Return a master redis client from config for sentinel connections, with retry.
 
     Args:
+    ----
         redis_conf: RedisConf object with host, port, master_name, etc.
         **kwargs: Additional arguments to pass to get_redis_client.
 
-    Returns:
+    Returns
+    -------
         Redis client instance
     """
     if not redis_conf:
         redis_conf = ConfigManager.get_redis_config()
 
     return get_redis_client(
         redis_conf.host,
```

### Comparing `numalogic_prometheus-0.4.1/numaprom/configs/config.yaml` & `numalogic_prometheus-0.4.4/numaprom/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.1/numaprom/default-configs/config.yaml` & `numalogic_prometheus-0.4.4/numaprom/default-configs/config.yaml`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.1/numaprom/entities.py` & `numalogic_prometheus-0.4.4/numaprom/entities.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from copy import copy
 from dataclasses import dataclass, field
 from enum import Enum
-from typing import List, Dict, Optional, Any, Union, OrderedDict, TypeVar
+from typing import Optional, Any, Union, TypeVar
+from collections import OrderedDict
 
 import numpy as np
 import numpy.typing as npt
 import orjson
 from typing_extensions import Self
 
-Vector = List[float]
-Matrix = Union[Vector, List[Vector], npt.NDArray[float]]
+Vector = list[float]
+Matrix = Union[Vector, list[Vector], npt.NDArray[float]]
 
 
 class Status(str, Enum):
     RAW = "raw"
     EXTRACTED = "extracted"
     PRE_PROCESSED = "pre_processed"
     INFERRED = "inferred"
@@ -45,17 +46,17 @@
     header: Header = Header.TRAIN_REQUEST
 
 
 @dataclass(repr=False)
 class StreamPayload(_BasePayload):
     win_raw_arr: Matrix
     win_arr: Matrix
-    win_ts_arr: List[str]
+    win_ts_arr: list[str]
     status: Status = Status.RAW
-    metadata: Dict[str, Any] = field(default_factory=dict)
+    metadata: dict[str, Any] = field(default_factory=dict)
     header: Header = Header.MODEL_INFERENCE
 
     @property
     def start_ts(self) -> str:
         return self.win_ts_arr[0]
 
     @property
@@ -63,15 +64,15 @@
         return self.win_ts_arr[-1]
 
     def get_stream_array(self, original=False) -> npt.NDArray[float]:
         if original:
             return np.asarray(self.win_raw_arr)
         return np.asarray(self.win_arr)
 
-    def get_metadata(self, key: str) -> Dict[str, Any]:
+    def get_metadata(self, key: str) -> dict[str, Any]:
         return copy(self.metadata[key])
 
     def set_win_arr(self, arr: Matrix) -> None:
         self.win_arr = arr
 
     def set_status(self, status: Status) -> None:
         self.status = status
@@ -80,16 +81,16 @@
         self.header = header
 
     def set_metadata(self, key: str, value) -> None:
         self.metadata[key] = value
 
     def __repr__(self) -> str:
         return (
-            "header: %s, win_raw_arr: %s, win_arr: %s, win_ts_arr: %s, composite_keys: %s, metadata: %s}"
-            % (
+            "header: {}, win_raw_arr: {}, win_arr: {}, win_ts_arr: {}, composite_keys:"
+            " {}, metadata: {}}}".format(
                 self.header,
                 list(self.win_raw_arr),
                 list(self.win_arr),
                 self.win_ts_arr,
                 self.composite_keys,
                 self.metadata,
             )
@@ -118,15 +119,15 @@
 class PrometheusPayload:
     timestamp_ms: int
     name: str
     namespace: str
     subsystem: Optional[str]
     type: str
     value: float
-    labels: Dict[str, str]
+    labels: dict[str, str]
 
     def as_json(self) -> bytes:
         return orjson.dumps(
             {
                 "TimestampMs": self.timestamp_ms,
                 "Name": self.name,
                 "Namespace": self.namespace,
@@ -148,17 +149,16 @@
             type=obj["Type"],
             value=obj["Value"],
             labels=obj["Labels"],
         )
 
     def __repr__(self) -> str:
         return (
-            "{timestamp_ms: %s, name: %s, namespace: %s, "
-            "subsystem: %s, type: %s, value: %s, labels: %s}"
-            % (
+            "{{timestamp_ms: {}, name: {}, namespace: {}, "
+            "subsystem: {}, type: {}, value: {}, labels: {}}}".format(
                 self.timestamp_ms,
                 self.name,
                 self.namespace,
                 self.subsystem,
                 self.type,
                 self.value,
                 self.labels,
```

### Comparing `numalogic_prometheus-0.4.1/numaprom/factory.py` & `numalogic_prometheus-0.4.4/numaprom/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.1/numaprom/tools.py` & `numalogic_prometheus-0.4.4/numaprom/tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 import socket
 import time
 from collections import OrderedDict
 from datetime import timedelta, datetime
 from functools import wraps
 from json import JSONDecodeError
-from typing import List
 
 import numpy as np
 import pandas as pd
 import pytz
 from numalogic.config import PostprocessFactory
 from numalogic.models.threshold import SigmoidThreshold
 from pynumaflow.function import Messages, Message
-
-from numaprom import get_logger, MetricConf
+from numaprom import LOGGER, MetricConf
 from numaprom.clients.prometheus import Prometheus
 from numaprom.entities import TrainerPayload, StreamPayload
 from numaprom.watcher import ConfigManager
 
-_LOGGER = get_logger(__name__)
-
 
 def catch_exception(func):
     @wraps(func)
     def inner_function(*args, **kwargs):
         try:
             return func(*args, **kwargs)
         except JSONDecodeError as err:
-            _LOGGER.exception("Error in json decode for %s: %r", func.__name__, err)
+            LOGGER.exception("Error in json decode for {name}: {err}", name=func.__name__, err=err)
         except Exception as ex:
-            _LOGGER.exception("Error in %s: %r", func.__name__, ex)
+            LOGGER.exception("Error in {name}: {err}", name=func.__name__, err=ex)
 
     return inner_function
 
 
 def msgs_forward(handler_func):
     @wraps(handler_func)
     def inner_function(*args, **kwargs):
@@ -74,15 +70,15 @@
             else:
                 msgs.append(Message.to_drop())
         return msgs
 
     return inner_function
 
 
-def create_composite_keys(msg: dict, keys: List[str]) -> OrderedDict:
+def create_composite_keys(msg: dict, keys: list[str]) -> OrderedDict:
     labels = msg.get("labels")
     result = OrderedDict()
     for k in keys:
         if k in msg:
             result[k] = msg[k]
         if k in labels:
             result[k] = labels[k]
@@ -102,21 +98,24 @@
     assert max_retries >= 1, "Max retries has to be at least 1"
 
     while retries < max_retries:
         try:
             get_ipv4_by_hostname(hostname, port)
         except socket.gaierror as ex:
             retries += 1
-            _LOGGER.warning(
-                "Failed to resolve hostname: %s: error: %r", hostname, ex, exc_info=True
+            LOGGER.warning(
+                "Failed to resolve hostname: {hostname}: error: {ex}",
+                hostname=hostname,
+                ex=ex,
+                exc_info=True,
             )
             time.sleep(sleep_sec)
         else:
             return True
-    _LOGGER.error("Failed to resolve hostname: %s even after retries!")
+    LOGGER.error("Failed to resolve hostname: {retries} even after retries!", retries=retries)
     return False
 
 
 def fetch_data(
     payload: TrainerPayload,
     metric_config: MetricConf,
     labels: dict,
@@ -134,109 +133,108 @@
         metric_name=payload.composite_keys["name"],
         labels_map=labels,
         return_labels=return_labels,
         start=start_dt.timestamp(),
         end=end_dt.timestamp(),
         step=metric_config.scrape_interval,
     )
-    _LOGGER.info(
-        "%s - Time taken to fetch data: %s, for df shape: %s",
-        payload.uuid,
-        time.time() - _start_time,
-        df.shape,
+    LOGGER.info(
+        "{uuid} - Time taken to fetch data: {time}, for df shape: {shape}",
+        uuid=payload.uuid,
+        time=time.time() - _start_time,
+        shape=df.shape,
     )
     return df
 
 
 def calculate_static_thresh(payload: StreamPayload, upper_limit: float):
-    """
-    Calculates anomaly scores using static thresholding.
-    """
+    """Calculates anomaly scores using static thresholding."""
     x = payload.get_stream_array(original=True)
     static_clf = SigmoidThreshold(upper_limit=upper_limit)
     static_scores = static_clf.score_samples(x)
     return static_scores
 
 
 class WindowScorer:
-    """
-    Class to calculate the final anomaly scores for the window.
+    """Class to calculate the final anomaly scores for the window.
 
     Args:
+    ----
         metric_conf: MetricConf instance
     """
 
     __slots__ = ("static_wt", "static_limit", "model_wt", "postproc_clf")
 
     def __init__(self, metric_conf: MetricConf):
         self.static_wt = metric_conf.static_threshold_wt
         self.static_limit = metric_conf.static_threshold
         self.model_wt = 1.0 - self.static_wt
 
         postproc_factory = PostprocessFactory()
         self.postproc_clf = postproc_factory.get_instance(metric_conf.numalogic_conf.postprocess)
 
     def get_final_winscore(self, payload: StreamPayload) -> float:
-        """
-        Returns the final normalized window score.
+        """Returns the final normalized window score.
 
         Performs soft voting ensembling if valid static threshold
         weight found in config.
 
         Args:
+        ----
             payload: StreamPayload instance
 
-        Returns:
+        Returns
+        -------
             Final score for the window
         """
         norm_winscore = self.get_winscore(payload)
 
         if not self.static_wt:
             return norm_winscore
 
         norm_static_winscore = self.get_static_winscore(payload)
         ensemble_score = (self.static_wt * norm_static_winscore) + (self.model_wt * norm_winscore)
 
-        _LOGGER.debug(
-            "%s - Model score: %s, Static score: %s, Static wt: %s",
-            payload.uuid,
-            norm_winscore,
-            norm_static_winscore,
-            self.static_wt,
+        LOGGER.debug(
+            "{uuid} - Model score: {m_score}, Static score: {s_score}, Static wt: {wt}",
+            uuid=payload.uuid,
+            m_score=norm_winscore,
+            s_score=norm_static_winscore,
+            wt=self.static_wt,
         )
 
         return ensemble_score
 
     def get_static_winscore(self, payload: StreamPayload) -> float:
-        """
-        Returns the normalized window score
+        """Returns the normalized window score
         calculated using the static threshold estimator.
 
         Args:
+        ----
             payload: StreamPayload instance
 
-        Returns:
+        Returns
+        -------
             Score for the window
         """
         static_scores = calculate_static_thresh(payload, self.static_limit)
         static_winscore = np.mean(static_scores)
         return self.postproc_clf.transform(static_winscore)
 
     def get_winscore(self, payload: StreamPayload):
-        """
-        Returns the normalized window score
+        """Returns the normalized window score.
 
         Args:
+        ----
             payload: StreamPayload instance
 
-        Returns:
+        Returns
+        -------
             Score for the window
         """
         scores = payload.get_stream_array()
         winscore = np.mean(scores)
         return self.postproc_clf.transform(winscore)
 
     def adjust_weights(self):
-        """
-        Adjust the soft voting weights depending on the streaming input.
-        """
+        """Adjust the soft voting weights depending on the streaming input."""
         raise NotImplementedError
```

### Comparing `numalogic_prometheus-0.4.1/numaprom/udf/filter.py` & `numalogic_prometheus-0.4.4/numaprom/udf/filter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 import os
 import json
 from typing import Optional
 
 from pynumaflow.function import Messages, Datum
 
-from numaprom import get_logger
+from numaprom import LOGGER
 from numaprom.tools import catch_exception, msg_forward
 
-_LOGGER = get_logger(__name__)
-
 
 @catch_exception
 @msg_forward
 def metric_filter(_: list[str], datum: Datum) -> Optional[Messages]:
-    """
-    UDF to filter metrics by labels
-    """
-    _LOGGER.debug("Received Msg: %s ", datum.value)
+    """UDF to filter metrics by labels."""
+    LOGGER.debug("Received Msg: {value} ", value=datum.value)
 
     msg = datum.value.decode("utf-8")
     data = json.loads(msg)
 
     label = os.getenv("LABEL")
     label_values = json.loads(os.getenv("LABEL_VALUES", "[]"))
 
     if label in data["labels"] and data["labels"][label] not in label_values:
         return None
 
-    _LOGGER.info("Sending Metric: %s ", data)
+    LOGGER.info("Sending Metric: {data} ", data=data)
     return msg
```

### Comparing `numalogic_prometheus-0.4.1/numaprom/udf/inference.py` & `numalogic_prometheus-0.4.4/numaprom/udf/threshold.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,115 +1,118 @@
+import os
 import time
-from numalogic.config import NumalogicConf
-from numalogic.models.autoencoder import AutoencoderTrainer
-from numalogic.registry import ArtifactData, RedisRegistry
-from numalogic.tools.data import StreamingDataset
+from collections import OrderedDict
+
+from numalogic.registry import RedisRegistry, LocalLRUCache
 from numalogic.tools.exceptions import RedisRegistryError
 from orjson import orjson
 from pynumaflow.function import Datum
-from torch.utils.data import DataLoader
 
-from numaprom import get_logger
+from numaprom import LOGGER
+from numaprom._constants import TRAIN_VTX_KEY, POSTPROC_VTX_KEY
 from numaprom.clients.sentinel import get_redis_client_from_conf
-from numaprom.entities import PayloadFactory
-from numaprom.entities import Status, StreamPayload, Header
-from numaprom.tools import msg_forward
+from numaprom.entities import Status, TrainerPayload, PayloadFactory, Header
+from numaprom.tools import conditional_forward, calculate_static_thresh
 from numaprom.watcher import ConfigManager
 
-_LOGGER = get_logger(__name__)
-REDIS_CLIENT = get_redis_client_from_conf()
-
+LOCAL_CACHE_TTL = int(os.getenv("LOCAL_CACHE_TTL", 3600))  # default ttl set to 1 hour
 
-def _run_inference(
-    payload: StreamPayload, artifact_data: ArtifactData, numalogic_conf: NumalogicConf
-) -> StreamPayload:
-    model = artifact_data.artifact
-    stream_data = payload.get_stream_array()
-    stream_loader = DataLoader(StreamingDataset(stream_data, numalogic_conf.model.conf["seq_len"]))
-
-    trainer = AutoencoderTrainer()
-    try:
-        recon_err = trainer.predict(model, dataloaders=stream_loader)
-    except Exception as err:
-        _LOGGER.exception("%s - Runtime error while performing inference: %r", payload.uuid, err)
-        raise RuntimeError("Failed to infer") from err
 
-    _LOGGER.info("%s - Successfully inferred", payload.uuid)
-
-    payload.set_win_arr(recon_err.numpy())
-    payload.set_status(Status.INFERRED)
-    payload.set_metadata("version", artifact_data.extras.get("version"))
-    return payload
+def _get_static_thresh_payload(payload, metric_config) -> bytes:
+    """Calculates static thresholding, and returns a serialized json bytes payload."""
+    static_scores = calculate_static_thresh(payload, metric_config.static_threshold)
+
+    payload.set_win_arr(static_scores)
+    payload.set_header(Header.STATIC_INFERENCE)
+    payload.set_status(Status.ARTIFACT_NOT_FOUND)
+    payload.set_metadata("version", -1)
+
+    LOGGER.info(
+        "{uuid} - Static thresholding complete for payload: {payload}",
+        uuid=payload.uuid,
+        payload=payload,
+    )
+    return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
 
 
-@msg_forward
-def inference(_: list[str], datum: Datum) -> bytes:
+@conditional_forward
+def threshold(_: list[str], datum: Datum) -> list[tuple[str, bytes]]:
     _start_time = time.perf_counter()
-
     _in_msg = datum.value.decode("utf-8")
 
-    # Construct payload object
+    # Construct payload objects
     payload = PayloadFactory.from_json(_in_msg)
-
-    # Check if payload needs static inference
-    if payload.header == Header.STATIC_INFERENCE:
-        _LOGGER.debug(
-            "%s - Models not found in the previous steps, forwarding for static thresholding. Keys: %s",
-            payload.uuid,
-            payload.composite_keys,
-        )
-        return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
+    train_payload = TrainerPayload(
+        uuid=payload.uuid, composite_keys=OrderedDict(payload.composite_keys)
+    )
 
     # Load config
     metric_config = ConfigManager.get_metric_config(payload.composite_keys)
-    numalogic_conf = metric_config.numalogic_conf
+    thresh_cfg = metric_config.numalogic_conf.threshold
 
-    # Load inference model
-    model_registry = RedisRegistry(client=REDIS_CLIENT)
+    # Check if payload needs static inference
+    if payload.header == Header.STATIC_INFERENCE:
+        LOGGER.info(
+            "{uuid} - Sending to trainer and performing static thresholding. Keys: {keys}",
+            uuid=payload.uuid,
+            keys=payload.composite_keys,
+        )
+        return [
+            (TRAIN_VTX_KEY, orjson.dumps(train_payload)),
+            (POSTPROC_VTX_KEY, _get_static_thresh_payload(payload, metric_config)),
+        ]
+
+    # load threshold artifact
+    local_cache = LocalLRUCache(ttl=LOCAL_CACHE_TTL)
+    model_registry = RedisRegistry(client=get_redis_client_from_conf(), cache_registry=local_cache)
     try:
-        artifact_data = model_registry.load(
+        thresh_artifact = model_registry.load(
             skeys=[payload.composite_keys["namespace"], payload.composite_keys["name"]],
-            dkeys=[numalogic_conf.model.name],
+            dkeys=[thresh_cfg.name],
         )
     except RedisRegistryError as err:
-        _LOGGER.exception(
-            "%s - Error while fetching inference artifact, keys: %s, err: %r",
-            payload.uuid,
-            payload.composite_keys,
-            err,
+        LOGGER.exception(
+            "{uuid} - Error while fetching threshold artifact, keys: {keys}, err: {err}",
+            uuid=payload.uuid,
+            keys=payload.composite_keys,
+            err=err,
         )
         payload.set_header(Header.STATIC_INFERENCE)
         payload.set_status(Status.RUNTIME_ERROR)
-        return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
-
-    if not artifact_data:
-        _LOGGER.info(
-            "%s - Inference artifact not found, forwarding for static thresholding. Keys: %s",
-            payload.uuid,
-            payload.composite_keys,
+        return [
+            (TRAIN_VTX_KEY, orjson.dumps(train_payload)),
+            (POSTPROC_VTX_KEY, _get_static_thresh_payload(payload, metric_config)),
+        ]
+    if not thresh_artifact:
+        LOGGER.info(
+            "{uuid} - Threshold artifact not found, performing static thresholding. Keys: {keys}",
+            uuid=payload.uuid,
+            keys=payload.composite_keys,
         )
         payload.set_header(Header.STATIC_INFERENCE)
         payload.set_status(Status.ARTIFACT_NOT_FOUND)
-        return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
-
-    # Check if current model is stale
-    if RedisRegistry.is_artifact_stale(artifact_data, int(metric_config.retrain_freq_hr)):
-        payload.set_header(Header.MODEL_STALE)
-
-    # Generate predictions
-    try:
-        payload = _run_inference(payload, artifact_data, numalogic_conf)
-    except RuntimeError:
-        _LOGGER.info(
-            "%s - Failed to infer, forwarding for static thresholding. Keys: %s",
-            payload.uuid,
-            payload.composite_keys,
-        )
-        payload.set_header(Header.STATIC_INFERENCE)
-        payload.set_status(Status.RUNTIME_ERROR)
-        return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
-
-    _LOGGER.info("%s - Sending Payload: %s ", payload.uuid, payload)
-    _LOGGER.debug(
-        "%s - Time taken in inference: %.4f sec", payload.uuid, time.perf_counter() - _start_time
+        return [
+            (TRAIN_VTX_KEY, orjson.dumps(train_payload)),
+            (POSTPROC_VTX_KEY, _get_static_thresh_payload(payload, metric_config)),
+        ]
+
+    messages = []
+    if payload.header == Header.MODEL_STALE:
+        messages.append((TRAIN_VTX_KEY, orjson.dumps(train_payload)))
+
+    # Calculate anomaly score
+    recon_err = payload.get_stream_array()
+    thresh_clf = thresh_artifact.artifact
+    y_score = thresh_clf.score_samples(recon_err)
+
+    # Prepare payload for forwarding
+    payload.set_win_arr(y_score)
+    payload.set_status(Status.THRESHOLD)
+    messages.append((POSTPROC_VTX_KEY, orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)))
+
+    LOGGER.info("{uuid} - Sending Payload: {payload} ", uuid=payload.uuid, payload=payload)
+    LOGGER.debug(
+        "{uuid} - Time taken in threshold: {time} sec",
+        uuid=payload.uuid,
+        time=time.perf_counter() - _start_time,
     )
-    return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
+    return messages
```

### Comparing `numalogic_prometheus-0.4.1/numaprom/udf/postprocess.py` & `numalogic_prometheus-0.4.4/numaprom/udf/postprocess.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import os
 import time
-from typing import List
 
 import numpy as np
 from orjson import orjson
 from pynumaflow.function import Datum
 from redis.exceptions import RedisError, RedisClusterException
 from redis.sentinel import MasterNotFoundError
 
-from numaprom import get_logger, UnifiedConf
+from numaprom import LOGGER, UnifiedConf
 from numaprom.clients.sentinel import get_redis_client_from_conf
 from numaprom.entities import Status, PrometheusPayload, StreamPayload, Header
 from numaprom.tools import msgs_forward, WindowScorer
 from numaprom.watcher import ConfigManager
 
-_LOGGER = get_logger(__name__)
-
 AUTH = os.getenv("REDIS_AUTH")
 
 
 def __save_to_redis(
     payload: StreamPayload, final_score: float, recreate: bool, unified_config: UnifiedConf
 ):
     r = get_redis_client_from_conf(recreate=recreate)
@@ -28,51 +25,53 @@
 
     r_keys = payload.composite_keys
     r_keys.pop("name")
     r_key = f"{':'.join(r_keys.values())}:{payload.end_ts}"
 
     final_score = -1 if np.isnan(final_score) else final_score
     r.hset(r_key, mapping={metric_name: final_score})
-    _LOGGER.info(
-        "%s - Saved to redis, redis_key: %s, metric: %s, anomaly_score: %.3f",
-        payload.uuid,
-        r_key,
-        metric_name,
-        final_score,
+    LOGGER.info(
+        "{uuid} - Saved to redis, redis_key: {redis_key}, metric: {metric_name}, "
+        "anomaly_score: {final_score}",
+        uuid=payload.uuid,
+        redis_key=r_key,
+        metric_name=metric_name,
+        final_score=final_score,
     )
 
     anomalies = []
     for m in unified_config.unified_metrics:
         if r.hexists(name=r_key, key=m):
             anomalies.append(float(r.hget(name=r_key, key=m).decode()))
         else:
-            _LOGGER.debug(
-                "%s - Unable to generate unified anomaly, missing metric: %s, redis_key: %s",
-                payload.uuid,
-                m,
-                r_key,
+            LOGGER.debug(
+                "{uuid} - Unable to generate unified anomaly, missing metric: "
+                "{metric}, redis_key: {redis_key}",
+                uuid=payload.uuid,
+                metric=m,
+                redis_key=r_key,
             )
             return -1, []
 
-    _LOGGER.debug("%s - Received all metrics, generating unified anomaly", payload.uuid)
+    LOGGER.debug("{uuid} - Received all metrics, generating unified anomaly", uuid=payload.uuid)
     unified_weights = unified_config.unified_weights
     if unified_weights:
         weighted_anomalies = np.multiply(anomalies, unified_weights)
         unified_anomaly = float(np.sum(weighted_anomalies) / np.sum(unified_weights))
-        _LOGGER.info(
-            "%s - Generating unified anomaly, using unified weights. Unified Anomaly: %s",
-            payload.uuid,
-            unified_anomaly,
+        LOGGER.info(
+            "{uuid} - Generating unified anomaly, using unified weights. Unified Anomaly: {anomaly}",
+            uuid=payload.uuid,
+            anomaly=unified_anomaly,
         )
     else:
         unified_anomaly = max(anomalies)
-        _LOGGER.info(
-            "%s - Generated unified anomaly, using max strategy. Unified Anomaly: %s",
-            payload.uuid,
-            unified_anomaly,
+        LOGGER.info(
+            "{uuid} - Generated unified anomaly, using max strategy. Unified Anomaly: {anomaly}",
+            uuid=payload.uuid,
+            anomaly=unified_anomaly,
         )
 
     r.delete(r_key)
     return unified_anomaly, anomalies
 
 
 def __construct_publisher_payload(
@@ -116,90 +115,100 @@
         subsystem=None,
         type="Gauge",
         value=max_anomaly,
         labels=labels,
     )
 
 
-def _publish(final_score: float, payload: StreamPayload) -> List[bytes]:
+def _publish(final_score: float, payload: StreamPayload) -> list[bytes]:
     unified_config = ConfigManager.get_unified_config(payload.composite_keys)
 
     publisher_json = __construct_publisher_payload(payload, final_score).as_json()
-    _LOGGER.info("%s - Payload sent to publisher: %s", payload.uuid, publisher_json)
+    LOGGER.info(
+        "{uuid} - Payload sent to publisher: {publisher_json}",
+        uuid=payload.uuid,
+        publisher_json=publisher_json,
+    )
 
     if not unified_config:
-        _LOGGER.debug(
-            "%s - Using default config, cannot generate a unified anomaly score", payload.uuid
+        LOGGER.debug(
+            "{uuid} - Using default config, cannot generate a unified anomaly score",
+            uuid=payload.uuid,
         )
         return [publisher_json]
 
     try:
         unified_anomaly, anomalies = __save_to_redis(
             payload=payload, final_score=final_score, recreate=False, unified_config=unified_config
         )
     except (RedisError, RedisClusterException, MasterNotFoundError) as warn:
-        _LOGGER.warning(
-            "%s - Redis connection failed, recreating the redis client; err: %r", payload.uuid, warn
+        LOGGER.warning(
+            "{uuid} - Redis connection failed, recreating the redis client; err: {warn}",
+            uuid=payload.uuid,
+            warn=warn,
         )
         unified_anomaly, anomalies = __save_to_redis(
             payload=payload, final_score=final_score, recreate=True, unified_config=unified_config
         )
 
     if unified_anomaly > -1:
         unified_json = __construct_unified_payload(
             payload, unified_anomaly, unified_config
         ).as_json()
-        _LOGGER.info(
-            "%s - Unified anomaly payload sent to publisher: %s", payload.uuid, unified_json
+        LOGGER.info(
+            "{uuid} - Unified anomaly payload sent to publisher: {unified_json}",
+            uuid=payload.uuid,
+            unified_json=unified_json,
         )
         return [publisher_json, unified_json]
     return [publisher_json]
 
 
 @msgs_forward
-def postprocess(_: List[str], datum: Datum) -> List[bytes]:
-    """
-    UDF for performing the following steps:
+def postprocess(_: list[str], datum: Datum) -> list[bytes]:
+    """UDF for performing the following steps:
 
     1. Postprocess the raw scores, e.g. bring the scores into a range of 0 - 10
     2. Calculate a unified anomaly score by combining multiple metrics
     3. Construct and publish a Prometheus Payload object
     """
     _start_time = time.perf_counter()
 
     _in_msg = datum.value.decode("utf-8")
     payload = StreamPayload(**orjson.loads(_in_msg))
 
     # Load config
     metric_config = ConfigManager.get_metric_config(payload.composite_keys)
 
-    _LOGGER.debug("%s - Received Payload: %r ", payload.uuid, payload)
+    LOGGER.debug("{uuid} - Received Payload: {payload} ", uuid=payload.uuid, payload=payload)
 
     winscorer = WindowScorer(metric_config)
 
     # Use only using static thresholding
     if payload.header == Header.STATIC_INFERENCE:
         final_score = winscorer.get_winscore(payload)
-        _LOGGER.info(
-            "%s - Final static threshold score: %s, keys: %s",
-            payload.uuid,
-            final_score,
-            payload.composite_keys,
+        LOGGER.info(
+            "{uuid} - Final static threshold score: {final_score}, keys: {keys}",
+            uuid=payload.uuid,
+            final_score=final_score,
+            keys=payload.composite_keys,
         )
 
     # Compute ensemble score otherwise
     else:
         final_score = winscorer.get_final_winscore(payload)
-        _LOGGER.info(
-            "%s - Final ensemble score: %s, static thresh wt: %s, keys: %s",
-            payload.uuid,
-            final_score,
-            metric_config.static_threshold_wt,
-            payload.composite_keys,
+        LOGGER.info(
+            "{uuid} - Final ensemble score: {ensemble_score}, static thresh wt: {thresh}, keys: {keys}",
+            uuid=payload.uuid,
+            ensemble_score=final_score,
+            thresh=metric_config.static_threshold_wt,
+            keys=payload.composite_keys,
         )
 
     payload.set_status(Status.POST_PROCESSED)
     messages = _publish(final_score, payload)
-    _LOGGER.debug(
-        "%s - Time taken in postprocess: %.4f sec", payload.uuid, time.perf_counter() - _start_time
+    LOGGER.debug(
+        "{uuid} - Time taken in postprocess: {time} sec",
+        uuid=payload.uuid,
+        time=time.perf_counter() - _start_time,
     )
     return messages
```

### Comparing `numalogic_prometheus-0.4.1/numaprom/udf/preprocess.py` & `numalogic_prometheus-0.4.4/numaprom/udf/preprocess.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,85 @@
 import os
 import time
-from typing import List
 
 import orjson
-from numalogic.registry import RedisRegistry
+from numalogic.registry import RedisRegistry, LocalLRUCache
 from numalogic.tools.exceptions import RedisRegistryError
 from pynumaflow.function import Datum
 
-from numaprom import get_logger
+from numaprom import LOGGER
 from numaprom.clients.sentinel import get_redis_client
 from numaprom.entities import Status, StreamPayload, Header
 from numaprom.tools import msg_forward
 from numaprom.watcher import ConfigManager
 
-_LOGGER = get_logger(__name__)
 
 AUTH = os.getenv("REDIS_AUTH")
 REDIS_CONF = ConfigManager.get_redis_config()
 REDIS_CLIENT = get_redis_client(
     REDIS_CONF.host,
     REDIS_CONF.port,
     password=AUTH,
     mastername=REDIS_CONF.master_name,
     recreate=False,
 )
+LOCAL_CACHE_TTL = int(os.getenv("LOCAL_CACHE_TTL", 3600))  # default ttl set to 1 hour
 
 
 @msg_forward
-def preprocess(_: List[str], datum: Datum) -> bytes:
+def preprocess(_: list[str], datum: Datum) -> bytes:
     _start_time = time.perf_counter()
     _in_msg = datum.value.decode("utf-8")
 
     payload = StreamPayload(**orjson.loads(_in_msg))
-    _LOGGER.info("%s - Received Payload: %r ", payload.uuid, payload)
+    LOGGER.info("{uuid} - Received Payload: {payload} ", uuid=payload.uuid, payload=payload)
 
     # Load config
     metric_config = ConfigManager.get_metric_config(payload.composite_keys)
     preprocess_cfgs = metric_config.numalogic_conf.preprocess
 
     # Load preprocess artifact
-    model_registry = RedisRegistry(client=REDIS_CLIENT)
+    local_cache = LocalLRUCache(ttl=LOCAL_CACHE_TTL)
+    model_registry = RedisRegistry(client=REDIS_CLIENT, cache_registry=local_cache)
+
     try:
         preproc_artifact = model_registry.load(
             skeys=[payload.composite_keys["namespace"], payload.composite_keys["name"]],
             dkeys=[_conf.name for _conf in preprocess_cfgs],
         )
     except RedisRegistryError as err:
-        _LOGGER.exception(
-            "%s - Error while fetching preproc artifact, keys: %s, err: %r",
-            payload.uuid,
-            payload.composite_keys,
-            err,
+        LOGGER.exception(
+            "{uuid} - Error while fetching preproc artifact, keys: {keys}, err: {err}",
+            uuid=payload.uuid,
+            keys=payload.composite_keys,
+            err=err,
         )
         payload.set_header(Header.STATIC_INFERENCE)
         payload.set_status(Status.RUNTIME_ERROR)
         return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
 
     if not preproc_artifact:
-        _LOGGER.info(
-            "%s - Preprocess artifact not found, forwarding for static thresholding. Keys: %s",
-            payload.uuid,
-            payload.composite_keys,
+        LOGGER.info(
+            "{uuid} - Preprocess artifact not found, forwarding for static thresholding. Keys: {keys}",
+            uuid=payload.uuid,
+            keys=payload.composite_keys,
         )
         payload.set_header(Header.STATIC_INFERENCE)
         payload.set_status(Status.ARTIFACT_NOT_FOUND)
         return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
 
     # Perform preprocessing
     x_raw = payload.get_stream_array()
     preproc_clf = preproc_artifact.artifact
     x_scaled = preproc_clf.transform(x_raw)
 
     # Prepare payload for forwarding
     payload.set_win_arr(x_scaled)
     payload.set_status(Status.PRE_PROCESSED)
 
-    _LOGGER.info("%s - Sending Payload: %r ", payload.uuid, payload)
-    _LOGGER.debug(
-        "%s - Time taken in preprocess: %.4f sec", payload.uuid, time.perf_counter() - _start_time
+    LOGGER.info("{uuid} - Sending Payload: {payload} ", uuid=payload.uuid, payload=payload)
+    LOGGER.debug(
+        "{uuid} - Time taken in preprocess: {time} sec",
+        uuid=payload.uuid,
+        time=time.perf_counter() - _start_time,
     )
     return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
```

### Comparing `numalogic_prometheus-0.4.1/numaprom/udf/window.py` & `numalogic_prometheus-0.4.4/numaprom/udf/window.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 import os
 import time
 import uuid
-from typing import Optional, List
+from typing import Optional
 
 import numpy as np
 import numpy.typing as npt
 from orjson import orjson
 from pynumaflow.function import Datum
 from redis.exceptions import RedisError, RedisClusterException
 
-from numaprom import get_logger
+from numaprom import LOGGER
 from numaprom.clients.sentinel import get_redis_client_from_conf
 from numaprom.entities import StreamPayload, Status, Header
 from numaprom.tools import msg_forward, create_composite_keys
 from numaprom.watcher import ConfigManager
 
-_LOGGER = get_logger(__name__)
-
 
 # TODO get the replacement value from config
 def _clean_arr(
     id_: str,
     ckeys: dict,
     arr: npt.NDArray[float],
     replace_val: float = 0.0,
     inf_replace: float = 1e10,
 ) -> npt.NDArray[float]:
     if not np.isfinite(arr).any():
-        _LOGGER.warning(
-            "%s - Non finite values encountered: %s for keys: %s", id_, list(arr), ckeys
+        LOGGER.warning(
+            "{id} - Non finite values encountered: {arr} for keys: {keys}",
+            id=id_,
+            arr=list(arr),
+            keys=ckeys,
         )
     return np.nan_to_num(arr, nan=replace_val, posinf=inf_replace, neginf=-inf_replace)
 
 
 def __aggregate_window(
     key: str, ts: str, value: float, win_size: int, buff_size: int, recreate: bool
 ) -> list[tuple[float, float]]:
-    """
-    Adds an element to the sliding window using a redis sorted set.
+    """Adds an element to the sliding window using a redis sorted set.
 
     Returns an empty list if adding the element does not create a new entry
     to the set.
     """
     redis_client = get_redis_client_from_conf(recreate=recreate)
     with redis_client.pipeline() as pl:
         pl.zadd(key, {f"{value}::{ts}": ts})
@@ -52,19 +52,17 @@
     if not _is_new:
         return []
     _window = list(map(lambda x: (float(x[0].decode().split("::")[0]), x[1]), _window))
     return _window
 
 
 @msg_forward
-def window(_: List[str], datum: Datum) -> Optional[bytes]:
-    """
-    UDF to construct windowing of the streaming input data, required by ML models.
-    """
-    _LOGGER.debug("Received Msg: %s ", datum.value)
+def window(_: list[str], datum: Datum) -> Optional[bytes]:
+    """UDF to construct windowing of the streaming input data, required by ML models."""
+    LOGGER.debug("Received Msg: {data} ", data=datum.value)
 
     _start_time = time.perf_counter()
     msg = orjson.loads(datum.value)
 
     metric_config = ConfigManager.get_metric_config(
         {"name": msg["name"], "namespace": msg["labels"]["namespace"]}
     )
@@ -82,15 +80,15 @@
 
     # Create sliding window
     try:
         elements = __aggregate_window(
             unique_key, msg["timestamp"], value, win_size, buff_size, recreate=False
         )
     except (RedisError, RedisClusterException) as warn:
-        _LOGGER.warning("Redis connection failed, recreating the redis client, err: %r", warn)
+        LOGGER.warning("Redis connection failed, recreating the redis client, err: {err}", err=warn)
         elements = __aggregate_window(
             unique_key, msg["timestamp"], value, win_size, buff_size, recreate=True
         )
 
     # Drop message if no of elements is less than sequence length needed
     if len(elements) < win_size:
         return None
@@ -110,12 +108,14 @@
         status=Status.EXTRACTED,
         win_raw_arr=win_arr,
         win_arr=win_arr.copy(),
         win_ts_arr=[str(_ts) for _, _ts in elements],
         metadata=dict(src_labels=msg["labels"]),
     )
 
-    _LOGGER.info("%s - Sending Payload: %r ", payload.uuid, payload)
-    _LOGGER.debug(
-        "%s - Time taken in window: %.4f sec", payload.uuid, time.perf_counter() - _start_time
+    LOGGER.info("{uuid} - Sending Payload: {payload} ", uuid=payload.uuid, payload=payload)
+    LOGGER.debug(
+        "{uuid} - Time taken in window: {time} sec",
+        uuid=payload.uuid,
+        time=time.perf_counter() - _start_time,
     )
     return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
```

### Comparing `numalogic_prometheus-0.4.1/numaprom/udsink/train.py` & `numalogic_prometheus-0.4.4/numaprom/udsink/train.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 import os
 import time
-from typing import List
 
 import numpy as np
 import pandas as pd
 from numalogic.config import PreprocessFactory, ModelInfo, ThresholdFactory, ModelFactory
 from numalogic.models.autoencoder import AutoencoderTrainer
 from numalogic.registry import RedisRegistry
 from numalogic.tools.data import StreamingDataset
 from numalogic.tools.exceptions import RedisRegistryError
 from numalogic.tools.types import redis_client_t
 from orjson import orjson
 from pynumaflow.sink import Datum, Responses, Response
 from sklearn.pipeline import make_pipeline
 from torch.utils.data import DataLoader
 
-from numaprom import get_logger
+from numaprom import LOGGER
 from numaprom.clients.sentinel import get_redis_client_from_conf
 from numaprom.entities import TrainerPayload
 from numaprom.tools import fetch_data
 from numaprom.watcher import ConfigManager
 
-_LOGGER = get_logger(__name__)
-
 
 REQUEST_EXPIRY = int(os.getenv("REQUEST_EXPIRY", 300))
 
 
 def clean_data(df: pd.DataFrame, limit=12) -> pd.DataFrame:
     df.replace([np.inf, -np.inf], np.nan, inplace=True)
     df = df.fillna(method="ffill", limit=limit)
@@ -42,21 +39,25 @@
     model_factory = ModelFactory()
     model = model_factory.get_instance(model_cfg)
     dataset = StreamingDataset(x, model.seq_len)
 
     trainer = AutoencoderTrainer(**trainer_cfg)
     trainer.fit(model, train_dataloaders=DataLoader(dataset, batch_size=64))
 
-    _LOGGER.debug("%s - Time taken to train model: %s", uuid, time.perf_counter() - _start_train)
+    LOGGER.debug(
+        "{uuid} - Time taken to train model: {time}",
+        uuid=uuid,
+        time=time.perf_counter() - _start_train,
+    )
 
     train_reconerr = trainer.predict(model, dataloaders=DataLoader(dataset, batch_size=64))
     return train_reconerr.numpy(), model
 
 
-def _preprocess(x_raw, preproc_cfg: List[ModelInfo]):
+def _preprocess(x_raw, preproc_cfg: list[ModelInfo]):
     preproc_factory = PreprocessFactory()
 
     if len(preproc_cfg) > 1:
         preproc_clfs = []
         for _cfg in preproc_cfg:
             _clf = preproc_factory.get_instance(_cfg)
             preproc_clfs.append(_clf)
@@ -83,27 +84,33 @@
     if value:
         return False
 
     redis_client.setex(r_key, time=REQUEST_EXPIRY, value=1)
     return True
 
 
-def train(datums: List[Datum]) -> Responses:
+def train(datums: list[Datum]) -> Responses:
     responses = Responses()
     redis_client = get_redis_client_from_conf()
 
     for _datum in datums:
         payload = TrainerPayload(**orjson.loads(_datum.value))
 
-        _LOGGER.debug("%s - Starting Training for keys: %s", payload.uuid, payload.composite_keys)
+        LOGGER.debug(
+            "{uuid} - Starting Training for keys: {keys}",
+            uuid=payload.uuid,
+            time=payload.composite_keys,
+        )
 
         is_new = _is_new_request(redis_client, payload)
         if not is_new:
-            _LOGGER.debug(
-                "%s - Skipping train request with keys: %s", payload.uuid, payload.composite_keys
+            LOGGER.debug(
+                "{uuid} - Skipping train request with keys: {keys}",
+                uuid=payload.uuid,
+                keys=payload.composite_keys,
             )
             responses.append(Response.as_success(_datum.id))
             continue
 
         metric_config = ConfigManager.get_metric_config(payload.composite_keys)
         model_cfg = metric_config.numalogic_conf.model
 
@@ -112,19 +119,20 @@
             metric_config,
             {"namespace": payload.composite_keys["namespace"]},
             hours=metric_config.train_hours,
         )
         train_df = clean_data(train_df)
 
         if len(train_df) < metric_config.min_train_size:
-            _LOGGER.warning(
-                "%s - Skipping training, train data less than minimum required: %s, df shape: %s",
-                payload.uuid,
-                metric_config.min_train_size,
-                train_df.shape,
+            LOGGER.warning(
+                "{uuid} - Skipping training, train data less than "
+                "minimum required: {min_train_size}, df shape: {shape}",
+                uuid=payload.uuid,
+                min_train_size=metric_config.min_train_size,
+                shape=train_df.shape,
             )
             responses.append(Response.as_success(_datum.id))
             continue
 
         preproc_cfgs = metric_config.numalogic_conf.preprocess
         x_train, preproc_clf = _preprocess(train_df.to_numpy(), preproc_cfgs)
 
@@ -144,62 +152,68 @@
                 skeys=skeys,
                 dkeys=[model_cfg.name],
                 artifact=anomaly_model,
                 uuid=payload.uuid,
                 train_size=train_df.shape[0],
             )
         except RedisRegistryError as err:
-            _LOGGER.exception(
-                "%s - Error while saving Model with skeys: %s, err: %r", payload.uuid, skeys, err
+            LOGGER.exception(
+                "{uuid} - Error while saving Model with skeys: {keys}, err: {err}",
+                uuid=payload.uuid,
+                keys=skeys,
+                err=err,
             )
         else:
-            _LOGGER.info(
-                "%s - Model saved with skeys: %s with version: %s", payload.uuid, skeys, version
+            LOGGER.info(
+                "{uuid} - Model saved with skeys: {keys} with version: {version}",
+                uuid=payload.uuid,
+                keys=skeys,
+                versio=version,
             )
         # Save preproc model
         try:
             version = model_registry.save(
                 skeys=skeys,
                 dkeys=[_conf.name for _conf in preproc_cfgs],
                 artifact=preproc_clf,
                 uuid=payload.uuid,
             )
         except RedisRegistryError as err:
-            _LOGGER.exception(
-                "%s - Error while saving Preproc model with skeys: %s, err: %r",
-                payload.uuid,
-                skeys,
-                err,
+            LOGGER.exception(
+                "{uuid} - Error while saving Preproc model with skeys: {keys}, err: {err}",
+                uuid=payload.uuid,
+                keys=skeys,
+                err=err,
             )
         else:
-            _LOGGER.info(
-                "%s - Preproc model saved with skeys: %s with version: %s",
-                payload.uuid,
-                skeys,
-                version,
+            LOGGER.info(
+                "{uuid} - Preproc model saved with skeys: {keys} with version: {version}",
+                uuid=payload.uuid,
+                keys=skeys,
+                versio=version,
             )
         # Save threshold model
         try:
             version = model_registry.save(
                 skeys=skeys,
                 dkeys=[thresh_cfg.name],
                 artifact=thresh_clf,
                 uuid=payload.uuid,
             )
         except RedisRegistryError as err:
-            _LOGGER.error(
-                "%s - Error while saving Threshold model with skeys: %s, err: %r",
-                payload.uuid,
-                skeys,
-                err,
+            LOGGER.error(
+                "{uuid} - Error while saving Threshold model with skeys: {keys}, err: {err}",
+                uuid=payload.uuid,
+                keys=skeys,
+                err=err,
             )
         else:
-            _LOGGER.info(
-                "%s - Threshold model saved with skeys: %s with version: %s",
-                payload.uuid,
-                skeys,
-                version,
+            LOGGER.info(
+                "{uuid} - Threshold model saved with skeys: {keys} with version: {version}",
+                uuid=payload.uuid,
+                skeys=skeys,
+                version=version,
             )
 
         responses.append(Response.as_success(_datum.id))
 
     return responses
```

### Comparing `numalogic_prometheus-0.4.1/numaprom/udsink/train_rollout.py` & `numalogic_prometheus-0.4.4/numaprom/udsink/train_rollout.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 import os
 import time
-from typing import List, Iterator
+from collections.abc import Iterator
 
 import numpy as np
 import pandas as pd
 from numalogic.config import PreprocessFactory, ModelInfo, ThresholdFactory, ModelFactory
 from numalogic.models.autoencoder import AutoencoderTrainer
 from numalogic.registry import RedisRegistry
 from numalogic.tools.data import StreamingDataset
 from numalogic.tools.exceptions import RedisRegistryError
 from numalogic.tools.types import redis_client_t
 from orjson import orjson
 from pynumaflow.sink import Datum, Responses, Response
 from sklearn.pipeline import make_pipeline
 from torch.utils.data import DataLoader
 
-from numaprom import get_logger, MetricConf
+from numaprom import LOGGER, MetricConf
 from numaprom.clients.sentinel import get_redis_client_from_conf
 from numaprom.entities import TrainerPayload
 from numaprom.tools import fetch_data
 from numaprom.watcher import ConfigManager
 
-_LOGGER = get_logger(__name__)
-
-REQUEST_EXPIRY = int(os.getenv("REQUEST_EXPIRY", 300))
+REQUEST_EXPIRY = int(os.getenv("REQUEST_EXPIRY", "300"))
 
 
 # TODO: extract all good hashes, including when there are 2 hashes at a time
 # TODO avoid filling inf with nan, or at least throw warning
 def clean_data(df: pd.DataFrame, hash_col: str, limit=12) -> pd.DataFrame:
     df.replace([np.inf, -np.inf], np.nan, inplace=True)
     df = df.fillna(method="ffill", limit=limit)
@@ -55,24 +53,26 @@
     model_factory = ModelFactory()
     model = model_factory.get_instance(model_cfg)
     dataset = StreamingDataset(x, model.seq_len)
 
     trainer = AutoencoderTrainer(**trainer_cfg)
     trainer.fit(model, train_dataloaders=DataLoader(dataset, batch_size=64))
 
-    _LOGGER.debug(
-        "%s - Time taken to train model: %.3f sec", uuid, time.perf_counter() - _start_train
+    LOGGER.debug(
+        "{uuid} - Time taken to train model: {time}} sec",
+        uuid=uuid,
+        time=time.perf_counter() - _start_train,
     )
 
     train_reconerr = trainer.predict(model, dataloaders=DataLoader(dataset, batch_size=64))
     # return the trainer to avoid Weakreference error
     return train_reconerr.numpy(), model, trainer
 
 
-def _preprocess(x_raw, preproc_cfgs: List[ModelInfo]):
+def _preprocess(x_raw, preproc_cfgs: list[ModelInfo]):
     preproc_factory = PreprocessFactory()
     preproc_clfs = []
     for _cfg in preproc_cfgs:
         _clf = preproc_factory.get_instance(_cfg)
         preproc_clfs.append(_clf)
     preproc_pl = make_pipeline(*preproc_clfs)
 
@@ -101,22 +101,26 @@
 def train_rollout(datums: Iterator[Datum]) -> Responses:
     responses = Responses()
     redis_client = get_redis_client_from_conf()
 
     for _datum in datums:
         payload = TrainerPayload(**orjson.loads(_datum.value))
 
-        _LOGGER.debug("%s - Starting Training for keys: %s", payload.uuid, payload.composite_keys)
+        LOGGER.debug(
+            "{uuid} - Starting Training for keys: {keys}",
+            uuid=payload.uuid,
+            keys=payload.composite_keys,
+        )
 
         is_new = _is_new_request(redis_client, payload)
         if not is_new:
-            _LOGGER.debug(
-                "%s - Skipping rollouts train request with keys: %s",
-                payload.uuid,
-                payload.composite_keys,
+            LOGGER.debug(
+                "{uuid} - Skipping rollouts train request with keys: {keys}",
+                uuid=payload.uuid,
+                keys=payload.composite_keys,
             )
             responses.append(Response.as_success(_datum.id))
             continue
 
         metric_config = ConfigManager.get_metric_config(payload.composite_keys)
 
         # TODO: standardize the label name
@@ -131,26 +135,29 @@
             {"namespace": payload.composite_keys["namespace"]},
             return_labels=[hash_label],
             hours=metric_config.train_hours,
         )
         try:
             train_df = clean_data(train_df, hash_label)
         except KeyError:
-            _LOGGER.error(
-                "%s - KeyError while data cleaning for train payload: %s", payload.uuid, payload
+            LOGGER.error(
+                "{uuid} - KeyError while data cleaning for train payload: {payload}",
+                uuid=payload.uuid,
+                payload=payload,
             )
             responses.append(Response.as_success(_datum.id))
             continue
 
         if len(train_df) < metric_config.min_train_size:
-            _LOGGER.warning(
-                "%s - Skipping training, train data less than minimum required: %s, df shape: %s",
-                payload.uuid,
-                metric_config.min_train_size,
-                train_df.shape,
+            LOGGER.warning(
+                "{uuid} - Skipping training, train data less than minimum "
+                "required: {min_train_size}, df shape: {shape}",
+                uuid=payload.uuid,
+                min_train_size=metric_config.min_train_size,
+                shape=train_df.shape,
             )
             responses.append(Response.as_success(_datum.id))
             continue
 
         _train_and_save(metric_config, payload, redis_client, train_df)
 
         responses.append(Response.as_success(_datum.id))
@@ -185,58 +192,64 @@
             skeys=skeys,
             dkeys=[model_cfg.name],
             artifact=anomaly_model,
             uuid=payload.uuid,
             train_size=train_df.shape[0],
         )
     except RedisRegistryError as err:
-        _LOGGER.exception(
-            "%s - Error while saving Model with skeys: %s, err: %r", payload.uuid, skeys, err
+        LOGGER.exception(
+            "{uuid} - Error while saving Model with skeys: {keys}, err: {err}",
+            uuid=payload.uuid,
+            keys=skeys,
+            err=err,
         )
     else:
-        _LOGGER.info(
-            "%s - Model saved with skeys: %s with version: %s", payload.uuid, skeys, version
+        LOGGER.info(
+            "{uuid} - Model saved with skeys: {keys} with version: {version}",
+            uuid=payload.uuid,
+            keys=skeys,
+            version=version,
         )
     # Save preproc model
     try:
         version = model_registry.save(
             skeys=skeys,
             dkeys=[_conf.name for _conf in preproc_cfgs],
             artifact=preproc_clf,
             uuid=payload.uuid,
         )
     except RedisRegistryError as err:
-        _LOGGER.exception(
-            "%s - Error while saving Preproc model with skeys: %s, err: %r",
-            payload.uuid,
-            skeys,
-            err,
+        LOGGER.exception(
+            "{uuid} - Error while saving Preproc model with skeys: {keys}, err: {err}",
+            uuid=payload.uuid,
+            keys=skeys,
+            err=err,
         )
     else:
-        _LOGGER.info(
-            "%s - Preproc model saved with skeys: %s with version: %s",
-            payload.uuid,
-            skeys,
-            version,
+        LOGGER.info(
+            "{uuid} - Preproc model saved with skeys: {keys} with version: {version}",
+            uuid=payload.uuid,
+            keys=skeys,
+            version=version,
         )
     # Save threshold model
     try:
         version = model_registry.save(
             skeys=skeys,
             dkeys=[thresh_cfg.name],
             artifact=thresh_clf,
             uuid=payload.uuid,
         )
     except RedisRegistryError as err:
-        _LOGGER.error(
-            "%s - Error while saving Threshold model with skeys: %s, err: %r",
-            payload.uuid,
-            skeys,
-            err,
+        LOGGER.error(
+            "{uuid} - Error while saving Threshold model with skeys: {keys}, err: {err}",
+            uuid=payload.uuid,
+            keys=skeys,
+            err=err,
         )
     else:
-        _LOGGER.info(
-            "%s - Threshold model saved with skeys: %s with version: %s",
-            payload.uuid,
-            skeys,
-            version,
+        LOGGER.info(
+            "{uuid} - Threshold model saved with skeys: {keys} with version: {version}",
+            uuid=payload.uuid,
+            keys=skeys,
+            version=version,
         )
```

### Comparing `numalogic_prometheus-0.4.1/numaprom/watcher.py` & `numalogic_prometheus-0.4.4/numaprom/watcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 from omegaconf import OmegaConf
 from watchdog.observers import Observer
 from numalogic.config import NumalogicConf
 from watchdog.events import FileSystemEventHandler
 
 from numaprom._config import PipelineConf, RedisConf, PrometheusConf, RegistryConf
 from numaprom._constants import CONFIG_DIR, DEFAULT_CONFIG_DIR
-from numaprom import DataConf, get_logger, AppConf, MetricConf, UnifiedConf
-
-_LOGGER = get_logger(__name__)
+from numaprom import DataConf, LOGGER, AppConf, MetricConf, UnifiedConf
 
 
 class ConfigManager:
     config = {}
 
     @staticmethod
     def load_configs():
@@ -46,15 +44,15 @@
         for _config in app_configs:
             cls.config["app_configs"][_config.namespace] = _config
 
         cls.config["default_configs"] = dict(map(lambda c: (c.namespace, c), default_configs))
         cls.config["default_numalogic"] = default_numalogic
         cls.config["pipeline_config"] = pipeline_config
 
-        _LOGGER.info("Successfully updated configs - %s", cls.config)
+        LOGGER.info("Successfully updated configs - {config}", config=cls.config)
         return cls.config
 
     @classmethod
     @lru_cache(maxsize=100)
     def get_app_config(cls, metric: str, namespace: str) -> Optional[AppConf]:
         if not cls.config:
             cls.update_configs()
@@ -134,15 +132,20 @@
         self.config_manger = ConfigManager
 
     def on_any_event(self, event):
         if event.event_type == "created" or event.event_type == "modified":
             _file = os.path.basename(event.src_path)
             _dir = os.path.basename(os.path.dirname(event.src_path))
 
-            _LOGGER.info("Watchdog received %s event - %s/%s", event.event_type, _dir, _file)
+            LOGGER.info(
+                "Watchdog received {event_type} event - {dir}/{file}",
+                event_type=event.event_type,
+                dir=_dir,
+                file=_file,
+            )
             self.config_manger.get_app_config.cache_clear()
             self.config_manger.update_configs()
 
 
 class Watcher:
     def __init__(self, directories=None, handler=FileSystemEventHandler()):
         if directories is None:
@@ -150,17 +153,17 @@
         self.observer = Observer()
         self.handler = handler
         self.directories = directories
 
     def run(self):
         for directory in self.directories:
             self.observer.schedule(self.handler, directory, recursive=True)
-            _LOGGER.info("\nWatcher Running in {}/\n".format(directory))
+            LOGGER.info(f"\nWatcher Running in {directory}/\n")
 
         self.observer.start()
         try:
             while True:
                 time.sleep(1)
         except KeyboardInterrupt:
             self.observer.stop()
         self.observer.join()
-        _LOGGER.info("\nWatcher Terminated\n")
+        LOGGER.info("\nWatcher Terminated\n")
```

### Comparing `numalogic_prometheus-0.4.1/pyproject.toml` & `numalogic_prometheus-0.4.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "numalogic-prometheus"
-version = "0.4.1"
+version = "0.4.4"
 description = "ML inference on numaflow using numalogic on Prometheus metrics"
 authors = ["Numalogic developers"]
 packages = [{ include = "numaprom" }]
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
     "Nandita Koppisetty <nandita.iitkgp@gmail.com>",
 ]
@@ -17,18 +17,19 @@
 ]
 repository = "https://github.com/numaproj/numalogic-prometheus"
 
 [tool.poetry.dependencies]
 python = "~3.10"
 redis = {extras = ["hiredis"], version = "^4.5" }
 pynumaflow = "~0.4.1"
-numalogic = {version = "0.4a0", extras = ["redis"], allow-prereleases = true}
+numalogic = {version = "~0.4", extras = ["redis"]}
 orjson = "^3.8.4"
 omegaconf = "^2.3.0"
 watchdog = "^3.0.0"
+loguru = "^0.7.0"
 
 [tool.poetry.group.mlflowserver]
 optional = true
 
 [tool.poetry.group.mlflowserver.dependencies]
 mlflow = "^2.2"
 
@@ -47,16 +48,15 @@
 [tool.black]
 line-length = 100
 include = '\.pyi?$'
 exclude = '''
 /(
     \.eggs
   | \.git
-  | \.hg
-  | \.mypy_cache
+  | \.hgdsadsadassmmm
   | \.tox
   | \.venv
   | \.idea
   | _build
   | buck-out
   | build
   | dist
```

### Comparing `numalogic_prometheus-0.4.1/PKG-INFO` & `numalogic_prometheus-0.4.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: numalogic-prometheus
-Version: 0.4.1
+Version: 0.4.4
 Summary: ML inference on numaflow using numalogic on Prometheus metrics
 Home-page: https://github.com/numaproj/numalogic-prometheus
 Author: Numalogic developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: numalogic[redis] (==0.4a0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: numalogic[redis] (>=0.4,<0.5)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
 Requires-Dist: orjson (>=3.8.4,<4.0.0)
 Requires-Dist: pynumaflow (>=0.4.1,<0.5.0)
 Requires-Dist: redis[hiredis] (>=4.5,<5.0)
 Requires-Dist: watchdog (>=3.0.0,<4.0.0)
 Project-URL: Repository, https://github.com/numaproj/numalogic-prometheus
```

