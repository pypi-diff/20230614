# Comparing `tmp/datayoga-1.87.0.tar.gz` & `tmp/datayoga-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datayoga-1.87.0.tar", max compression
+gzip compressed data, was "datayoga-1.9.0.tar", max compression
```

## Comparing `datayoga-1.87.0.tar` & `datayoga-1.9.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      633 2023-06-14 09:20:08.913631 datayoga-1.87.0/README.md
--rw-r--r--   0        0        0     1284 2023-06-14 09:20:25.194420 datayoga-1.87.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-14 09:20:08.913631 datayoga-1.87.0/src/datayoga/__init__.py
--rw-r--r--   0        0        0     5623 2023-06-14 09:20:08.913631 datayoga-1.87.0/src/datayoga/__main__.py
--rw-r--r--   0        0        0     3280 2023-06-14 09:20:08.913631 datayoga-1.87.0/src/datayoga/cli_helpers.py
--rw-r--r--   0        0        0     2023 1970-01-01 00:00:00.000000 datayoga-1.87.0/PKG-INFO
+-rw-r--r--   0        0        0      497 2022-11-23 19:28:55.950277 datayoga-1.9.0/README.md
+-rw-r--r--   0        0        0     1202 2022-11-23 19:29:20.762231 datayoga-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga-1.9.0/src/datayoga/__init__.py
+-rw-r--r--   0        0        0     4600 2022-11-23 19:28:55.950277 datayoga-1.9.0/src/datayoga/__main__.py
+-rw-r--r--   0        0        0     1398 2022-11-23 19:28:55.950277 datayoga-1.9.0/src/datayoga/cli_helpers.py
+-rw-r--r--   0        0        0     1687 1970-01-01 00:00:00.000000 datayoga-1.9.0/setup.py
+-rw-r--r--   0        0        0     1843 1970-01-01 00:00:00.000000 datayoga-1.9.0/PKG-INFO
```

### Comparing `datayoga-1.87.0/pyproject.toml` & `datayoga-1.9.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datayoga"
-version = "1.87.0"
+version = "1.9.0"
 description = "DataYoga command line interface"
 authors = ["DataYoga <admin@datayoga.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 include = [
 ]
 
@@ -13,24 +13,22 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3.7',
         'Topic :: Database'
 ]
 
 [tool.poetry.dependencies]
-certifi = "^2022.12.7"
 click = "^8.0.3"
 datayoga-core = "1.*"
 jsonschema = "^4.4.0"
 python = "^3.7"
 PyYAML = "^6.0"
 
 mock = { version = "^4.0.3", optional = true }
 pytest = { version = "^7.1.2", optional = true }
-pytest-asyncio = { version = "^0.20.1", optional = true }
 pytest-describe = { version = "^2.0.1", optional = true }
 pytest-mock = { version = "^3.7.0", optional = true }
 pytest-timeout = { version = "^2.1.0", optional = true }
 requests-mock = { version = "^1.9.3", optional = true }
 
 [tool.poetry.extras]
 test = ["mock", "pytest", "pytest-describe", "pytest-mock", "pytest-timeout", "requests-mock"]
```

### Comparing `datayoga-1.87.0/src/datayoga/__main__.py` & `datayoga-1.9.0/src/datayoga/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 #!/usr/bin/env python
-
 import asyncio
 import logging
 import os
 import shutil
-import sys
 from os import path
 from pathlib import Path
-from typing import Optional
 
 import click
 import datayoga_core as dy
 import jsonschema
-from datayoga_core import prometheus, utils
-from pkg_resources import DistributionNotFound, get_distribution
-
 from datayoga import cli_helpers
+from datayoga.cli_helpers import handle_critical
+from datayoga_core import utils
+from pkg_resources import get_distribution
 
 CONTEXT_SETTINGS = dict(max_content_width=120)
 LOG_LEVEL_OPTION = [click.option(
     "--loglevel", '-log-level', type=click.Choice(
         ["DEBUG", "INFO", "WARN", "ERROR", "CRITICAL"],
         case_sensitive=False),
     default="INFO", show_default=True)]
@@ -28,23 +25,16 @@
 
 # create console handler with a higher log level
 ch = logging.StreamHandler()
 ch.setFormatter(cli_helpers.CustomFormatter())
 logger.addHandler(ch)
 
 
-def get_dy_distribution() -> str:
-    try:
-        return get_distribution("datayoga").version
-    except DistributionNotFound:
-        return "0.0.0"
-
-
 @click.group(name="datayoga", help="DataYoga command line tool")
-@click.version_option(get_dy_distribution())
+@click.version_option(get_distribution("datayoga").version)
 def cli():
     pass
 
 
 @cli.command(name="init", help="Scaffolds a new folder with sample configuration files")
 @click.argument("project_name")
 @cli_helpers.add_options(LOG_LEVEL_OPTION)
@@ -65,77 +55,60 @@
         for root, dirs, files in os.walk(project_name):
             for paths, permissions in ((files, "644"), (dirs, "755")):
                 for path in paths:
                     os.chmod(os.path.join(root, path), int(permissions, 8))
 
         print(f"Initialized {project_name} successfully")
     except Exception as e:
-        cli_helpers.handle_critical(logger, f"Error while initializing {project_name}", e)
+        handle_critical(logger, f"Error while initializing {project_name}", e)
 
 
 @cli.command(name="validate", help="Validates a job in dry run mode")
 @cli_helpers.add_options(LOG_LEVEL_OPTION)
 def validate(
         loglevel: str
 ):
     set_logging_level(loglevel)
 
 
 @cli.command(name="run", help="Runs a job", context_settings=CONTEXT_SETTINGS)
-@click.argument("job_name")
-@click.option('--dir', 'directory', help="DataYoga directory", default=".", show_default=True)
-@click.option('--exporter-port', help="Enables Prometheus exporter on specified port", type=int)
+@click.argument("job")
+@click.option('--dir', help="DataYoga directory", default=".", show_default=True)
 @cli_helpers.add_options(LOG_LEVEL_OPTION)
 def run(
-    job_name: str,
-    directory: str,
-    exporter_port: Optional[int],
+    job: str,
+    dir: str,
     loglevel: str
 ):
     set_logging_level(loglevel)
 
-    logger.info("Runner started...")
-
-    # validate the connections
-    connections_file = path.join(directory, "connections.yaml")
-    try:
-        connections = utils.read_yaml(connections_file)
-        logger.debug(f"connections: {connections}")
-        connections_schema = dy.get_connections_json_schema()
-        jsonschema.validate(instance=connections, schema=connections_schema)
-    except jsonschema.exceptions.ValidationError as schema_error:
-        # print a validation message with the source lines
-        cli_helpers.pprint_yaml_validation_error(connections_file, schema_error, logger)
-        sys.exit(1)
-
-    # validate the job
-    job_file = path.join(directory, "jobs", job_name.replace(".", os.sep) + ".yaml")
     try:
+        logger.info("Runner started...")
+        job_file = path.join(dir, "jobs", job.replace(".", os.sep) + ".yaml")
         job_settings = utils.read_yaml(job_file)
         logger.debug(f"job_settings: {job_settings}")
 
+        connections = utils.read_yaml(path.join(dir, "connections.yaml"))
+        logger.debug(f"connections: {connections}")
+
+        jsonschema.validate(instance=connections, schema=utils.read_json(
+            utils.get_resource_path(os.path.join("schemas", "connections.schema.json"))))
+
         context = dy.Context({
             "connections": connections,
-            "data_path": path.join(directory, "data"),
+            "data_path": path.join(dir, "data"),
             "job_name": Path(job_file).stem
         })
 
         job = dy.compile(job_settings)
 
-        if exporter_port:
-            prometheus.start(exporter_port)
-            logger.info(f"Prometheus exporter started on port {exporter_port}")
-
-        producer = job.producer
+        producer = job.input
         logger.info(f"Producing from {producer.__module__}")
         job.init(context)
         asyncio.run(job.run())
-    except jsonschema.exceptions.ValidationError as schema_error:
-        # print a validation message with the source lines
-        cli_helpers.pprint_yaml_validation_error(job_file, schema_error, logger)
     except Exception as e:
         cli_helpers.handle_critical(logger, "Error while running a job", e)
 
 
 @cli.command(name="test", help="Unit test one or more job using data test definitions")
 @cli_helpers.add_options(LOG_LEVEL_OPTION)
 def test(
```

### Comparing `datayoga-1.87.0/PKG-INFO` & `datayoga-1.9.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: datayoga
-Version: 1.87.0
+Version: 1.9.0
 Summary: DataYoga command line interface
 License: Apache-2.0
 Author: DataYoga
 Author-email: admin@datayoga.io
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Database
 Provides-Extra: test
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: certifi (>=2022.12.7,<2023.0.0)
 Requires-Dist: click (>=8.0.3,<9.0.0)
-Requires-Dist: datayoga-core (==1.*)
+Requires-Dist: datayoga-core (>=1.0.0,<2.0.0)
 Requires-Dist: jsonschema (>=4.4.0,<5.0.0)
-Requires-Dist: mock (>=4.0.3,<5.0.0) ; extra == "test"
-Requires-Dist: pytest (>=7.1.2,<8.0.0) ; extra == "test"
-Requires-Dist: pytest-asyncio (>=0.20.1,<0.21.0)
-Requires-Dist: pytest-describe (>=2.0.1,<3.0.0) ; extra == "test"
-Requires-Dist: pytest-mock (>=3.7.0,<4.0.0) ; extra == "test"
-Requires-Dist: pytest-timeout (>=2.1.0,<3.0.0) ; extra == "test"
-Requires-Dist: requests-mock (>=1.9.3,<2.0.0) ; extra == "test"
+Requires-Dist: mock (>=4.0.3,<5.0.0); extra == "test"
+Requires-Dist: pytest (>=7.1.2,<8.0.0); extra == "test"
+Requires-Dist: pytest-describe (>=2.0.1,<3.0.0); extra == "test"
+Requires-Dist: pytest-mock (>=3.7.0,<4.0.0); extra == "test"
+Requires-Dist: pytest-timeout (>=2.1.0,<3.0.0); extra == "test"
+Requires-Dist: requests-mock (>=1.9.3,<2.0.0); extra == "test"
 Project-URL: url, https://datayoga.io
 Description-Content-Type: text/markdown
 
 # DataYoga CLI
 
 ## Development
 
@@ -62,18 +61,7 @@
 
 ## Run CLI in Development Mode
 
 ```bash
 python ./cli/src/datayoga/__main__.py
 ```
 
-## Running tests
-
-### Core
-
-```
-cd core
-pip install .
-pip install .[test]
-PYTHONPATH=src python -m pytest -s --log-cli-level=DEBUG
-```
-
```

