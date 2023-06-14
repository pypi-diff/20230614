# Comparing `tmp/bmsdna_lakeapi-0.8.2.tar.gz` & `tmp/bmsdna_lakeapi-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.8.2.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.8.3.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.8.2.tar` & `bmsdna_lakeapi-0.8.3.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     1081 2023-06-13 04:48:33.999102 bmsdna_lakeapi-0.8.2/LICENSE
--rw-r--r--   0        0        0     8929 2023-06-13 04:48:33.999102 bmsdna_lakeapi-0.8.2/README.md
--rw-r--r--   0        0        0      337 2023-06-13 04:48:33.999102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 04:48:33.999102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1185 2023-06-13 04:48:33.999102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      566 2023-06-13 04:48:33.999102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     6876 2023-06-13 04:48:33.999102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0    10460 2023-06-13 04:48:33.999102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6091 2023-06-13 04:48:33.999102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-06-13 04:48:33.999102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    11077 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    12618 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/dataframe.py
--rw-r--r--   0        0        0    15585 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6887 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     1479 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/partition_utils.py
--rw-r--r--   0        0        0     6763 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     4291 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     3763 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/sql_endpoint.py
--rw-r--r--   0        0        0     3109 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2478 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1847 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      339 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1790 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1095 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     3535 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/utils/fast_api_utils.py
--rw-r--r--   0        0        0     1999 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/pyproject.toml
--rw-r--r--   0        0        0    10127 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/LICENSE
+-rw-r--r--   0        0        0     8929 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/README.md
+-rw-r--r--   0        0        0      337 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1138 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      566 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     6965 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0    10460 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6042 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    11027 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    12557 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/dataframe.py
+-rw-r--r--   0        0        0     7443 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/detail_endpoint.py
+-rw-r--r--   0        0        0     9751 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6887 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     1479 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/partition_utils.py
+-rw-r--r--   0        0        0     6763 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     4319 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     3748 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/sql_endpoint.py
+-rw-r--r--   0        0        0     3136 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2456 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1837 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      339 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1784 2023-06-14 07:23:35.811083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1084 2023-06-14 07:23:35.811083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     3535 2023-06-14 07:23:35.811083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/utils/fast_api_utils.py
+-rw-r--r--   0        0        0     2017 2023-06-14 07:23:35.811083 bmsdna_lakeapi-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0    10127 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.8.3/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.8.2/LICENSE` & `bmsdna_lakeapi-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.2/README.md` & `bmsdna_lakeapi-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/api/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from dataclasses import dataclass
-from typing import Awaitable, Callable, Final
 from fastapi import FastAPI, Request
 from bmsdna.lakeapi.core.config import BasicConfig, Configs, get_default_config
 from bmsdna.lakeapi.core.route import init_routes
 import os
 
 
 @dataclass(frozen=True)
```

### Comparing `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/context/df_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from abc import abstractmethod, ABC, abstractproperty
+from abc import abstractmethod, ABC
 from datetime import datetime, timezone
 from bmsdna.lakeapi.core.types import FileTypes
 from typing import Optional, List, Tuple, Any, TYPE_CHECKING, Union
 import pyarrow as pa
 from deltalake import DeltaTable
 import pyarrow.dataset
 import pypika.queries
@@ -38,15 +38,15 @@
         ...
 
     @abstractmethod
     def to_arrow_table(self) -> pa.Table:
         ...
 
     @abstractmethod
-    def to_arrow_recordbatch(self) -> pa.RecordBatchReader:
+    def to_arrow_recordbatch(self, chunk_size: int = 10000) -> pa.RecordBatchReader:
         ...
 
     @abstractmethod
     def query_builder(self) -> pypika.queries.QueryBuilder:
         ...
 
     def write_json(self, file_name: str):
@@ -118,15 +118,18 @@
         uri: str,
         file_type: FileTypes,
         partitions: Optional[List[Tuple[str, str, Any]]],
     ) -> Optional[pa.dataset.Dataset | pa.Table]:
         match file_type:
             case "parquet":
                 import pyarrow.dataset as ds
-                return pa.dataset.dataset(uri, format=ds.ParquetFileFormat(read_options={"coerce_int96_timestamp_unit": "us"}))
+
+                return pa.dataset.dataset(
+                    uri, format=ds.ParquetFileFormat(read_options={"coerce_int96_timestamp_unit": "us"})
+                )
             case "ipc" | "arrow" | "feather" | "csv" | "orc":
                 return pa.dataset.dataset(uri, format=file_type)
             case "ndjson" | "json":
                 import pandas
 
                 pd = pandas.read_json(uri, orient="records", lines=file_type == "ndjson")
 
@@ -136,15 +139,17 @@
 
                 pd = pl.read_avro(uri).to_arrow()
                 return pd
             case "delta":
                 dt = DeltaTable(
                     uri,
                 )
-                return dt.to_pyarrow_dataset(partitions=partitions, parquet_read_options={"coerce_int96_timestamp_unit": "us"})
+                return dt.to_pyarrow_dataset(
+                    partitions=partitions, parquet_read_options={"coerce_int96_timestamp_unit": "us"}
+                )
             case _:
                 raise Exception(f"Not supported file type {file_type}")
 
     @abstractmethod
     def register_arrow(self, name: str, ds: Union[pyarrow.dataset.Dataset, pyarrow.Table]):
         ...
```

### Comparing `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/context/df_polars.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-from datetime import datetime
 from bmsdna.lakeapi.context.df_base import ExecutionContext, ResultData, get_sql
 
 
 import pyarrow as pa
 from typing import List, Optional, Tuple, Union, cast, TYPE_CHECKING, Any
-import threading
 from bmsdna.lakeapi.core.types import FileTypes
 import pyarrow.dataset
 import pypika.queries
 import pypika.terms
 import pypika
 from uuid import uuid4
```

### Comparing `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-import ast
 import os
 import re
-from dataclasses import dataclass, field
+from dataclasses import dataclass
 from datetime import datetime
 from typing import (
     Any,
-    Awaitable,
     Callable,
     Dict,
-    Iterable,
     List,
     Literal,
     Optional,
     Sequence,
     Tuple,
     TypedDict,
     Union,
```

### Comparing `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/dataframe.py` & `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import asyncio
 import hashlib
 import os
-from dataclasses import field
 from typing import (
     Any,
-    Callable,
     List,
     Literal,
     Optional,
     Tuple,
     Union,
     cast,
     get_args,
-    overload,
 )
 
 import pyarrow as pa
 import pyarrow.parquet as pq
 import pyarrow.parquet
 from aiocache import Cache, cached
 from aiocache.serializers import PickleSerializer
```

### Comparing `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/model.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/partition_utils.py` & `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/partition_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/response.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/route.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import inspect
 from typing import Literal, Tuple, cast
 
 from fastapi import APIRouter, Depends, Request
 from bmsdna.lakeapi.context import get_context_by_engine
 
 from bmsdna.lakeapi.core.config import BasicConfig, Configs
 from bmsdna.lakeapi.core.log import get_logger
@@ -15,17 +14,17 @@
 
 
 def init_routes(configs: Configs, basic_config: BasicConfig):
     from bmsdna.lakeapi.context.df_duckdb import DuckDbExecutionContext
 
     from bmsdna.lakeapi.core.endpoint import (
         get_response_model,
-        create_detailed_meta_endpoint,
         create_config_endpoint,
     )
+    from bmsdna.lakeapi.core.detail_endpoint import create_detailed_meta_endpoint
     from bmsdna.lakeapi.core.sql_endpoint import create_sql_endpoint
 
     all_lake_api_routers.append((basic_config, configs))
     router = APIRouter()
     metadata = []
 
     with DuckDbExecutionContext() as context:
```

### Comparing `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/sql_endpoint.py` & `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/sql_endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Optional, Callable, Union
+from typing import Optional, Union
 import duckdb
 from fastapi import APIRouter, BackgroundTasks, Header, Query, Request
 from bmsdna.lakeapi.context.df_base import ExecutionContext
 from bmsdna.lakeapi.core.config import BasicConfig, Config, Configs, Param, SearchConfig
 from bmsdna.lakeapi.core.dataframe import Dataframe
 from bmsdna.lakeapi.core.types import OutputFileType
 from bmsdna.lakeapi.core.response import create_response
```

### Comparing `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from typing import Any, List, Literal, cast
 from datetime import datetime, date, time, timedelta
 from decimal import Decimal
-from typing import Type, Optional, TYPE_CHECKING
+from typing import Type, Optional
 from typing_extensions import TypedDict
 from polars.datatypes.convert import DataTypeMappings
 from pydantic import BaseModel
 
 
 Engines = Literal["duckdb", "polars"]
 
@@ -105,14 +105,15 @@
     fields: "Optional[list[MetadataSchemaField]]"
     inner: "Optional[MetadataSchemaFieldType]"
 
 
 class MetadataSchemaField(BaseModel):
     name: str
     type: MetadataSchemaFieldType
+    max_str_length: Optional[int] = None
 
 
 @dataclass
 class SearchConfig:
     name: str
     columns: List[str]
```

### Comparing `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/uservalidation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from typing import List, Sequence
+from typing import Sequence
 from fastapi import Depends, HTTPException, Request, status
 from fastapi.security import HTTPBasic, HTTPBasicCredentials
 from bmsdna.lakeapi.core.config import BasicConfig, Configs, UserConfig
 from bmsdna.lakeapi.core.yaml import get_yaml
-import inspect
 from aiocache import cached, Cache
 from aiocache.serializers import PickleSerializer
 from bmsdna.lakeapi.core.env import CACHE_EXPIRATION_TIME_SECONDS
 from fastapi import FastAPI, Response
 
 cache = cached(
     ttl=CACHE_EXPIRATION_TIME_SECONDS * 10000,
```

### Comparing `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import polars as pl
 from deltalake import write_deltalake, DeltaTable
-import os
 import pyarrow as pa
 from polars import LazyFrame, DataFrame
 from typing import cast, Any, Optional
 from functools import partial
 import pickle
```

### Comparing `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/tools/useradd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import argon2
-from typing import cast, List, Optional
+from typing import cast, Optional
 import secrets
 import string
 
 
 def generate_strong_password():
     # define the alphabet
     letters = string.ascii_letters
```

### Comparing `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/tools/validateschema.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import jsonschema
 import json
 import yaml
 from python2jsonschema import get_json_schema_for_type
 from bmsdna.lakeapi.core.config import Config, YamlData
-import os
 
 
 def validate_schema(schema_file: str, yaml_file: str):
     schema = get_json_schema_for_type(YamlData)
     with open(schema_file, "w") as str:
         json.dump(schema, str, indent=4)
```

### Comparing `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/utils/fast_api_utils.py` & `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/utils/fast_api_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.2/pyproject.toml` & `bmsdna_lakeapi-0.8.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.8.2"
+version = "0.8.3"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pyyaml = "^6.0"
 aiocache = "^0.12.1"
 pypika = "^0.48.9"
-duckdb = "^0.8.0"
+duckdb = "^0.8.1"
 polars = "^0.18.0"
 
 # schema stuff
 jsonschema = {version = "^4.17.3", optional=true}
 python2jsonschema = { version ="^0.8", optional=true}
 
 # polars stuff
@@ -33,14 +33,15 @@
 
 
 [tool.poetry.group.dev.dependencies]
 pyright = "^1.1.308"
 black = "^23.3.0"
 uvicorn = "^0.22.0"
 psutil = "^5.9.5"
+pycln = "^2.1.5"
 
 
 
 
 
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `bmsdna_lakeapi-0.8.2/PKG-INFO` & `bmsdna_lakeapi-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.8.2
+Version: 0.8.3
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Provides-Extra: auth
 Provides-Extra: polars
 Provides-Extra: schema
 Provides-Extra: useradd
 Requires-Dist: aiocache (>=0.12.1,<0.13.0)
 Requires-Dist: argon2-cffi (>=21.3.0,<22.0.0) ; extra == "auth"
 Requires-Dist: deltalake (>=0.10.0,<0.11.0)
-Requires-Dist: duckdb (>=0.8.0,<0.9.0)
+Requires-Dist: duckdb (>=0.8.1,<0.9.0)
 Requires-Dist: fastapi (>=0.96.0,<0.97.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0) ; extra == "schema"
 Requires-Dist: polars (>=0.18.0,<0.19.0)
 Requires-Dist: pyjwt (>=2.6.0,<3.0.0) ; extra == "auth"
 Requires-Dist: pypika (>=0.48.9,<0.49.0)
 Requires-Dist: python2jsonschema (>=0.8,<0.9) ; extra == "schema"
 Requires-Dist: pyyaml (>=6.0,<7.0)
```

