# Comparing `tmp/griffon-0.2.5.tar.gz` & `tmp/griffon-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griffon-0.2.5.tar", last modified: Fri May 26 14:39:19 2023, max compression
+gzip compressed data, was "griffon-0.2.6.tar", last modified: Mon May 29 09:30:55 2023, max compression
```

## Comparing `griffon-0.2.5.tar` & `griffon-0.2.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:39:19.517255 griffon-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 14:39:02.000000 griffon-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-26 14:39:19.517255 griffon-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-26 14:39:02.000000 griffon-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:39:19.513256 griffon-0.2.5/griffon/
--rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:39:19.513256 griffon-0.2.5/griffon/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/autocomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:39:19.513256 griffon-0.2.5/griffon/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:39:19.513256 griffon-0.2.5/griffon/commands/entities/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26909 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/entities/community_component_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    27403 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/entities/corgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/entities/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/entities/osidb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/plugin_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:39:19.517255 griffon-0.2.5/griffon/commands/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/plugins/bugzilla.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/plugins/cve_mitre.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/plugins/cvelib.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/plugins/fcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/plugins/go_vuln.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/plugins/osv.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/plugins/semgrep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/process.py
--rw-r--r--   0 runner    (1001) docker     (123)    26911 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    52663 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:39:19.517255 griffon-0.2.5/griffon/services/
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/services/core_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    35881 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/services/core_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    20730 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/services/core_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:39:19.517255 griffon-0.2.5/griffon/static/
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/static/default_griffonrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:39:19.513256 griffon-0.2.5/griffon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-26 14:39:19.000000 griffon-0.2.5/griffon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-26 14:39:19.000000 griffon-0.2.5/griffon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 14:39:19.000000 griffon-0.2.5/griffon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-26 14:39:19.000000 griffon-0.2.5/griffon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-26 14:39:19.000000 griffon-0.2.5/griffon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-26 14:39:19.000000 griffon-0.2.5/griffon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-26 14:39:02.000000 griffon-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 14:39:19.517255 griffon-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-26 14:39:02.000000 griffon-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:39:19.517255 griffon-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-26 14:39:02.000000 griffon-0.2.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-26 14:39:02.000000 griffon-0.2.5/tests/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-26 14:39:02.000000 griffon-0.2.5/tests/test_manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-26 14:39:02.000000 griffon-0.2.5/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-26 14:39:02.000000 griffon-0.2.5/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-26 14:39:02.000000 griffon-0.2.5/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-26 14:39:02.000000 griffon-0.2.5/tests/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-26 14:39:02.000000 griffon-0.2.5/tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:30:55.925374 griffon-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-29 09:30:36.000000 griffon-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-29 09:30:55.925374 griffon-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-29 09:30:36.000000 griffon-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:30:55.921374 griffon-0.2.6/griffon/
+-rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:30:55.921374 griffon-0.2.6/griffon/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/autocomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:30:55.921374 griffon-0.2.6/griffon/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/commands/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/commands/docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:30:55.921374 griffon-0.2.6/griffon/commands/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/commands/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26909 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/commands/entities/community_component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27403 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/commands/entities/corgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/commands/entities/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/commands/entities/osidb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/commands/plugin_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:30:55.925374 griffon-0.2.6/griffon/commands/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/commands/plugins/bugzilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/commands/plugins/cve_mitre.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/commands/plugins/cvelib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/commands/plugins/fcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/commands/plugins/go_vuln.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/commands/plugins/osv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/commands/plugins/semgrep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/commands/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26911 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/commands/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/commands/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52758 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:30:55.925374 griffon-0.2.6/griffon/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/services/core_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35881 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/services/core_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20730 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/services/core_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:30:55.925374 griffon-0.2.6/griffon/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-29 09:30:36.000000 griffon-0.2.6/griffon/static/default_griffonrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:30:55.921374 griffon-0.2.6/griffon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-29 09:30:55.000000 griffon-0.2.6/griffon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-29 09:30:55.000000 griffon-0.2.6/griffon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 09:30:55.000000 griffon-0.2.6/griffon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-29 09:30:55.000000 griffon-0.2.6/griffon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-29 09:30:55.000000 griffon-0.2.6/griffon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-29 09:30:55.000000 griffon-0.2.6/griffon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-29 09:30:36.000000 griffon-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 09:30:55.925374 griffon-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-29 09:30:36.000000 griffon-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:30:55.925374 griffon-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-29 09:30:36.000000 griffon-0.2.6/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-29 09:30:36.000000 griffon-0.2.6/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-29 09:30:36.000000 griffon-0.2.6/tests/test_manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-29 09:30:36.000000 griffon-0.2.6/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-29 09:30:36.000000 griffon-0.2.6/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-29 09:30:36.000000 griffon-0.2.6/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-29 09:30:36.000000 griffon-0.2.6/tests/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-29 09:30:36.000000 griffon-0.2.6/tests/test_unit.py
```

### Comparing `griffon-0.2.5/LICENSE` & `griffon-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/PKG-INFO` & `griffon-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griffon
-Version: 0.2.5
+Version: 0.2.6
 Summary: Red Hat Product Security CLI
 Home-page: https://github.com/RedHatProductSecurity/griffon
 Author: James Fuller, Red Hat Product Security
 License: MIT
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `griffon-0.2.5/README.md` & `griffon-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/griffon/__init__.py` & `griffon-0.2.6/griffon/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import osidb_bindings
 from osidb_bindings.bindings.python_client.models import Affect, Flaw, Tracker
 from pkg_resources import resource_filename  # type: ignore
 from rich.logging import RichHandler
 
 from griffon.output import console
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 
 if "CORGI_API_URL" not in os.environ:
     print("Must set CORGI_API_URL environment variable.")
     exit(1)
 CORGI_API_URL = os.environ["CORGI_API_URL"]
 
 if "OSIDB_API_URL" not in os.environ:
```

### Comparing `griffon-0.2.5/griffon/autocomplete/__init__.py` & `griffon-0.2.6/griffon/autocomplete/__init__.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/griffon/cli.py` & `griffon-0.2.6/griffon/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -107,26 +107,34 @@
     default=get_config_option("default", "verbosity", 0),
     help="Verbose output, more detailed search results, can be used multiple times (e.g. -vvv).",
 )  # noqa
 @click.option("--no-progress-bar", is_flag=True, help="Disable progress bar.")
 @click.option("--no-color", is_flag=True, help="Disable output of color ansi esc sequences.")
 @click.option("--no-wrap", is_flag=True, help="Disable wrapping of text output.")
 @click.option(
+    "--width",
+    "terminal_width",
+    default=get_config_option("default", "terminal_width", 1000),
+    help="Terminal width (default is 1000).",
+)
+@click.option(
     "--profile",
     "profile",
     type=click.Choice(list_config_sections()),
     default=get_config_option(
         "default",
         "profile",
     ),
     help="Activate profile, defined in .griffonrc.",
 )
 @click.option("--editor/--no-editor", default=True, help="Allow text editor prompt.")
 @click.pass_context
-def cli(ctx, debug, format, verbose, no_progress_bar, no_color, no_wrap, profile, editor):
+def cli(
+    ctx, debug, format, verbose, no_progress_bar, no_color, no_wrap, terminal_width, profile, editor
+):
     """Red Hat product security CLI"""
 
     if ctx.invoked_subcommand is None:
         click.echo(ctx.parent.get_help())
 
     if not debug:
         config_logging(level="INFO")
@@ -141,13 +149,16 @@
     ctx.obj["FORMAT"] = format
     ctx.obj["VERBOSE"] = verbose
     ctx.obj["NO_PROGRESS_BAR"] = no_progress_bar
     ctx.obj["NO_COLOR"] = no_color
     ctx.obj["NO_WRAP"] = get_config_option("default", "no_wrap", False)
     if no_wrap:
         ctx.obj["NO_WRAP"] = no_wrap
+    ctx.obj["TERMINAL_WIDTH"] = get_config_option("default", "width", 1000)
+    if terminal_width:
+        ctx.obj["TERMINAL_WIDTH"] = terminal_width
     ctx.obj["PROFILE"] = profile
     ctx.obj["SHORT_VERSION_VALUES"] = True
     ctx.obj["EDITOR"] = editor
 
 
 cli.help = "Red Hat Product Security CLI"
```

### Comparing `griffon-0.2.5/griffon/commands/configure.py` & `griffon-0.2.6/griffon/commands/configure.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/griffon/commands/docs.py` & `griffon-0.2.6/griffon/commands/docs.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/griffon/commands/entities/__init__.py` & `griffon-0.2.6/griffon/commands/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/griffon/commands/entities/community_component_registry.py` & `griffon-0.2.6/griffon/commands/entities/community_component_registry.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/griffon/commands/entities/corgi.py` & `griffon-0.2.6/griffon/commands/entities/corgi.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/griffon/commands/entities/helpers.py` & `griffon-0.2.6/griffon/commands/entities/helpers.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/griffon/commands/entities/osidb.py` & `griffon-0.2.6/griffon/commands/entities/osidb.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/griffon/commands/plugin_commands.py` & `griffon-0.2.6/griffon/commands/plugin_commands.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/griffon/commands/plugins/bugzilla.py` & `griffon-0.2.6/griffon/commands/plugins/bugzilla.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/griffon/commands/plugins/cve_mitre.py` & `griffon-0.2.6/griffon/commands/plugins/cve_mitre.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/griffon/commands/plugins/go_vuln.py` & `griffon-0.2.6/griffon/commands/plugins/go_vuln.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/griffon/commands/plugins/osv.py` & `griffon-0.2.6/griffon/commands/plugins/osv.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/griffon/commands/plugins/semgrep.py` & `griffon-0.2.6/griffon/commands/plugins/semgrep.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/griffon/commands/process.py` & `griffon-0.2.6/griffon/commands/process.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/griffon/commands/queries.py` & `griffon-0.2.6/griffon/commands/queries.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/griffon/commands/reports.py` & `griffon-0.2.6/griffon/commands/reports.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/griffon/output.py` & `griffon-0.2.6/griffon/output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1037,14 +1037,16 @@
     if ctx and ctx.obj["NO_COLOR"]:
         console.no_color = True
     format = OUTPUT_FORMAT.JSON
     if ctx and "FORMAT" in ctx.obj:
         format = OUTPUT_FORMAT(ctx.obj["FORMAT"])
     if format is OUTPUT_FORMAT.TEXT:
         no_wrap = ctx.obj["NO_WRAP"]
+        terminal_width = ctx.obj["TERMINAL_WIDTH"]
+        console.width = int(terminal_width)
         if ctx.info_name == "product-summary":
             text_output_product_summary(ctx, output, format, exclude_products, no_wrap=no_wrap)
         if ctx.info_name == "products-contain-component":
             text_output_products_contain_component(
                 ctx, output, exclude_products, exclude_components, no_wrap=no_wrap
             )
         if ctx.info_name == "components-contain-component":
```

### Comparing `griffon-0.2.5/griffon/services/__init__.py` & `griffon-0.2.6/griffon/services/__init__.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/griffon/services/core_process.py` & `griffon-0.2.6/griffon/services/core_process.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/griffon/services/core_queries.py` & `griffon-0.2.6/griffon/services/core_queries.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/griffon/services/core_reports.py` & `griffon-0.2.6/griffon/services/core_reports.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/griffon/static/default_griffonrc` & `griffon-0.2.6/griffon/static/default_griffonrc`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [default]
 format = text
 history_log = ~/.griffon/history.log
 profile = default
 verbosity = 0
-no_wrap = True
+no_wrap = False
+terminal_width = 1000
 sfm2_api_url = http://localhost:5600
 custom_plugin_dir = ~/.griffon/plugins/
 editor = vi
 exclude_components = -container-source
     -debuginfo
     -debugsource
     -static
```

### Comparing `griffon-0.2.5/griffon.egg-info/PKG-INFO` & `griffon-0.2.6/griffon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griffon
-Version: 0.2.5
+Version: 0.2.6
 Summary: Red Hat Product Security CLI
 Home-page: https://github.com/RedHatProductSecurity/griffon
 Author: James Fuller, Red Hat Product Security
 License: MIT
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `griffon-0.2.5/griffon.egg-info/SOURCES.txt` & `griffon-0.2.6/griffon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/pyproject.toml` & `griffon-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/setup.py` & `griffon-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/tests/test_cli.py` & `griffon-0.2.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/tests/test_entities.py` & `griffon-0.2.6/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/tests/test_manage.py` & `griffon-0.2.6/tests/test_manage.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/tests/test_plugins.py` & `griffon-0.2.6/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/tests/test_process.py` & `griffon-0.2.6/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/tests/test_queries.py` & `griffon-0.2.6/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/tests/test_reports.py` & `griffon-0.2.6/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.5/tests/test_unit.py` & `griffon-0.2.6/tests/test_unit.py`

 * *Files identical despite different names*

