# Comparing `tmp/milatools-0.0.8.tar.gz` & `tmp/milatools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "milatools-0.0.8.tar", max compression
+gzip compressed data, was "milatools-0.0.9.tar", max compression
```

## Comparing `milatools-0.0.8.tar` & `milatools-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3459 2022-08-09 19:23:11.175840 milatools-0.0.8/README.md
--rw-r--r--   0        0        0        0 2021-08-31 16:31:42.761447 milatools-0.0.8/milatools/__init__.py
--rw-r--r--   0        0        0        0 2022-08-09 19:23:11.176055 milatools-0.0.8/milatools/cli/__init__.py
--rw-r--r--   0        0        0    23019 2022-08-09 19:23:11.177267 milatools-0.0.8/milatools/cli/__main__.py
--rw-r--r--   0        0        0     8612 2022-08-09 19:23:11.177665 milatools-0.0.8/milatools/cli/profile.py
--rw-r--r--   0        0        0    12058 2022-08-09 19:23:11.178231 milatools-0.0.8/milatools/cli/utils.py
--rw-r--r--   0        0        0     4917 2022-01-19 23:00:25.874924 milatools-0.0.8/milatools/datalocate.py
--rwxr-xr-x   0        0        0      222 2022-06-02 23:00:29.428379 milatools-0.0.8/milatools/listenvs.sh
--rw-r--r--   0        0        0     2199 2022-05-27 21:35:45.895325 milatools-0.0.8/milatools/runners.py
--rwxr-xr-x   0        0        0      205 2022-06-02 22:54:30.054273 milatools-0.0.8/milatools/start-jupyter.sh
--rw-r--r--   0        0        0       18 2022-08-09 19:23:20.637077 milatools-0.0.8/milatools/version.py
--rw-r--r--   0        0        0      801 2022-08-09 19:23:20.612741 milatools-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4463 2022-08-09 19:23:41.144165 milatools-0.0.8/setup.py
--rw-r--r--   0        0        0     4315 2022-08-09 19:23:41.144522 milatools-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     3459 2022-08-09 19:23:11.175840 milatools-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2021-08-31 16:31:42.761447 milatools-0.0.9/milatools/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:23:11.176055 milatools-0.0.9/milatools/cli/__init__.py
+-rw-r--r--   0        0        0    23019 2022-08-09 19:23:11.177267 milatools-0.0.9/milatools/cli/__main__.py
+-rw-r--r--   0        0        0     8612 2022-08-09 19:23:11.177665 milatools-0.0.9/milatools/cli/profile.py
+-rw-r--r--   0        0        0    12388 2022-08-16 19:33:38.790650 milatools-0.0.9/milatools/cli/utils.py
+-rw-r--r--   0        0        0     4917 2022-01-19 23:00:25.874924 milatools-0.0.9/milatools/datalocate.py
+-rwxr-xr-x   0        0        0      222 2022-06-02 23:00:29.428379 milatools-0.0.9/milatools/listenvs.sh
+-rw-r--r--   0        0        0     2199 2022-05-27 21:35:45.895325 milatools-0.0.9/milatools/runners.py
+-rwxr-xr-x   0        0        0      205 2022-06-02 22:54:30.054273 milatools-0.0.9/milatools/start-jupyter.sh
+-rw-r--r--   0        0        0       18 2022-08-19 17:35:42.903000 milatools-0.0.9/milatools/version.py
+-rw-r--r--   0        0        0      801 2022-08-19 17:35:42.879343 milatools-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4463 2022-08-19 17:35:48.835170 milatools-0.0.9/setup.py
+-rw-r--r--   0        0        0     4315 2022-08-19 17:35:48.835535 milatools-0.0.9/PKG-INFO
```

### Comparing `milatools-0.0.8/README.md` & `milatools-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `milatools-0.0.8/milatools/cli/__main__.py` & `milatools-0.0.9/milatools/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `milatools-0.0.8/milatools/cli/profile.py` & `milatools-0.0.9/milatools/cli/profile.py`

 * *Files identical despite different names*

### Comparing `milatools-0.0.8/milatools/cli/utils.py` & `milatools-0.0.9/milatools/cli/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -379,15 +379,20 @@
 
     def ensure_allocation(self):
         remote = Remote(hostname="->", connection=self.connection).with_bash()
         proc, results = remote.extract(
             shjoin(["salloc", *self.alloc]),
             patterns={"node_name": "salloc: Nodes ([^ ]+) are ready for job"},
         )
-        return results["node_name"], proc
+        # The node name can look like 'cn-c001', or 'cn-c[001-003]', or
+        # 'cn-c[001,008]', or 'cn-c001,rtx8', etc. We will only connect to a
+        # single one, though, so we will simply pick the first one.
+        node_name = re.split(pattern="[,-]", string=results["node_name"])[0]
+        node_name = node_name.replace("[", "")
+        return node_name, proc
 
 
 class SSHConfig:
     """Wrapper around sshconf with some extra niceties."""
 
     def __init__(self, path):
         self.cfg = read_ssh_config(path)
```

### Comparing `milatools-0.0.8/milatools/datalocate.py` & `milatools-0.0.9/milatools/datalocate.py`

 * *Files identical despite different names*

### Comparing `milatools-0.0.8/milatools/runners.py` & `milatools-0.0.9/milatools/runners.py`

 * *Files identical despite different names*

### Comparing `milatools-0.0.8/pyproject.toml` & `milatools-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "milatools"
-version = "0.0.8"
+version = "0.0.9"
 description = "Tools to work with the Mila cluster"
 authors = ["Olivier Breuleux <breuleux@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/mila-iqia/milatools"
 repository = "https://github.com/mila-iqia/milatools"
 license = "MIT"
```

### Comparing `milatools-0.0.8/setup.py` & `milatools-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'sshconf>=0.2.2,<0.3.0']
 
 entry_points = \
 {'console_scripts': ['mila = milatools.cli.__main__:main']}
 
 setup_kwargs = {
     'name': 'milatools',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Tools to work with the Mila cluster',
     'long_description': "\n# milatools\n\nThe milatools package provides the `mila` command, which is meant to help with connecting to and interacting with the Mila cluster.\n\n\n## Install\n\nRequires Python >= 3.8\n\n```bash\npip install milatools\n```\n\nOr, for bleeding edge version:\n\n```bash\npip install git+https://github.com/mila-iqia/milatools.git\n```\n\nAfter installing `milatools`, start with `mila init`:\n\n```bash\nmila init\n```\n\n\n## Commands\n\n### mila init\n\nSet up your access to the mila cluster interactively. Have your username and password ready!\n\n* Set up your SSH config for easy connection with `ssh mila`\n* Set up your public key if you don't already have them\n* Copy your public key over to the cluster for passwordless auth\n* Set up a public key on the login node to enable ssh into compute nodes\n\n\n### mila docs/intranet\n\n* Use `mila docs <search terms>` to search the Mila technical documentation\n* Use `mila intranet <search terms>` to search the Mila intranet\n\nBoth commands open a browser window. If no search terms are given you are taken to the home page.\n\n\n### mila code\n\nConnect a VSCode instance to a compute node. `mila code` first allocates a compute node using slurm (you can pass slurm options as well using `--alloc`), and then calls the `code` command with the appropriate options to start a remote coding session on the allocated node.\n\nYou can simply Ctrl+C the process to end the session.\n\n```\nusage: mila code [-h] [--alloc ...] [--job VALUE] [--node VALUE] PATH\n\npositional arguments:\n  PATH          Path to open on the remote machine\n\noptional arguments:\n  -h, --help    show this help message and exit\n  --alloc ...   Extra options to pass to slurm\n  --job VALUE   Job ID to connect to\n  --node VALUE  Node to connect to\n```\n\nFor example:\n\n```bash\nmila code path/to/my/experiment\n```\n\nThe `--alloc` option may be used to pass extra arguments to `salloc` when allocating a node (for example, `--alloc --gres=cpu:8` to allocate 8 CPUs). `--alloc` should be at the end, because it will take all of the arguments that come after it.\n\nIf you already have an allocation on a compute node, you may use the `--node NODENAME` or `--job JOBID` options to connect to that node.\n\n\n### mila serve\n\nThe purpose of `mila serve` is to make it easier to start notebooks, logging servers, etc. on the compute nodes and connect to them.\n\n```\nusage: mila serve [-h] {connect,kill,list,lab,notebook,tensorboard,mlflow,aim} ...\n\npositional arguments:\n  {connect,kill,list,lab,notebook,tensorboard,mlflow,aim}\n    connect             Reconnect to a persistent server.\n    kill                Kill a persistent server.\n    list                List active servers.\n    lab                 Start a Jupyterlab server.\n    notebook            Start a Jupyter Notebook server.\n    tensorboard         Start a Tensorboard server.\n    mlflow              Start an MLFlow server.\n    aim                 Start an AIM server.\n\noptional arguments:\n  -h, --help            show this help message and exit\n```\n\nFor example, to start jupyterlab with one GPU, you may write:\n\n```bash\nmila serve lab --alloc --gres gpu:1\n```\n\nYou can of course write any SLURM arguments after `--alloc`.\n\nEnding the connection will end the server, but the `--persist` flag can be used to prevent that. In that case you would be able to write `mila serve connect jupyter-lab` in order to reconnect to your running instance. Use `mila serve list` and `mila serve kill` to view and manage any running instances.\n",
     'author': 'Olivier Breuleux',
     'author_email': 'breuleux@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/mila-iqia/milatools',
```

### Comparing `milatools-0.0.8/PKG-INFO` & `milatools-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milatools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools to work with the Mila cluster
 Home-page: https://github.com/mila-iqia/milatools
 License: MIT
 Author: Olivier Breuleux
 Author-email: breuleux@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

