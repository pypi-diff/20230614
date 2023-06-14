# Comparing `tmp/pymemuc-0.4.0.tar.gz` & `tmp/pymemuc-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymemuc-0.4.0.tar", max compression
+gzip compressed data, was "pymemuc-0.4.1.tar", max compression
```

## Comparing `pymemuc-0.4.0.tar` & `pymemuc-0.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1057 2023-06-13 23:37:00.709973 pymemuc-0.4.0/LICENSE
--rw-r--r--   0        0        0     1586 2023-06-13 23:37:00.709973 pymemuc-0.4.0/README.md
--rw-r--r--   0        0        0      386 2023-06-13 23:37:00.709973 pymemuc-0.4.0/pymemuc/__init__.py
--rw-r--r--   0        0        0    23116 2023-06-13 23:37:00.709973 pymemuc-0.4.0/pymemuc/_command.py
--rw-r--r--   0        0        0      465 2023-06-13 23:37:00.709973 pymemuc-0.4.0/pymemuc/_constants.py
--rw-r--r--   0        0        0     5146 2023-06-13 23:37:00.709973 pymemuc-0.4.0/pymemuc/_control.py
--rw-r--r--   0        0        0     1214 2023-06-13 23:37:00.709973 pymemuc-0.4.0/pymemuc/_decorators.py
--rw-r--r--   0        0        0    15149 2023-06-13 23:37:00.709973 pymemuc-0.4.0/pymemuc/_manage.py
--rw-r--r--   0        0        0     4139 2023-06-13 23:37:00.713973 pymemuc-0.4.0/pymemuc/_memuc.py
--rw-r--r--   0        0        0      891 2023-06-13 23:37:00.713973 pymemuc-0.4.0/pymemuc/exceptions.py
--rw-r--r--   0        0        0     2953 2023-06-13 23:37:00.713973 pymemuc-0.4.0/pymemuc/pymemuc.py
--rw-r--r--   0        0        0      379 2023-06-13 23:37:00.713973 pymemuc-0.4.0/pymemuc/vminfo.py
--rw-r--r--   0        0        0     1665 2023-06-13 23:37:21.774173 pymemuc-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 pymemuc-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-06-14 01:21:02.159552 pymemuc-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1586 2023-06-14 01:21:02.159552 pymemuc-0.4.1/README.md
+-rw-r--r--   0        0        0      386 2023-06-14 01:21:02.159552 pymemuc-0.4.1/pymemuc/__init__.py
+-rw-r--r--   0        0        0    23116 2023-06-14 01:21:02.159552 pymemuc-0.4.1/pymemuc/_command.py
+-rw-r--r--   0        0        0      465 2023-06-14 01:21:02.159552 pymemuc-0.4.1/pymemuc/_constants.py
+-rw-r--r--   0        0        0     5146 2023-06-14 01:21:02.159552 pymemuc-0.4.1/pymemuc/_control.py
+-rw-r--r--   0        0        0     1214 2023-06-14 01:21:02.159552 pymemuc-0.4.1/pymemuc/_decorators.py
+-rw-r--r--   0        0        0    15149 2023-06-14 01:21:02.159552 pymemuc-0.4.1/pymemuc/_manage.py
+-rw-r--r--   0        0        0     4624 2023-06-14 01:21:02.159552 pymemuc-0.4.1/pymemuc/_memuc.py
+-rw-r--r--   0        0        0      891 2023-06-14 01:21:02.159552 pymemuc-0.4.1/pymemuc/exceptions.py
+-rw-r--r--   0        0        0     3014 2023-06-14 01:21:02.159552 pymemuc-0.4.1/pymemuc/pymemuc.py
+-rw-r--r--   0        0        0      379 2023-06-14 01:21:02.159552 pymemuc-0.4.1/pymemuc/vminfo.py
+-rw-r--r--   0        0        0     1665 2023-06-14 01:21:21.368139 pymemuc-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 pymemuc-0.4.1/PKG-INFO
```

### Comparing `pymemuc-0.4.0/LICENSE` & `pymemuc-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymemuc-0.4.0/README.md` & `pymemuc-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pymemuc-0.4.0/pymemuc/_command.py` & `pymemuc-0.4.1/pymemuc/_command.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.4.0/pymemuc/_control.py` & `pymemuc-0.4.1/pymemuc/_control.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.4.0/pymemuc/_decorators.py` & `pymemuc-0.4.1/pymemuc/_decorators.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.4.0/pymemuc/_manage.py` & `pymemuc-0.4.1/pymemuc/_manage.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.4.0/pymemuc/_memuc.py` & `pymemuc-0.4.1/pymemuc/_memuc.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 if WINREG_EN:
     # pylint: disable=import-error
     from winreg import HKEY_LOCAL_MACHINE, ConnectRegistry, OpenKey, QueryValueEx
 
 ST_INFO = None
 if WIN32:
+    import ctypes
     from subprocess import (
         REALTIME_PRIORITY_CLASS,
         STARTF_USESHOWWINDOW,
         STARTF_USESTDHANDLES,
         STARTUPINFO,
         SW_HIDE,
     )
@@ -48,14 +49,22 @@
     ]:
         with suppress(FileNotFoundError):
             akey = OpenKey(ConnectRegistry(None, HKEY_LOCAL_MACHINE), key)
             return str(join(normpath(QueryValueEx(akey, "InstallLocation")[0]), "Memu"))
     raise PyMemucError("MEmuc not found, is it installed?")
 
 
+@staticmethod
+def _terminate_process(process: Popen):
+    """Terminate a process forcefully on Windows."""
+    handle = ctypes.windll.kernel32.OpenProcess(1, False, process.pid)
+    ctypes.windll.kernel32.TerminateProcess(handle, -1)
+    ctypes.windll.kernel32.CloseHandle(handle)
+
+
 def memuc_run(
     self: "PyMemuc", args: list[str], non_blocking=False, timeout=None
 ) -> Tuple[int, str]:
     """run a command with memuc.exe.
     Memuc can support non-blocking commands, returning a task id.
     A timeout can be specified if memuc is expected to hang,
     but this will not work with non-blocking commands.
@@ -79,24 +88,29 @@
         args.append("-t")
     self.logger.debug("pymemuc._memuc.memuc_run:")
     self.logger.debug(f"\tCommand: \"{' '.join(args)}\"")
     try:
         with Popen(
             args,
             shell=False,
+            bufsize=-1,
             stdout=PIPE,
             stderr=PIPE,
             startupinfo=ST_INFO,
             close_fds=True,
             universal_newlines=True,
         ) as process:
             try:
                 result, _ = process.communicate(timeout=timeout)
             except TimeoutExpired as err:
-                process.kill()
+                if WIN32:
+                    # pylint: disable=protected-access
+                    self._terminate_process(process)
+                else:
+                    process.kill()
                 result, _ = process.communicate()
                 raise PyMemucTimeoutExpired(err) from err
             if lines := result.splitlines():
                 self.logger.debug(f"\tOutput: {lines.pop(0)}")
                 for line in lines:
                     self.logger.debug(f"\t\t{line}")
             return (0, result)
```

### Comparing `pymemuc-0.4.0/pymemuc/exceptions.py` & `pymemuc-0.4.1/pymemuc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.4.0/pymemuc/pymemuc.py` & `pymemuc-0.4.1/pymemuc/pymemuc.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,20 @@
         import_vm,
         list_vm_info,
         randomize_vm,
         rename_vm,
         set_configuration_vm,
         vm_is_running,
     )
-    from ._memuc import _get_memu_top_level, check_task_status, memuc_run
+    from ._memuc import (
+        _get_memu_top_level,
+        _terminate_process,
+        check_task_status,
+        memuc_run,
+    )
 
     def __init__(self, memuc_path: Union[str, None] = None, debug=False) -> None:
         """initialize the class, automatically finding memuc.exe if windows registry is supported,
         otherwise a path must be specified"""
         self.debug = debug
         self.logger = self._configure_logger()
         self.logger.debug("PyMemuc: Debug mode enabled")
```

### Comparing `pymemuc-0.4.0/pyproject.toml` & `pymemuc-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pymemuc"
-version = "v0.4.0"
+version = "v0.4.1"
 description = "A Memuc.exe wrapper for Python"
 readme = "README.md"
 authors = ["Martin Miglio <code@martinmiglio.dev>"]
 license = "MIT"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pymemuc-0.4.0/PKG-INFO` & `pymemuc-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymemuc
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Memuc.exe wrapper for Python
 Home-page: https://github.com/martinmiglio/pymemuc
 License: MIT
 Keywords: memu,memuc,wrapper,api
 Author: Martin Miglio
 Author-email: code@martinmiglio.dev
 Requires-Python: >=3.9,<4.0
```

