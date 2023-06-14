# Comparing `tmp/reliably_cli-0.6.2.tar.gz` & `tmp/reliably_cli-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliably_cli-0.6.2.tar", last modified: Thu Jun  8 09:53:33 2023, max compression
+gzip compressed data, was "reliably_cli-0.7.0.tar", last modified: Wed Jun 14 09:03:33 2023, max compression
```

## Comparing `reliably_cli-0.6.2.tar` & `reliably_cli-0.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2023-06-08 09:53:10.817398 reliably_cli-0.6.2/LICENSE
--rw-r--r--   0        0        0     1478 2023-06-08 09:53:10.817398 reliably_cli-0.6.2/README.md
--rw-r--r--   0        0        0     3015 2023-06-08 09:53:33.981644 reliably_cli-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      114 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/__init__.py
--rw-r--r--   0        0        0      881 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/__main__.py
--rw-r--r--   0        0        0      166 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/__version__.py
--rw-r--r--   0        0        0     1221 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/agent/__init__.py
--rw-r--r--   0        0        0     1545 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/agent/cli.py
--rw-r--r--   0        0        0     2770 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/agent/plan/__init__.py
--rw-r--r--   0        0        0     1352 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/agent/plan/providers/__init__.py
--rw-r--r--   0        0        0     3493 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/agent/plan/providers/github.py
--rw-r--r--   0        0        0     1215 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/client.py
--rw-r--r--   0        0        0     1087 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/config/__init__.py
--rw-r--r--   0        0        0     3552 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/config/cli.py
--rw-r--r--   0        0        0     2403 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/config/types.py
--rw-r--r--   0        0        0      566 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/format.py
--rw-r--r--   0        0        0      126 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/log.py
--rw-r--r--   0        0        0        0 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/services/__init__.py
--rw-r--r--   0        0        0      211 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/services/cli.py
--rw-r--r--   0        0        0     2388 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/services/org.py
--rw-r--r--   0        0        0    10148 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/services/plan.py
--rw-r--r--   0        0        0     2068 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/types.py
--rw-r--r--   0        0        0      662 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/tests/conftest.py
--rw-r--r--   0        0        0      581 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/tests/test_cli.py
--rw-r--r--   0        0        0     3573 1970-01-01 00:00:00.000000 reliably_cli-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-14 09:03:11.431223 reliably_cli-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1478 2023-06-14 09:03:11.431223 reliably_cli-0.7.0/README.md
+-rw-r--r--   0        0        0     3015 2023-06-14 09:03:33.520431 reliably_cli-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      114 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/__init__.py
+-rw-r--r--   0        0        0      881 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/__main__.py
+-rw-r--r--   0        0        0      166 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/__version__.py
+-rw-r--r--   0        0        0     1221 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/agent/__init__.py
+-rw-r--r--   0        0        0     1545 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/agent/cli.py
+-rw-r--r--   0        0        0     2770 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/agent/plan/__init__.py
+-rw-r--r--   0        0        0     1352 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/agent/plan/providers/__init__.py
+-rw-r--r--   0        0        0     3493 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/agent/plan/providers/github.py
+-rw-r--r--   0        0        0     1215 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/client.py
+-rw-r--r--   0        0        0     1087 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/config/__init__.py
+-rw-r--r--   0        0        0     3552 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/config/cli.py
+-rw-r--r--   0        0        0     2403 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/config/types.py
+-rw-r--r--   0        0        0      566 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/format.py
+-rw-r--r--   0        0        0      126 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/log.py
+-rw-r--r--   0        0        0        0 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/services/__init__.py
+-rw-r--r--   0        0        0      211 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/services/cli.py
+-rw-r--r--   0        0        0     2388 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/services/org.py
+-rw-r--r--   0        0        0    11933 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/services/plan.py
+-rw-r--r--   0        0        0     2690 2023-06-14 09:03:11.439224 reliably_cli-0.7.0/reliably_cli/types.py
+-rw-r--r--   0        0        0      662 2023-06-14 09:03:11.439224 reliably_cli-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0      581 2023-06-14 09:03:11.439224 reliably_cli-0.7.0/tests/test_cli.py
+-rw-r--r--   0        0        0     3573 1970-01-01 00:00:00.000000 reliably_cli-0.7.0/PKG-INFO
```

### Comparing `reliably_cli-0.6.2/LICENSE` & `reliably_cli-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.2/README.md` & `reliably_cli-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.2/pyproject.toml` & `reliably_cli-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "rich>=13.3.1",
     "chaostoolkit-addons>=0.4.0",
     "chaostoolkit>=1.15.0",
     "chaostoolkit-lib>=1.33.1",
     "chaostoolkit-reliably>=0.22.0",
     "orjson>=3.8.10",
 ]
-version = "0.6.2"
+version = "0.7.0"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 Homepage = "https://reliably.com/"
 Repository = "https://github.com/reliablyhq/cli"
```

### Comparing `reliably_cli-0.6.2/reliably_cli/__main__.py` & `reliably_cli-0.7.0/reliably_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.2/reliably_cli/agent/__init__.py` & `reliably_cli-0.7.0/reliably_cli/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.2/reliably_cli/agent/cli.py` & `reliably_cli-0.7.0/reliably_cli/agent/cli.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.2/reliably_cli/agent/plan/__init__.py` & `reliably_cli-0.7.0/reliably_cli/agent/plan/__init__.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.2/reliably_cli/agent/plan/providers/__init__.py` & `reliably_cli-0.7.0/reliably_cli/agent/plan/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.2/reliably_cli/agent/plan/providers/github.py` & `reliably_cli-0.7.0/reliably_cli/agent/plan/providers/github.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.2/reliably_cli/client.py` & `reliably_cli-0.7.0/reliably_cli/client.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.2/reliably_cli/config/__init__.py` & `reliably_cli-0.7.0/reliably_cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.2/reliably_cli/config/cli.py` & `reliably_cli-0.7.0/reliably_cli/config/cli.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.2/reliably_cli/config/types.py` & `reliably_cli-0.7.0/reliably_cli/config/types.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.2/reliably_cli/format.py` & `reliably_cli-0.7.0/reliably_cli/format.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.2/reliably_cli/services/org.py` & `reliably_cli-0.7.0/reliably_cli/services/org.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.2/reliably_cli/services/plan.py` & `reliably_cli-0.7.0/reliably_cli/services/plan.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import contextlib
 import logging
 import logging.handlers
 import os
+import tempfile
 import traceback
 from datetime import datetime, timezone
 from pathlib import Path
 from typing import Any, Generator
 from uuid import UUID
 
 import httpx
@@ -18,15 +19,21 @@
 from chaoslib.types import Journal, Schedule, Strategy
 from ruamel.yaml import YAML
 
 from ..client import api_client
 from ..config import ensure_config_is_set, get_settings
 from ..format import format_as
 from ..log import console
-from ..types import FormatOption, Plan
+from ..types import (
+    Environment,
+    EnvironmentSecret,
+    EnvironmentSecretAsFile,
+    FormatOption,
+    Plan,
+)
 
 cli = typer.Typer(help="Manage and execute Reliably plans from your terminal")
 
 
 @cli.command()
 def get(
     plan_id: UUID,
@@ -61,14 +68,15 @@
 def execute(
     plan_id: UUID,
     result_file: Path = typer.Option("./result.json", writable=True),
     log_stdout: bool = typer.Option(False, is_flag=True),
     log_file: Path = typer.Option("./run.log", writable=True),
     set_status: bool = typer.Option(False, is_flag=True),
     skip_context: bool = typer.Option(False, is_flag=True),
+    load_environment: bool = typer.Option(False, is_flag=True),
     control_file: list[Path] = typer.Option(
         lambda: [], dir_okay=False, readable=True
     ),
     var_file: list[Path] = typer.Option(
         lambda: [], dir_okay=False, readable=True
     ),
 ) -> None:
@@ -98,14 +106,18 @@
         os.environ["RELIABLY_PLAN_ID"] = str(p.id)
 
     experiment_id = p.definition.experiments[0]
     base_url = f"{settings.service.host}/api/v1/organization"
     base_url = f"{base_url}/{settings.organization.id}"
     experiment_url = f"{base_url}/experiments/{experiment_id}/raw"
 
+    if load_environment:
+        tempdir = tempfile.TemporaryDirectory()
+        load_environment_into_memory(p, tempdir.name)
+
     with console.status("Executing..."):
         if set_status:
             send_status(p.id, "running")
 
         with reconfigure_chaostoolkit_logger(log_file, log_stdout):
             try:
                 journal = run_chaostoolkit(
@@ -166,14 +178,49 @@
                         del provider["arguments"]
                     ctrl = {ctrl_name: control}
                     global_controls.update(ctrl)
 
     return global_controls
 
 
+def load_environment_into_memory(plan: Plan, target_dir: str) -> None:
+    with console.status("Loading environment..."):
+        if not plan.definition.environment:
+            return None
+
+        with api_client() as client:
+            env_id = str(plan.definition.environment.id)
+            r = client.get(f"/environments/{env_id}/clear")
+            env = Environment.parse_obj(r.json())
+            if env:
+                path_mapping = {}
+                for s in env.secrets.__root__:
+                    if isinstance(s, EnvironmentSecretAsFile):
+                        new_path = Path(target_dir, s.path.lstrip("/"))
+                        new_path.parent.mkdir(mode=0o710, parents=True)
+                        new_path.write_text(s.value.get_secret_value())
+                        new_path.chmod(0o770)
+
+                        path_mapping[s.path] = str(new_path)
+
+                for e in env.envvars.__root__:
+                    if e.value in path_mapping:
+                        os.environ[e.var_name] = path_mapping[e.value]
+                    else:
+                        os.environ[e.var_name] = e.value
+
+                for s in env.secrets.__root__:
+                    if isinstance(s, EnvironmentSecret):
+                        v = s.value.get_secret_value()
+                        if v in path_mapping:
+                            os.environ[s.var_name] = path_mapping[v]
+                        else:
+                            os.environ[s.var_name] = v
+
+
 def send_status(plan_id: UUID, status: str, error: str | None = None) -> None:
     with api_client() as client:
         payload = {"status": status, "error": error}
         r = client.put(f"/plans/{str(plan_id)}/status", json=payload)
         if r.status_code == 404:
             console.print("plan not found")
             raise typer.Exit(code=1)
```

### Comparing `reliably_cli-0.6.2/reliably_cli/types.py` & `reliably_cli-0.7.0/reliably_cli/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Literal
 
 import orjson
-from pydantic import UUID4, BaseModel
+from pydantic import UUID4, BaseModel, SecretStr
 
-__all__ = ["Plan", "FormatOption", "Organization"]
+__all__ = ["Plan", "FormatOption", "Organization", "Environment"]
 
 
 def _json_dumps(*args, **kwargs) -> str:  # type: ignore[no-untyped-def]
     return orjson.dumps(*args, **kwargs).decode("utf-8")
 
 
 def _json_loads(obj: str, *args, **kwargs) -> Any:  # type: ignore[no-untyped-def]  # noqa
@@ -88,7 +88,41 @@
     name: str
     created_date: datetime
 
 
 class Organizations(BaseSchema):
     count: int
     items: list[Organization]
+
+
+class EnvironmentVar(BaseSchema):
+    var_name: str
+    value: str
+
+
+class EnvironmentVars(BaseSchema):
+    __root__: List[EnvironmentVar]
+
+
+class EnvironmentSecret(BaseSchema):
+    key: str
+    var_name: str
+    value: SecretStr
+
+
+class EnvironmentSecretAsFile(BaseSchema):
+    key: str
+    value: SecretStr
+    path: str
+
+
+class EnvironmentSecrets(BaseSchema):
+    __root__: List[EnvironmentSecretAsFile | EnvironmentSecret]
+
+
+class Environment(BaseSchema):
+    id: UUID4
+    org_id: UUID4
+    created_date: datetime
+    name: str
+    envvars: EnvironmentVars
+    secrets: EnvironmentSecrets
```

### Comparing `reliably_cli-0.6.2/tests/conftest.py` & `reliably_cli-0.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.2/tests/test_cli.py` & `reliably_cli-0.7.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.2/PKG-INFO` & `reliably_cli-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reliably-cli
-Version: 0.6.2
+Version: 0.7.0
 Summary: Reliably CLI
 Author-Email: Sylvain Hellegouarch <sylvain@reliably.com>
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reliably-cli Version: 0.6.2 Summary: Reliably CLI
+Metadata-Version: 2.1 Name: reliably-cli Version: 0.7.0 Summary: Reliably CLI
 Author-Email: Sylvain Hellegouarch
 reliably.com> License: Apache-2.0 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Development Status :: 4 - Beta Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Utilities Project-URL: Homepage, https://reliably.com/
```

