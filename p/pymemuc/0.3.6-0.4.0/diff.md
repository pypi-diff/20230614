# Comparing `tmp/pymemuc-0.3.6.tar.gz` & `tmp/pymemuc-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymemuc-0.3.6.tar", max compression
+gzip compressed data, was "pymemuc-0.4.0.tar", max compression
```

## Comparing `pymemuc-0.3.6.tar` & `pymemuc-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1057 2023-06-12 04:30:57.265317 pymemuc-0.3.6/LICENSE
--rw-r--r--   0        0        0     1586 2023-06-12 04:30:57.265317 pymemuc-0.3.6/README.md
--rw-r--r--   0        0        0      386 2023-06-12 04:30:57.269317 pymemuc-0.3.6/pymemuc/__init__.py
--rw-r--r--   0        0        0    22761 2023-06-12 04:30:57.269317 pymemuc-0.3.6/pymemuc/_command.py
--rw-r--r--   0        0        0      465 2023-06-12 04:30:57.269317 pymemuc-0.3.6/pymemuc/_constants.py
--rw-r--r--   0        0        0     4984 2023-06-12 04:30:57.269317 pymemuc-0.3.6/pymemuc/_control.py
--rw-r--r--   0        0        0     1214 2023-06-12 04:30:57.269317 pymemuc-0.3.6/pymemuc/_decorators.py
--rw-r--r--   0        0        0    13670 2023-06-12 04:30:57.269317 pymemuc-0.3.6/pymemuc/_manage.py
--rw-r--r--   0        0        0     4134 2023-06-12 04:30:57.269317 pymemuc-0.3.6/pymemuc/_memuc.py
--rw-r--r--   0        0        0      891 2023-06-12 04:30:57.269317 pymemuc-0.3.6/pymemuc/exceptions.py
--rw-r--r--   0        0        0     2941 2023-06-12 04:30:57.269317 pymemuc-0.3.6/pymemuc/pymemuc.py
--rw-r--r--   0        0        0      379 2023-06-12 04:30:57.269317 pymemuc-0.3.6/pymemuc/vminfo.py
--rw-r--r--   0        0        0     1665 2023-06-12 04:31:16.737548 pymemuc-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 pymemuc-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-06-13 23:37:00.709973 pymemuc-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1586 2023-06-13 23:37:00.709973 pymemuc-0.4.0/README.md
+-rw-r--r--   0        0        0      386 2023-06-13 23:37:00.709973 pymemuc-0.4.0/pymemuc/__init__.py
+-rw-r--r--   0        0        0    23116 2023-06-13 23:37:00.709973 pymemuc-0.4.0/pymemuc/_command.py
+-rw-r--r--   0        0        0      465 2023-06-13 23:37:00.709973 pymemuc-0.4.0/pymemuc/_constants.py
+-rw-r--r--   0        0        0     5146 2023-06-13 23:37:00.709973 pymemuc-0.4.0/pymemuc/_control.py
+-rw-r--r--   0        0        0     1214 2023-06-13 23:37:00.709973 pymemuc-0.4.0/pymemuc/_decorators.py
+-rw-r--r--   0        0        0    15149 2023-06-13 23:37:00.709973 pymemuc-0.4.0/pymemuc/_manage.py
+-rw-r--r--   0        0        0     4139 2023-06-13 23:37:00.713973 pymemuc-0.4.0/pymemuc/_memuc.py
+-rw-r--r--   0        0        0      891 2023-06-13 23:37:00.713973 pymemuc-0.4.0/pymemuc/exceptions.py
+-rw-r--r--   0        0        0     2953 2023-06-13 23:37:00.713973 pymemuc-0.4.0/pymemuc/pymemuc.py
+-rw-r--r--   0        0        0      379 2023-06-13 23:37:00.713973 pymemuc-0.4.0/pymemuc/vminfo.py
+-rw-r--r--   0        0        0     1665 2023-06-13 23:37:21.774173 pymemuc-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 pymemuc-0.4.0/PKG-INFO
```

### Comparing `pymemuc-0.3.6/LICENSE` & `pymemuc-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.6/README.md` & `pymemuc-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.6/pymemuc/_command.py` & `pymemuc-0.4.0/pymemuc/_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -469,14 +469,15 @@
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
     :param vm_name: VM name. Defaults to None.
     :type vm_name: str, optional
     :param timeout: Timeout for the command. Defaults to 10.
     :type timeout: int, optional
     :raises PyMemucIndexError: an error if neither a vm index or a vm name is specified
+    :raises PyMemucError: an error if the command failed
     :return: the list of packages installed on the VM
     :rtype: list[str]
     """
     try:
         if vm_index is not None:
             _, output = self.memuc_run(
                 ["-i", str(vm_index), "getappinfolist"],
@@ -487,14 +488,20 @@
             _, output = self.memuc_run(
                 ["-n", vm_name, "getappinfolist"],
                 timeout=timeout,
                 non_blocking=False,
             )
         else:
             raise PyMemucIndexError("Please specify either a vm index or a vm name")
+        # check if 'cmd: Can't find service: package' is in the output
+        if "cmd: Can't find service: package" in output:
+            raise PyMemucError(
+                "Failed to get the list of apps installed on the VM, "
+                "please make sure the VM is running"
+            )
         output = output.split("\n")
         output = [line.replace("package:", "") for line in output if line != ""]
         return output
     except PyMemucTimeoutExpired:
         return []
```

### Comparing `pymemuc-0.3.6/pymemuc/_control.py` & `pymemuc-0.4.0/pymemuc/_control.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,44 +6,49 @@
 from ._decorators import _retryable
 from .exceptions import PyMemucError, PyMemucIndexError
 
 if TYPE_CHECKING:
     from pymemuc import PyMemuc
 
 
+# pylint: disable=too-many-arguments
 @_retryable
 def start_vm(
     self: "PyMemuc",
     vm_index: Union[int, None] = None,
     vm_name: Union[str, None] = None,
+    headless=False,
     non_blocking=False,
     timeout=None,
 ) -> Literal[True]:
     """Start a VM, must specify either a vm index or a vm name
 
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
     :param vm_name: VM name. Defaults to None.
     :type vm_name: str, optional
+    :param headless: Whether to start the VM in headless mode. Defaults to False.
+    :type headless: bool, optional
     :param non_blocking: Whether to run the command in the background. Defaults to False.
     :type non_blocking: bool, optional
     :param timeout: Timeout in seconds. Cannot be used if non blocking. Defaults to None.
     :type timeout: int, optional
     :raises PyMemucIndexError: an error if neither a vm index or a vm name is specified
     :return: True if the vm was started successfully
     :rtype: Literal[True]
     """
     if vm_index is not None:
-        status, output = self.memuc_run(
-            ["-i", str(vm_index), "start"], non_blocking, timeout
-        )
+        args = ["-i", str(vm_index), "start"]
     elif vm_name is not None:
-        status, output = self.memuc_run(["-n", vm_name, "start"], non_blocking, timeout)
+        args = ["-n", vm_name, "start"]
     else:
         raise PyMemucIndexError("Please specify either a vm index or a vm name")
+    if headless:
+        args.append("-b")
+    status, output = self.memuc_run(args, non_blocking, timeout)
     success = status == 0 and output is not None and "SUCCESS" in output
     if not success:
         raise PyMemucError(f"Failed to start VM: {output}")
     return True
 
 
 @_retryable
```

### Comparing `pymemuc-0.3.6/pymemuc/_decorators.py` & `pymemuc-0.4.0/pymemuc/_decorators.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.6/pymemuc/_manage.py` & `pymemuc-0.4.0/pymemuc/_manage.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,32 +61,39 @@
 
 
 def clone_vm(
     self: "PyMemuc",
     vm_index: Union[int, None] = None,
     vm_name: Union[str, None] = None,
     new_name=None,
+    non_blocking=False,
 ) -> Literal[True]:
     """Clone a VM, must specify either a vm index or a vm name
 
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
     :param vm_name: VM name. Defaults to None.
     :type vm_name: str, optional
     :param new_name: Cloned VM name. Defaults to None.
     :type new_name: str, optional
+    :param non_blocking: Whether to run the command in the background. Defaults to False.
+    :type non_blocking: bool, optional
     :raises PyMemucIndexError: an error if neither a vm index or a vm name is specified
     :return: True if the vm was cloned successfully
     :rtype: Literal[True]
     """
     new_name_cmd = ["-r", new_name] if new_name is not None else []
     if vm_index is not None:
-        status, output = self.memuc_run(["-i", str(vm_index), "clone", *new_name_cmd])
+        status, output = self.memuc_run(
+            ["-i", str(vm_index), "clone", *new_name_cmd], non_blocking
+        )
     elif vm_name is not None:
-        status, output = self.memuc_run(["-n", vm_name, "clone", *new_name_cmd])
+        status, output = self.memuc_run(
+            ["-n", vm_name, "clone", *new_name_cmd], non_blocking
+        )
     else:
         raise PyMemucIndexError("Please specify either a vm index or a vm name")
     success = status == 0 and output is not None and "SUCCESS" in output
     if not success:
         raise PyMemucError(f"Failed to clone VM: {output}")
     return True
 
@@ -176,14 +183,46 @@
         if not success:
             raise PyMemucError(f"Failed to rename VM: {output}")
         return True
     except PyMemucTimeoutExpired as err:
         raise PyMemucError("Failed to rename VM: Timeout expired") from err
 
 
+def compress_vm(
+    self: "PyMemuc",
+    vm_index: Union[int, None] = None,
+    vm_name: Union[str, None] = None,
+    non_blocking=False,
+) -> Literal[True]:
+    """Compress a VM, must specify either a vm index or a vm name
+
+    :param vm_index: VM index. Defaults to None.
+    :type vm_index: int, optional
+    :param vm_name: VM name. Defaults to None.
+    :type vm_name: str, optional
+    :param non_blocking: Whether to run the command in the background. Defaults to False.
+    :type non_blocking: bool, optional
+    :raises PyMemucIndexError: an error if neither a vm index or a vm name is specified
+    :raises PyMemucError: an error if the vm compress failed
+    :return: True if the vm was compressed successfully
+    :rtype: Literal[True]
+    """
+
+    if vm_index is not None:
+        status, output = self.memuc_run(["-i", str(vm_index), "compress"], non_blocking)
+    elif vm_name is not None:
+        status, output = self.memuc_run(["-n", vm_name, "compress"], non_blocking)
+    else:
+        raise PyMemucIndexError("Please specify either a vm index or a vm name")
+    success = status == 0 and output is not None and "SUCCESS" in output
+    if not success:
+        raise PyMemucError(f"Failed to compress VM: {output}")
+    return True
+
+
 def list_vm_info(
     self: "PyMemuc",
     vm_index: Union[int, None] = None,
     vm_name: Union[str, None] = None,
     running=False,
     disk_info=False,
 ) -> list[VMInfo]:
```

### Comparing `pymemuc-0.3.6/pymemuc/_memuc.py` & `pymemuc-0.4.0/pymemuc/_memuc.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     :raises PyMemucTimeoutExpired: an error if the command timed out
     """
     # sourcery skip: extract-method
     args.insert(0, self.memuc_path)
     if timeout is not None and non_blocking:
         raise PyMemucException("Cannot use timeout and non_blocking at the same time")
     if non_blocking:
-        args += "-t"
+        args.append("-t")
     self.logger.debug("pymemuc._memuc.memuc_run:")
     self.logger.debug(f"\tCommand: \"{' '.join(args)}\"")
     try:
         with Popen(
             args,
             shell=False,
             stdout=PIPE,
```

### Comparing `pymemuc-0.3.6/pymemuc/exceptions.py` & `pymemuc-0.4.0/pymemuc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.6/pymemuc/pymemuc.py` & `pymemuc-0.4.0/pymemuc/pymemuc.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         uninstall_apk_vm,
         zoom_in_vm,
         zoom_out_vm,
     )
     from ._control import reboot_vm, start_vm, stop_all_vm, stop_vm
     from ._manage import (
         clone_vm,
+        compress_vm,
         create_vm,
         delete_vm,
         export_vm,
         get_configuration_vm,
         import_vm,
         list_vm_info,
         randomize_vm,
@@ -72,19 +73,19 @@
                 "Windows Registry is not supported on this platform,"
                 + " you must specify the path to memuc.exe manually"
             )
 
     def _configure_logger(self):
         """Configure the logger for the class"""
         logger = logging.getLogger(__name__)
+        logger.propagate = False
         logger.setLevel(logging.DEBUG if self.debug else logging.INFO)
 
         # Create a handler for console output
         console_handler = logging.StreamHandler()
-        console_handler.propagate = False
         console_handler.setLevel(logging.DEBUG)
         formatter = logging.Formatter(
             "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
         )
         console_handler.setFormatter(formatter)
 
         # Add the handler to the logger
```

### Comparing `pymemuc-0.3.6/pyproject.toml` & `pymemuc-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pymemuc"
-version = "v0.3.6"
+version = "v0.4.0"
 description = "A Memuc.exe wrapper for Python"
 readme = "README.md"
 authors = ["Martin Miglio <code@martinmiglio.dev>"]
 license = "MIT"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pymemuc-0.3.6/PKG-INFO` & `pymemuc-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymemuc
-Version: 0.3.6
+Version: 0.4.0
 Summary: A Memuc.exe wrapper for Python
 Home-page: https://github.com/martinmiglio/pymemuc
 License: MIT
 Keywords: memu,memuc,wrapper,api
 Author: Martin Miglio
 Author-email: code@martinmiglio.dev
 Requires-Python: >=3.9,<4.0
```

