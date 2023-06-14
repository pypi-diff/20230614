# Comparing `tmp/eons-2.5.9.tar.gz` & `tmp/eons-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eons-2.5.9.tar", last modified: Sun May 21 03:57:14 2023, max compression
+gzip compressed data, was "eons-2.6.0.tar", last modified: Wed Jun 14 01:27:57 2023, max compression
```

## Comparing `eons-2.5.9.tar` & `eons-2.6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:57:14.158999 eons-2.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)    22214 2023-05-21 03:57:14.158999 eons-2.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22007 2023-05-21 03:56:58.000000 eons-2.5.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:57:14.154999 eons-2.5.9/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:57:14.154999 eons-2.5.9/pkg/eons/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-21 03:57:06.000000 eons-2.5.9/pkg/eons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    88370 2023-05-21 03:57:06.000000 eons-2.5.9/pkg/eons/eons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:57:14.154999 eons-2.5.9/pkg/eons/method/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-21 03:56:52.000000 eons-2.5.9/pkg/eons/method/External.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 03:57:06.000000 eons-2.5.9/pkg/eons/method/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:57:14.158999 eons-2.5.9/pkg/eons/resolve/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 03:57:06.000000 eons-2.5.9/pkg/eons/resolve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-21 03:56:52.000000 eons-2.5.9/pkg/eons/resolve/resolve_find_by_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-21 03:56:52.000000 eons-2.5.9/pkg/eons/resolve/resolve_import_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-21 03:56:52.000000 eons-2.5.9/pkg/eons/resolve/resolve_install_from_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-21 03:56:52.000000 eons-2.5.9/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-21 03:56:52.000000 eons-2.5.9/pkg/eons/resolve/resolve_install_with_pip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:57:14.154999 eons-2.5.9/pkg/eons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22214 2023-05-21 03:57:14.000000 eons-2.5.9/pkg/eons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-21 03:57:14.000000 eons-2.5.9/pkg/eons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 03:57:14.000000 eons-2.5.9/pkg/eons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-21 03:57:14.000000 eons-2.5.9/pkg/eons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-21 03:57:14.000000 eons-2.5.9/pkg/eons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-21 03:57:06.000000 eons-2.5.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-21 03:57:14.158999 eons-2.5.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:27:57.259849 eons-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-06-14 01:27:57.259849 eons-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-06-14 01:27:37.000000 eons-2.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:27:57.251849 eons-2.6.0/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:27:57.251849 eons-2.6.0/pkg/eons/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 01:27:47.000000 eons-2.6.0/pkg/eons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89323 2023-06-14 01:27:47.000000 eons-2.6.0/pkg/eons/eons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:27:57.255849 eons-2.6.0/pkg/eons/method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-14 01:27:27.000000 eons-2.6.0/pkg/eons/method/External.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:27:47.000000 eons-2.6.0/pkg/eons/method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:27:57.259849 eons-2.6.0/pkg/eons/resolve/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:27:47.000000 eons-2.6.0/pkg/eons/resolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-06-14 01:27:27.000000 eons-2.6.0/pkg/eons/resolve/resolve_find_by_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-14 01:27:27.000000 eons-2.6.0/pkg/eons/resolve/resolve_import_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-14 01:27:27.000000 eons-2.6.0/pkg/eons/resolve/resolve_install_from_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-14 01:27:27.000000 eons-2.6.0/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-14 01:27:27.000000 eons-2.6.0/pkg/eons/resolve/resolve_install_with_pip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:27:57.255849 eons-2.6.0/pkg/eons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-06-14 01:27:57.000000 eons-2.6.0/pkg/eons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-14 01:27:57.000000 eons-2.6.0/pkg/eons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:27:57.000000 eons-2.6.0/pkg/eons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-14 01:27:57.000000 eons-2.6.0/pkg/eons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-14 01:27:57.000000 eons-2.6.0/pkg/eons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-14 01:27:47.000000 eons-2.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-14 01:27:57.259849 eons-2.6.0/setup.cfg
```

### Comparing `eons-2.5.9/PKG-INFO` & `eons-2.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.5.9
+Version: 2.6.0
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -39,14 +39,15 @@
  * [emi](https://github.com/eons-dev/bin_emi)
 
 Arguments available to all Eons Executors:
 * `-v` or `--verbose` (count, i.e `-vv` = 2) or `--verbosity #`, where # is some number, or the `verbosity` environment or config value: will show more information and increase the logging level, e.g. print debug messages; see [log-levels](#log-levels), below for more info.
 * `--config` or `-c` (string): the path to a json config file from which other values may be retrieved.
 * `--no-repo` or the `no_repo` environment or config value (bool, i.e. 'True', 'true', etc.): whether or not to enable reaching out to online servers for code (see Dynamic Functionality, below).
 * `--log-file` or the `log_file` environment or config value (string; supports formatting, e.g. '/var/log/eons/{this.name}.log'): optional value for logging to a file in addition to stderr.
+* `--log-time-stardate` or the `log_time_stardate` environment or config value (bool): whether or not to use [Eons Official Time](https://github.com/eons-dev/eot.exe) stardate time in logs (default is `true`).
 * `--log-indentation` (bool): whether or not tab out logs; see [indentation](#indentation), below.
 * `--log-tab-width` (int): how many spaces to use for indentation; see [indentation](#indentation), below.
 * `--log-aggregate` (bool): whether or not to send logs to a remote aggregation service; see [aggregation](#aggregation), below.
 * `--log-aggregate-url` (string): the url of the remote aggregation service; see [aggregation](#aggregation), below.
 
 ## Features
```

### Comparing `eons-2.5.9/README.md` & `eons-2.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
  * [emi](https://github.com/eons-dev/bin_emi)
 
 Arguments available to all Eons Executors:
 * `-v` or `--verbose` (count, i.e `-vv` = 2) or `--verbosity #`, where # is some number, or the `verbosity` environment or config value: will show more information and increase the logging level, e.g. print debug messages; see [log-levels](#log-levels), below for more info.
 * `--config` or `-c` (string): the path to a json config file from which other values may be retrieved.
 * `--no-repo` or the `no_repo` environment or config value (bool, i.e. 'True', 'true', etc.): whether or not to enable reaching out to online servers for code (see Dynamic Functionality, below).
 * `--log-file` or the `log_file` environment or config value (string; supports formatting, e.g. '/var/log/eons/{this.name}.log'): optional value for logging to a file in addition to stderr.
+* `--log-time-stardate` or the `log_time_stardate` environment or config value (bool): whether or not to use [Eons Official Time](https://github.com/eons-dev/eot.exe) stardate time in logs (default is `true`).
 * `--log-indentation` (bool): whether or not tab out logs; see [indentation](#indentation), below.
 * `--log-tab-width` (int): how many spaces to use for indentation; see [indentation](#indentation), below.
 * `--log-aggregate` (bool): whether or not to send logs to a remote aggregation service; see [aggregation](#aggregation), below.
 * `--log-aggregate-url` (string): the url of the remote aggregation service; see [aggregation](#aggregation), below.
 
 ## Features
```

### Comparing `eons-2.5.9/pkg/eons/eons.py` & `eons-2.6.0/pkg/eons/eons.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import logging
 import os
+import shutil
+from copy import deepcopy
+import builtins
 import sys
 import pkgutil
 import importlib.machinery
 import importlib.util
 import types
-import builtins
+import traceback
+import jsonpickle
+from pathlib import Path
+from subprocess import Popen
+from subprocess import PIPE
+from subprocess import STDOUT
+import inspect
+import operator
+import re
 import argparse
 import requests
-import jsonpickle
 import yaml
 from requests_futures.sessions import FuturesSession
-from pathlib import Path
 from tqdm import tqdm
 from zipfile import ZipFile
 from distutils.dir_util import mkpath
 from eot import EOT
-import operator
-import traceback
-from copy import deepcopy
-import shutil
-from subprocess import Popen
-from subprocess import PIPE
-from subprocess import STDOUT
-import inspect
-import re
 
 ######## START CONTENT ########
 def INVALID_NAME():
 	return "INVALID_NAME"
 
 class ActualType(type):
 	def __repr__(self):
@@ -321,173 +321,14 @@
 		setattr(logging.getLogger(), methodName, logForLevel)
 		setattr(logging, methodName, logToRoot)
 
 
 jsonpickle.handlers.registry.register(util.DotDict, util.DotDictPickler)
 
 
-# A DataContainer allows Data to be stored and worked with.
-# This class is intended to be derived from and added to.
-# Each DataContainer is comprised of multiple Data (see Datum.py for more).
-# NOTE: DataContainers are, themselves Data. Thus, you can nest your child classes however you would like.
-class DataContainer(Datum):
-
-	def __init__(this, name=INVALID_NAME()):
-		super().__init__(name)
-
-		# The data *this contains.
-		this.data = []
-
-
-	# RETURNS: an empty, invalid Datum.
-	def InvalidDatum(this):
-		ret = Datum()
-		ret.Invalidate()
-		return ret
-
-
-	# Sort things! Requires by be a valid attribute of all Data.
-	def SortData(this, by):
-		this.data.sort(key=operator.attrgetter(by))
-
-
-	# Adds a Datum to *this
-	def AddDatum(this, datum):
-		this.data.append(datum)
-
-
-	# RETURNS: a Datum with datumAttribute equal to match, an invalid Datum if none found.
-	def GetDatumBy(this, datumAttribute, match):
-		for d in this.data:
-			try: # within for loop 'cause maybe there's an issue with only 1 Datum and the rest are fine.
-				if (str(util.GetAttr(d, datumAttribute)) == str(match)):
-					return d
-			except Exception as e:
-				logging.error(f"{this.name} - {e.message}")
-				continue
-		return this.InvalidDatum()
-
-
-	# RETURNS: a Datum of the given name, an invalid Datum if none found.
-	def GetDatum(this, name):
-		return this.GetDatumBy('name', name)
-
-
-	# Removes all Data in toRem from *this.
-	# RETURNS: the Data removed
-	def RemoveData(this, toRem):
-		# logging.debug(f"Removing {toRem}")
-		this.data = [d for d in this.data if d not in toRem]
-		return toRem
-
-
-	# Removes all Data which match toRem along the given attribute
-	def RemoveDataBy(this, datumAttribute, toRem):
-		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) in list(map(str, toRem))]
-		return this.RemoveData(toRem)
-
-
-	# Removes all Data in *this except toKeep.
-	# RETURNS: the Data removed
-	def KeepOnlyData(this, toKeep):
-		toRem = [d for d in this.data if d not in toKeep]
-		return this.RemoveData(toRem)
-
-
-	# Removes all Data except those that match toKeep along the given attribute
-	# RETURNS: the Data removed
-	def KeepOnlyDataBy(this, datumAttribute, toKeep):
-		# logging.debug(f"Keeping only class with a {datumAttribute} of {toKeep}")
-		# toRem = []
-		# for d in this.class:
-		#	 shouldRem = False
-		#	 for k in toKeep:
-		#		 if (str(util.GetAttr(d, datumAttribute)) == str(k)):
-		#			 logging.debug(f"found {k} in {d.__dict__}")
-		#			 shouldRem = True
-		#			 break
-		#	 if (shouldRem):
-		#		 toRem.append(d)
-		#	 else:
-		#		 logging.debug(f"{k} not found in {d.__dict__}")
-		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) not in list(map(str, toKeep))]
-		return this.RemoveData(toRem)
-
-
-	# Removes all Data with the name "INVALID NAME"
-	# RETURNS: the removed Data
-	def RemoveAllUnlabeledData(this):
-		toRem = []
-		for d in this.data:
-			if (d.name =="INVALID NAME"):
-				toRem.append(d)
-		return this.RemoveData(toRem)
-
-
-	# Removes all invalid Data
-	# RETURNS: the removed Data
-	def RemoveAllInvalidData(this):
-		toRem = []
-		for d in this.data:
-			if (not d.IsValid()):
-				toRem.append(d)
-		return this.RemoveData(toRem)
-
-
-	# Removes all Data that have an attribute value relative to target.
-	# The given relation can be things like operator.le (i.e. <=)
-	#   See https://docs.python.org/3/library/operator.html for more info.
-	# If ignoreNames is specified, any Data of those names will be ignored.
-	# RETURNS: the Data removed
-	def RemoveDataRelativeToTarget(this, datumAttribute, relation, target, ignoreNames = []):
-		try:
-			toRem = []
-			for d in this.data:
-				if (ignoreNames and d.name in ignoreNames):
-					continue
-				if (relation(util.GetAttr(d, datumAttribute), target)):
-					toRem.append(d)
-			return this.RemoveData(toRem)
-		except Exception as e:
-			logging.error(f"{this.name} - {e.message}")
-			return []
-
-
-	# Removes any Data that have the same datumAttribute as a previous Datum, keeping only the first.
-	# RETURNS: The Data removed
-	def RemoveDuplicateDataOf(this, datumAttribute):
-		toRem = [] # list of Data
-		alreadyProcessed = [] # list of strings, not whatever datumAttribute is.
-		for d1 in this.data:
-			skip = False
-			for dp in alreadyProcessed:
-				if (str(util.GetAttr(d1, datumAttribute)) == dp):
-					skip = True
-					break
-			if (skip):
-				continue
-			for d2 in this.data:
-				if (d1 is not d2 and str(util.GetAttr(d1, datumAttribute)) == str(util.GetAttr(d2, datumAttribute))):
-					logging.info(f"Removing duplicate Datum {d2} with unique id {util.GetAttr(d2, datumAttribute)}")
-					toRem.append(d2)
-					alreadyProcessed.append(str(util.GetAttr(d1, datumAttribute)))
-		return this.RemoveData(toRem)
-
-
-	# Adds all Data from otherDataContainer to *this.
-	# If there are duplicate Data identified by the attribute preventDuplicatesOf, they are removed.
-	# RETURNS: the Data removed, if any.
-	def ImportDataFrom(this, otherDataContainer, preventDuplicatesOf=None):
-		this.data.extend(otherDataContainer.data);
-		if (preventDuplicatesOf is not None):
-			return this.RemoveDuplicateDataOf(preventDuplicatesOf)
-		return []
-
-
-
 # FunctorTracker is a global singleton which keeps a record of all functors that are currently in the call stack.
 # Functors should add and remove themselves from this list when they are called.
 class FunctorTracker:
 	def __init__(this):
 		# Singletons man...
 		if "instance" not in FunctorTracker.__dict__:
 			logging.debug(f"Creating new FunctorTracker: {this}")
@@ -612,15 +453,15 @@
 		this.configNameOverrides = {}
 
 		# Rolling back can be disabled by setting this to False.
 		this.enableRollback = True
 
 		# Numerical result indication the success or failure of *this.
 		# Set automatically.
-		# 0 is invalid; 1 is best; higher numbers are usually worse.
+		# 0 is success; 1 is no change; higher numbers are some kind of error.
 		this.result = 0
 
 		# Whether or not we should pass on exceptions when calls fail.
 		this.raiseExceptions = True
 
 		# Ease of use members
 		# These can be calculated in Function and Rollback, respectively.
@@ -632,14 +473,18 @@
 
 		# The progenitor of *this.
 		this.executor = None
 
 		# Those which come next (in order).
 		this.next = []
 
+		# Callback method
+		this.callbacks = util.DotDict()
+		this.callbacks.fetch = None
+
 
 	# Override this and do whatever!
 	# This is purposefully vague.
 	def Function(this):
 		pass
 
 
@@ -755,15 +600,15 @@
 	# Wrapper around setattr
 	def Set(this, varName, value, evaluateExpressions=True):
 		value = this.EvaluateToType(value, evaluateExpressions)
 		for key, var in this.configNameOverrides.items():
 			if (varName == key):
 				varName = var
 				break
-		logging.debug(f"Setting ({type(value)}) {varName} = {value}")
+		logging.info(f"{varName} = {value} ({type(value)})")
 		setattr(this, varName, value)
 
 
 	# Will try to get a value for the given varName from:
 	#	first: this
 	#	second: whatever was called before *this
 	#	third: the executor (args > config > environment)
@@ -794,18 +639,23 @@
 			if (loc not in this.fetchLocations.keys()):
 				# Maybe the location is meant for executor, precursor, etc.
 				continue
 
 			ret, found = this.fetchLocations[loc](varName, default, fetchFrom, attempted)
 			if (found):
 				logging.debug(f"...{this.name} got {varName} from {loc}.")
+				if (this.callbacks.fetch):
+					this.callbacks.fetch(varName = varName, location = loc, value = ret)
 				if (start):
 					return ret
 				return ret, True
 
+		if (this.callbacks.fetch):
+			this.callbacks.fetch(varName = varName, location = 'default', value = default)
+
 		if (start):
 			logging.debug(f"...{this.name} could not find {varName}; using default: {default}.")
 			return default
 		else:
 			return default, False
 
 
@@ -1066,63 +916,63 @@
 				logging.error(f"ERROR: {e}")
 				util.LogStack()
 
 
 	# Make functor.
 	# Don't worry about this; logic is abstracted to Function
 	def __call__(this, *args, **kwargs) :
-		logging.debug(f"{this.name} ({args}, {kwargs}) {{")
+		logging.info(f"{this.name} ({args}, {kwargs}) {{")
 		FunctorTracker.Push(this)
 
 		ret = None
 		nextRet = None
 		
 		try:
 			this.WarmUp(*args, **kwargs)
 			logging.debug(f"{this.name}({this.args}, {this.kwargs})")
 
 			getattr(this, f"Before{this.callMethod}")()
 			ret = getattr(this, this.callMethod)()
 
 			if (getattr(this, f"Did{this.callMethod}Succeed")()):
-					this.result = 1
+					this.result = 0
 					# logging.info(f"{this.name} successful!")
 					nextRet = this.CallNext()
 			elif (this.enableRollback):
 				logging.warning(f"{this.name} failed. Attempting Rollback...")
 				ret = getattr(this, this.rollbackMethod)()
 				if (getattr(this, f"Did{this.rollbackMethod}Succeed")()):
-					this.result = 2
+					this.result = 1
 					# logging.info(f"Rollback succeeded. All is well.")
 					nextRet = this.CallNext()
 				else:
-					this.result = 3
+					this.result = 2
 					logging.error(f"ROLLBACK FAILED! SYSTEM STATE UNKNOWN!!!")
 			else:
-				this.result = 4
+				this.result = 3
 				logging.error(f"{this.name} failed.")
 
 			getattr(this, f"After{this.callMethod}")()
 
 		except Exception as e:
 			if (this.raiseExceptions):
 				raise e
 			else:
 				logging.error(f"ERROR: {e}")
 				util.LogStack()
 
-		if (this.raiseExceptions and this.result > 2):
+		if (this.raiseExceptions and this.result > 1):
 			raise FunctorError(f"{this.name} failed with result {this.result}")
 
 		if (nextRet is not None):
 			ret = nextRet
 
-		logging.debug(f"return {ret}")
+		logging.info(f"return {ret}")
 		FunctorTracker.Pop(this)
-		logging.debug(f"}} ({this.name})")
+		logging.info(f"}} ({this.name})")
 
 		return ret
 
 
 	# Adapter for @recoverable.
 	# See Recoverable.py for details
 	def GetExecutor(this):
@@ -1202,14 +1052,386 @@
 		envVar = os.getenv(varName.upper())
 		if (envVar is not None):
 			return envVar, True
 		return default, False
 
 	######## END: Fetch Locations ########
 
+
+class FetchCallbackFunctor(Functor):
+
+	def __init__(this, name = "FetchCallbackFunctor"):
+		super().__init__(name)
+
+		this.requiredKWArgs.append('varName')
+		this.requiredKWArgs.append('location')
+		this.requiredKWArgs.append('value')
+
+		this.functionSucceeded = True
+		this.enableRollback = False
+
+# ExecutorTracker is a global singleton which keeps a record of all Executors that have been launched.
+# This can be abused quite a bit, so please try to restrict usage of this to only:
+# * Ease of use global functions
+#
+# Thanks! 
+class ExecutorTracker:
+	def __init__(this):
+		# Singletons man...
+		if "instance" not in ExecutorTracker.__dict__:
+			logging.debug(f"Creating new ExecutorTracker: {this}")
+			ExecutorTracker.instance = this
+		else:
+			return None
+
+		this.executors = [None]
+
+	@staticmethod
+	def Instance():
+		if "instance" not in ExecutorTracker.__dict__:
+			ExecutorTracker()
+		return ExecutorTracker.instance
+
+	@staticmethod
+	def Push(executor):
+		ExecutorTracker.Instance().executors.append(executor)
+
+		# Adding the executor to our list here increases its reference count.
+		# Executors are supposed to remove themselves from this list when they are deleted.
+		# A python object cannot be deleted if it has references.
+		# Thus, we forcibly decrease the reference count and rely on Exectuor's self-reporting to avoid accessing deallocated memory.
+		# This appears to cause segfaults on some systems, so we'll just live with the fact that Executors will never be destroyed.
+		# If you want your executor to stop being tracked, do it yourself. :(
+		#
+		# ctypes.pythonapi.Py_DecRef(ctypes.py_object(executor))
+
+		logging.debug(f"Now tracking Executor: {executor}")
+
+	@staticmethod
+	def Pop(executor):
+		try:
+			ExecutorTracker.Instance().executors.remove(executor)
+			logging.debug(f"No longer tracking Executor: {executor}")
+		except:
+			pass
+
+	@staticmethod
+	def GetLatest():
+		return ExecutorTracker.Instance().executors[-1]
+
+
+# Global Fetch() function.
+# Uses the latest registered Executor
+def Fetch(varName, default=None, fetchFrom=None, start=True, attempted=None):
+    return ExecutorTracker.GetLatest().Fetch(varName, default, fetchFrom, start, attempted)
+
+# Ease-of-use wrapper for the global Fetch()
+def f(varName, default=None, fetchFrom=None, start=True, attempted=None):
+    Fetch(varName, default, fetchFrom, start, attempted)
+
+def METHOD_PENDING_POPULATION(obj, *args, **kwargs):
+	raise MethodPendingPopulation("METHOD PENDING POPULATION")
+
+# Use the @method() decorator to turn any class function into an eons Method Functor.
+# Methods are Functors which can be implicitly transferred between classes (see Functor.PopulateMethods)
+# Using Methods also gives us full control over the execution of your code; meaning, we can change how Python interprets what you wrote!
+# All Methods will be stored in the method member of your Functor. However, you shouldn't need to access that.
+#
+# If you would like to specify a custom implementation, set the 'impl' kwarg (e.g. @method(impl='MyMethodImplementation'))
+# Beside 'impl', all key-word arguments provided to the @method() decorator will be set as member variables of the created Method.
+# For example, to set whether or not the Method should be propagated, you can use @method(propagate=True).
+# This means, you can create a custom means of interpreting your code with your own feature set and still use this @method decorator.
+# Perhaps you'd like something along the lines of: @method(impl='MakeAwesome', awesomeness=10000).
+# NOTE: in order for impl to work, the implementation class must already be Registered (or this must be called from an appropriate @recoverable function).
+def method(impl='Method', **kwargs):
+
+	# Class decorator with __set_name__, as described here: https://stackoverflow.com/questions/2366713/can-a-decorator-of-an-instance-method-access-the-class
+	class MethodDecorator:
+		def __init__(this, function):
+			this.function = function
+
+		# Apparently, this is called when the decorated function is constructed.
+		def __set_name__(this, cls, functionName):
+			logging.debug(f"Constructing new method for {this.function} in {cls}")
+
+			# Create and configure a new Method
+
+			method = SelfRegistering(impl)
+			method.Constructor(this.function, cls)
+			for key, value in kwargs.items():
+				setattr(method, key, value)
+
+			# Store the new method in the class
+			if (not hasattr(cls, 'classMethods') or not isinstance(cls.classMethods, dict)):
+				cls.classMethods = {}
+			cls.classMethods[functionName] = method
+
+			# Self-destruct by replacing the decorated function.
+			# We rely on Functor.PopulateMethods to re-establish the method as callable.
+			# It seems like this just outright removes the methods. There may be an issue with using __get__ this way.
+			# Regardless deleting the method is okay as long as we add it back before anyone notices.
+			setattr(cls, functionName, METHOD_PENDING_POPULATION.__get__(cls))
+
+	return MethodDecorator
+
+class Method(Functor):
+
+	def __init__(this, name=INVALID_NAME()):
+		super().__init__(name)
+
+		# Methods do not fetch from the environment by default.
+		this.fetchFrom.remove('environment')
+
+		# Whether or not *this should be combined with other Methods of the same name.
+		this.inheritMethods = True
+
+		# Where should inherited methods be inserted?
+		# First here means "before *this".
+		# If False, inherited code will be run after *this.
+		this.inheritedMethodsFirst = True # otherwise ...Last
+
+		# Propagation allows for Functors called after that which defines *this to also call *this.
+		# This system allows for partial, implicit inheritance.
+		# By default, Methods will not be propagated. Use @propagate to enable propagation.
+		this.propagate = False
+
+		# We don't care about these checks right now.
+		# Plus, we can't exactly wrap 2 functions even if we wanted to Rollback.
+		this.functionSucceeded = True
+		this.rollbackSucceeded = True
+		this.enableRollback = False
+
+		# The source code of the function we're implementing.
+		this.source = ""
+
+		# The instance of the class to which *this belongs.
+		# i.e. the object that called *this, aka 'owner', 'caller', etc.
+		this.object = None
+
+		this.original = util.DotDict()
+		this.original.cls = None
+		this.original.function = None
+
+
+	# Make *this execute the code in this.source
+	def UpdateSource(this):
+		wrappedFunctionName = f'_eons_method_{this.name}'
+		completeSource = f'''\
+def {wrappedFunctionName}(this):
+{this.source}
+'''
+		if (this.executor and this.executor.verbosity > 3):
+			logging.debug(f"Source for {this.name} is:\n{completeSource}")
+		code = compile(completeSource, '', 'exec')
+		exec(code)
+		exec(f'this.Function = {wrappedFunctionName}.__get__(this, this.__class__)')
+
+
+
+	# Parse arguments and update the source code
+	# TODO: Implement full python parser to avoid bad string replacement (e.g. "def func(self):... self.selfImprovement" => "... this.object.this.object.Improvement").
+	def PopulateFrom(this, function):
+		this.source = ':'.join(inspect.getsource(function).split(':')[1:]) #Remove the first function definition
+
+		args = inspect.signature(function, follow_wrapped=False).parameters
+		thisSymbol = next(iter(args))
+		#del args[thisSymbol] # ??? 'mappingproxy' object does not support item deletion
+		this.source = this.source.replace(thisSymbol, 'this.object')
+
+		first = True
+		for arg in args.values(): #args.values[1:] also doesn't work.
+			if (first):
+				first = False
+				continue
+
+			replaceWith = arg.name
+
+			if (arg.kind == inspect.Parameter.VAR_POSITIONAL):
+				replaceWith = 'this.args'
+
+			elif (arg.kind == inspect.Parameter.VAR_KEYWORD):
+				replaceWith = 'this.kwargs'
+
+			else:
+				if (arg.default != inspect.Parameter.empty):
+					this.optionalKWArgs[arg.name] = arg.default
+				else:
+					this.requiredKWArgs.append(arg.name)
+				replaceWith = f'this.{arg.name}'
+
+				if (arg.kind in [inspect.Parameter.POSITIONAL_OR_KEYWORD, inspect.Parameter.POSITIONAL_ONLY]):
+					this.argMapping.append(arg.name)
+
+			this.source = this.source.replace(arg.name, replaceWith)
+
+
+	# When properly constructing a Method, rely only on the function *this should implement.
+	# The class and all other properties are irrelevant. However, they are provided and intended for debugging only.
+	def Constructor(this, function, cls):
+		this.name = function.__name__
+		this.original.cls = cls
+		this.original.function = function
+
+		this.PopulateFrom(function)
+		
+		# UpdateSource is called by Functor.PopulateMethods()
+		# this.UpdateSource()
+
+
+	# Grab any known and necessary args from this.kwargs before any Fetch calls are made.
+	def PopulatePrecursor(this):
+		if (not this.object):
+			raise MissingArgumentError(f"Call {this.name} from a class instance: {this.original.cls.__name__}.{this.name}(...). Maybe Functor.PopulateMethods() hasn't been called yet?")
+
+		this.executor = this.object.executor
+
+		if ('precursor' in this.kwargs):
+			this.precursor = this.kwargs.pop('precursor')
+		else:
+			this.precursor = None
+
+
+	# Next is set by Functor.PopulateMethods.
+	# We  definitely don't want to Fetch 'next'.
+	def PopulateNext(this):
+		pass
+
+
+	# Method.next should be a list of other Methods, as opposed to the standard string; so, instead of Executor.Execute..., we can directly invoke whatever is next.
+	# We skip all validation here.
+	# We also don't pass any args that were given in the initial function call. Those can all be Fetched from 'precursor'.
+	def CallNext(this):
+		if (not this.next):
+			return None
+
+		for next in this.next:
+			next(precursor=this)
+
+
+# The standard Functor extends Functor to add a set of standard members and methods.
+# This is similar to the standard library in C and C++
+# You must inherit from *this if you would like to use the functionality *this provides. The methods defined will not be propagated.
+class StandardFunctor(Functor):
+	def __init__(this, name="Standard Functor"):
+		super().__init__(name)
+
+	# Override this and do whatever!
+	# This is purposefully vague.
+	def Function(this):
+		pass
+
+
+	# Undo any changes made by UserFunction.
+	# Please override this too!
+	def Rollback(this):
+		pass
+
+
+	# Override this to check results of operation and report on status.
+	# Override this to perform whatever success checks are necessary.
+	def DidFunctionSucceed(this):
+		return this.functionSucceeded
+
+
+	# RETURN whether or not the Rollback was successful.
+	# Override this to perform whatever success checks are necessary.
+	def DidRollbackSucceed(this):
+		return this.rollbackSucceeded
+
+
+	######## START: UTILITIES ########
+
+	# RETURNS: an opened file object for writing.
+	# Creates the path if it does not exist.
+	@method()
+	def CreateFile(this, file, mode="w+"):
+		Path(os.path.dirname(os.path.abspath(file))).mkdir(parents=True, exist_ok=True)
+		return open(file, mode)
+
+	# Copy a file or folder from source to destination.
+	# This really shouldn't be so hard...
+	# root allows us to interpret '/' as something other than the top of the filesystem.
+	@method()
+	def Copy(this, source, destination, root='/'):
+		if (source.startswith('/')):
+			source = str(Path(root).joinpath(source[1:]).resolve())
+		else:
+			source = str(Path(source).resolve())
+		
+		destination = str(Path(destination).resolve())
+		
+		Path(destination).parent.mkdir(parents=True, exist_ok=True)
+
+		if (os.path.isfile(source)):
+			logging.debug(f"Copying file {source} to {destination}")
+			try:
+				shutil.copy(source, destination)
+			except shutil.Error as exc:
+				errors = exc.args[0]
+				for error in errors:
+					src, dst, msg = error
+					logging.debug(f"{msg}")
+		elif (os.path.isdir(source)):
+			logging.debug(f"Copying directory {source} to {destination}")
+			try:
+				shutil.copytree(source, destination)
+			except shutil.Error as exc:
+				errors = exc.args[0]
+				for error in errors:
+					src, dst, msg = error
+					logging.debug(f"{msg}")
+		else:
+			logging.error(f"Could not find source to copy: {source}")
+
+	# Delete a file or folder
+	@method()
+	def Delete(this, target):
+		if (not os.path.exists(target)):
+			logging.debug(f"Unable to delete nonexistent target: {target}")
+			return
+		if (os.path.isfile(target)):
+			logging.debug(f"Deleting file {target}")
+			os.remove(target)
+		elif (os.path.isdir(target)):
+			logging.debug(f"Deleting directory {target}")
+			try:
+				shutil.rmtree(target)
+			except shutil.Error as exc:
+				errors = exc.args[0]
+				for error in errors:
+					src, dst, msg = error
+					logging.debug(f"{msg}")
+
+	# Run whatever.
+	# DANGEROUS!!!!!
+	# RETURN: Return value and, optionally, the output as a list of lines.
+	@method()
+	def RunCommand(this, command, saveout=False, raiseExceptions=True):
+		logging.debug(f"================ Running command: {command} ================")
+		process = Popen(command, stdout=PIPE, stderr=STDOUT, shell=True)
+		output = []
+		while process.poll() is None:
+			line = process.stdout.readline().decode('utf8')[:-1]
+			if (saveout):
+				output.append(line)
+			if (line):
+				logging.debug(f"| {line}")  # [:-1] to strip excessive new lines.
+
+		message = f"Command returned {process.returncode}: {command}"
+		logging.debug(message)
+		if (raiseExceptions and process.returncode is not None and process.returncode):
+			raise CommandUnsuccessful(message)
+		
+		logging.debug(f"================ Completed command: {command} ================")
+		if (saveout):
+			return process.returncode, output
+		
+		return process.returncode
+	######## END: UTILITIES ########
+
 #from .Executor import Executor # don't import this, it'll be circular!
 
 # @recoverable
 # Decorating another function with this method will engage the error recovery system provided by *this.
 # To use this, you must define a GetExecutor() method in your class and decorate the functions you want to recover from.
 # For more info, see Executor.ResolveError and the README.md
 def recoverable(function):
@@ -1282,62 +1504,324 @@
 		return ret
 
 	#  We failed to resolve the error. Die
 	sys.tracebacklimit = 0 # traceback is NOT helpful here.
 	raise FailedErrorResolution(f"Tried and failed to resolve: {error} STACK: {executor.errorResolutionStack}. See earlier logs (in debug) for traceback.")
 
 
-# ExecutorTracker is a global singleton which keeps a record of all Executors that have been launched.
-# This can be abused quite a bit, so please try to restrict usage of this to only:
-# * Ease of use global functions
+# A DataContainer allows Data to be stored and worked with.
+# This class is intended to be derived from and added to.
+# Each DataContainer is comprised of multiple Data (see Datum.py for more).
+# NOTE: DataContainers are, themselves Data. Thus, you can nest your child classes however you would like.
+class DataContainer(Datum):
+
+	def __init__(this, name=INVALID_NAME()):
+		super().__init__(name)
+
+		# The data *this contains.
+		this.data = []
+
+
+	# RETURNS: an empty, invalid Datum.
+	def InvalidDatum(this):
+		ret = Datum()
+		ret.Invalidate()
+		return ret
+
+
+	# Sort things! Requires by be a valid attribute of all Data.
+	def SortData(this, by):
+		this.data.sort(key=operator.attrgetter(by))
+
+
+	# Adds a Datum to *this
+	def AddDatum(this, datum):
+		this.data.append(datum)
+
+
+	# RETURNS: a Datum with datumAttribute equal to match, an invalid Datum if none found.
+	def GetDatumBy(this, datumAttribute, match):
+		for d in this.data:
+			try: # within for loop 'cause maybe there's an issue with only 1 Datum and the rest are fine.
+				if (str(util.GetAttr(d, datumAttribute)) == str(match)):
+					return d
+			except Exception as e:
+				logging.error(f"{this.name} - {e.message}")
+				continue
+		return this.InvalidDatum()
+
+
+	# RETURNS: a Datum of the given name, an invalid Datum if none found.
+	def GetDatum(this, name):
+		return this.GetDatumBy('name', name)
+
+
+	# Removes all Data in toRem from *this.
+	# RETURNS: the Data removed
+	def RemoveData(this, toRem):
+		# logging.debug(f"Removing {toRem}")
+		this.data = [d for d in this.data if d not in toRem]
+		return toRem
+
+
+	# Removes all Data which match toRem along the given attribute
+	def RemoveDataBy(this, datumAttribute, toRem):
+		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) in list(map(str, toRem))]
+		return this.RemoveData(toRem)
+
+
+	# Removes all Data in *this except toKeep.
+	# RETURNS: the Data removed
+	def KeepOnlyData(this, toKeep):
+		toRem = [d for d in this.data if d not in toKeep]
+		return this.RemoveData(toRem)
+
+
+	# Removes all Data except those that match toKeep along the given attribute
+	# RETURNS: the Data removed
+	def KeepOnlyDataBy(this, datumAttribute, toKeep):
+		# logging.debug(f"Keeping only class with a {datumAttribute} of {toKeep}")
+		# toRem = []
+		# for d in this.class:
+		#	 shouldRem = False
+		#	 for k in toKeep:
+		#		 if (str(util.GetAttr(d, datumAttribute)) == str(k)):
+		#			 logging.debug(f"found {k} in {d.__dict__}")
+		#			 shouldRem = True
+		#			 break
+		#	 if (shouldRem):
+		#		 toRem.append(d)
+		#	 else:
+		#		 logging.debug(f"{k} not found in {d.__dict__}")
+		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) not in list(map(str, toKeep))]
+		return this.RemoveData(toRem)
+
+
+	# Removes all Data with the name "INVALID NAME"
+	# RETURNS: the removed Data
+	def RemoveAllUnlabeledData(this):
+		toRem = []
+		for d in this.data:
+			if (d.name =="INVALID NAME"):
+				toRem.append(d)
+		return this.RemoveData(toRem)
+
+
+	# Removes all invalid Data
+	# RETURNS: the removed Data
+	def RemoveAllInvalidData(this):
+		toRem = []
+		for d in this.data:
+			if (not d.IsValid()):
+				toRem.append(d)
+		return this.RemoveData(toRem)
+
+
+	# Removes all Data that have an attribute value relative to target.
+	# The given relation can be things like operator.le (i.e. <=)
+	#   See https://docs.python.org/3/library/operator.html for more info.
+	# If ignoreNames is specified, any Data of those names will be ignored.
+	# RETURNS: the Data removed
+	def RemoveDataRelativeToTarget(this, datumAttribute, relation, target, ignoreNames = []):
+		try:
+			toRem = []
+			for d in this.data:
+				if (ignoreNames and d.name in ignoreNames):
+					continue
+				if (relation(util.GetAttr(d, datumAttribute), target)):
+					toRem.append(d)
+			return this.RemoveData(toRem)
+		except Exception as e:
+			logging.error(f"{this.name} - {e.message}")
+			return []
+
+
+	# Removes any Data that have the same datumAttribute as a previous Datum, keeping only the first.
+	# RETURNS: The Data removed
+	def RemoveDuplicateDataOf(this, datumAttribute):
+		toRem = [] # list of Data
+		alreadyProcessed = [] # list of strings, not whatever datumAttribute is.
+		for d1 in this.data:
+			skip = False
+			for dp in alreadyProcessed:
+				if (str(util.GetAttr(d1, datumAttribute)) == dp):
+					skip = True
+					break
+			if (skip):
+				continue
+			for d2 in this.data:
+				if (d1 is not d2 and str(util.GetAttr(d1, datumAttribute)) == str(util.GetAttr(d2, datumAttribute))):
+					logging.info(f"Removing duplicate Datum {d2} with unique id {util.GetAttr(d2, datumAttribute)}")
+					toRem.append(d2)
+					alreadyProcessed.append(str(util.GetAttr(d1, datumAttribute)))
+		return this.RemoveData(toRem)
+
+
+	# Adds all Data from otherDataContainer to *this.
+	# If there are duplicate Data identified by the attribute preventDuplicatesOf, they are removed.
+	# RETURNS: the Data removed, if any.
+	def ImportDataFrom(this, otherDataContainer, preventDuplicatesOf=None):
+		this.data.extend(otherDataContainer.data);
+		if (preventDuplicatesOf is not None):
+			return this.RemoveDuplicateDataOf(preventDuplicatesOf)
+		return []
+
+
+
+# Use an ErrorStringParser for each "parsers" in order to avoid having to override the GetObjectFromError method and create a new class for every error you want to handle.
+# ErrorStringParsers enable ErrorResolutions to be created on a per-functionality, rather than per-error basis, reducing the total amount of duplicate code.
+# Each error has a different string. In order to get the object of the error, we have to know where the object starts and ends.
+# NOTE: this assumes only 1 object per string. Maybe fancier parsing logic can be added in the future.
 #
-# Thanks! 
-class ExecutorTracker:
-	def __init__(this):
-		# Singletons man...
-		if "instance" not in ExecutorTracker.__dict__:
-			logging.debug(f"Creating new ExecutorTracker: {this}")
-			ExecutorTracker.instance = this
+# startPosition is always positive
+# endPosition is always negative
+class ErrorStringParser:
+
+	def __init__(this, applicableError, startPosition, endPosition):
+		this.applicableError = applicableError
+		this.startPosition = startPosition
+		this.endPosition = endPosition
+
+	def Parse(this, errorString):
+		end = this.endPosition
+		if (not end):
+			end = len(errorString)
+		return errorString[this.startPosition:end]
+
+
+# ErrorResolution is a Functor which can be executed when an Exception is raised.
+# The goal of this class is to do some kind of work that will fix the problem on the second try of whatever generated the error.
+class ErrorResolution(StandardFunctor):
+
+	def __init__(this, name=INVALID_NAME()):
+		super().__init__(name)
+
+		# What errors, as ErrorStringParser objects, is *this prepared to handle?
+		this.parsers = []
+
+		this.error = None
+		this.errorType = ""
+		this.errorString = ""
+		this.errorObject = ""
+		this.errorResolutionStack = {}
+
+		# Provided directly from the recoverable decorator.
+		this.optionalKWArgs["obj"] = None
+		this.optionalKWArgs["function"] = None
+
+		# We do want to know whether or not we should attempt to run whatever failed again.
+		# So, let's store that in functionSucceeded. Meaning if this.functionSucceeded, try the original method again.
+		# No rollback, by default and definitely don't throw Exceptions.
+		this.enableRollback = False
+		this.functionSucceeded = True
+		this.raiseExceptions = False
+
+		this.errorShouldBeResolved = False
+
+
+
+	# Put your logic here!
+	def Resolve(this):
+		# You get the following members:
+		# this.error (an Exception)
+		# this.errorString (a string cast of the Exception)
+		# this.errorType (a string)
+		# this.errorObjet (a string or whatever you return from GetObjectFromError())
+
+		# You get the following guarantees:
+		# *this has not been called on this particular error before.
+		# the error given is applicable to *this per this.parsers
+
+		###############################################
+		# Please throw errors if something goes wrong #
+		# Otherwise, set this.errorShouldBeResolved   #
+		###############################################
+		
+		pass
+
+
+
+	# Helper method for creating ErrorStringParsers
+	# To use this, simply take an example output and replace the object you want to extract with "OBJECT"
+	def ApplyTo(this, error, exampleString):
+		match = re.search('OBJECT', exampleString)
+		this.parsers.append(ErrorStringParser(error, match.start(), match.end() - len(exampleString)))
+
+
+	# Get the type of this.error as a string.
+	def GetErrorType(this):
+		return type(this.error).__name__
+
+
+	# Get an actionable object from the error.
+	# For example, if the error is 'ModuleNotFoundError', what is the module?
+	def GetObjectFromError(this):
+		for parser in this.parsers:
+			if (parser.applicableError != this.errorType):
+				continue
+
+			this.errorObject = parser.Parse(this.errorString)
+			return
+
+		raise ErrorResolutionError(f"{this.name} cannot parse error object from ({this.errorType}): {str(this.error)}.")
+
+
+	# Determine if this resolution method is applicable.
+	def CanProcess(this):
+		return this.GetErrorType() in [parser.applicableError for parser in this.parsers]
+
+
+	# Grab any known and necessary args from this.kwargs before any Fetch calls are made.
+	def ParseInitialArgs(this):
+		super().ParseInitialArgs()
+		if ('error' in this.kwargs):
+			this.error = this.kwargs.pop('error')
+			# Just assume the error is an actual Exception object.
 		else:
-			return None
+			raise ErrorResolutionError(f"{this.name} was not given an error to resolve.")
 
-		this.executors = [None]
+		this.errorString = str(this.error)
+		this.errorType = this.GetErrorType()
 
-	@staticmethod
-	def Instance():
-		if "instance" not in ExecutorTracker.__dict__:
-			ExecutorTracker()
-		return ExecutorTracker.instance
+		# Internal member to avoid processing duplicates
+		this.errorResolutionStack = this.executor.errorResolutionStack
 
-	@staticmethod
-	def Push(executor):
-		ExecutorTracker.Instance().executors.append(executor)
 
-		# Adding the executor to our list here increases its reference count.
-		# Executors are supposed to remove themselves from this list when they are deleted.
-		# A python object cannot be deleted if it has references.
-		# Thus, we forcibly decrease the reference count and rely on Exectuor's self-reporting to avoid accessing deallocated memory.
-		# This appears to cause segfaults on some systems, so we'll just live with the fact that Executors will never be destroyed.
-		# If you want your executor to stop being tracked, do it yourself. :(
-		#
-		# ctypes.pythonapi.Py_DecRef(ctypes.py_object(executor))
+	# Error resolution is unchained.
+	def PopulateNext(this):
+		this.next = []
 
-		logging.debug(f"Now tracking Executor: {executor}")
 
-	@staticmethod
-	def Pop(executor):
-		try:
-			ExecutorTracker.Instance().executors.remove(executor)
-			logging.debug(f"No longer tracking Executor: {executor}")
-		except:
-			pass
+	# Override of Functor method.
+	# We'll keep calling this until an error is raised.
+	def Function(this):
+		this.functionSucceeded = True
+		this.errorShouldBeResolved = True
+		
+		if (not this.CanProcess()):
+			this.errorShouldBeResolved = False
+			return this.errorResolutionStack, this.errorShouldBeResolved
 
-	@staticmethod
-	def GetLatest():
-		return ExecutorTracker.Instance().executors[-1]
+		if (not this.errorString in this.errorResolutionStack.keys()):
+			this.errorResolutionStack.update({this.errorString:[]})
+		
+		if (this.name in this.errorResolutionStack[this.errorString]):
+			raise FailedErrorResolution(f"{this.name} already tried and failed to resolve {this.errorType}: {this.errorString}.")
+
+		this.GetObjectFromError()
+
+		try:
+			this.Resolve()
+		except Exception as e:
+			logging.error(f"Error resolution with {this.name} failed: {e}")
+			util.LogStack()
+			this.functionSucceeded = False
+		
+		this.errorResolutionStack[this.errorString].append(this.name)
+		return this.errorResolutionStack, this.errorShouldBeResolved
 
 
 # Executor: a base class for user interfaces.
 # An Executor is a functor and can be executed as such.
 # For example
 #	class MyExecutor(Executor):
 #		def __init__(this):
@@ -1349,14 +1833,15 @@
 class Executor(DataContainer, Functor):
 
 	def __init__(this, name=INVALID_NAME(), descriptionStr="Eons python framework. Extend as thou wilt."):
 		this.SetupLogging()
 
 		super().__init__(name)
 
+		this.optionalKWArgs['log_time_stardate'] = True
 		this.optionalKWArgs['log_indentation'] = True
 		this.optionalKWArgs['log_tab_width'] = 2
 		this.optionalKWArgs['log_aggregate'] = True
 		this.optionalKWArgs['log_aggregate_url'] = "https://eons.sh/log"
 
 		this.resolveErrors = True
 		this.errorRecursionDepth = 0
@@ -1485,15 +1970,15 @@
 			util.AddLoggingLevel('recovery', logging.ERROR+1)
 		except:
 			# Could already be setup.
 			pass
 
 		class CustomFormatter(logging.Formatter):
 
-			preFormat = util.console.GetColorCode('white', 'dark') + '%(asctime)s '
+			preFormat = util.console.GetColorCode('white', 'dark') + '__TIME__ '
 			levelName = '[%(levelname)8s] '
 			indentation = util.console.GetColorCode('blue', 'dark', styles=['faint']) + '__INDENTATION__' + util.console.GetColorCode('white', 'dark', styles=['none'])
 			message = '%(message)s '
 			postFormat = util.console.GetColorCode('white', 'dark') + '(%(filename)s:%(lineno)s)' + util.console.resetStyle
 
 			formats = {
 				logging.DEBUG: preFormat + levelName + indentation + util.console.GetColorCode('cyan', 'dark') + message + postFormat,
@@ -1511,42 +1996,48 @@
 				if (hasattr(logging.getLogger(), 'setupBy')):
 					executor = getattr(logging.getLogger(), 'setupBy')
 
 					# The executor won't have populated its optionalKWArgs until after this method is effected.
 					# So we wait until the last optional arg is set to start using the executor.
 					if (not hasattr(executor, 'log_aggregate_url')):
 						executor = None
-				
-				# Add indentation.
-				if (executor
-					and executor.log_indentation
-					and executor.log_tab_width
-					):
-					log_fmt = log_fmt.replace('__INDENTATION__', f"|{' ' * (executor.log_tab_width - 1)}" * (FunctorTracker.GetCount() - 1)) # -1 because we're already in a Functor.
+
+				if (executor):
+					# Add indentation.
+					if (executor.log_indentation and executor.log_tab_width):
+						log_fmt = log_fmt.replace('__INDENTATION__', f"|{' ' * (executor.log_tab_width - 1)}" * (FunctorTracker.GetCount() - 1)) # -1 because we're already in a Functor.
+					else:
+						log_fmt = log_fmt.replace('__INDENTATION__', ' ')
+
+					# Add time.
+					if (executor.log_time_stardate):
+						log_fmt = log_fmt.replace('__TIME__', f"{EOT.GetStardate()}")
+					else:
+						log_fmt = log_fmt.replace('__TIME__', "%(asctime)s")
+
+					# Aggregate logs remotely.
+					if (executor.log_aggregate 
+						and executor.repo.username is not None 
+						and executor.repo.password is not None
+						and record.module != 'connectionpool' # Prevent recursion.
+						):
+						aggregateEndpoint = executor.log_aggregate_url
+						log = {
+							'level': record.levelname,
+							'message': record.getMessage(), # TODO: Sanitize to prevent 400 errors.
+							'source': executor.name,
+							'timestamp': EOT.GetStardate()
+						}
+						try:
+							executor.asyncSession.put(aggregateEndpoint, json=log, auth=(executor.repo.username, executor.repo.password))
+						except Exception as e:
+							pass
 				else:
 					log_fmt = log_fmt.replace('__INDENTATION__', ' ')
-
-				# Aggregate logs remotely.
-				if (executor
-					and executor.log_aggregate 
-					and executor.repo.username is not None 
-					and executor.repo.password is not None
-					and record.module != 'connectionpool' # Prevent recursion.
-					):
-					aggregateEndpoint = executor.log_aggregate_url
-					log = {
-						'level': record.levelname,
-						'message': record.getMessage(), # TODO: Sanitize to prevent 400 errors.
-						'source': executor.name,
-						'timestamp': EOT.GetStardate()
-					}
-					try:
-						executor.asyncSession.put(aggregateEndpoint, json=log, auth=(executor.repo.username, executor.repo.password))
-					except Exception as e:
-						pass
+					log_fmt = log_fmt.replace('__TIME__', "%(asctime)s")
 
 				formatter = logging.Formatter(log_fmt, datefmt = '%H:%M:%S')
 				return formatter.format(record)
 
 		# Skip setting up logging if it's already been done.
 		if (hasattr(logging.getLogger(), 'setupBy')):
 			return
@@ -2051,470 +2542,7 @@
 		for key, val in this.extraArgs.items():
 			if (key == varName):
 				return val, True
 		return default, False
 
 	######## END: Fetch Locations ########
 
-
-def METHOD_PENDING_POPULATION(obj, *args, **kwargs):
-	raise MethodPendingPopulation("METHOD PENDING POPULATION")
-
-# Use the @method() decorator to turn any class function into an eons Method Functor.
-# Methods are Functors which can be implicitly transferred between classes (see Functor.PopulateMethods)
-# Using Methods also gives us full control over the execution of your code; meaning, we can change how Python interprets what you wrote!
-# All Methods will be stored in the method member of your Functor. However, you shouldn't need to access that.
-#
-# If you would like to specify a custom implementation, set the 'impl' kwarg (e.g. @method(impl='MyMethodImplementation'))
-# Beside 'impl', all key-word arguments provided to the @method() decorator will be set as member variables of the created Method.
-# For example, to set whether or not the Method should be propagated, you can use @method(propagate=True).
-# This means, you can create a custom means of interpreting your code with your own feature set and still use this @method decorator.
-# Perhaps you'd like something along the lines of: @method(impl='MakeAwesome', awesomeness=10000).
-# NOTE: in order for impl to work, the implementation class must already be Registered (or this must be called from an appropriate @recoverable function).
-def method(impl='Method', **kwargs):
-
-	# Class decorator with __set_name__, as described here: https://stackoverflow.com/questions/2366713/can-a-decorator-of-an-instance-method-access-the-class
-	class MethodDecorator:
-		def __init__(this, function):
-			this.function = function
-
-		# Apparently, this is called when the decorated function is constructed.
-		def __set_name__(this, cls, functionName):
-			logging.debug(f"Constructing new method for {this.function} in {cls}")
-
-			# Create and configure a new Method
-
-			method = SelfRegistering(impl)
-			method.Constructor(this.function, cls)
-			for key, value in kwargs.items():
-				setattr(method, key, value)
-
-			# Store the new method in the class
-			if (not hasattr(cls, 'classMethods') or not isinstance(cls.classMethods, dict)):
-				cls.classMethods = {}
-			cls.classMethods[functionName] = method
-
-			# Self-destruct by replacing the decorated function.
-			# We rely on Functor.PopulateMethods to re-establish the method as callable.
-			# It seems like this just outright removes the methods. There may be an issue with using __get__ this way.
-			# Regardless deleting the method is okay as long as we add it back before anyone notices.
-			setattr(cls, functionName, METHOD_PENDING_POPULATION.__get__(cls))
-
-	return MethodDecorator
-
-class Method(Functor):
-
-	def __init__(this, name=INVALID_NAME()):
-		super().__init__(name)
-
-		# Methods do not fetch from the environment by default.
-		this.fetchFrom.remove('environment')
-
-		# Whether or not *this should be combined with other Methods of the same name.
-		this.inheritMethods = True
-
-		# Where should inherited methods be inserted?
-		# First here means "before *this".
-		# If False, inherited code will be run after *this.
-		this.inheritedMethodsFirst = True # otherwise ...Last
-
-		# Propagation allows for Functors called after that which defines *this to also call *this.
-		# This system allows for partial, implicit inheritance.
-		# By default, Methods will not be propagated. Use @propagate to enable propagation.
-		this.propagate = False
-
-		# We don't care about these checks right now.
-		# Plus, we can't exactly wrap 2 functions even if we wanted to Rollback.
-		this.functionSucceeded = True
-		this.rollbackSucceeded = True
-		this.enableRollback = False
-
-		# The source code of the function we're implementing.
-		this.source = ""
-
-		# The instance of the class to which *this belongs.
-		# i.e. the object that called *this, aka 'owner', 'caller', etc.
-		this.object = None
-
-		this.original = util.DotDict()
-		this.original.cls = None
-		this.original.function = None
-
-
-	# Make *this execute the code in this.source
-	def UpdateSource(this):
-		wrappedFunctionName = f'_eons_method_{this.name}'
-		completeSource = f'''\
-def {wrappedFunctionName}(this):
-{this.source}
-'''
-		if (this.executor and this.executor.verbosity > 3):
-			logging.debug(f"Source for {this.name} is:\n{completeSource}")
-		code = compile(completeSource, '', 'exec')
-		exec(code)
-		exec(f'this.Function = {wrappedFunctionName}.__get__(this, this.__class__)')
-
-
-
-	# Parse arguments and update the source code
-	# TODO: Implement full python parser to avoid bad string replacement (e.g. "def func(self):... self.selfImprovement" => "... this.object.this.object.Improvement").
-	def PopulateFrom(this, function):
-		this.source = ':'.join(inspect.getsource(function).split(':')[1:]) #Remove the first function definition
-
-		args = inspect.signature(function, follow_wrapped=False).parameters
-		thisSymbol = next(iter(args))
-		#del args[thisSymbol] # ??? 'mappingproxy' object does not support item deletion
-		this.source = this.source.replace(thisSymbol, 'this.object')
-
-		first = True
-		for arg in args.values(): #args.values[1:] also doesn't work.
-			if (first):
-				first = False
-				continue
-
-			replaceWith = arg.name
-
-			if (arg.kind == inspect.Parameter.VAR_POSITIONAL):
-				replaceWith = 'this.args'
-
-			elif (arg.kind == inspect.Parameter.VAR_KEYWORD):
-				replaceWith = 'this.kwargs'
-
-			else:
-				if (arg.default != inspect.Parameter.empty):
-					this.optionalKWArgs[arg.name] = arg.default
-				else:
-					this.requiredKWArgs.append(arg.name)
-				replaceWith = f'this.{arg.name}'
-
-				if (arg.kind in [inspect.Parameter.POSITIONAL_OR_KEYWORD, inspect.Parameter.POSITIONAL_ONLY]):
-					this.argMapping.append(arg.name)
-
-			this.source = this.source.replace(arg.name, replaceWith)
-
-
-	# When properly constructing a Method, rely only on the function *this should implement.
-	# The class and all other properties are irrelevant. However, they are provided and intended for debugging only.
-	def Constructor(this, function, cls):
-		this.name = function.__name__
-		this.original.cls = cls
-		this.original.function = function
-
-		this.PopulateFrom(function)
-		
-		# UpdateSource is called by Functor.PopulateMethods()
-		# this.UpdateSource()
-
-
-	# Grab any known and necessary args from this.kwargs before any Fetch calls are made.
-	def PopulatePrecursor(this):
-		if (not this.object):
-			raise MissingArgumentError(f"Call {this.name} from a class instance: {this.original.cls.__name__}.{this.name}(...). Maybe Functor.PopulateMethods() hasn't been called yet?")
-
-		this.executor = this.object.executor
-
-		if ('precursor' in this.kwargs):
-			this.precursor = this.kwargs.pop('precursor')
-		else:
-			this.precursor = None
-
-
-	# Next is set by Functor.PopulateMethods.
-	# We  definitely don't want to Fetch 'next'.
-	def PopulateNext(this):
-		pass
-
-
-	# Method.next should be a list of other Methods, as opposed to the standard string; so, instead of Executor.Execute..., we can directly invoke whatever is next.
-	# We skip all validation here.
-	# We also don't pass any args that were given in the initial function call. Those can all be Fetched from 'precursor'.
-	def CallNext(this):
-		if (not this.next):
-			return None
-
-		for next in this.next:
-			next(precursor=this)
-
-
-# The standard Functor extends Functor to add a set of standard members and methods.
-# This is similar to the standard library in C and C++
-# You must inherit from *this if you would like to use the functionality *this provides. The methods defined will not be propagated.
-class StandardFunctor(Functor):
-	def __init__(this, name="Standard Functor"):
-		super().__init__(name)
-
-	# Override this and do whatever!
-	# This is purposefully vague.
-	def Function(this):
-		pass
-
-
-	# Undo any changes made by UserFunction.
-	# Please override this too!
-	def Rollback(this):
-		pass
-
-
-	# Override this to check results of operation and report on status.
-	# Override this to perform whatever success checks are necessary.
-	def DidFunctionSucceed(this):
-		return this.functionSucceeded
-
-
-	# RETURN whether or not the Rollback was successful.
-	# Override this to perform whatever success checks are necessary.
-	def DidRollbackSucceed(this):
-		return this.rollbackSucceeded
-
-
-	######## START: UTILITIES ########
-
-	# RETURNS: an opened file object for writing.
-	# Creates the path if it does not exist.
-	@method()
-	def CreateFile(this, file, mode="w+"):
-		Path(os.path.dirname(os.path.abspath(file))).mkdir(parents=True, exist_ok=True)
-		return open(file, mode)
-
-	# Copy a file or folder from source to destination.
-	# This really shouldn't be so hard...
-	# root allows us to interpret '/' as something other than the top of the filesystem.
-	@method()
-	def Copy(this, source, destination, root='/'):
-		if (source.startswith('/')):
-			source = str(Path(root).joinpath(source[1:]).resolve())
-		else:
-			source = str(Path(source).resolve())
-		
-		destination = str(Path(destination).resolve())
-		
-		Path(destination).parent.mkdir(parents=True, exist_ok=True)
-
-		if (os.path.isfile(source)):
-			logging.debug(f"Copying file {source} to {destination}")
-			try:
-				shutil.copy(source, destination)
-			except shutil.Error as exc:
-				errors = exc.args[0]
-				for error in errors:
-					src, dst, msg = error
-					logging.debug(f"{msg}")
-		elif (os.path.isdir(source)):
-			logging.debug(f"Copying directory {source} to {destination}")
-			try:
-				shutil.copytree(source, destination)
-			except shutil.Error as exc:
-				errors = exc.args[0]
-				for error in errors:
-					src, dst, msg = error
-					logging.debug(f"{msg}")
-		else:
-			logging.error(f"Could not find source to copy: {source}")
-
-	# Delete a file or folder
-	@method()
-	def Delete(this, target):
-		if (not os.path.exists(target)):
-			logging.debug(f"Unable to delete nonexistent target: {target}")
-			return
-		if (os.path.isfile(target)):
-			logging.debug(f"Deleting file {target}")
-			os.remove(target)
-		elif (os.path.isdir(target)):
-			logging.debug(f"Deleting directory {target}")
-			try:
-				shutil.rmtree(target)
-			except shutil.Error as exc:
-				errors = exc.args[0]
-				for error in errors:
-					src, dst, msg = error
-					logging.debug(f"{msg}")
-
-	# Run whatever.
-	# DANGEROUS!!!!!
-	# RETURN: Return value and, optionally, the output as a list of lines.
-	@method()
-	def RunCommand(this, command, saveout=False, raiseExceptions=True):
-		logging.debug(f"================ Running command: {command} ================")
-		process = Popen(command, stdout=PIPE, stderr=STDOUT, shell=True)
-		output = []
-		while process.poll() is None:
-			line = process.stdout.readline().decode('utf8')[:-1]
-			if (saveout):
-				output.append(line)
-			if (line):
-				logging.debug(f"| {line}")  # [:-1] to strip excessive new lines.
-
-		message = f"Command returned {process.returncode}: {command}"
-		logging.debug(message)
-		if (raiseExceptions and process.returncode is not None and process.returncode):
-			raise CommandUnsuccessful(message)
-		
-		logging.debug(f"================ Completed command: {command} ================")
-		if (saveout):
-			return process.returncode, output
-		
-		return process.returncode
-	######## END: UTILITIES ########
-
-
-# Global Fetch() function.
-# Uses the latest registered Executor
-def Fetch(varName, default=None, fetchFrom=None, start=True, attempted=None):
-    return ExecutorTracker.GetLatest().Fetch(varName, default, fetchFrom, start, attempted)
-
-# Ease-of-use wrapper for the global Fetch()
-def f(varName, default=None, fetchFrom=None, start=True, attempted=None):
-    Fetch(varName, default, fetchFrom, start, attempted)
-
-# Use an ErrorStringParser for each "parsers" in order to avoid having to override the GetObjectFromError method and create a new class for every error you want to handle.
-# ErrorStringParsers enable ErrorResolutions to be created on a per-functionality, rather than per-error basis, reducing the total amount of duplicate code.
-# Each error has a different string. In order to get the object of the error, we have to know where the object starts and ends.
-# NOTE: this assumes only 1 object per string. Maybe fancier parsing logic can be added in the future.
-#
-# startPosition is always positive
-# endPosition is always negative
-class ErrorStringParser:
-
-	def __init__(this, applicableError, startPosition, endPosition):
-		this.applicableError = applicableError
-		this.startPosition = startPosition
-		this.endPosition = endPosition
-
-	def Parse(this, errorString):
-		end = this.endPosition
-		if (not end):
-			end = len(errorString)
-		return errorString[this.startPosition:end]
-
-
-# ErrorResolution is a Functor which can be executed when an Exception is raised.
-# The goal of this class is to do some kind of work that will fix the problem on the second try of whatever generated the error.
-class ErrorResolution(StandardFunctor):
-
-	def __init__(this, name=INVALID_NAME()):
-		super().__init__(name)
-
-		# What errors, as ErrorStringParser objects, is *this prepared to handle?
-		this.parsers = []
-
-		this.error = None
-		this.errorType = ""
-		this.errorString = ""
-		this.errorObject = ""
-		this.errorResolutionStack = {}
-
-		# Provided directly from the recoverable decorator.
-		this.optionalKWArgs["obj"] = None
-		this.optionalKWArgs["function"] = None
-
-		# We do want to know whether or not we should attempt to run whatever failed again.
-		# So, let's store that in functionSucceeded. Meaning if this.functionSucceeded, try the original method again.
-		# No rollback, by default and definitely don't throw Exceptions.
-		this.enableRollback = False
-		this.functionSucceeded = True
-		this.raiseExceptions = False
-
-		this.errorShouldBeResolved = False
-
-
-
-	# Put your logic here!
-	def Resolve(this):
-		# You get the following members:
-		# this.error (an Exception)
-		# this.errorString (a string cast of the Exception)
-		# this.errorType (a string)
-		# this.errorObjet (a string or whatever you return from GetObjectFromError())
-
-		# You get the following guarantees:
-		# *this has not been called on this particular error before.
-		# the error given is applicable to *this per this.parsers
-
-		###############################################
-		# Please throw errors if something goes wrong #
-		# Otherwise, set this.errorShouldBeResolved   #
-		###############################################
-		
-		pass
-
-
-
-	# Helper method for creating ErrorStringParsers
-	# To use this, simply take an example output and replace the object you want to extract with "OBJECT"
-	def ApplyTo(this, error, exampleString):
-		match = re.search('OBJECT', exampleString)
-		this.parsers.append(ErrorStringParser(error, match.start(), match.end() - len(exampleString)))
-
-
-	# Get the type of this.error as a string.
-	def GetErrorType(this):
-		return type(this.error).__name__
-
-
-	# Get an actionable object from the error.
-	# For example, if the error is 'ModuleNotFoundError', what is the module?
-	def GetObjectFromError(this):
-		for parser in this.parsers:
-			if (parser.applicableError != this.errorType):
-				continue
-
-			this.errorObject = parser.Parse(this.errorString)
-			return
-
-		raise ErrorResolutionError(f"{this.name} cannot parse error object from ({this.errorType}): {str(this.error)}.")
-
-
-	# Determine if this resolution method is applicable.
-	def CanProcess(this):
-		return this.GetErrorType() in [parser.applicableError for parser in this.parsers]
-
-
-	# Grab any known and necessary args from this.kwargs before any Fetch calls are made.
-	def ParseInitialArgs(this):
-		super().ParseInitialArgs()
-		if ('error' in this.kwargs):
-			this.error = this.kwargs.pop('error')
-			# Just assume the error is an actual Exception object.
-		else:
-			raise ErrorResolutionError(f"{this.name} was not given an error to resolve.")
-
-		this.errorString = str(this.error)
-		this.errorType = this.GetErrorType()
-
-		# Internal member to avoid processing duplicates
-		this.errorResolutionStack = this.executor.errorResolutionStack
-
-
-	# Error resolution is unchained.
-	def PopulateNext(this):
-		this.next = []
-
-
-	# Override of Functor method.
-	# We'll keep calling this until an error is raised.
-	def Function(this):
-		this.functionSucceeded = True
-		this.errorShouldBeResolved = True
-		
-		if (not this.CanProcess()):
-			this.errorShouldBeResolved = False
-			return this.errorResolutionStack, this.errorShouldBeResolved
-
-		if (not this.errorString in this.errorResolutionStack.keys()):
-			this.errorResolutionStack.update({this.errorString:[]})
-		
-		if (this.name in this.errorResolutionStack[this.errorString]):
-			raise FailedErrorResolution(f"{this.name} already tried and failed to resolve {this.errorType}: {this.errorString}.")
-
-		this.GetObjectFromError()
-
-		try:
-			this.Resolve()
-		except Exception as e:
-			logging.error(f"Error resolution with {this.name} failed: {e}")
-			util.LogStack()
-			this.functionSucceeded = False
-		
-		this.errorResolutionStack[this.errorString].append(this.name)
-		return this.errorResolutionStack, this.errorShouldBeResolved
-
```

### Comparing `eons-2.5.9/pkg/eons/method/External.py` & `eons-2.6.0/pkg/eons/method/External.py`

 * *Files identical despite different names*

### Comparing `eons-2.5.9/pkg/eons/resolve/resolve_find_by_fetch.py` & `eons-2.6.0/pkg/eons/resolve/resolve_find_by_fetch.py`

 * *Files identical despite different names*

### Comparing `eons-2.5.9/pkg/eons/resolve/resolve_import_module.py` & `eons-2.6.0/pkg/eons/resolve/resolve_import_module.py`

 * *Files identical despite different names*

### Comparing `eons-2.5.9/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py` & `eons-2.6.0/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py`

 * *Files identical despite different names*

### Comparing `eons-2.5.9/pkg/eons.egg-info/PKG-INFO` & `eons-2.6.0/pkg/eons.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.5.9
+Version: 2.6.0
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -39,14 +39,15 @@
  * [emi](https://github.com/eons-dev/bin_emi)
 
 Arguments available to all Eons Executors:
 * `-v` or `--verbose` (count, i.e `-vv` = 2) or `--verbosity #`, where # is some number, or the `verbosity` environment or config value: will show more information and increase the logging level, e.g. print debug messages; see [log-levels](#log-levels), below for more info.
 * `--config` or `-c` (string): the path to a json config file from which other values may be retrieved.
 * `--no-repo` or the `no_repo` environment or config value (bool, i.e. 'True', 'true', etc.): whether or not to enable reaching out to online servers for code (see Dynamic Functionality, below).
 * `--log-file` or the `log_file` environment or config value (string; supports formatting, e.g. '/var/log/eons/{this.name}.log'): optional value for logging to a file in addition to stderr.
+* `--log-time-stardate` or the `log_time_stardate` environment or config value (bool): whether or not to use [Eons Official Time](https://github.com/eons-dev/eot.exe) stardate time in logs (default is `true`).
 * `--log-indentation` (bool): whether or not tab out logs; see [indentation](#indentation), below.
 * `--log-tab-width` (int): how many spaces to use for indentation; see [indentation](#indentation), below.
 * `--log-aggregate` (bool): whether or not to send logs to a remote aggregation service; see [aggregation](#aggregation), below.
 * `--log-aggregate-url` (string): the url of the remote aggregation service; see [aggregation](#aggregation), below.
 
 ## Features
```

### Comparing `eons-2.5.9/pkg/eons.egg-info/SOURCES.txt` & `eons-2.6.0/pkg/eons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eons-2.5.9/setup.cfg` & `eons-2.6.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eons
-version = 2.5.9
+version = 2.6.0
 author = Eons
 author_email = support@eons.llc
 description = Eons Python Framework
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/eons.lib
@@ -18,20 +18,20 @@
 
 [options]
 package_dir = 
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	requests_futures
-	eot
-	requests
-	pyyaml
 	tqdm
 	jsonpickle
+	pyyaml
+	requests
+	eot
+	requests_futures
 
 [options.packages.find]
 where = pkg
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

