# Comparing `tmp/pytest-embedded-qemu-1.3.1.tar.gz` & `tmp/pytest_embedded_qemu-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-embedded-qemu-1.3.1.tar", last modified: Tue Jun  6 08:56:26 2023, max compression
+gzip compressed data, was "pytest_embedded_qemu-1.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest-embedded-qemu-1.3.1.tar` & `pytest_embedded_qemu-1.3.2.tar`

### file list

```diff
@@ -1,16 +1,9 @@
-drwxr-xr-x   0 fuhanxi   (1000) fuhanxi   (1000)        0 2023-06-06 08:56:26.382211 pytest-embedded-qemu-1.3.1/
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     1580 2023-06-06 08:56:26.382211 pytest-embedded-qemu-1.3.1/PKG-INFO
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)      552 2023-06-06 08:04:34.000000 pytest-embedded-qemu-1.3.1/README.md
-drwxr-xr-x   0 fuhanxi   (1000) fuhanxi   (1000)        0 2023-06-06 08:56:26.382211 pytest-embedded-qemu-1.3.1/pytest_embedded_qemu/
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)      295 2023-05-10 06:49:19.000000 pytest-embedded-qemu-1.3.1/pytest_embedded_qemu/__init__.py
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     3335 2023-06-02 06:32:41.000000 pytest-embedded-qemu-1.3.1/pytest_embedded_qemu/app.py
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)      414 2023-06-02 06:32:41.000000 pytest-embedded-qemu-1.3.1/pytest_embedded_qemu/dut.py
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     2388 2023-06-02 06:32:41.000000 pytest-embedded-qemu-1.3.1/pytest_embedded_qemu/qemu.py
-drwxr-xr-x   0 fuhanxi   (1000) fuhanxi   (1000)        0 2023-06-06 08:56:26.382211 pytest-embedded-qemu-1.3.1/pytest_embedded_qemu.egg-info/
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     1580 2023-06-06 08:56:26.000000 pytest-embedded-qemu-1.3.1/pytest_embedded_qemu.egg-info/PKG-INFO
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)      355 2023-06-06 08:56:26.000000 pytest-embedded-qemu-1.3.1/pytest_embedded_qemu.egg-info/SOURCES.txt
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)        1 2023-06-06 08:56:26.000000 pytest-embedded-qemu-1.3.1/pytest_embedded_qemu.egg-info/dependency_links.txt
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)       57 2023-06-06 08:56:26.000000 pytest-embedded-qemu-1.3.1/pytest_embedded_qemu.egg-info/requires.txt
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)       21 2023-06-06 08:56:26.000000 pytest-embedded-qemu-1.3.1/pytest_embedded_qemu.egg-info/top_level.txt
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)       38 2023-06-06 08:56:26.382211 pytest-embedded-qemu-1.3.1/setup.cfg
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     1885 2023-06-06 08:49:39.000000 pytest-embedded-qemu-1.3.1/setup.py
+-rw-r--r--   0        0        0     1094 2023-06-14 02:29:37.924594 pytest_embedded_qemu-1.3.2/LICENSE
+-rw-r--r--   0        0        0      552 2023-06-14 02:29:37.924594 pytest_embedded_qemu-1.3.2/README.md
+-rw-r--r--   0        0        0     2952 2023-06-14 02:29:37.924594 pytest_embedded_qemu-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      369 2023-06-14 02:29:37.924594 pytest_embedded_qemu-1.3.2/pytest_embedded_qemu/__init__.py
+-rw-r--r--   0        0        0     6294 2023-06-14 02:29:37.924594 pytest_embedded_qemu-1.3.2/pytest_embedded_qemu/app.py
+-rw-r--r--   0        0        0      414 2023-06-14 02:29:37.924594 pytest_embedded_qemu-1.3.2/pytest_embedded_qemu/dut.py
+-rw-r--r--   0        0        0     2586 2023-06-14 02:29:37.924594 pytest_embedded_qemu-1.3.2/pytest_embedded_qemu/qemu.py
+-rw-r--r--   0        0        0     3773 2023-06-14 02:29:37.924594 pytest_embedded_qemu-1.3.2/tests/test_qemu.py
+-rw-r--r--   0        0        0     1901 1970-01-01 00:00:00.000000 pytest_embedded_qemu-1.3.2/PKG-INFO
```

### Comparing `pytest-embedded-qemu-1.3.1/PKG-INFO` & `pytest_embedded_qemu-1.3.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-qemu
-Version: 1.3.1
-Summary: pytest embedded plugin for qemu, not target chip
-Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
-Author: Fu Hanxi
-Author-email: fuhanxi@espressif.com
-License: MIT
+Version: 1.3.2
+Summary: Make pytest-embedded plugin work with QEMU.
+Author-email: Fu Hanxi <fuhanxi@espressif.com>
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Testing
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Testing
+Requires-Dist: pytest-embedded~=1.3.2
+Requires-Dist: pytest-embedded-idf~=1.3.2 ; extra == "idf"
+Project-URL: changelog, https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md
+Project-URL: documentation, https://docs.espressif.com/projects/pytest-embedded/en/latest/
+Project-URL: homepage, https://github.com/espressif/pytest-embedded
+Project-URL: repository, https://github.com/espressif/pytest-embedded
 Provides-Extra: idf
 
 ### pytest-embedded-qemu
 
 pytest embedded service for running tests on QEMU instead of the real target.
 
 Extra Functionalities:
@@ -40,7 +43,8 @@
         - `dut`: duplicate the `qemu` output to `pexpect_proc`.
 
    .. group-tab:: `pytest-embedded-idf` NOT activated
 
         - `qemu`: enable the fixture
         - `dut`: duplicate the `qemu` output to `pexpect_proc`.
 ```
+
```

### Comparing `pytest-embedded-qemu-1.3.1/README.md` & `pytest_embedded_qemu-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pytest-embedded-qemu-1.3.1/pytest_embedded_qemu/qemu.py` & `pytest_embedded_qemu-1.3.2/pytest_embedded_qemu/qemu.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import os
 import shlex
-from typing import Optional
+import typing as t
 
 from pytest_embedded.log import DuplicateStdoutPopen
 
-from . import DEFAULT_IMAGE_FN, QemuApp
+from . import DEFAULT_IMAGE_FN
+
+if t.TYPE_CHECKING:
+    from .app import QemuApp
 
 
 class Qemu(DuplicateStdoutPopen):
     """
     QEMU class
     """
 
@@ -21,19 +24,19 @@
     QEMU_DEFAULT_FMT = '-nographic -machine {}'
 
     QEMU_STRAP_MODE_FMT = '-global driver=esp32.gpio,property=strap_mode,value={}'
     QEMU_SERIAL_TCP_FMT = '-serial tcp::{},server,nowait'
 
     def __init__(
         self,
-        qemu_image_path: Optional[str] = None,
-        qemu_prog_path: Optional[str] = None,
-        qemu_cli_args: Optional[str] = None,
-        qemu_extra_args: Optional[str] = None,
-        app: Optional[QemuApp] = None,
+        qemu_image_path: t.Optional[str] = None,
+        qemu_prog_path: t.Optional[str] = None,
+        qemu_cli_args: t.Optional[str] = None,
+        qemu_extra_args: t.Optional[str] = None,
+        app: t.Optional['QemuApp'] = None,
         **kwargs,
     ):
         """
         Args:
             qemu_image_path: QEMU image path
             qemu_prog_path: QEMU program path
             qemu_cli_args: QEMU CLI arguments
@@ -53,22 +56,28 @@
             cmd=[qemu_prog_path, *qemu_cli_args, *qemu_extra_args] + ['-drive', f'file={image_path},if=mtd,format=raw'],
             **kwargs,
         )
 
     @property
     def qemu_prog_name(self):
         if self.app:
-            return self.QEMU_PROG_FMT.format('xtensa' if self.app.is_xtensa else 'riscv32')
+            try:
+                return self.QEMU_PROG_FMT.format('xtensa' if self.app.is_xtensa else 'riscv32')
+            except AttributeError:
+                pass
 
         return self.QEMU_PROG_PATH
 
     @property
     def qemu_default_args(self):
         if self.app:
-            return self.QEMU_DEFAULT_FMT.format(self.app.target)
+            try:
+                return self.QEMU_DEFAULT_FMT.format(self.app.target)
+            except AttributeError:
+                pass
 
         return self.QEMU_DEFAULT_ARGS
 
     def _hard_reset(self):
         """
         This is a fake hard_reset. Keep this API to keep the consistency.
         """
```

