# Comparing `tmp/eons-2.5.8.tar.gz` & `tmp/eons-2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eons-2.5.8.tar", last modified: Thu May 18 21:54:04 2023, max compression
+gzip compressed data, was "eons-2.5.9.tar", last modified: Sun May 21 03:57:14 2023, max compression
```

## Comparing `eons-2.5.8.tar` & `eons-2.5.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:54:04.988934 eons-2.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-05-18 21:54:04.988934 eons-2.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19582 2023-05-18 21:53:48.000000 eons-2.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:54:04.984934 eons-2.5.8/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:54:04.984934 eons-2.5.8/pkg/eons/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-18 21:53:56.000000 eons-2.5.8/pkg/eons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    87237 2023-05-18 21:53:56.000000 eons-2.5.8/pkg/eons/eons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:54:04.984934 eons-2.5.8/pkg/eons/method/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-18 21:53:41.000000 eons-2.5.8/pkg/eons/method/External.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:53:56.000000 eons-2.5.8/pkg/eons/method/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:54:04.988934 eons-2.5.8/pkg/eons/resolve/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:53:56.000000 eons-2.5.8/pkg/eons/resolve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-18 21:53:41.000000 eons-2.5.8/pkg/eons/resolve/resolve_find_by_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-18 21:53:41.000000 eons-2.5.8/pkg/eons/resolve/resolve_import_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-18 21:53:41.000000 eons-2.5.8/pkg/eons/resolve/resolve_install_from_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-18 21:53:41.000000 eons-2.5.8/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-18 21:53:41.000000 eons-2.5.8/pkg/eons/resolve/resolve_install_with_pip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:54:04.984934 eons-2.5.8/pkg/eons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-05-18 21:54:04.000000 eons-2.5.8/pkg/eons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-18 21:54:04.000000 eons-2.5.8/pkg/eons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:54:04.000000 eons-2.5.8/pkg/eons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-18 21:54:04.000000 eons-2.5.8/pkg/eons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-18 21:54:04.000000 eons-2.5.8/pkg/eons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-18 21:53:56.000000 eons-2.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-18 21:54:04.988934 eons-2.5.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:57:14.158999 eons-2.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    22214 2023-05-21 03:57:14.158999 eons-2.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22007 2023-05-21 03:56:58.000000 eons-2.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:57:14.154999 eons-2.5.9/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:57:14.154999 eons-2.5.9/pkg/eons/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-21 03:57:06.000000 eons-2.5.9/pkg/eons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88370 2023-05-21 03:57:06.000000 eons-2.5.9/pkg/eons/eons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:57:14.154999 eons-2.5.9/pkg/eons/method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-21 03:56:52.000000 eons-2.5.9/pkg/eons/method/External.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 03:57:06.000000 eons-2.5.9/pkg/eons/method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:57:14.158999 eons-2.5.9/pkg/eons/resolve/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 03:57:06.000000 eons-2.5.9/pkg/eons/resolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-21 03:56:52.000000 eons-2.5.9/pkg/eons/resolve/resolve_find_by_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-21 03:56:52.000000 eons-2.5.9/pkg/eons/resolve/resolve_import_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-21 03:56:52.000000 eons-2.5.9/pkg/eons/resolve/resolve_install_from_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-21 03:56:52.000000 eons-2.5.9/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-21 03:56:52.000000 eons-2.5.9/pkg/eons/resolve/resolve_install_with_pip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:57:14.154999 eons-2.5.9/pkg/eons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22214 2023-05-21 03:57:14.000000 eons-2.5.9/pkg/eons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-21 03:57:14.000000 eons-2.5.9/pkg/eons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 03:57:14.000000 eons-2.5.9/pkg/eons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-21 03:57:14.000000 eons-2.5.9/pkg/eons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-21 03:57:14.000000 eons-2.5.9/pkg/eons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-21 03:57:06.000000 eons-2.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-21 03:57:14.158999 eons-2.5.9/setup.cfg
```

### Comparing `eons-2.5.8/PKG-INFO` & `eons-2.5.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.5.8
+Version: 2.5.9
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -35,18 +35,22 @@
 
 For example implementations, check out:
  * [apie](https://github.com/eons-dev/bin_apie)
  * [ebbs](https://github.com/eons-dev/bin_ebbs)
  * [emi](https://github.com/eons-dev/bin_emi)
 
 Arguments available to all Eons Executors:
-* `-v` or `--verbose` (count, i.e `-vv` = 2) or `--verbosity #`, where # is some number, or the `verbosity` environment or config value: will show more information and increase the logging level, e.g. print debug messages (3 for debug; 2 for info).
+* `-v` or `--verbose` (count, i.e `-vv` = 2) or `--verbosity #`, where # is some number, or the `verbosity` environment or config value: will show more information and increase the logging level, e.g. print debug messages; see [log-levels](#log-levels), below for more info.
 * `--config` or `-c` (string): the path to a json config file from which other values may be retrieved.
 * `--no-repo` or the `no_repo` environment or config value (bool, i.e. 'True', 'true', etc.): whether or not to enable reaching out to online servers for code (see Dynamic Functionality, below).
 * `--log-file` or the `log_file` environment or config value (string; supports formatting, e.g. '/var/log/eons/{this.name}.log'): optional value for logging to a file in addition to stderr.
+* `--log-indentation` (bool): whether or not tab out logs; see [indentation](#indentation), below.
+* `--log-tab-width` (int): how many spaces to use for indentation; see [indentation](#indentation), below.
+* `--log-aggregate` (bool): whether or not to send logs to a remote aggregation service; see [aggregation](#aggregation), below.
+* `--log-aggregate-url` (string): the url of the remote aggregation service; see [aggregation](#aggregation), below.
 
 ## Features
 
 Eons supports 5 major features:
 * Get inputs to functors by drilling down through multiple layers.
 * Allow functors to change behavior with their order of execution.
 * Provide functionality by downloading functors on the fly.
@@ -161,14 +165,47 @@
 | :---              | :---         |    :----:   |  :---:  |            :---:              |     :---:    |
 | Classic           |is a|:heavy_check_mark:|:x:|:heavy_check_mark:|:heavy_check_mark:|
 | Implicit          |how does|:x:|:heavy_check_mark:|:heavy_check_mark:|:x:|
 | External          |has a|:heavy_check_mark:|:x:|:x:|:x:|
 
 You are not restricted to a single kind of inheritance. You can, and are encouraged, to use all forms of inheritance in your code!
 
+## Logging
+
+Eons attempts to provide a detailed, robust, and pleasant logging experience. We use the [logging](https://docs.python.org/3/library/logging.html) module, and shim in additional features through our log formatter.
+
+### Log Levels
+
+The log level may be set by the `verbosity` or `-v` flags.
+Children and other modules of Eons may employ their own logging levels. However, Eons provides the following levels by default:
+0. `CRITICAL`: only get notified if absolutely necessary.
+1. `WARNING`: get notified about potential problems.
+2. `INFO`: see what's generally going on.
+3. `DEBUG` + urllib3 WARNING: see what's really going on.
+4. Empty: reserved for modules.
+5. `DEBUG`: see everything.
+
+### Log Features
+
+#### Indentation
+
+To make logs easier to read, each Functor can be optionally tabbed out as it might be in source code, allowing you to readily see the scope where a log occurs. Each indentation begins with a `|` character and is followed by a number of spaces equal to the tab width minus one. For example, using a tab width of 2, a log line at the top level would be `| ...`, while a log at the second level would be `| | ...`.
+
+This feature is enabled by default. To disable it you can set `log_indentation` to `False`.
+
+To configure the size of the indentation, you can set `log_tab_width` to the number of spaces you want to use. For example a tab width of 1 would be just `|`, while a tab width of 4 would be `|   `.
+
+#### Aggregation
+
+For security information and event management (SIEM), Eons supports sending logs to a remote endpoint.
+
+This will only be done if a valid repo username and password are provided. If you provide a username and password, but don't want to send your logs to a remote server, you can set `log_aggregate` to `False`. 
+
+You may also set the `log_aggregate_url` to wherever you'd like to send your logs. By default, this is set to `https://eons.sh/log`.
+
 ## Performance
 
 At Eons LLC, we always prefer functionality over performance. This is the same as the whole "don't prematurely optimize" argument. With that said, optimizing is always good and we try to do it as much as possible.
 
 Please let us know if you are hitting any bottlenecks in this or any of our other libraries! 
 
 ## Design
```

### Comparing `eons-2.5.8/README.md` & `eons-2.5.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -20,18 +20,22 @@
 
 For example implementations, check out:
  * [apie](https://github.com/eons-dev/bin_apie)
  * [ebbs](https://github.com/eons-dev/bin_ebbs)
  * [emi](https://github.com/eons-dev/bin_emi)
 
 Arguments available to all Eons Executors:
-* `-v` or `--verbose` (count, i.e `-vv` = 2) or `--verbosity #`, where # is some number, or the `verbosity` environment or config value: will show more information and increase the logging level, e.g. print debug messages (3 for debug; 2 for info).
+* `-v` or `--verbose` (count, i.e `-vv` = 2) or `--verbosity #`, where # is some number, or the `verbosity` environment or config value: will show more information and increase the logging level, e.g. print debug messages; see [log-levels](#log-levels), below for more info.
 * `--config` or `-c` (string): the path to a json config file from which other values may be retrieved.
 * `--no-repo` or the `no_repo` environment or config value (bool, i.e. 'True', 'true', etc.): whether or not to enable reaching out to online servers for code (see Dynamic Functionality, below).
 * `--log-file` or the `log_file` environment or config value (string; supports formatting, e.g. '/var/log/eons/{this.name}.log'): optional value for logging to a file in addition to stderr.
+* `--log-indentation` (bool): whether or not tab out logs; see [indentation](#indentation), below.
+* `--log-tab-width` (int): how many spaces to use for indentation; see [indentation](#indentation), below.
+* `--log-aggregate` (bool): whether or not to send logs to a remote aggregation service; see [aggregation](#aggregation), below.
+* `--log-aggregate-url` (string): the url of the remote aggregation service; see [aggregation](#aggregation), below.
 
 ## Features
 
 Eons supports 5 major features:
 * Get inputs to functors by drilling down through multiple layers.
 * Allow functors to change behavior with their order of execution.
 * Provide functionality by downloading functors on the fly.
@@ -146,14 +150,47 @@
 | :---              | :---         |    :----:   |  :---:  |            :---:              |     :---:    |
 | Classic           |is a|:heavy_check_mark:|:x:|:heavy_check_mark:|:heavy_check_mark:|
 | Implicit          |how does|:x:|:heavy_check_mark:|:heavy_check_mark:|:x:|
 | External          |has a|:heavy_check_mark:|:x:|:x:|:x:|
 
 You are not restricted to a single kind of inheritance. You can, and are encouraged, to use all forms of inheritance in your code!
 
+## Logging
+
+Eons attempts to provide a detailed, robust, and pleasant logging experience. We use the [logging](https://docs.python.org/3/library/logging.html) module, and shim in additional features through our log formatter.
+
+### Log Levels
+
+The log level may be set by the `verbosity` or `-v` flags.
+Children and other modules of Eons may employ their own logging levels. However, Eons provides the following levels by default:
+0. `CRITICAL`: only get notified if absolutely necessary.
+1. `WARNING`: get notified about potential problems.
+2. `INFO`: see what's generally going on.
+3. `DEBUG` + urllib3 WARNING: see what's really going on.
+4. Empty: reserved for modules.
+5. `DEBUG`: see everything.
+
+### Log Features
+
+#### Indentation
+
+To make logs easier to read, each Functor can be optionally tabbed out as it might be in source code, allowing you to readily see the scope where a log occurs. Each indentation begins with a `|` character and is followed by a number of spaces equal to the tab width minus one. For example, using a tab width of 2, a log line at the top level would be `| ...`, while a log at the second level would be `| | ...`.
+
+This feature is enabled by default. To disable it you can set `log_indentation` to `False`.
+
+To configure the size of the indentation, you can set `log_tab_width` to the number of spaces you want to use. For example a tab width of 1 would be just `|`, while a tab width of 4 would be `|   `.
+
+#### Aggregation
+
+For security information and event management (SIEM), Eons supports sending logs to a remote endpoint.
+
+This will only be done if a valid repo username and password are provided. If you provide a username and password, but don't want to send your logs to a remote server, you can set `log_aggregate` to `False`. 
+
+You may also set the `log_aggregate_url` to wherever you'd like to send your logs. By default, this is set to `https://eons.sh/log`.
+
 ## Performance
 
 At Eons LLC, we always prefer functionality over performance. This is the same as the whole "don't prematurely optimize" argument. With that said, optimizing is always good and we try to do it as much as possible.
 
 Please let us know if you are hitting any bottlenecks in this or any of our other libraries! 
 
 ## Design
```

### Comparing `eons-2.5.8/pkg/eons/eons.py` & `eons-2.5.9/pkg/eons/eons.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 import importlib.util
 import types
 import builtins
 import argparse
 import requests
 import jsonpickle
 import yaml
+from requests_futures.sessions import FuturesSession
 from pathlib import Path
 from tqdm import tqdm
 from zipfile import ZipFile
 from distutils.dir_util import mkpath
+from eot import EOT
 import operator
 import traceback
 from copy import deepcopy
 import shutil
 from subprocess import Popen
 from subprocess import PIPE
 from subprocess import STDOUT
@@ -1347,14 +1349,19 @@
 class Executor(DataContainer, Functor):
 
 	def __init__(this, name=INVALID_NAME(), descriptionStr="Eons python framework. Extend as thou wilt."):
 		this.SetupLogging()
 
 		super().__init__(name)
 
+		this.optionalKWArgs['log_indentation'] = True
+		this.optionalKWArgs['log_tab_width'] = 2
+		this.optionalKWArgs['log_aggregate'] = True
+		this.optionalKWArgs['log_aggregate_url'] = "https://eons.sh/log"
+
 		this.resolveErrors = True
 		this.errorRecursionDepth = 0
 		this.errorResolutionStack = {}
 		this.resolveErrorsWith = [ # order matters: FIFO (first is first).
 			'find_by_fetch',
 			'install_from_repo_with_default_package_type',
 			'install_from_repo',
@@ -1414,14 +1421,17 @@
 		this.configFileExtensions = [
 			"json",
 			"yaml",
 			"yml",
 			"py",
 		]
 
+		# We can't Fetch from everywhere while we're getting things going. However, these should be safe,
+		this.fetchFromDuringSetup = ['args', 'config', 'environment']
+
 		this.Configure()
 		this.RegisterIncludedClasses()
 		this.AddArgs()
 
 
 	# Destructors do not work reliably in python.
 	# NOTE: you CANNOT delete *this without first Pop()ing it from the ExecutorTracker.
@@ -1454,14 +1464,15 @@
 		this.fetchFrom.remove('executor') # No no no no!
 		this.fetchFrom.remove('precursor') # Not applicable here.
 
 		# Usually, Executors shunt work off to other Functors, so we leave these True unless a child needs to check its work.
 		this.functionSucceeded = True
 		this.rollbackSucceeded = True
 
+		this.asyncSession = FuturesSession()
 
 	# Add a place to search for SelfRegistering classes.
 	# These should all be relative to the invoking working directory (i.e. whatever './' is at time of calling Executor())
 	def RegisterDirectory(this, directory):
 		this.registerDirectories.append(os.path.abspath(os.path.join(this.cwd,directory)))
 
 
@@ -1491,22 +1502,52 @@
 				logging.ERROR: preFormat + levelName + indentation + util.console.GetColorCode('red', 'dark') + message + postFormat,
 				logging.RECOVERY: preFormat + levelName + indentation + util.console.GetColorCode('green', 'light') + message + postFormat,
 				logging.CRITICAL: preFormat + levelName + indentation + util.console.GetColorCode('red', 'light', styles=['bold']) + message + postFormat
 			}
 
 			def format(this, record):
 				log_fmt = this.formats.get(record.levelno)
-				if (hasattr(logging.getLogger(), 'tab_logs') and getattr(logging.getLogger(), 'tab_logs')):
-					tabWidth = 4
-					if (hasattr(logging.getLogger(), 'tab_width')):
-						tabWidth = getattr(logging.getLogger(), 'tab_width')
-					tabWidth = int(tabWidth) - 1
-					log_fmt = log_fmt.replace('__INDENTATION__', f"|{' ' * tabWidth}" * (FunctorTracker.GetCount() - 1)) # -1 because we're already in a Functor.
+
+				executor = None
+				if (hasattr(logging.getLogger(), 'setupBy')):
+					executor = getattr(logging.getLogger(), 'setupBy')
+
+					# The executor won't have populated its optionalKWArgs until after this method is effected.
+					# So we wait until the last optional arg is set to start using the executor.
+					if (not hasattr(executor, 'log_aggregate_url')):
+						executor = None
+				
+				# Add indentation.
+				if (executor
+					and executor.log_indentation
+					and executor.log_tab_width
+					):
+					log_fmt = log_fmt.replace('__INDENTATION__', f"|{' ' * (executor.log_tab_width - 1)}" * (FunctorTracker.GetCount() - 1)) # -1 because we're already in a Functor.
 				else:
 					log_fmt = log_fmt.replace('__INDENTATION__', ' ')
+
+				# Aggregate logs remotely.
+				if (executor
+					and executor.log_aggregate 
+					and executor.repo.username is not None 
+					and executor.repo.password is not None
+					and record.module != 'connectionpool' # Prevent recursion.
+					):
+					aggregateEndpoint = executor.log_aggregate_url
+					log = {
+						'level': record.levelname,
+						'message': record.getMessage(), # TODO: Sanitize to prevent 400 errors.
+						'source': executor.name,
+						'timestamp': EOT.GetStardate()
+					}
+					try:
+						executor.asyncSession.put(aggregateEndpoint, json=log, auth=(executor.repo.username, executor.repo.password))
+					except Exception as e:
+						pass
+
 				formatter = logging.Formatter(log_fmt, datefmt = '%H:%M:%S')
 				return formatter.format(record)
 
 		# Skip setting up logging if it's already been done.
 		if (hasattr(logging.getLogger(), 'setupBy')):
 			return
 
@@ -1523,21 +1564,20 @@
 		if (not hasattr(logging.getLogger(), 'setupBy')):
 			return
 		if (not logging.getLogger().setupBy == this):
 			return
 		delattr(logging.getLogger(), 'setupBy')
 
 
-
 	# Logging to stderr is easy, since it will always happen.
 	# However, we also want the user to be able to log to a file, possibly set in the config.json, which requires a Fetch().
 	# Thus, setting up the log file handler has to occur later than the initial SetupLogging call.
 	# Calling this multiple times will add multiple log handlers.
 	def SetLogFile(this):
-		this.Set('log_file', this.Fetch('log_file', None, ['args', 'config', 'environment']))
+		this.Set('log_file', this.Fetch('log_file', None, this.fetchFromDuringSetup))
 		if (this.log_file is None):
 			return
 
 		log_filePath = Path(this.log_file).resolve()
 		if (not log_filePath.exists()):
 			log_filePath.parent.mkdir(parents=True, exist_ok=True)
 			log_filePath.touch()
@@ -1647,44 +1687,37 @@
 		for key, default in details.items():
 			this.repo[key] = this.Fetch(f"repo_{key}", default=default)
 
 
 	# How do we get the verbosity level and what do we do with it?
 	# This method should set log levels, etc.
 	def SetVerbosity(this, fetch=True):
-
-		fetchFrom = ['args', 'config', 'environment']
-
 		if (fetch):
 			# Take the highest of -v vs --verbosity
-			verbosity = this.EvaluateToType(this.Fetch('verbosity', 0, fetchFrom))
+			verbosity = this.EvaluateToType(this.Fetch('verbosity', 0, this.fetchFromDuringSetup))
 			if (verbosity > this.verbosity):
 				logging.debug(f"Setting verbosity to {verbosity}") # debug statements will be available when using external systems, like pytest.
 				this.verbosity = verbosity
 
 		if (this.verbosity == 0):
 			logging.getLogger().handlers[0].setLevel(logging.CRITICAL)
 			logging.getLogger().setLevel(logging.CRITICAL)
 		if (this.verbosity == 1):
 			logging.getLogger().handlers[0].setLevel(logging.WARNING)
 			logging.getLogger().setLevel(logging.WARNING)
 		elif (this.verbosity == 2):
 			logging.getLogger().handlers[0].setLevel(logging.INFO)
 			logging.getLogger().setLevel(logging.INFO)
-		elif(this.verbosity >= 3):
+		elif (this.verbosity >= 3):
 			logging.getLogger().handlers[0].setLevel(logging.DEBUG)
 			logging.getLogger().setLevel(logging.DEBUG)
-
-		if (fetch):
-			tabLogs, foundTabLogs = this.Fetch('tab_logs', False, fetchFrom, start=False)
-			tabLogs = this.EvaluateToType(tabLogs)
-			if (tabLogs or (this.verbosity >= 3 and not foundTabLogs)):
-				setattr(logging.getLogger(), 'tab_logs', True)
-				tabWidth = this.Fetch('logging_tab_width', 2, fetchFrom)
-				setattr(logging.getLogger(), 'tab_width', int(tabWidth))
+			logging.getLogger('urllib3').setLevel(logging.WARNING)
+		
+		if (this.verbosity >= 5):
+			logging.getLogger('urllib3').setLevel(logging.DEBUG)
 
 
 	# Do the argparse thing.
 	# Extra arguments are converted from --this-format to this_format, without preceding dashes. For example, --repo-url ... becomes repo_url ...
 	# NOTE: YOU CANNOT USE @recoverable METHODS HERE!
 	def ParseArgs(this):
 		this.parsedArgs, extraArgs = this.argparser.parse_known_args()
```

### Comparing `eons-2.5.8/pkg/eons/method/External.py` & `eons-2.5.9/pkg/eons/method/External.py`

 * *Files identical despite different names*

### Comparing `eons-2.5.8/pkg/eons/resolve/resolve_find_by_fetch.py` & `eons-2.5.9/pkg/eons/resolve/resolve_find_by_fetch.py`

 * *Files identical despite different names*

### Comparing `eons-2.5.8/pkg/eons/resolve/resolve_import_module.py` & `eons-2.5.9/pkg/eons/resolve/resolve_import_module.py`

 * *Files identical despite different names*

### Comparing `eons-2.5.8/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py` & `eons-2.5.9/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py`

 * *Files identical despite different names*

### Comparing `eons-2.5.8/pkg/eons.egg-info/PKG-INFO` & `eons-2.5.9/pkg/eons.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.5.8
+Version: 2.5.9
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -35,18 +35,22 @@
 
 For example implementations, check out:
  * [apie](https://github.com/eons-dev/bin_apie)
  * [ebbs](https://github.com/eons-dev/bin_ebbs)
  * [emi](https://github.com/eons-dev/bin_emi)
 
 Arguments available to all Eons Executors:
-* `-v` or `--verbose` (count, i.e `-vv` = 2) or `--verbosity #`, where # is some number, or the `verbosity` environment or config value: will show more information and increase the logging level, e.g. print debug messages (3 for debug; 2 for info).
+* `-v` or `--verbose` (count, i.e `-vv` = 2) or `--verbosity #`, where # is some number, or the `verbosity` environment or config value: will show more information and increase the logging level, e.g. print debug messages; see [log-levels](#log-levels), below for more info.
 * `--config` or `-c` (string): the path to a json config file from which other values may be retrieved.
 * `--no-repo` or the `no_repo` environment or config value (bool, i.e. 'True', 'true', etc.): whether or not to enable reaching out to online servers for code (see Dynamic Functionality, below).
 * `--log-file` or the `log_file` environment or config value (string; supports formatting, e.g. '/var/log/eons/{this.name}.log'): optional value for logging to a file in addition to stderr.
+* `--log-indentation` (bool): whether or not tab out logs; see [indentation](#indentation), below.
+* `--log-tab-width` (int): how many spaces to use for indentation; see [indentation](#indentation), below.
+* `--log-aggregate` (bool): whether or not to send logs to a remote aggregation service; see [aggregation](#aggregation), below.
+* `--log-aggregate-url` (string): the url of the remote aggregation service; see [aggregation](#aggregation), below.
 
 ## Features
 
 Eons supports 5 major features:
 * Get inputs to functors by drilling down through multiple layers.
 * Allow functors to change behavior with their order of execution.
 * Provide functionality by downloading functors on the fly.
@@ -161,14 +165,47 @@
 | :---              | :---         |    :----:   |  :---:  |            :---:              |     :---:    |
 | Classic           |is a|:heavy_check_mark:|:x:|:heavy_check_mark:|:heavy_check_mark:|
 | Implicit          |how does|:x:|:heavy_check_mark:|:heavy_check_mark:|:x:|
 | External          |has a|:heavy_check_mark:|:x:|:x:|:x:|
 
 You are not restricted to a single kind of inheritance. You can, and are encouraged, to use all forms of inheritance in your code!
 
+## Logging
+
+Eons attempts to provide a detailed, robust, and pleasant logging experience. We use the [logging](https://docs.python.org/3/library/logging.html) module, and shim in additional features through our log formatter.
+
+### Log Levels
+
+The log level may be set by the `verbosity` or `-v` flags.
+Children and other modules of Eons may employ their own logging levels. However, Eons provides the following levels by default:
+0. `CRITICAL`: only get notified if absolutely necessary.
+1. `WARNING`: get notified about potential problems.
+2. `INFO`: see what's generally going on.
+3. `DEBUG` + urllib3 WARNING: see what's really going on.
+4. Empty: reserved for modules.
+5. `DEBUG`: see everything.
+
+### Log Features
+
+#### Indentation
+
+To make logs easier to read, each Functor can be optionally tabbed out as it might be in source code, allowing you to readily see the scope where a log occurs. Each indentation begins with a `|` character and is followed by a number of spaces equal to the tab width minus one. For example, using a tab width of 2, a log line at the top level would be `| ...`, while a log at the second level would be `| | ...`.
+
+This feature is enabled by default. To disable it you can set `log_indentation` to `False`.
+
+To configure the size of the indentation, you can set `log_tab_width` to the number of spaces you want to use. For example a tab width of 1 would be just `|`, while a tab width of 4 would be `|   `.
+
+#### Aggregation
+
+For security information and event management (SIEM), Eons supports sending logs to a remote endpoint.
+
+This will only be done if a valid repo username and password are provided. If you provide a username and password, but don't want to send your logs to a remote server, you can set `log_aggregate` to `False`. 
+
+You may also set the `log_aggregate_url` to wherever you'd like to send your logs. By default, this is set to `https://eons.sh/log`.
+
 ## Performance
 
 At Eons LLC, we always prefer functionality over performance. This is the same as the whole "don't prematurely optimize" argument. With that said, optimizing is always good and we try to do it as much as possible.
 
 Please let us know if you are hitting any bottlenecks in this or any of our other libraries! 
 
 ## Design
```

### Comparing `eons-2.5.8/pkg/eons.egg-info/SOURCES.txt` & `eons-2.5.9/pkg/eons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

