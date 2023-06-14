# Comparing `tmp/osin-1.9.2.tar.gz` & `tmp/osin-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osin-1.9.2.tar", max compression
+gzip compressed data, was "osin-2.0.0.tar", max compression
```

## Comparing `osin-1.9.2.tar` & `osin-2.0.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0     1064 2022-12-26 08:13:34.023654 osin-1.9.2/LICENSE
--rw-r--r--   0        0        0     1367 2022-12-26 08:13:34.023654 osin-1.9.2/README.md
--rw-r--r--   0        0        0       93 2022-12-26 08:13:34.023654 osin-1.9.2/osin/__init__.py
--rw-r--r--   0        0        0     1705 2022-12-26 08:13:34.023654 osin-1.9.2/osin/__main__.py
--rw-r--r--   0        0        0        0 2022-12-26 08:13:34.023654 osin-1.9.2/osin/apis/__init__.py
--rw-r--r--   0        0        0     2050 2022-12-26 08:13:34.027654 osin-1.9.2/osin/apis/local_osin.py
--rw-r--r--   0        0        0    11582 2022-12-26 08:13:34.027654 osin-1.9.2/osin/apis/osin.py
--rw-r--r--   0        0        0     1815 2022-12-26 08:13:34.027654 osin-1.9.2/osin/apis/remote_exp.py
--rw-r--r--   0        0        0     6226 2022-12-26 08:13:34.027654 osin-1.9.2/osin/apis/remote_osin.py
--rw-r--r--   0        0        0      865 2022-12-26 08:13:34.027654 osin-1.9.2/osin/app.py
--rw-r--r--   0        0        0      243 2022-12-26 08:13:34.027654 osin-1.9.2/osin/config.py
--rw-r--r--   0        0        0        0 2022-12-26 08:13:34.027654 osin-1.9.2/osin/controllers/__init__.py
--rw-r--r--   0        0        0     4636 2022-12-26 08:13:34.027654 osin-1.9.2/osin/controllers/exp.py
--rw-r--r--   0        0        0    10281 2022-12-26 08:13:34.027654 osin-1.9.2/osin/controllers/report.py
--rw-r--r--   0        0        0      195 2022-12-26 08:13:34.027654 osin-1.9.2/osin/controllers/views.py
--rw-r--r--   0        0        0       41 2022-12-26 08:13:34.027654 osin-1.9.2/osin/formats/__init__.py
--rw-r--r--   0        0        0     9776 2022-12-26 08:13:34.027654 osin-1.9.2/osin/formats/hdf5.py
--rw-r--r--   0        0        0        0 2022-12-26 08:13:34.027654 osin-1.9.2/osin/integrations/__init__.py
--rw-r--r--   0        0        0     2658 2022-12-26 08:13:34.027654 osin-1.9.2/osin/integrations/ream.py
--rw-r--r--   0        0        0     2798 2022-12-26 08:13:34.027654 osin-1.9.2/osin/misc.py
--rw-r--r--   0        0        0      459 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/__init__.py
--rw-r--r--   0        0        0      904 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/base.py
--rw-r--r--   0        0        0     2711 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/exp.py
--rw-r--r--   0        0        0     1073 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/exp_data.py
--rw-r--r--   0        0        0        0 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/migration/__init__.py
--rw-r--r--   0        0        0      795 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/migration/v_1_6_2_1_7_0.backup
--rw-r--r--   0        0        0      536 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/report/__init__.py
--rw-r--r--   0        0        0     5450 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/report/auto_table.py
--rw-r--r--   0        0        0     3238 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/report/base_report.py
--rw-r--r--   0        0        0     1802 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/report/dbmodel.py
--rw-r--r--   0        0        0    15138 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/report/index_schema.py
--rw-r--r--   0        0        0     6765 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/report.py.backup
--rw-r--r--   0        0        0      411 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/views.py
--rw-r--r--   0        0        0     1119 2022-12-26 08:13:34.027654 osin-1.9.2/osin/params_helper.py
--rw-r--r--   0        0        0     2348 2022-12-26 08:13:34.027654 osin-1.9.2/osin/repository.py
--rw-r--r--   0        0        0      294 2022-12-26 08:13:34.027654 osin-1.9.2/osin/types/__init__.py
--rw-r--r--   0        0        0     2204 2022-12-26 08:13:34.027654 osin-1.9.2/osin/types/param_schema.py
--rw-r--r--   0        0        0     3845 2022-12-26 08:13:34.027654 osin-1.9.2/osin/types/primitive_type.py
--rw-r--r--   0        0        0     1983 2022-12-26 08:13:34.027654 osin-1.9.2/osin/types/pyobject.py
--rw-r--r--   0        0        0     3953 2022-12-26 08:13:34.027654 osin-1.9.2/osin/types/pyobject_type.py
--rw-r--r--   0        0        0      562 2022-12-26 08:13:34.027654 osin-1.9.2/pyproject.toml
--rw-r--r--   0        0        0     2397 1970-01-01 00:00:00.000000 osin-1.9.2/setup.py
--rw-r--r--   0        0        0     2258 1970-01-01 00:00:00.000000 osin-1.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-14 19:54:43.853765 osin-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1367 2023-06-14 19:54:43.853765 osin-2.0.0/README.md
+-rw-r--r--   0        0        0       93 2023-06-14 19:54:43.853765 osin-2.0.0/osin/__init__.py
+-rw-r--r--   0        0        0     2651 2023-06-14 19:54:43.853765 osin-2.0.0/osin/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-14 19:54:43.853765 osin-2.0.0/osin/apis/__init__.py
+-rw-r--r--   0        0        0     1537 2023-06-14 19:54:43.853765 osin-2.0.0/osin/apis/local_osin.py
+-rw-r--r--   0        0        0    11387 2023-06-14 19:54:43.853765 osin-2.0.0/osin/apis/osin.py
+-rw-r--r--   0        0        0     1808 2023-06-14 19:54:43.853765 osin-2.0.0/osin/apis/remote_exp.py
+-rw-r--r--   0        0        0     6226 2023-06-14 19:54:43.853765 osin-2.0.0/osin/apis/remote_osin.py
+-rw-r--r--   0        0        0      865 2023-06-14 19:54:43.853765 osin-2.0.0/osin/app.py
+-rw-r--r--   0        0        0      243 2023-06-14 19:54:43.853765 osin-2.0.0/osin/config.py
+-rw-r--r--   0        0        0        0 2023-06-14 19:54:43.853765 osin-2.0.0/osin/controllers/__init__.py
+-rw-r--r--   0        0        0     5727 2023-06-14 19:54:43.853765 osin-2.0.0/osin/controllers/exp.py
+-rw-r--r--   0        0        0    10281 2023-06-14 19:54:43.853765 osin-2.0.0/osin/controllers/report.py
+-rw-r--r--   0        0        0      195 2023-06-14 19:54:43.853765 osin-2.0.0/osin/controllers/views.py
+-rw-r--r--   0        0        0       41 2023-06-14 19:54:43.853765 osin-2.0.0/osin/formats/__init__.py
+-rw-r--r--   0        0        0    10512 2023-06-14 19:54:43.853765 osin-2.0.0/osin/formats/hdf5.py
+-rw-r--r--   0        0        0        0 2023-06-14 19:54:43.853765 osin-2.0.0/osin/integrations/__init__.py
+-rw-r--r--   0        0        0     5035 2023-06-14 19:54:43.853765 osin-2.0.0/osin/integrations/ream.py
+-rw-r--r--   0        0        0     2852 2023-06-14 19:54:43.853765 osin-2.0.0/osin/misc.py
+-rw-r--r--   0        0        0      459 2023-06-14 19:54:43.853765 osin-2.0.0/osin/models/__init__.py
+-rw-r--r--   0        0        0      904 2023-06-14 19:54:43.853765 osin-2.0.0/osin/models/base.py
+-rw-r--r--   0        0        0     2896 2023-06-14 19:54:43.853765 osin-2.0.0/osin/models/exp.py
+-rw-r--r--   0        0        0     1274 2023-06-14 19:54:43.853765 osin-2.0.0/osin/models/exp_data.py
+-rw-r--r--   0        0        0        0 2023-06-14 19:54:43.853765 osin-2.0.0/osin/models/migration/__init__.py
+-rw-r--r--   0        0        0      795 2023-06-14 19:54:43.853765 osin-2.0.0/osin/models/migration/v_1_6_2_1_7_0.backup
+-rw-r--r--   0        0        0      536 2023-06-14 19:54:43.853765 osin-2.0.0/osin/models/report/__init__.py
+-rw-r--r--   0        0        0     5450 2023-06-14 19:54:43.853765 osin-2.0.0/osin/models/report/auto_table.py
+-rw-r--r--   0        0        0     3238 2023-06-14 19:54:43.853765 osin-2.0.0/osin/models/report/base_report.py
+-rw-r--r--   0        0        0     1802 2023-06-14 19:54:43.853765 osin-2.0.0/osin/models/report/dbmodel.py
+-rw-r--r--   0        0        0    15138 2023-06-14 19:54:43.853765 osin-2.0.0/osin/models/report/index_schema.py
+-rw-r--r--   0        0        0     6765 2023-06-14 19:54:43.853765 osin-2.0.0/osin/models/report.py.backup
+-rw-r--r--   0        0        0      411 2023-06-14 19:54:43.853765 osin-2.0.0/osin/models/views.py
+-rw-r--r--   0        0        0     4763 2023-06-14 19:54:43.853765 osin-2.0.0/osin/params_helper.py
+-rw-r--r--   0        0        0     2348 2023-06-14 19:54:43.853765 osin-2.0.0/osin/repository.py
+-rw-r--r--   0        0        0      508 2023-06-14 19:54:43.853765 osin-2.0.0/osin/types/__init__.py
+-rw-r--r--   0        0        0     2204 2023-06-14 19:54:43.853765 osin-2.0.0/osin/types/param_schema.py
+-rw-r--r--   0        0        0     3845 2023-06-14 19:54:43.853765 osin-2.0.0/osin/types/primitive_type.py
+-rw-r--r--   0        0        0     2694 2023-06-14 19:54:43.853765 osin-2.0.0/osin/types/pyobject/__init__.py
+-rw-r--r--   0        0        0     1064 2023-06-14 19:54:43.853765 osin-2.0.0/osin/types/pyobject/base.py
+-rw-r--r--   0        0        0     2059 2023-06-14 19:54:43.853765 osin-2.0.0/osin/types/pyobject/html.py
+-rw-r--r--   0        0        0     3953 2023-06-14 19:54:43.853765 osin-2.0.0/osin/types/pyobject_type.py
+-rw-r--r--   0        0        0      573 2023-06-14 19:54:43.853765 osin-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2258 1970-01-01 00:00:00.000000 osin-2.0.0/PKG-INFO
```

### Comparing `osin-1.9.2/LICENSE` & `osin-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osin-1.9.2/README.md` & `osin-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `osin-1.9.2/osin/apis/local_osin.py` & `osin-2.0.0/osin/apis/local_osin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,14 @@
-import atexit
-import shutil
-from datetime import datetime
 from pathlib import Path
-from typing import Dict, List, Optional, Set, Union
+from typing import List, Optional, Union
 
-import orjson
-from loguru import logger
 from osin.apis.osin import Osin
-from osin.apis.remote_exp import RemoteExp, RemoteExpRun
-from osin.misc import get_caller_python_script, orjson_dumps
+from osin.apis.remote_exp import RemoteExpRun
 from osin.models.base import init_db
-from osin.models.exp import Exp, ExpRun, NestedPrimitiveOutput, RunMetadata
-from osin.models.exp_data import ExampleData, Record
-from osin.params_helper import DataClassInstance, param_as_dict
-from osin.repository import OsinRepository
-from osin.types import NestedPrimitiveOutputSchema, ParamSchema, PyObject
-from osin.types.primitive_type import validate_primitive_data
+from osin.models.exp import Exp, ExpRun
 
 
 class LocalOsin(Osin):
     def __init__(self, osin_dir: Union[Path, str]):
         super().__init__(osin_dir)
         init_db(self.osin_keeper.get_db_file())
```

### Comparing `osin-1.9.2/osin/apis/osin.py` & `osin-2.0.0/osin/apis/osin.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,19 +5,24 @@
 import shutil
 from typing import Dict, List, Optional, Set, Union
 from loguru import logger
 import orjson
 
 from osin.apis.remote_exp import RemoteExp, RemoteExpRun
 from osin.misc import get_caller_python_script, orjson_dumps
-from osin.models.exp import Exp, ExpRun, NestedPrimitiveOutput, RunMetadata
+from osin.models.exp import (
+    Exp,
+    ExpRun,
+    NestedPrimitiveOutput,
+    RunMetadata,
+)
 from osin.repository import OsinRepository
 from osin.types import NestedPrimitiveOutputSchema, PyObject
 
-from osin.params_helper import DataClassInstance, param_as_dict
+from ream.params_helper import DataClassInstance, param_as_dict
 from osin.types.param_schema import ParamSchema
 from osin.types.primitive_type import validate_primitive_data
 from osin.models.exp_data import ExampleData, Record
 
 
 class Osin(ABC):
     """This class provides two methods to communicate with Osin, either locally or remotely via http protocol"""
@@ -40,15 +45,15 @@
 
     def init_exp(
         self,
         name: str,
         version: int,
         description: Optional[str] = None,
         program: Optional[str] = None,
-        params: Optional[Union[DataClassInstance, List[DataClassInstance]]] = None,
+        params: Optional[Dict[str, DataClassInstance]] = None,
         aggregated_primitive_outputs: Optional[NestedPrimitiveOutputSchema] = None,
         update_param_schema: bool = False,
     ) -> RemoteExp:
         """Init an experiment in Osin.
 
         If the experiment already exists, the input version must be the latest one, and the parameters must match.
         If the experiment does not exist, it will be created with the given parameters.
@@ -58,79 +63,78 @@
             version: Version of the experiment
             description: Description of the experiment
             program: The python program to invoke the experiment
             params: The parameters of the experiment.
             aggregated_primitive_outputs: The aggregated outputs of the experiment.
                 If not provided, it will be inferred automatically when the experiment is run.
         """
+        params = params or {}
+
         exp = self._find_latest_exp(name)
         if exp is None:
             exp = self._create_exp(
                 Exp(
                     name=name,
                     description=description,
                     version=version,
                     program=program or get_caller_python_script(),
-                    params=[
-                        ParamSchema.get_schema(p)
-                        for p in (params if isinstance(params, list) else [params])
-                    ],
+                    params={ns: ParamSchema.get_schema(p) for ns, p in params.items()},
                     aggregated_primitive_outputs=aggregated_primitive_outputs,
                 )
             )
         else:
             if exp.version > version:
                 raise ValueError("Cannot create an older version of an experiment")
             elif exp.version == version:
                 if update_param_schema:
-                    exp.params = [
-                        ParamSchema.get_schema(p)
-                        for p in (params if isinstance(params, list) else [params])
-                    ]
+                    exp.params = {
+                        ns: ParamSchema.get_schema(p) for ns, p in params.items()
+                    }
                     self._update_exp(exp.id, exp, ["params"])
             else:
                 exp = self._create_exp(
                     Exp(
                         name=name,
                         description=description,
                         version=version,
                         program=program or get_caller_python_script(),
-                        params=[
-                            ParamSchema.get_schema(p)
-                            for p in (params if isinstance(params, list) else [params])
-                        ],
+                        params={
+                            ns: ParamSchema.get_schema(p) for ns, p in params.items()
+                        },
                         aggregated_primitive_outputs=aggregated_primitive_outputs,
                     )
                 )
 
         return RemoteExp(
             id=exp.id,
             name=exp.name,
             version=exp.version,
             params=exp.params,
             aggregated_primitive_outputs=exp.aggregated_primitive_outputs,
             osin=self,
         )
 
     def new_exp_run(
-        self, exp: RemoteExp, params: Union[DataClassInstance, List[DataClassInstance]]
+        self,
+        exp: RemoteExp,
+        params: Dict[str, DataClassInstance],
     ) -> RemoteExpRun:
         """Create a new run for an experiment."""
-        output = {}
-        for param in params if isinstance(params, list) else [params]:
-            output.update(param_as_dict(param))
-        exp_run = self._create_exprun(ExpRun(exp=exp.id, params=output))
+        ser_params = {}
+        for ns, param in params.items():
+            ser_params[ns] = param_as_dict(param)
+        exp_run = self._create_exprun(ExpRun(exp=exp.id, params=ser_params))
 
         rundir = self.osin_keeper.get_exp_run_dir(exp, exp_run)
         if rundir.exists():
             shutil.rmtree(rundir)
         rundir.mkdir(parents=True)
 
         with open(rundir / "params.json", "wb") as f:
-            f.write(orjson_dumps(output, option=orjson.OPT_INDENT_2))
+            f.write(orjson_dumps(ser_params, option=orjson.OPT_INDENT_2))
 
         remote_exp_run = RemoteExpRun(
             id=exp_run.id,
             exp=exp,
             rundir=rundir,
             created_time=exp_run.created_time,
             finished_time=None,
```

### Comparing `osin-1.9.2/osin/apis/remote_exp.py` & `osin-2.0.0/osin/apis/remote_exp.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,20 +19,21 @@
 
 
 @dataclass
 class RemoteExp:
     id: int
     name: str
     version: int
-    params: List[ParamSchema]
+    params: Dict[str, ParamSchema]
     aggregated_primitive_outputs: Optional[NestedPrimitiveOutputSchema]
     osin: Osin
 
     def new_exp_run(
-        self, params: Union[DataClassInstance, List[DataClassInstance]]
+        self,
+        params: dict[str, DataClassInstance],
     ) -> RemoteExpRun:
         return self.osin.new_exp_run(self, params)
 
 
 @dataclass
 class RemoteExpRun:
     # id to the experiment run in osin
```

### Comparing `osin-1.9.2/osin/apis/remote_osin.py` & `osin-2.0.0/osin/apis/remote_osin.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.2/osin/app.py` & `osin-2.0.0/osin/app.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.2/osin/controllers/exp.py` & `osin-2.0.0/osin/controllers/exp.py`

 * *Files 14% similar despite different names*

```diff
@@ -93,24 +93,63 @@
             sorted_order = "ascending"
     else:
         sorted_by = None
         sorted_order = "ascending"
 
     try:
         exp_run_data, n_examples = format.load_exp_run_data(
-            h5file, fields, limit, offset, sorted_by, sorted_order
+            h5file,
+            fields,
+            limit,
+            offset,
+            sorted_by,
+            sorted_order,
+            with_complex_size=True,
         )
     except KeyError:
-        raise BadRequest(f"The key `{sorted_by}` does not exist to sort by")
+        if sorted_by is not None:
+            raise BadRequest(f"The key `{sorted_by}` does not exist to sort by")
+        else:
+            raise
 
     out = exp_run_data.to_dict()
     out["n_examples"] = n_examples
     return jsonify(out)
 
 
+@exprun_bp.route(
+    f"/{exprun_bp.name}/<id>/data/individual/<example_id>", methods=["GET"]
+)
+def get_individual_exp_run_data(id: int, example_id: str):
+    try:
+        exp_run: ExpRun = ExpRun.get_by_id(id)
+    except DoesNotExist:
+        raise NotFound(f"ExpRun with id {id} does not exist")
+
+    osin = OsinRepository.get_instance()
+    format = osin.get_exp_run_data_format(exp_run.exp, exp_run)
+    h5file = osin.get_exp_run_data_file(exp_run.exp, exp_run)
+
+    if "fields" in request.args:
+        fields = request.args["fields"].split(",")
+        primitive = "primitive" in fields
+        complex = "complex" in fields
+    else:
+        primitive = True
+        complex = True
+
+    try:
+        exdata = format.get_example_data(
+            h5file, example_id, primitive, complex, with_complex_size=True
+        )
+    except KeyError as e:
+        raise BadRequest(str(e))
+    return jsonify(exdata.to_dict())
+
+
 @exprun_bp.route(f"/{exprun_bp.name}/<id>/upload", methods=["POST"])
 def upload_exp_run_data(id: int):
     try:
         exp_run: ExpRun = ExpRun.get_by_id(id)
     except DoesNotExist:
         raise NotFound(f"ExpRun with id {id} does not exist")
```

### Comparing `osin-1.9.2/osin/controllers/report.py` & `osin-2.0.0/osin/controllers/report.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.2/osin/formats/hdf5.py` & `osin-2.0.0/osin/formats/hdf5.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     Tuple,
     TypeVar,
     Union,
 )
 
 from numpy import sort
 from osin.models import ExpRunData, ExampleData, Record
+from osin.models.exp_data import RecordWithComplexSize
 from osin.types import NestedPrimitiveOutput, PyObject
 from h5py import Group, File, Empty
 
 
 class Hdf5Format:
     """An interface for storing experiment data"""
 
@@ -62,24 +63,26 @@
         self,
         infile: Union[Path, str],
         fields: Optional[Dict[str, Set[str]]] = None,
         limit: int = -1,
         offset: int = 0,
         sorted_by: Optional[str] = None,
         sorted_order: Literal["ascending", "descending"] = "ascending",
+        with_complex_size: bool = False,
     ) -> Tuple[ExpRunData, int]:
         """Load experiment run data from a file.
 
         Args:
             infile: The file to load from
             fields: A dictionary of fields to load. If None, load all fields
             limit: The maximum number of individual records to load. If -1, load all records. Only apply to `individual` property
             offset: The offset to start loading from. Only apply to `individual` property
             sorted_by: The field to sort by. Only apply to `individual` property. Support either: id, name, or `data.<nested_field>` where `nested_field` is a field in the primitive or complex object
             sorted_order: The order to sort by. Only apply to `individual` property
+            with_complex_size: return the number of complex objects for each individual example
         """
         if fields is None:
             fields = {
                 "aggregated": {"primitive", "complex"},
                 "individual": {"primitive", "complex"},
             }
 
@@ -141,53 +144,75 @@
                     selected_examples.sort(
                         key=lambda x: sorted_keys[x[0]],
                         reverse=sorted_order == "descending",
                     )
                     selected_examples = selected_examples[offset : offset + limit]
 
                 for example_id, ex_group in selected_examples:
-                    if example_id not in expdata.individual:
-                        example = ExampleData(
-                            id=ex_group.attrs["id"],
-                            name=ex_group.attrs["name"],
-                        )
+                    assert example_id not in expdata.individual
+                    if with_complex_size:
+                        data = RecordWithComplexSize(n_complex=len(ex_group["complex"]))
+                    else:
+                        data = Record()
+                    example = ExampleData(
+                        id=ex_group.attrs["id"],
+                        name=ex_group.attrs["name"],
+                        data=data,
+                    )
 
-                        if "primitive" in fields["individual"]:
-                            example.data.primitive = self._load_nested_primitive_object(
-                                ex_group["primitive"]
+                    if "primitive" in fields["individual"]:
+                        example.data.primitive = self._load_nested_primitive_object(
+                            ex_group["primitive"]
+                        )
+                    if "complex" in fields["individual"]:
+                        for key, value in ex_group["complex"].items():
+                            pyobject_class = PyObject.from_classpath(
+                                ex_group["complex"].attrs[key]
                             )
-                        if "complex" in fields["individual"]:
-                            for key, value in ex_group["complex"].items():
-                                pyobject_class = PyObject.from_classpath(
-                                    ex_group["complex"].attrs[key]
-                                )
-                                example.data.complex[key] = pyobject_class.from_hdf5(
-                                    value[()]
-                                )
-                        expdata.individual[example_id] = example
-                    else:
-                        if "primitive" in fields["individual"]:
-                            expdata.individual[
-                                example_id
-                            ].data.primitive = self._load_nested_primitive_object(
-                                ex_group["primitive"]
+                            example.data.complex[key] = pyobject_class.from_hdf5(
+                                value[()]
                             )
-
-                        if "complex" in fields["individual"]:
-                            for key, value in ex_group["complex"].items():
-                                pyobject_class = PyObject.from_classpath(
-                                    ex_group.attrs[key]
-                                )
-                                expdata.individual[example_id].data.complex[
-                                    key
-                                ] = pyobject_class.from_hdf5(value[()])
+                    expdata.individual[example_id] = example
 
             n_examples = len(f["individual"])
         return expdata, n_examples
 
+    def get_example_data(
+        self,
+        infile: Union[Path, str],
+        example_id: str,
+        primitive: bool,
+        complex: bool,
+        with_complex_size: bool = False,
+    ) -> ExampleData:
+        with File(infile, "r") as f:
+            if example_id not in f["individual"]:
+                raise KeyError(f"example id `{example_id}` not found")
+
+            ex_group = f["individual"][example_id]
+            if with_complex_size:
+                data = RecordWithComplexSize(n_complex=len(ex_group["complex"]))
+            else:
+                data = Record()
+
+            example = ExampleData(
+                id=ex_group.attrs["id"], name=ex_group.attrs["name"], data=data
+            )
+            if primitive:
+                example.data.primitive = self._load_nested_primitive_object(
+                    ex_group["primitive"]
+                )
+            if complex:
+                for key, value in ex_group["complex"].items():
+                    pyobject_class = PyObject.from_classpath(
+                        ex_group["complex"].attrs[key]
+                    )
+                    example.data.complex[key] = pyobject_class.from_hdf5(value[()])
+            return example
+
     def _update_nested_primitive_object(
         self, group: Group, primitive_object: NestedPrimitiveOutput
     ):
         for key, value in primitive_object.items():
             self._validate_key(key)
             if isinstance(value, dict):
                 subgroup = group.create_group(key, track_order=True)
```

### Comparing `osin-1.9.2/osin/misc.py` & `osin-2.0.0/osin/misc.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,16 @@
         raise ValueError("expect a not-null object")
     return obj
 
 
 def _orjson_default(obj):
     if isinstance(obj, Path):
         return str(obj)
+    if isinstance(obj, set):
+        return list(obj)
     raise TypeError(f"Object of type {obj.__class__.__name__} is not JSON serializable")
 
 
 class Directory:
     def __init__(self, root: Path, dirname: str = "directory"):
         self.root = root
         self.root.mkdir(exist_ok=True, parents=True)
```

### Comparing `osin-1.9.2/osin/models/base.py` & `osin-2.0.0/osin/models/base.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.2/osin/models/exp.py` & `osin-2.0.0/osin/models/exp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from __future__ import annotations
 from dataclasses import dataclass
 from datetime import datetime
 import os
 import socket
+from osin.types.pyobject_type import PyObjectType
 from peewee import (
     CharField,
     ForeignKeyField,
     TextField,
     IntegerField,
     BooleanField,
     DateTimeField,
     AutoField,
 )
 from playhouse.sqlite_ext import JSONField
 import psutil
 from osin.models.base import BaseModel
 from osin.misc import json_dumps
-from gena.custom_fields import DataClassField, ListDataClassField
+from gena.custom_fields import DataClassField, ListDataClassField, DictDataClassField
 from osin.types import (
     NestedPrimitiveOutput,
     NestedPrimitiveOutputSchema,
     ParamSchema,
 )
 
 
@@ -55,26 +56,27 @@
         )
 
     id: int = AutoField()  # type: ignore
     name: str = CharField(null=False)  # type: ignore
     version: int = IntegerField(null=False)  # type: ignore
     description: str = TextField()  # type: ignore
     program: str = TextField()  # type: ignore
-    params: list[ParamSchema] = ListDataClassField(ParamSchema)  # type: ignore
+    params: dict[str, ParamSchema] = DictDataClassField(ParamSchema)  # type: ignore
     aggregated_primitive_outputs: NestedPrimitiveOutputSchema = DataClassField(NestedPrimitiveOutputSchema, null=True)  # type: ignore
 
 
 class ExpRun(BaseModel):
     id: int = AutoField()  # type: ignore
     exp: Exp = ForeignKeyField(Exp, backref="runs", on_delete="CASCADE")  # type: ignore
     is_deleted: bool = BooleanField(default=False, index=True)  # type: ignore
     is_finished: bool = BooleanField(default=False, index=True)  # type: ignore
     is_successful: bool = BooleanField(default=False, index=True)  # type: ignore
     # whether the schema of the outputs is not consistent with the experiment.
     has_invalid_agg_output_schema: bool = BooleanField(default=False, index=True)  # type: ignore
     created_time: datetime = DateTimeField(default=datetime.utcnow)  # type: ignore
     finished_time: datetime = DateTimeField(null=True)  # type: ignore
+    # parameters of the experiment run, each param is associated with a namespace (key of the top-level dict)
     params: dict = JSONField(default={}, json_dumps=json_dumps)  # type: ignore
     metadata: RunMetadata = DataClassField(RunMetadata, null=True)  # type: ignore
     aggregated_primitive_outputs: NestedPrimitiveOutput = JSONField(default={}, json_dumps=json_dumps)  # type: ignore
 
     exp_id: int
```

### Comparing `osin-1.9.2/osin/models/exp_data.py` & `osin-2.0.0/osin/models/exp_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class Record:
     primitive: NestedPrimitiveOutput = field(default_factory=dict)
     complex: Dict[str, PyObject] = field(default_factory=dict)
 
     def to_dict(self):
         return {
             "primitive": self.primitive,
-            "complex": {k: v.to_dict() for k, v in self.complex.items()},
+            "complex": [(k, v.to_dict()) for k, v in self.complex.items()],
         }
 
 
 @dataclass
 class ExampleData:
     id: str
     name: str
@@ -38,7 +38,17 @@
     individual: Dict[str, ExampleData] = field(default_factory=dict)
 
     def to_dict(self):
         return {
             "aggregated": self.aggregated.to_dict(),
             "individual": [v.to_dict() for k, v in self.individual.items()],
         }
+
+
+@dataclass
+class RecordWithComplexSize(Record):
+    n_complex: int = field(default=0)
+
+    def to_dict(self):
+        o = super().to_dict()
+        o["n_complex"] = self.n_complex
+        return o
```

### Comparing `osin-1.9.2/osin/models/migration/v_1_6_2_1_7_0.backup` & `osin-2.0.0/osin/models/migration/v_1_6_2_1_7_0.backup`

 * *Files identical despite different names*

### Comparing `osin-1.9.2/osin/models/report/__init__.py` & `osin-2.0.0/osin/models/report/__init__.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.2/osin/models/report/auto_table.py` & `osin-2.0.0/osin/models/report/auto_table.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.2/osin/models/report/base_report.py` & `osin-2.0.0/osin/models/report/base_report.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.2/osin/models/report/dbmodel.py` & `osin-2.0.0/osin/models/report/dbmodel.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.2/osin/models/report/index_schema.py` & `osin-2.0.0/osin/models/report/index_schema.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.2/osin/models/report.py.backup` & `osin-2.0.0/osin/models/report.py.backup`

 * *Files identical despite different names*

### Comparing `osin-1.9.2/osin/repository.py` & `osin-2.0.0/osin/repository.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.2/osin/types/param_schema.py` & `osin-2.0.0/osin/types/param_schema.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.2/osin/types/primitive_type.py` & `osin-2.0.0/osin/types/primitive_type.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.2/osin/types/pyobject.py` & `osin-2.0.0/osin/types/pyobject/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,18 @@
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
+from collections.abc import Mapping
 from dataclasses import dataclass
-from typing import Any, Generic, List, Type, TypeVar
+from typing import Any, Union, Sequence, Optional
 
 import numpy as np
 import orjson
 from osin.misc import orjson_dumps
-from osin.types.primitive_type import NestedPrimitiveOutput
-from osin.types.pyobject_type import PyObjectType
-
-T = TypeVar("T", np.ndarray, bytes)
-
-
-class PyObject(ABC, Generic[T]):
-    def get_classpath(self) -> str:
-        return PyObjectType.from_type_hint(self.__class__).path
-
-    @staticmethod
-    def from_classpath(classpath: str) -> Type[PyObject]:
-        # we know that variants of pyobject must be member of this module
-        return globals()[classpath.split(".")[-1]]
-
-    @abstractmethod
-    def serialize_hdf5(self) -> T:
-        pass
-
-    @staticmethod
-    @abstractmethod
-    def from_hdf5(value: T) -> PyObject:
-        pass
-
-    @abstractmethod
-    def to_dict(self) -> dict:
-        pass
-
-
-@dataclass
-class OTable(PyObject[bytes]):
-    rows: List[NestedPrimitiveOutput]
-
-    def serialize_hdf5(self) -> bytes:
-        return orjson_dumps({"rows": self.rows})
-
-    @staticmethod
-    def from_hdf5(value: bytes) -> OTable:
-        return OTable(**orjson.loads(value))
-
-    def to_dict(self) -> dict:
-        return {
-            "type": "table",
-            "rows": self.rows,
-        }
+from osin.types.pyobject.base import PyObject
+from osin.types.pyobject.html import OHTML, OListHTML
 
 
 @dataclass
 class OImage(PyObject[np.ndarray]):
     object: np.ndarray
 
     def serialize_hdf5(self) -> np.ndarray:
@@ -78,7 +35,72 @@
 
     @staticmethod
     def from_hdf5(value: np.ndarray) -> OAudio:
         raise NotImplementedError()
 
     def to_dict(self) -> dict:
         raise NotImplementedError()
+
+
+OTableRow = Mapping[str, Optional[Union[str, float, int, bool, OHTML, OListHTML]]]
+OTableCellTypeToClass: dict[str, type[OHTML] | type[OListHTML]] = {
+    "html": OHTML,
+    "html-list": OListHTML,
+}
+
+
+@dataclass
+class OTable(PyObject[bytes]):
+    rows: Sequence[OTableRow]
+
+    def serialize_hdf5(self) -> bytes:
+        return orjson_dumps(
+            {
+                "rows": [
+                    {
+                        k: c.to_dict() if isinstance(c, PyObject) else c
+                        for k, c in row.items()
+                    }
+                    for row in self.rows
+                ],
+            }
+        )
+
+    @staticmethod
+    def from_hdf5(value: bytes) -> OTable:
+        return OTable(
+            [
+                {
+                    k: OTableCellTypeToClass[c["type"]].from_dict(c)
+                    if isinstance(c, dict)
+                    else c  # type: ignore
+                    for k, c in row.items()
+                }
+                for row in orjson.loads(value)["rows"]
+            ]
+        )
+
+    def to_dict(self) -> dict:
+        if len(self.rows) == 0:
+            header = []
+        else:
+            header = list(self.rows[0].keys())
+
+        return {
+            "type": "table",
+            "header": header,
+            "rows": [
+                {
+                    k: c.to_dict() if isinstance(c, PyObject) else c
+                    for k, c in row.items()
+                }
+                for row in self.rows
+            ],
+        }
+
+
+def from_classpath(classpath: str) -> type[PyObject]:
+    # we know that variants of pyobject must be member of this module
+    return globals()[classpath.split(".")[-1]]
+
+
+PyObject.from_classpath = from_classpath
```

### Comparing `osin-1.9.2/osin/types/pyobject_type.py` & `osin-2.0.0/osin/types/pyobject_type.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.2/pyproject.toml` & `osin-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "osin"
-version = "1.9.2"
+version = "2.0.0"
 description = "Research and Experiments"
 authors = ["Binh Vu <binh@toan2.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 Flask = "^2.2.2"
 peewee = "^3.15.2"
 tornado = "^6.2"
 gena = "^1.6.4"
 loguru = "^0.6.0"
-orjson = "^3.8.2"
-h5py = "^3.7.0"
+orjson = ">= 3.9.0, < 4.0.0"
+h5py = "^3.8.0"
 psutil = "^5.9.2"
 python-slugify = "^6.1.2"
-t2-yada = "^1.0.5"
-ream2 = "^1.6.2"
+t2-yada = "^1.2.0"
+ream2 = "^2.8.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.10.0"
 pytest = "^7.1.3"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `osin-1.9.2/PKG-INFO` & `osin-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: osin
-Version: 1.9.2
+Version: 2.0.0
 Summary: Research and Experiments
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Flask (>=2.2.2,<3.0.0)
 Requires-Dist: gena (>=1.6.4,<2.0.0)
-Requires-Dist: h5py (>=3.7.0,<4.0.0)
+Requires-Dist: h5py (>=3.8.0,<4.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
-Requires-Dist: orjson (>=3.8.2,<4.0.0)
+Requires-Dist: orjson (>=3.9.0,<4.0.0)
 Requires-Dist: peewee (>=3.15.2,<4.0.0)
 Requires-Dist: psutil (>=5.9.2,<6.0.0)
 Requires-Dist: python-slugify (>=6.1.2,<7.0.0)
-Requires-Dist: ream2 (>=1.6.2,<2.0.0)
-Requires-Dist: t2-yada (>=1.0.5,<2.0.0)
+Requires-Dist: ream2 (>=2.8.0,<3.0.0)
+Requires-Dist: t2-yada (>=1.2.0,<2.0.0)
 Requires-Dist: tornado (>=6.2,<7.0)
 Description-Content-Type: text/markdown
 
 # osin &middot; [![PyPI](https://img.shields.io/pypi/v/osin)](https://pypi.org/project/osin)
 
 There are existing systems (e.g., neptune.ai, sacred) helping you organize, log data of your experiments. However, typically, the tasks of running the experiments are your responsible to bear. If you update your code and need to re-run your experiments, you may want to delete previous runs, which would be painful to have to do manually many times.
```

