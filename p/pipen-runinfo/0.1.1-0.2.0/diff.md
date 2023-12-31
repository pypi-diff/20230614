# Comparing `tmp/pipen_runinfo-0.1.1.tar.gz` & `tmp/pipen_runinfo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_runinfo-0.1.1.tar", max compression
+gzip compressed data, was "pipen_runinfo-0.2.0.tar", max compression
```

## Comparing `pipen_runinfo-0.1.1.tar` & `pipen_runinfo-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2755 2023-06-10 21:59:57.160728 pipen_runinfo-0.1.1/README.md
--rw-r--r--   0        0        0     6622 2023-06-10 21:59:57.160728 pipen_runinfo-0.1.1/pipen_runinfo.py
--rw-r--r--   0        0        0     1057 2023-06-10 21:59:57.160728 pipen_runinfo-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3536 1970-01-01 00:00:00.000000 pipen_runinfo-0.1.1/setup.py
--rw-r--r--   0        0        0     3349 1970-01-01 00:00:00.000000 pipen_runinfo-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2713 2023-06-14 17:21:55.036975 pipen_runinfo-0.2.0/README.md
+-rw-r--r--   0        0        0     7139 2023-06-14 17:21:55.036975 pipen_runinfo-0.2.0/pipen_runinfo.py
+-rw-r--r--   0        0        0     1057 2023-06-14 17:21:55.036975 pipen_runinfo-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 pipen_runinfo-0.2.0/setup.py
+-rw-r--r--   0        0        0     3307 1970-01-01 00:00:00.000000 pipen_runinfo-0.2.0/PKG-INFO
```

### Comparing `pipen_runinfo-0.1.1/README.md` & `pipen_runinfo-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -76,12 +76,11 @@
 
 ### `job.runinfo.time`
 
 The time spent on the job, and more, generated by `time -v` command.
 
 ### `job.runinfo.device`
 
-The device information of the job, generated by `lshw` command.
-Note that only processor, memory, display and storage are included.
+The device (cpu and memory) information of the job, generated by `lscpu`/`lsmem` command.
 
 
 [1]: https://github.com/pwwang/pipen
```

### Comparing `pipen_runinfo-0.1.1/pipen_runinfo.py` & `pipen_runinfo-0.2.0/pipen_runinfo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,49 @@
 from __future__ import annotations
 
+import textwrap
 from typing import TYPE_CHECKING, List
 from pathlib import Path
 
 from pipen import plugin
 from pipen.job import Job
 
 if TYPE_CHECKING:
     from pipen import Proc, Pipen
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 
 # Monkey-path Job.CMD_WRAPPER_TEMPLATE to time the script
 Job.CMD_WRAPPER_TEMPLATE = Job.CMD_WRAPPER_TEMPLATE.replace(
     "{job.strcmd}",
-    "/usr/bin/time -o {job.metadir}/job.runinfo.time -v {job.strcmd}",
+    textwrap.dedent(
+        """
+        # Check if GNU time is available
+        if env time -V &>/dev/null; then
+            jobcmd="env time -o {job.metadir}/job.runinfo.time -v {job.strcmd}"
+        else
+            echo "GNU time is not available, job is not timed." > {job.metadir}/job.runinfo.time
+            jobcmd="{job.strcmd}"
+        fi
+
+        eval $jobcmd"""  # noqa: E501
+    ),
 ).replace(
     "{postscript}",
-    "{postscript}\n\n"
-    "lshw -quiet -notime -sanitize -short -class processor -class memory "
-    "-class display -class storage 2>/dev/null "
-    "> {job.metadir}/job.runinfo.device"
+    textwrap.dedent(
+        """
+        {postscript}
+
+        echo "# CPU" > {job.metadir}/job.runinfo.device
+        lscpu >> {job.metadir}/job.runinfo.device
+        echo "" >> {job.metadir}/job.runinfo.device
+        echo "# Memory" >> {job.metadir}/job.runinfo.device
+        lsmem --summary=only >> {job.metadir}/job.runinfo.device
+        """
+    ),
 )
 
 
 SESSION_INFO_PYTHON = r"""
 def _session_info(show_path: bool, include_submodule: bool):
     try:
         from importlib import metadata as importlib_metadata
@@ -38,15 +57,15 @@
     if show_path:
         lines.append("Name\t__version__\timportlib.metadata\tPath\n")
         lines.append(f"python\t{sys.version}\t-\t{sys.executable}\n")
     else:
         lines.append("Name\t__version__\timportlib.metadata\n")
         lines.append(f"python\t{sys.version}\t-\n")
 
-    for name, module in sys.modules.items():
+    for name, module in sys.modules.copy().items():
         if not include_submodule and "." in name:
             continue
 
         ver = getattr(
             module,
             "__version__",
             getattr(module, "version", "-"),
```

### Comparing `pipen_runinfo-0.1.1/pyproject.toml` & `pipen_runinfo-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipen-runinfo"
-version = "0.1.1"
+version = "0.2.0"
 description = "Generate running information for jobs in pipen pipelines"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `pipen_runinfo-0.1.1/setup.py` & `pipen_runinfo-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 ['pipen>=0.10.1,<0.11.0']
 
 entry_points = \
 {'pipen': ['runinfo = pipen_runinfo:PipenRuninfoPlugin']}
 
 setup_kwargs = {
     'name': 'pipen-runinfo',
-    'version': '0.1.1',
+    'version': '0.2.0',
     'description': 'Generate running information for jobs in pipen pipelines',
-    'long_description': '# pipen-runinfo\n\nGenerate running information for jobs in [pipen][1] pipelines.\n\nIncluding session info (packages and versions), time, and device info.\n\n## Install\n\n```bash\npip install -U pipen-runinfo\n```\n\n## Enable/Disable the plugin\n\nThe plugin is registered via entrypoints. It\'s by default enabled. To disable it: plugins=[..., "no:runinfo"], or uninstall this plugin.\n\n## Plugin options\n\n- `runinfo_lang`: The name of the language to run the job script for session info.\n    Default is `None`, which means it will be inferred from the `proc.lang`\n    This should be a process-level option, unless you only have one single\n    process in your pipeline.\n- `runinfo_path`: Whether to include paths for the modules in the session information.\n    Default is `True`.\n    This option could be either specified in the process-level or the pipeline-level.\n    Only works for `python`.\n- `runinfo_submod`: Whether to include submodules in the session information.\n    Default is `False`.\n    This option could be either specified in the process-level or the pipeline-level.\n    Only works for `python`.\n\n## Supported languages for session info\n\n`python`, `R`, `bash`, and `fish`.\n\n## Usage\n\nThe plugin will generate 3 files in the job directory of the pipeline.\n\n### `job.runinfo.session`\n\nThe session information of the job, including the interpreter, packages and their versions.\n\n#### Python\n\nGenerates a TSV file with the following columns:\n\n- `Name`: The name of the module, or python itself\n- `__version__`: The version fetched by `module.__version__` or `module.version`\n- `importlib.metadata`: The version fetched by `importlib.metadata.version(package)`\n- `Path`: The path of the module (only if `runinfo_path` is `True`)\n\n#### R\n\nGenerates a text file `sessionInfo()` output.\n\n#### Bash\n\nGenerates a TSV file with the following columns:\n\n- `SHELL`: The value of `$SHELL`\n- `BASH_VERSION`: The value of `$BASH_VERSION`\n- `BASH_ARGV0`: The value of `$BASH_ARGV0`\n- `BASH_SOURCE`: The value of `$BASH_SOURCE`\n- `proc-exe`: The real path of the executable from `/proc/<pid>/exe`\n- `proc-exe-version`: The version of the executable from `/proc/<pid>/exe --version`\n\n#### Fish\n\nGenerates a TSV file with the following columns:\n\n- `SHELL`: The value of `$SHELL`\n- `FISH_VERSION`: The value of `$FISH_VERSION`\n- `proc-exe`: The real path of the executable from `/proc/<pid>/exe`\n- `proc-exe-version`: The version of the executable from `/proc/<pid>/exe --version`\n\n### `job.runinfo.time`\n\nThe time spent on the job, and more, generated by `time -v` command.\n\n### `job.runinfo.device`\n\nThe device information of the job, generated by `lshw` command.\nNote that only processor, memory, display and storage are included.\n\n\n[1]: https://github.com/pwwang/pipen\n',
+    'long_description': '# pipen-runinfo\n\nGenerate running information for jobs in [pipen][1] pipelines.\n\nIncluding session info (packages and versions), time, and device info.\n\n## Install\n\n```bash\npip install -U pipen-runinfo\n```\n\n## Enable/Disable the plugin\n\nThe plugin is registered via entrypoints. It\'s by default enabled. To disable it: plugins=[..., "no:runinfo"], or uninstall this plugin.\n\n## Plugin options\n\n- `runinfo_lang`: The name of the language to run the job script for session info.\n    Default is `None`, which means it will be inferred from the `proc.lang`\n    This should be a process-level option, unless you only have one single\n    process in your pipeline.\n- `runinfo_path`: Whether to include paths for the modules in the session information.\n    Default is `True`.\n    This option could be either specified in the process-level or the pipeline-level.\n    Only works for `python`.\n- `runinfo_submod`: Whether to include submodules in the session information.\n    Default is `False`.\n    This option could be either specified in the process-level or the pipeline-level.\n    Only works for `python`.\n\n## Supported languages for session info\n\n`python`, `R`, `bash`, and `fish`.\n\n## Usage\n\nThe plugin will generate 3 files in the job directory of the pipeline.\n\n### `job.runinfo.session`\n\nThe session information of the job, including the interpreter, packages and their versions.\n\n#### Python\n\nGenerates a TSV file with the following columns:\n\n- `Name`: The name of the module, or python itself\n- `__version__`: The version fetched by `module.__version__` or `module.version`\n- `importlib.metadata`: The version fetched by `importlib.metadata.version(package)`\n- `Path`: The path of the module (only if `runinfo_path` is `True`)\n\n#### R\n\nGenerates a text file `sessionInfo()` output.\n\n#### Bash\n\nGenerates a TSV file with the following columns:\n\n- `SHELL`: The value of `$SHELL`\n- `BASH_VERSION`: The value of `$BASH_VERSION`\n- `BASH_ARGV0`: The value of `$BASH_ARGV0`\n- `BASH_SOURCE`: The value of `$BASH_SOURCE`\n- `proc-exe`: The real path of the executable from `/proc/<pid>/exe`\n- `proc-exe-version`: The version of the executable from `/proc/<pid>/exe --version`\n\n#### Fish\n\nGenerates a TSV file with the following columns:\n\n- `SHELL`: The value of `$SHELL`\n- `FISH_VERSION`: The value of `$FISH_VERSION`\n- `proc-exe`: The real path of the executable from `/proc/<pid>/exe`\n- `proc-exe-version`: The version of the executable from `/proc/<pid>/exe --version`\n\n### `job.runinfo.time`\n\nThe time spent on the job, and more, generated by `time -v` command.\n\n### `job.runinfo.device`\n\nThe device (cpu and memory) information of the job, generated by `lscpu`/`lsmem` command.\n\n\n[1]: https://github.com/pwwang/pipen\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'py_modules': modules,
     'install_requires': install_requires,
```

### Comparing `pipen_runinfo-0.1.1/PKG-INFO` & `pipen_runinfo-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipen-runinfo
-Version: 0.1.1
+Version: 0.2.0
 Summary: Generate running information for jobs in pipen pipelines
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -93,13 +93,12 @@
 
 ### `job.runinfo.time`
 
 The time spent on the job, and more, generated by `time -v` command.
 
 ### `job.runinfo.device`
 
-The device information of the job, generated by `lshw` command.
-Note that only processor, memory, display and storage are included.
+The device (cpu and memory) information of the job, generated by `lscpu`/`lsmem` command.
 
 
 [1]: https://github.com/pwwang/pipen
```

