# Comparing `tmp/pipen_args-0.9.8.tar.gz` & `tmp/pipen_args-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_args-0.9.8.tar", max compression
+gzip compressed data, was "pipen_args-0.9.9.tar", max compression
```

## Comparing `pipen_args-0.9.8.tar` & `pipen_args-0.9.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2560 2023-05-25 05:33:52.478197 pipen_args-0.9.8/README.md
--rw-r--r--   0        0        0      969 2023-05-25 05:33:52.478197 pipen_args-0.9.8/pipen_args/__init__.py
--rw-r--r--   0        0        0     3871 2023-05-25 05:33:52.478197 pipen_args-0.9.8/pipen_args/defaults.py
--rw-r--r--   0        0        0     9821 2023-05-25 05:33:52.482197 pipen_args-0.9.8/pipen_args/parser_.py
--rw-r--r--   0        0        0     8133 2023-05-25 05:33:52.482197 pipen_args-0.9.8/pipen_args/plugin.py
--rw-r--r--   0        0        0     3277 2023-05-25 05:33:52.482197 pipen_args-0.9.8/pipen_args/procgroup.py
--rw-r--r--   0        0        0       22 2023-05-25 05:33:52.482197 pipen_args-0.9.8/pipen_args/version.py
--rw-r--r--   0        0        0     1185 2023-05-25 05:33:52.482197 pipen_args-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     3410 1970-01-01 00:00:00.000000 pipen_args-0.9.8/setup.py
--rw-r--r--   0        0        0     3251 1970-01-01 00:00:00.000000 pipen_args-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     2560 2023-05-26 06:05:03.758537 pipen_args-0.9.9/README.md
+-rw-r--r--   0        0        0      969 2023-05-26 06:05:03.758537 pipen_args-0.9.9/pipen_args/__init__.py
+-rw-r--r--   0        0        0     3871 2023-05-26 06:05:03.758537 pipen_args-0.9.9/pipen_args/defaults.py
+-rw-r--r--   0        0        0     9821 2023-05-26 06:05:03.758537 pipen_args-0.9.9/pipen_args/parser_.py
+-rw-r--r--   0        0        0     8338 2023-05-26 06:05:03.758537 pipen_args-0.9.9/pipen_args/plugin.py
+-rw-r--r--   0        0        0     3277 2023-05-26 06:05:03.758537 pipen_args-0.9.9/pipen_args/procgroup.py
+-rw-r--r--   0        0        0       22 2023-05-26 06:05:03.758537 pipen_args-0.9.9/pipen_args/version.py
+-rw-r--r--   0        0        0     1185 2023-05-26 06:05:03.758537 pipen_args-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     3410 1970-01-01 00:00:00.000000 pipen_args-0.9.9/setup.py
+-rw-r--r--   0        0        0     3251 1970-01-01 00:00:00.000000 pipen_args-0.9.9/PKG-INFO
```

### Comparing `pipen_args-0.9.8/README.md` & `pipen_args-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pipen_args-0.9.8/pipen_args/__init__.py` & `pipen_args-0.9.9/pipen_args/__init__.py`

 * *Files identical despite different names*

### Comparing `pipen_args-0.9.8/pipen_args/defaults.py` & `pipen_args-0.9.9/pipen_args/defaults.py`

 * *Files identical despite different names*

### Comparing `pipen_args-0.9.8/pipen_args/parser_.py` & `pipen_args-0.9.9/pipen_args/parser_.py`

 * *Files identical despite different names*

### Comparing `pipen_args-0.9.8/pipen_args/plugin.py` & `pipen_args-0.9.9/pipen_args/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import sys
 from argparse import ArgumentError
 from typing import TYPE_CHECKING
 from pathlib import Path
 
 from argx import Namespace
 from simpleconf import ProfileConfig
 from pipen import plugin
@@ -27,14 +28,19 @@
     """Automatically parse arguments and load configs for pipen pipelines"""
     name = "args"
     version = __version__
 
     @plugin.impl
     async def on_init(pipen: Pipen) -> None:
         """Parse and update the config"""
+        if sys.argv[0].startswith("@pipen-"):  # pragma: no cover
+            # Allow not to parse args when we just want to load the pipeline
+            # by other plugins
+            return
+
         config = pipen._kwargs
         config["plugin_opts"]["args_hide"] = False
         parser = Parser()
         # Init the parser
         try:
             parser.init(pipen)
         except ArgumentError:
```

### Comparing `pipen_args-0.9.8/pipen_args/procgroup.py` & `pipen_args-0.9.9/pipen_args/procgroup.py`

 * *Files identical despite different names*

### Comparing `pipen_args-0.9.8/pyproject.toml` & `pipen_args-0.9.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipen-args"
-version = "0.9.8"
+version = "0.9.9"
 description = "Command-line argument parser for pipen."
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/pipen-args"
 repository = "https://github.com/pwwang/pipen-args"
```

### Comparing `pipen_args-0.9.8/setup.py` & `pipen_args-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['pipen-annotate>=0.7.1,<0.8.0']
 
 entry_points = \
 {'pipen': ['args = pipen_args.plugin:ArgsPlugin']}
 
 setup_kwargs = {
     'name': 'pipen-args',
-    'version': '0.9.8',
+    'version': '0.9.9',
     'description': 'Command-line argument parser for pipen.',
     'long_description': '# pipen-args\n\nCommand line argument parser for [pipen][1]\n\n## Usage\n\n```python\nfrom pipen import Proc, Pipen\n\n\nclass Process(Proc):\n    """My process\n\n    Input:\n        a: Input data\n    """\n    input = \'a\'\n    input_data = range(10)\n    script = \'echo {{in.a}}\'\n\nPipen().set_start(Process).run()\n```\n\n```shell\n$ python example.py --help\nUsage: test.py [-h | -h+] [options]\n\nUndescribed process.\nUse `@configfile` to load default values for the options.\n\nPipeline Options:\n  --name NAME           The name for the pipeline, will affect the default workdir and\n                        outdir. [default: pipen-0]\n  --profile PROFILE     The default profile from the configuration to run the pipeline.\n                        This profile will be used unless a profile is specified in the\n                        process or in the .run method of pipen. You can check the\n                        available profiles by running `pipen profile`\n  --outdir OUTDIR       The output directory of the pipeline [default: ./<name>-output]\n  --forks FORKS         How many jobs to run simultaneously by the scheduler\n  --scheduler SCHEDULER\n                        The scheduler to run the jobs\n\nNamespace <in>:\n  --in.a A [A ...]      Input data\n\nOptional Arguments:\n  -h, --help, -h+, --help+\n                        show help message (with + to show more options) and exit\n```\n\nSee more examples in `tests/pipelines/` folder.\n\n## Plugin options\n\n- `args_hide`: (process level) Hide the arguments in the help message. Default: `False`\n- `args_group`: (pipeline level) The group name for the arguments. Default: `pipeline options`\n- `args_flatten`: (pipeline level) Flatten the arguments in the help message when there is only one process in the pipeline. Default: `auto` (flatten if single process, otherwise not)\n\n\n## Metadata for Proc envs items\n\nThe metadata in the docstring of env items determines how the arguments are defined.\n\n```python\nclass Process(Proc):\n    """My process\n\n    # other docstring sections\n\n    Envs:\n        a (<metadata>): ...\n    """\n```\n\nThe metadata could be key-value pairs separated by `;`. The separator `:` or `=` is used to\nseparate the key and value. The value is optional. If the value is not specified, it\nwill be set to `True`. The keys are valid arguments of `argx.ArgumentParser.add_argument`, except that `hidden` will be interpreted as `show=False` in `argx.ArgumentParser.add_argument`. If the value of `choices` is not specified, the subkeys of the env item will be used as the choices.\n\n[1]: https://github.com/pwwang/pipen\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/pipen-args',
```

### Comparing `pipen_args-0.9.8/PKG-INFO` & `pipen_args-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipen-args
-Version: 0.9.8
+Version: 0.9.9
 Summary: Command-line argument parser for pipen.
 Home-page: https://github.com/pwwang/pipen-args
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

