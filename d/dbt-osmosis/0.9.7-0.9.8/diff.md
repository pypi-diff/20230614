# Comparing `tmp/dbt-osmosis-0.9.7.tar.gz` & `tmp/dbt_osmosis-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-osmosis-0.9.7.tar", max compression
+gzip compressed data, was "dbt_osmosis-0.9.8.tar", max compression
```

## Comparing `dbt-osmosis-0.9.7.tar` & `dbt_osmosis-0.9.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11357 2022-05-31 01:49:38.666272 dbt-osmosis-0.9.7/LICENSE
--rw-r--r--   0        0        0    13964 2022-10-11 02:26:54.926633 dbt-osmosis-0.9.7/README.md
--rw-r--r--   0        0        0     2864 2022-10-23 16:35:09.412023 dbt-osmosis-0.9.7/pyproject.toml
--rw-r--r--   0        0        0        0 2022-06-07 03:38:40.889892 dbt-osmosis-0.9.7/src/dbt_osmosis/__init__.py
--rw-r--r--   0        0        0      103 2022-10-11 02:26:54.929422 dbt-osmosis-0.9.7/src/dbt_osmosis/__main__.py
--rw-r--r--   0        0        0    14886 2022-10-04 23:18:21.263197 dbt-osmosis-0.9.7/src/dbt_osmosis/app.py
--rw-r--r--   0        0        0        0 2022-06-07 03:51:33.818720 dbt-osmosis-0.9.7/src/dbt_osmosis/core/__init__.py
--rw-r--r--   0        0        0    12515 2022-09-03 23:42:45.525357 dbt-osmosis-0.9.7/src/dbt_osmosis/core/audit_macros.jinja2
--rw-r--r--   0        0        0     6292 2022-10-04 19:11:59.036775 dbt-osmosis-0.9.7/src/dbt_osmosis/core/diff.py
--rw-r--r--   0        0        0      193 2022-05-31 01:49:38.674195 dbt-osmosis-0.9.7/src/dbt_osmosis/core/exceptions.py
--rw-r--r--   0        0        0     2666 2022-08-04 23:42:14.515694 dbt-osmosis-0.9.7/src/dbt_osmosis/core/log_controller.py
--rw-r--r--   0        0        0      462 2022-10-02 06:16:05.701039 dbt-osmosis-0.9.7/src/dbt_osmosis/core/macros.py
--rw-r--r--   0        0        0    59176 2022-10-14 17:44:33.702142 dbt-osmosis-0.9.7/src/dbt_osmosis/core/osmosis.py
--rw-r--r--   0        0        0     1197 2022-10-14 17:32:18.785360 dbt-osmosis-0.9.7/src/dbt_osmosis/core/patch.py
--rw-r--r--   0        0        0    12734 2022-10-04 22:33:44.902333 dbt-osmosis-0.9.7/src/dbt_osmosis/core/server.py
--rw-r--r--   0        0        0    21350 2022-10-23 16:36:23.081671 dbt-osmosis-0.9.7/src/dbt_osmosis/core/server_v2.py
--rw-r--r--   0        0        0     1214 2022-10-11 02:26:58.065802 dbt-osmosis-0.9.7/src/dbt_osmosis/dbt_templater/LICENSE.md
--rw-r--r--   0        0        0      550 2022-10-11 02:26:58.066112 dbt-osmosis-0.9.7/src/dbt_osmosis/dbt_templater/__init__.py
--rw-r--r--   0        0        0     5867 2022-10-14 20:34:27.159330 dbt-osmosis-0.9.7/src/dbt_osmosis/dbt_templater/templater.py
--rw-r--r--   0        0        0    20111 2022-10-23 16:41:37.220600 dbt-osmosis-0.9.7/src/dbt_osmosis/main.py
--rw-r--r--   0        0        0      554 2022-10-01 18:07:37.984895 dbt-osmosis-0.9.7/src/dbt_osmosis/requirements.txt
--rw-r--r--   0        0        0     4470 2022-10-23 16:29:58.684558 dbt-osmosis-0.9.7/src/dbt_osmosis/sqlfluff_util.py
--rw-r--r--   0        0        0    16194 1970-01-01 00:00:00.000000 dbt-osmosis-0.9.7/setup.py
--rw-r--r--   0        0        0    16553 1970-01-01 00:00:00.000000 dbt-osmosis-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-05-31 01:49:38.666272 dbt_osmosis-0.9.8/LICENSE
+-rw-r--r--   0        0        0    14085 2022-10-28 22:08:29.554600 dbt_osmosis-0.9.8/README.md
+-rw-r--r--   0        0        0     2864 2022-11-22 08:15:59.940771 dbt_osmosis-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-06-07 03:38:40.889892 dbt_osmosis-0.9.8/src/dbt_osmosis/__init__.py
+-rw-r--r--   0        0        0      103 2022-10-11 02:26:54.929422 dbt_osmosis-0.9.8/src/dbt_osmosis/__main__.py
+-rw-r--r--   0        0        0    14886 2022-10-04 23:18:21.263197 dbt_osmosis-0.9.8/src/dbt_osmosis/app.py
+-rw-r--r--   0        0        0        0 2022-06-07 03:51:33.818720 dbt_osmosis-0.9.8/src/dbt_osmosis/core/__init__.py
+-rw-r--r--   0        0        0    12515 2022-09-03 23:42:45.525357 dbt_osmosis-0.9.8/src/dbt_osmosis/core/audit_macros.jinja2
+-rw-r--r--   0        0        0     6292 2022-10-04 19:11:59.036775 dbt_osmosis-0.9.8/src/dbt_osmosis/core/diff.py
+-rw-r--r--   0        0        0      193 2022-05-31 01:49:38.674195 dbt_osmosis-0.9.8/src/dbt_osmosis/core/exceptions.py
+-rw-r--r--   0        0        0     2666 2022-08-04 23:42:14.515694 dbt_osmosis-0.9.8/src/dbt_osmosis/core/log_controller.py
+-rw-r--r--   0        0        0      462 2022-10-02 06:16:05.701039 dbt_osmosis-0.9.8/src/dbt_osmosis/core/macros.py
+-rw-r--r--   0        0        0    59176 2022-10-14 17:44:33.702142 dbt_osmosis-0.9.8/src/dbt_osmosis/core/osmosis.py
+-rw-r--r--   0        0        0     1197 2022-10-14 17:32:18.785360 dbt_osmosis-0.9.8/src/dbt_osmosis/core/patch.py
+-rw-r--r--   0        0        0    12734 2022-10-04 22:33:44.902333 dbt_osmosis-0.9.8/src/dbt_osmosis/core/server.py
+-rw-r--r--   0        0        0    21350 2022-10-23 16:36:23.081671 dbt_osmosis-0.9.8/src/dbt_osmosis/core/server_v2.py
+-rw-r--r--   0        0        0     1214 2022-10-11 02:26:58.065802 dbt_osmosis-0.9.8/src/dbt_osmosis/dbt_templater/LICENSE.md
+-rw-r--r--   0        0        0      550 2022-10-11 02:26:58.066112 dbt_osmosis-0.9.8/src/dbt_osmosis/dbt_templater/__init__.py
+-rw-r--r--   0        0        0     5867 2022-10-14 20:34:27.159330 dbt_osmosis-0.9.8/src/dbt_osmosis/dbt_templater/templater.py
+-rw-r--r--   0        0        0    20111 2022-10-23 16:41:37.220600 dbt_osmosis-0.9.8/src/dbt_osmosis/main.py
+-rw-r--r--   0        0        0      554 2022-10-01 18:07:37.984895 dbt_osmosis-0.9.8/src/dbt_osmosis/requirements.txt
+-rw-r--r--   0        0        0     4677 2022-11-22 08:15:37.824305 dbt_osmosis-0.9.8/src/dbt_osmosis/sqlfluff_util.py
+-rw-r--r--   0        0        0    16317 1970-01-01 00:00:00.000000 dbt_osmosis-0.9.8/setup.py
+-rw-r--r--   0        0        0    16674 1970-01-01 00:00:00.000000 dbt_osmosis-0.9.8/PKG-INFO
```

### Comparing `dbt-osmosis-0.9.7/LICENSE` & `dbt_osmosis-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-osmosis-0.9.7/README.md` & `dbt_osmosis-0.9.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -311,7 +311,9 @@
 ## Roadmap
 
 These features are being actively developed and will be merged into the next few minor releases
 
 1. Complete high performance dbt server solution for running & compiling dbt SQL statements
 2. Extend git diff functionality to pin revisions of models in dedicated schema(s) in the warehouse  
 3. Complete build out of `sources` tools
+
+![graph](https://repobeats.axiom.co/api/embed/df37714aa5780fc79871c60e6fc623f8f8e45c35.svg "Repobeats analytics image")
```

### Comparing `dbt-osmosis-0.9.7/pyproject.toml` & `dbt_osmosis-0.9.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-osmosis"
-version = "0.9.7"
+version = "0.9.8"
 description = "A dbt server and suite of optional developer tools to make developing with dbt delightful."
 authors = ["z3z1ma <butler.alex2010@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

### Comparing `dbt-osmosis-0.9.7/src/dbt_osmosis/app.py` & `dbt_osmosis-0.9.8/src/dbt_osmosis/app.py`

 * *Files identical despite different names*

### Comparing `dbt-osmosis-0.9.7/src/dbt_osmosis/core/audit_macros.jinja2` & `dbt_osmosis-0.9.8/src/dbt_osmosis/core/audit_macros.jinja2`

 * *Files identical despite different names*

### Comparing `dbt-osmosis-0.9.7/src/dbt_osmosis/core/diff.py` & `dbt_osmosis-0.9.8/src/dbt_osmosis/core/diff.py`

 * *Files identical despite different names*

### Comparing `dbt-osmosis-0.9.7/src/dbt_osmosis/core/log_controller.py` & `dbt_osmosis-0.9.8/src/dbt_osmosis/core/log_controller.py`

 * *Files identical despite different names*

### Comparing `dbt-osmosis-0.9.7/src/dbt_osmosis/core/osmosis.py` & `dbt_osmosis-0.9.8/src/dbt_osmosis/core/osmosis.py`

 * *Files identical despite different names*

### Comparing `dbt-osmosis-0.9.7/src/dbt_osmosis/core/patch.py` & `dbt_osmosis-0.9.8/src/dbt_osmosis/core/patch.py`

 * *Files identical despite different names*

### Comparing `dbt-osmosis-0.9.7/src/dbt_osmosis/core/server.py` & `dbt_osmosis-0.9.8/src/dbt_osmosis/core/server.py`

 * *Files identical despite different names*

### Comparing `dbt-osmosis-0.9.7/src/dbt_osmosis/core/server_v2.py` & `dbt_osmosis-0.9.8/src/dbt_osmosis/core/server_v2.py`

 * *Files identical despite different names*

### Comparing `dbt-osmosis-0.9.7/src/dbt_osmosis/dbt_templater/LICENSE.md` & `dbt_osmosis-0.9.8/src/dbt_osmosis/dbt_templater/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-osmosis-0.9.7/src/dbt_osmosis/dbt_templater/__init__.py` & `dbt_osmosis-0.9.8/src/dbt_osmosis/dbt_templater/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-osmosis-0.9.7/src/dbt_osmosis/dbt_templater/templater.py` & `dbt_osmosis-0.9.8/src/dbt_osmosis/dbt_templater/templater.py`

 * *Files identical despite different names*

### Comparing `dbt-osmosis-0.9.7/src/dbt_osmosis/main.py` & `dbt_osmosis-0.9.8/src/dbt_osmosis/main.py`

 * *Files identical despite different names*

### Comparing `dbt-osmosis-0.9.7/src/dbt_osmosis/requirements.txt` & `dbt_osmosis-0.9.8/src/dbt_osmosis/requirements.txt`

 * *Files identical despite different names*

### Comparing `dbt-osmosis-0.9.7/src/dbt_osmosis/sqlfluff_util.py` & `dbt_osmosis-0.9.8/src/dbt_osmosis/sqlfluff_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,18 +6,21 @@
 from typing import Dict, Optional, Union
 
 from sqlfluff.cli.commands import get_linter_and_formatter
 from sqlfluff.cli.outputstream import FileOutput
 from sqlfluff.core.config import ConfigLoader, FluffConfig
 
 # Cache linters (up to 50 though its arbitrary)
-get_linter = lru_cache(maxsize=50)(lambda cfg, stream: get_linter_and_formatter(cfg, stream)[0])
+# DISABLING CACHE until tests prove it valuable
+# get_linter = lru_cache(maxsize=50)(lambda cfg, stream: get_linter_and_formatter(cfg, stream)[0])
+get_linter = lambda cfg, stream: get_linter_and_formatter(cfg, stream)[0]
 
-# Cache config to prevent wasted frames
-@lru_cache(maxsize=50)
+# Cache config to prevent wasted frames / disk seeks in high concurrency
+# DISABLING CACHE until tests prove it valuable
+# @lru_cache(maxsize=50)
 def get_config(
     dbt_project_root: Path,
     extra_config_path: Optional[Path] = None,
     ignore_local_config: bool = False,
     require_dialect: bool = True,
     **kwargs,
 ) -> FluffConfig:
```

### Comparing `dbt-osmosis-0.9.7/setup.py` & `dbt_osmosis-0.9.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,17 @@
 entry_points = \
 {'console_scripts': ['dbt-osmosis = dbt_osmosis.main:cli',
                      'dbt-osmosis-proxy = dbt_osmosis.server:cli'],
  'sqlfluff': ['dbt_templater = dbt_osmosis.dbt_templater']}
 
 setup_kwargs = {
     'name': 'dbt-osmosis',
-    'version': '0.9.7',
+    'version': '0.9.8',
     'description': 'A dbt server and suite of optional developer tools to make developing with dbt delightful.',
-    'long_description': '# dbt-osmosis\n\n<!--![GitHub Actions](https://github.com/z3z1ma/dbt-osmosis/actions/workflows/master.yml/badge.svg)-->\n\n![PyPI](https://img.shields.io/pypi/v/dbt-osmosis)\n![Downloads](https://pepy.tech/badge/dbt-osmosis)\n![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-green.svg)\n![black](https://img.shields.io/badge/code%20style-black-000000.svg)\n[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://z3z1ma-dbt-osmosis-srcdbt-osmosisapp-4y67qs.streamlitapp.com/)\n\n\n## Primary Objectives\n\nHello and welcome to the project! [dbt-osmosis](https://github.com/z3z1ma/dbt-osmosis) 🌊 serves to enhance the developer experience significantly. We do this through providing 4 core features:\n\n1. Automated schema YAML management.\n    \n    1a. `dbt-osmosis yaml refactor --project-dir ... --profiles-dir ...`\n\n    > Automatically generate documentation based on upstream documented columns, organize yaml files based on configurable rules defined in dbt_project.yml, scaffold new yaml files based on the same rules, inject columns from data warehouse schema if missing in yaml and remove columns no longer present in data warehouse (organize -> document)\n\n    1b. `dbt-osmosis yaml organize --project-dir ... --profiles-dir ...`\n\n    > Organize yaml files based on configurable rules defined in dbt_project.yml, scaffold new yaml files based on the same rules\n\n    1c. `dbt-osmosis yaml document --project-dir ... --profiles-dir ...`\n\n    > Automatically generate documentation based on upstream documented columns\n\n2. A highly performant dbt server which integrates with tools such as dbt-power-user for VS Code to enable interactive querying + realtime compilation from your IDE\n\n    2a. `dbt-osmosis server serve --project-dir ... --profiles-dir ...`\n\n    > Spins up a FastAPI server. Can be passed --register-project to automatically register your local project. API documentation is available at /docs endpoint where interestingly enough, you can query your data warehouse or compile SQL via the Try It function\n\n3. Workbench for dbt Jinja SQL. This workbench is powered by streamlit and the badge at the top of the readme will take you to a demo on streamlit cloud with jaffle_shop loaded (requires extra `pip install dbt-osmosis[workbench]`). \n\n    3a. `dbt-osmosis workbench --project-dir ... --profiles-dir ...`\n\n    > Spins up a streamlit app. This workbench offers similar functionality to the osmosis server + power-user combo without a reliance on VS code. Realtime compilation, query execution, pandas profiling all via copying and pasting whatever you are working on into the workbenchat your leisure. Spin it up and down as needed.\n\n4. Diffs for data model outputs to model outputs across git revisions \n\n    4a. `dbt-osmosis diff -m some_model  --project-dir ... --profiles-dir ...`\n\n    > Run diffs on models dynamically. This pulls the state of the model before changes from your git history, injects it as a node to the dbt manifest, compiles the old and modified nodes, and diffs their query results optionally writing nodes to temp tables before running the diff query for warehouses with performance or query complexity limits (👀 bigquery)\n    \n## References\n\n[Server Reference](#server)\n\n[Workbench Reference](#workbench)\n\n[YAML Reference](#yaml-management)\n\n[Python API Reference](#python-api)\n\n____\n\n## Server\n\n```sh\n# Command to start server\ndbt-osmosis server serve --host ... --port ...\n```\n\nThe server is self documenting via open API. From the open API docs you can compile SQL or run it to get an idea of the requests and responses. Furthermore the server supports multiple dbt projects out of the box. This means the server can `/register` 10s to 100s of projects and selectively compile or run against a specific one via an `X-dbt-Project` header. It is stress tested at high loads and volumes, higher than its ever likely to be put through as primarily a dev accelerator but it could be used in a production application too and is the focus of much of the development in the repo. It is Apache 2.0 licensed which differentiates it from dbt-core server. Furthermore it is more focused on SQL than "models" as it is not a replacement for the CLI nor does it aspire to be. Instead it is more of a database adapter/interface of sorts which lets it be really good at one thing.\n\n![server-docs](/screenshots/osmosis_server_docs.png)\n\nStarting the server is easy. Its most interesting and impactful integration is through [dbt-power-user](https://github.com/innoverio/vscode-dbt-power-user) which in the near term will hide away the details of starting or managing the server and simply provide a high quality developer experience out-of-the-box.\n\n![server-start](/screenshots/osmosis_server_startup.png)\n\n____\n\n## Workbench\n\nDemo the workbench 👇 \n\n[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://z3z1ma-dbt-osmosis-srcdbt-osmosisapp-4y67qs.streamlitapp.com/)\n\n \n```sh\npip install dbt-osmosis[workbench]\n\n# Command to start server\ndbt-osmosis workbench\n```\n\nPress "r" to reload the workbench at any time.\n\n\n✔️ dbt Editor with instant dbt compilation side-by-side or pivoted\n\n✔️ Full control over model and workbench theme, light and dark mode\n\n✔️ Query Tester, test the model you are working on for instant feedback\n\n✔️ Data Profiler (leverages pandas-profiling)\n\n\n**Editor** \n\nThe editor is able to compile models with control+enter or dynamically as you type. Its speedy! You can choose any target defined in your profiles yml for compilation and execution.\n\n![editor](/screenshots/osmosis_editor_main.png?raw=true "dbt-osmosis Workbench")\n\nYou can pivot the editor for a fuller view while workbenching some dbt SQL.\n\n![pivot](/screenshots/osmosis_editor_pivot.png?raw=true "dbt-osmosis Pivot Layout")\n\n\n**Test Query**\n\nTest dbt models as you work against whatever profile you have selected and inspect the results. This allows very fast iterative feedback loops not possible with VS Code alone.\n\n![test-model](/screenshots/osmosis_tester.png?raw=true "dbt-osmosis Test Model")\n\n**Profile Model Results**\n\nProfile your datasets on the fly while you develop without switching context. Allows for more refined interactive data modelling when dataset fits in memory.\n\n![profile-data](/screenshots/osmosis_profile.png?raw=true "dbt-osmosis Profile Data")\n\n\n**Useful Links and RSS Feed**\n\nSome useful links and RSS feeds at the bottom. 🤓\n\n![profile-data](/screenshots/osmosis_links.png?raw=true "dbt-osmosis Profile Data")\n\n____\n\n\n## YAML Management\n\ndbt-osmosis yaml management is extremely powerful and ready to use as-is. To get familiar, you should run it on a fresh branch and ensure everything is backed in source control. You\'ll wonder why its not in dbt-core. Enjoy!\n\nYou should set a base config in your dbt_project.yml and ensure any models within the scope of your execution plan will inherit a config/preference. Example below.\n\n```yaml\nmodels:\n\n    your_dbt_project:\n\n        # This config will apply to your whole project\n        +dbt-osmosis: "schema/model.yml"\n\n        staging:\n\n            # This config will apply to your staging directory\n            +dbt-osmosis: "folder.yml"\n\n            +tags: \n                - "staged"\n\n            +materialized: view\n\n            monday:\n                intermediate:\n                    +materialized: ephemeral\n\n        marts:\n\n            # Underscore prefixed model name as recommended in dbt best practices for everything in "marts" folder\n            +dbt-osmosis: "_model.yml"\n\n            +tags: \n                - "mart"\n\n            supply_chain: \n```\n\n## Features\n\n### Standardize organization of schema files (and provide ability to define and conform with code)\n\n- Config can be set on per directory basis if desired utilizing `dbt_project.yml`, all models which are processed require direct or inherited config `+dbt-osmosis:`. If even one dir is missing the config, we close gracefully and inform user to update dbt_project.yml. No assumed defaults. Placing our config under your dbt project name in `models:` is enough to set a default for the project since the config applies to all subdirectories. \n\n    Note: You can **change these configs as often as you like** or try them all, dbt-osmosis will take care of restructuring your project schema files-- _no human effort required_. \n\n    A directory can be configured to conform to any one of the following standards:\n\n    - Can be one schema file to one model file sharing the same name and directory ie. \n\n            staging/\n                stg_customer.sql\n                stg_customer.yml\n                stg_order.sql\n                stg_order.yml\n\n        - `+dbt-osmosis: "model.yml"`\n\n    - Can be one schema file per directory wherever model files reside named schema.yml, ie.\n\n            staging/\n                schema.yml\n                stg_customer.sql\n                stg_order.sql\n\n        - `+dbt-osmosis: "schema.yml"`\n    - Can be one schema file per directory wherever model files reside named after its containing folder, ie. \n\n            staging/\n                stg_customer.sql\n                stg_order.sql\n                staging.yml\n\n        - `+dbt-osmosis: "folder.yml"`\n\n    - Can be one schema file to one model file sharing the same name _nested_ in a schema subdir wherever model files reside, ie. \n\n            staging/\n                stg_order.sql\n                stg_customer.sql\n                schema/\n                    stg_customer.yml\n                    stg_order.yml\n\n        - `+dbt-osmosis: "schema/model.yml"`\n\n    - Can be one schema file to one model file sharing the same name and directory, models prefixed with underscore for IDE sorting ie. \n\n            staging/\n                _stg_customer.yml\n                _stg_order.yml\n                stg_customer.sql\n                stg_order.sql\n\n        - `+dbt-osmosis: "_model.yml"`\n\n### Build and Inject Non-documented models\n\n- Injected models will automatically conform to above config per directory based on location of model file. \n\n- This means you can focus fully on modelling; and documentation, including yaml updates or creation, will automatically follow at any time with simple invocation of dbt-osmosis\n\n### Propagate existing column level documentation downward to children\n\n- Build column level knowledge graph accumulated and updated from furthest identifiable origin (ancestors) to immediate parents\n\n- Will automatically populate undocumented columns of the same name with passed down knowledge accumulated within the context of the models upstream dependency tree\n\n- This means you can freely generate models and all columns you pull into the models SQL that already have been documented will be automatically learned/propagated. Again the focus for analysts is almost fully on modelling and yaml work is an afterthought / less heavy of a manual lift.\n\n### Order Matters\n\nIn a full run [ `dbt-osmosis yaml refactor` ] we will:\n\n1. Conform dbt project\n    - Configuration lives in `dbt_project.yml` --> we require our config to run, can be at root level of `models:` to apply a default convention to a project \n    or can be folder by folder, follows dbt config resolution where config is overridden by scope. \n    Config is called `+dbt-osmosis: "folder.yml" | "schema.yml" | "model.yml" | "schema/model.yml" | "_model.yml"`\n2. Bootstrap models to ensure all models exist\n3. Recompile Manifest\n4. Propagate definitions downstream to undocumented models solely within the context of each models dependency tree\n\n\n## Python API\n\nThough each core function is useful enough to stand as its own package, dbt osmosis sits as a unified interface primarily because all of these functions are built off of the same core API structures in the dbt osmosis package. dbt osmosis provides one of the cleanest interfaces to interacting with dbt if you aren\'t keen to play with dbt on-the-rails (like me) or you want to extend what osmosis can do, see below examples for how to interface with it from Python.\n\n```python\n# Programmatic Examples:\nfrom dbt_osmosis.core import DbtProject, DbtYamlManager\nfrom dbt_osmosis.diff import diff_and_print_to_console\n\n# Some dbt osmosis YAML management 📜\ndbt_yaml_manager = DbtYamlManager(\n    project_dir="/Users/alexanderbutler/Documents/harness/analytics-pipelines/projects/meltano/harness/transform",\n    target="prod",\n)\n\n# review the generated plan\ndbt_yaml_manager.pretty_print_restructure_plan(dbt_yaml_manager.draft_project_structure_update_plan())\n\n# organize your dbt project based on declarative config\ndbt_yaml_manager.commit_project_restructure_to_disk()\n\n# propagate column level documentation down the DAG\ndbt_yaml_manager.propagate_documentation_downstream()\n\n\n\n# Massively simplified dbt interfaces you likely won\'t find elsewhere 👏\n\nrunner = DbtProject(\n    project_dir="/Users/alexanderbutler/Documents/harness/analytics-pipelines/projects/meltano/harness/transform",\n    target="prod",\n)\n\n# execute macros through a simple interface without subprocesses\nrunner.execute_macro(\n    "create_schema",\n    kwargs={"relation": relation},\n)\n\n# compile SQL as easy as this 🤟\nrunner.compile_sql("select * from {{ ref(\'stg_salesforce__users\') }}")\n\n# run SQL too\nresult = runner.execute_sql("select * from {{ ref(\'stg_salesforce__users\') }}")\nresult.table.print_csv()\n\n# leverage git to diff the OUTPUT of a model from git HEAD \n# to your revision on disk to safely audit changes as you work\ndiff_and_print_to_console("fct_sales", pk="order_id", runner=runner)  \n```\n\n## Roadmap\n\nThese features are being actively developed and will be merged into the next few minor releases\n\n1. Complete high performance dbt server solution for running & compiling dbt SQL statements\n2. Extend git diff functionality to pin revisions of models in dedicated schema(s) in the warehouse  \n3. Complete build out of `sources` tools\n',
+    'long_description': '# dbt-osmosis\n\n<!--![GitHub Actions](https://github.com/z3z1ma/dbt-osmosis/actions/workflows/master.yml/badge.svg)-->\n\n![PyPI](https://img.shields.io/pypi/v/dbt-osmosis)\n![Downloads](https://pepy.tech/badge/dbt-osmosis)\n![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-green.svg)\n![black](https://img.shields.io/badge/code%20style-black-000000.svg)\n[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://z3z1ma-dbt-osmosis-srcdbt-osmosisapp-4y67qs.streamlitapp.com/)\n\n\n## Primary Objectives\n\nHello and welcome to the project! [dbt-osmosis](https://github.com/z3z1ma/dbt-osmosis) 🌊 serves to enhance the developer experience significantly. We do this through providing 4 core features:\n\n1. Automated schema YAML management.\n    \n    1a. `dbt-osmosis yaml refactor --project-dir ... --profiles-dir ...`\n\n    > Automatically generate documentation based on upstream documented columns, organize yaml files based on configurable rules defined in dbt_project.yml, scaffold new yaml files based on the same rules, inject columns from data warehouse schema if missing in yaml and remove columns no longer present in data warehouse (organize -> document)\n\n    1b. `dbt-osmosis yaml organize --project-dir ... --profiles-dir ...`\n\n    > Organize yaml files based on configurable rules defined in dbt_project.yml, scaffold new yaml files based on the same rules\n\n    1c. `dbt-osmosis yaml document --project-dir ... --profiles-dir ...`\n\n    > Automatically generate documentation based on upstream documented columns\n\n2. A highly performant dbt server which integrates with tools such as dbt-power-user for VS Code to enable interactive querying + realtime compilation from your IDE\n\n    2a. `dbt-osmosis server serve --project-dir ... --profiles-dir ...`\n\n    > Spins up a FastAPI server. Can be passed --register-project to automatically register your local project. API documentation is available at /docs endpoint where interestingly enough, you can query your data warehouse or compile SQL via the Try It function\n\n3. Workbench for dbt Jinja SQL. This workbench is powered by streamlit and the badge at the top of the readme will take you to a demo on streamlit cloud with jaffle_shop loaded (requires extra `pip install dbt-osmosis[workbench]`). \n\n    3a. `dbt-osmosis workbench --project-dir ... --profiles-dir ...`\n\n    > Spins up a streamlit app. This workbench offers similar functionality to the osmosis server + power-user combo without a reliance on VS code. Realtime compilation, query execution, pandas profiling all via copying and pasting whatever you are working on into the workbenchat your leisure. Spin it up and down as needed.\n\n4. Diffs for data model outputs to model outputs across git revisions \n\n    4a. `dbt-osmosis diff -m some_model  --project-dir ... --profiles-dir ...`\n\n    > Run diffs on models dynamically. This pulls the state of the model before changes from your git history, injects it as a node to the dbt manifest, compiles the old and modified nodes, and diffs their query results optionally writing nodes to temp tables before running the diff query for warehouses with performance or query complexity limits (👀 bigquery)\n    \n## References\n\n[Server Reference](#server)\n\n[Workbench Reference](#workbench)\n\n[YAML Reference](#yaml-management)\n\n[Python API Reference](#python-api)\n\n____\n\n## Server\n\n```sh\n# Command to start server\ndbt-osmosis server serve --host ... --port ...\n```\n\nThe server is self documenting via open API. From the open API docs you can compile SQL or run it to get an idea of the requests and responses. Furthermore the server supports multiple dbt projects out of the box. This means the server can `/register` 10s to 100s of projects and selectively compile or run against a specific one via an `X-dbt-Project` header. It is stress tested at high loads and volumes, higher than its ever likely to be put through as primarily a dev accelerator but it could be used in a production application too and is the focus of much of the development in the repo. It is Apache 2.0 licensed which differentiates it from dbt-core server. Furthermore it is more focused on SQL than "models" as it is not a replacement for the CLI nor does it aspire to be. Instead it is more of a database adapter/interface of sorts which lets it be really good at one thing.\n\n![server-docs](/screenshots/osmosis_server_docs.png)\n\nStarting the server is easy. Its most interesting and impactful integration is through [dbt-power-user](https://github.com/innoverio/vscode-dbt-power-user) which in the near term will hide away the details of starting or managing the server and simply provide a high quality developer experience out-of-the-box.\n\n![server-start](/screenshots/osmosis_server_startup.png)\n\n____\n\n## Workbench\n\nDemo the workbench 👇 \n\n[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://z3z1ma-dbt-osmosis-srcdbt-osmosisapp-4y67qs.streamlitapp.com/)\n\n \n```sh\npip install dbt-osmosis[workbench]\n\n# Command to start server\ndbt-osmosis workbench\n```\n\nPress "r" to reload the workbench at any time.\n\n\n✔️ dbt Editor with instant dbt compilation side-by-side or pivoted\n\n✔️ Full control over model and workbench theme, light and dark mode\n\n✔️ Query Tester, test the model you are working on for instant feedback\n\n✔️ Data Profiler (leverages pandas-profiling)\n\n\n**Editor** \n\nThe editor is able to compile models with control+enter or dynamically as you type. Its speedy! You can choose any target defined in your profiles yml for compilation and execution.\n\n![editor](/screenshots/osmosis_editor_main.png?raw=true "dbt-osmosis Workbench")\n\nYou can pivot the editor for a fuller view while workbenching some dbt SQL.\n\n![pivot](/screenshots/osmosis_editor_pivot.png?raw=true "dbt-osmosis Pivot Layout")\n\n\n**Test Query**\n\nTest dbt models as you work against whatever profile you have selected and inspect the results. This allows very fast iterative feedback loops not possible with VS Code alone.\n\n![test-model](/screenshots/osmosis_tester.png?raw=true "dbt-osmosis Test Model")\n\n**Profile Model Results**\n\nProfile your datasets on the fly while you develop without switching context. Allows for more refined interactive data modelling when dataset fits in memory.\n\n![profile-data](/screenshots/osmosis_profile.png?raw=true "dbt-osmosis Profile Data")\n\n\n**Useful Links and RSS Feed**\n\nSome useful links and RSS feeds at the bottom. 🤓\n\n![profile-data](/screenshots/osmosis_links.png?raw=true "dbt-osmosis Profile Data")\n\n____\n\n\n## YAML Management\n\ndbt-osmosis yaml management is extremely powerful and ready to use as-is. To get familiar, you should run it on a fresh branch and ensure everything is backed in source control. You\'ll wonder why its not in dbt-core. Enjoy!\n\nYou should set a base config in your dbt_project.yml and ensure any models within the scope of your execution plan will inherit a config/preference. Example below.\n\n```yaml\nmodels:\n\n    your_dbt_project:\n\n        # This config will apply to your whole project\n        +dbt-osmosis: "schema/model.yml"\n\n        staging:\n\n            # This config will apply to your staging directory\n            +dbt-osmosis: "folder.yml"\n\n            +tags: \n                - "staged"\n\n            +materialized: view\n\n            monday:\n                intermediate:\n                    +materialized: ephemeral\n\n        marts:\n\n            # Underscore prefixed model name as recommended in dbt best practices for everything in "marts" folder\n            +dbt-osmosis: "_model.yml"\n\n            +tags: \n                - "mart"\n\n            supply_chain: \n```\n\n## Features\n\n### Standardize organization of schema files (and provide ability to define and conform with code)\n\n- Config can be set on per directory basis if desired utilizing `dbt_project.yml`, all models which are processed require direct or inherited config `+dbt-osmosis:`. If even one dir is missing the config, we close gracefully and inform user to update dbt_project.yml. No assumed defaults. Placing our config under your dbt project name in `models:` is enough to set a default for the project since the config applies to all subdirectories. \n\n    Note: You can **change these configs as often as you like** or try them all, dbt-osmosis will take care of restructuring your project schema files-- _no human effort required_. \n\n    A directory can be configured to conform to any one of the following standards:\n\n    - Can be one schema file to one model file sharing the same name and directory ie. \n\n            staging/\n                stg_customer.sql\n                stg_customer.yml\n                stg_order.sql\n                stg_order.yml\n\n        - `+dbt-osmosis: "model.yml"`\n\n    - Can be one schema file per directory wherever model files reside named schema.yml, ie.\n\n            staging/\n                schema.yml\n                stg_customer.sql\n                stg_order.sql\n\n        - `+dbt-osmosis: "schema.yml"`\n    - Can be one schema file per directory wherever model files reside named after its containing folder, ie. \n\n            staging/\n                stg_customer.sql\n                stg_order.sql\n                staging.yml\n\n        - `+dbt-osmosis: "folder.yml"`\n\n    - Can be one schema file to one model file sharing the same name _nested_ in a schema subdir wherever model files reside, ie. \n\n            staging/\n                stg_order.sql\n                stg_customer.sql\n                schema/\n                    stg_customer.yml\n                    stg_order.yml\n\n        - `+dbt-osmosis: "schema/model.yml"`\n\n    - Can be one schema file to one model file sharing the same name and directory, models prefixed with underscore for IDE sorting ie. \n\n            staging/\n                _stg_customer.yml\n                _stg_order.yml\n                stg_customer.sql\n                stg_order.sql\n\n        - `+dbt-osmosis: "_model.yml"`\n\n### Build and Inject Non-documented models\n\n- Injected models will automatically conform to above config per directory based on location of model file. \n\n- This means you can focus fully on modelling; and documentation, including yaml updates or creation, will automatically follow at any time with simple invocation of dbt-osmosis\n\n### Propagate existing column level documentation downward to children\n\n- Build column level knowledge graph accumulated and updated from furthest identifiable origin (ancestors) to immediate parents\n\n- Will automatically populate undocumented columns of the same name with passed down knowledge accumulated within the context of the models upstream dependency tree\n\n- This means you can freely generate models and all columns you pull into the models SQL that already have been documented will be automatically learned/propagated. Again the focus for analysts is almost fully on modelling and yaml work is an afterthought / less heavy of a manual lift.\n\n### Order Matters\n\nIn a full run [ `dbt-osmosis yaml refactor` ] we will:\n\n1. Conform dbt project\n    - Configuration lives in `dbt_project.yml` --> we require our config to run, can be at root level of `models:` to apply a default convention to a project \n    or can be folder by folder, follows dbt config resolution where config is overridden by scope. \n    Config is called `+dbt-osmosis: "folder.yml" | "schema.yml" | "model.yml" | "schema/model.yml" | "_model.yml"`\n2. Bootstrap models to ensure all models exist\n3. Recompile Manifest\n4. Propagate definitions downstream to undocumented models solely within the context of each models dependency tree\n\n\n## Python API\n\nThough each core function is useful enough to stand as its own package, dbt osmosis sits as a unified interface primarily because all of these functions are built off of the same core API structures in the dbt osmosis package. dbt osmosis provides one of the cleanest interfaces to interacting with dbt if you aren\'t keen to play with dbt on-the-rails (like me) or you want to extend what osmosis can do, see below examples for how to interface with it from Python.\n\n```python\n# Programmatic Examples:\nfrom dbt_osmosis.core import DbtProject, DbtYamlManager\nfrom dbt_osmosis.diff import diff_and_print_to_console\n\n# Some dbt osmosis YAML management 📜\ndbt_yaml_manager = DbtYamlManager(\n    project_dir="/Users/alexanderbutler/Documents/harness/analytics-pipelines/projects/meltano/harness/transform",\n    target="prod",\n)\n\n# review the generated plan\ndbt_yaml_manager.pretty_print_restructure_plan(dbt_yaml_manager.draft_project_structure_update_plan())\n\n# organize your dbt project based on declarative config\ndbt_yaml_manager.commit_project_restructure_to_disk()\n\n# propagate column level documentation down the DAG\ndbt_yaml_manager.propagate_documentation_downstream()\n\n\n\n# Massively simplified dbt interfaces you likely won\'t find elsewhere 👏\n\nrunner = DbtProject(\n    project_dir="/Users/alexanderbutler/Documents/harness/analytics-pipelines/projects/meltano/harness/transform",\n    target="prod",\n)\n\n# execute macros through a simple interface without subprocesses\nrunner.execute_macro(\n    "create_schema",\n    kwargs={"relation": relation},\n)\n\n# compile SQL as easy as this 🤟\nrunner.compile_sql("select * from {{ ref(\'stg_salesforce__users\') }}")\n\n# run SQL too\nresult = runner.execute_sql("select * from {{ ref(\'stg_salesforce__users\') }}")\nresult.table.print_csv()\n\n# leverage git to diff the OUTPUT of a model from git HEAD \n# to your revision on disk to safely audit changes as you work\ndiff_and_print_to_console("fct_sales", pk="order_id", runner=runner)  \n```\n\n## Roadmap\n\nThese features are being actively developed and will be merged into the next few minor releases\n\n1. Complete high performance dbt server solution for running & compiling dbt SQL statements\n2. Extend git diff functionality to pin revisions of models in dedicated schema(s) in the warehouse  \n3. Complete build out of `sources` tools\n\n![graph](https://repobeats.axiom.co/api/embed/df37714aa5780fc79871c60e6fc623f8f8e45c35.svg "Repobeats analytics image")\n',
     'author': 'z3z1ma',
     'author_email': 'butler.alex2010@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/z3z1ma/dbt-osmosis',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `dbt-osmosis-0.9.7/PKG-INFO` & `dbt_osmosis-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-osmosis
-Version: 0.9.7
+Version: 0.9.8
 Summary: A dbt server and suite of optional developer tools to make developing with dbt delightful.
 Home-page: https://github.com/z3z1ma/dbt-osmosis
 License: Apache 2.0
 Keywords: dbt,server,streamlit,git,diff
 Author: z3z1ma
 Author-email: butler.alex2010@gmail.com
 Requires-Python: >=3.8,<3.11
@@ -369,7 +369,9 @@
 
 These features are being actively developed and will be merged into the next few minor releases
 
 1. Complete high performance dbt server solution for running & compiling dbt SQL statements
 2. Extend git diff functionality to pin revisions of models in dedicated schema(s) in the warehouse  
 3. Complete build out of `sources` tools
 
+![graph](https://repobeats.axiom.co/api/embed/df37714aa5780fc79871c60e6fc623f8f8e45c35.svg "Repobeats analytics image")
+
```

