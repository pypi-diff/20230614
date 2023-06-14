# Comparing `tmp/pytest-embedded-idf-1.3.1.tar.gz` & `tmp/pytest_embedded_idf-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-embedded-idf-1.3.1.tar", last modified: Tue Jun  6 08:56:25 2023, max compression
+gzip compressed data, was "pytest_embedded_idf-1.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest-embedded-idf-1.3.1.tar` & `pytest_embedded_idf-1.3.2.tar`

### file list

```diff
@@ -1,18 +1,11 @@
-drwxr-xr-x   0 fuhanxi   (1000) fuhanxi   (1000)        0 2023-06-06 08:56:25.725546 pytest-embedded-idf-1.3.1/
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     1544 2023-06-06 08:56:25.725546 pytest-embedded-idf-1.3.1/PKG-INFO
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)      520 2023-06-06 08:04:34.000000 pytest-embedded-idf-1.3.1/README.md
-drwxr-xr-x   0 fuhanxi   (1000) fuhanxi   (1000)        0 2023-06-06 08:56:25.722213 pytest-embedded-idf-1.3.1/pytest_embedded_idf/
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)      598 2023-05-31 13:02:58.000000 pytest-embedded-idf-1.3.1/pytest_embedded_idf/__init__.py
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     8830 2023-06-02 06:32:41.000000 pytest-embedded-idf-1.3.1/pytest_embedded_idf/app.py
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)    11005 2023-06-06 08:04:34.000000 pytest-embedded-idf-1.3.1/pytest_embedded_idf/dut.py
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     1055 2023-06-02 06:32:41.000000 pytest-embedded-idf-1.3.1/pytest_embedded_idf/linux.py
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     9584 2023-06-02 06:32:41.000000 pytest-embedded-idf-1.3.1/pytest_embedded_idf/serial.py
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)    25144 2023-06-06 08:04:34.000000 pytest-embedded-idf-1.3.1/pytest_embedded_idf/unity_tester.py
-drwxr-xr-x   0 fuhanxi   (1000) fuhanxi   (1000)        0 2023-06-06 08:56:25.725546 pytest-embedded-idf-1.3.1/pytest_embedded_idf.egg-info/
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     1544 2023-06-06 08:56:25.000000 pytest-embedded-idf-1.3.1/pytest_embedded_idf.egg-info/PKG-INFO
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)      413 2023-06-06 08:56:25.000000 pytest-embedded-idf-1.3.1/pytest_embedded_idf.egg-info/SOURCES.txt
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)        1 2023-06-06 08:56:25.000000 pytest-embedded-idf-1.3.1/pytest_embedded_idf.egg-info/dependency_links.txt
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)       85 2023-06-06 08:56:25.000000 pytest-embedded-idf-1.3.1/pytest_embedded_idf.egg-info/requires.txt
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)       20 2023-06-06 08:56:25.000000 pytest-embedded-idf-1.3.1/pytest_embedded_idf.egg-info/top_level.txt
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)       38 2023-06-06 08:56:25.725546 pytest-embedded-idf-1.3.1/setup.cfg
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     1911 2023-06-06 08:49:39.000000 pytest-embedded-idf-1.3.1/setup.py
+-rw-r--r--   0        0        0     1094 2023-06-14 02:29:37.920594 pytest_embedded_idf-1.3.2/LICENSE
+-rw-r--r--   0        0        0      520 2023-06-14 02:29:37.920594 pytest_embedded_idf-1.3.2/README.md
+-rw-r--r--   0        0        0     2986 2023-06-14 02:29:37.920594 pytest_embedded_idf-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      675 2023-06-14 02:29:37.920594 pytest_embedded_idf-1.3.2/pytest_embedded_idf/__init__.py
+-rw-r--r--   0        0        0     9180 2023-06-14 02:29:37.920594 pytest_embedded_idf-1.3.2/pytest_embedded_idf/app.py
+-rw-r--r--   0        0        0    11005 2023-06-14 02:29:37.920594 pytest_embedded_idf-1.3.2/pytest_embedded_idf/dut.py
+-rw-r--r--   0        0        0     1055 2023-06-14 02:29:37.920594 pytest_embedded_idf-1.3.2/pytest_embedded_idf/linux.py
+-rw-r--r--   0        0        0     9581 2023-06-14 02:29:37.920594 pytest_embedded_idf-1.3.2/pytest_embedded_idf/serial.py
+-rw-r--r--   0        0        0    25160 2023-06-14 02:29:37.920594 pytest_embedded_idf-1.3.2/pytest_embedded_idf/unity_tester.py
+-rw-r--r--   0        0        0    18665 2023-06-14 02:29:37.920594 pytest_embedded_idf-1.3.2/tests/test_idf.py
+-rw-r--r--   0        0        0     1937 1970-01-01 00:00:00.000000 pytest_embedded_idf-1.3.2/PKG-INFO
```

### Comparing `pytest-embedded-idf-1.3.1/README.md` & `pytest_embedded_idf-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pytest-embedded-idf-1.3.1/pytest_embedded_idf/__init__.py` & `pytest_embedded_idf-1.3.2/pytest_embedded_idf/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Make pytest-embedded plugin work with ESP-IDF."""
+
 import importlib
 
 from pytest_embedded.utils import lazy_load
 
 from .app import IdfApp
 from .linux import LinuxDut, LinuxSerial
 from .unity_tester import CaseTester, UnittestMenuCase
@@ -26,7 +28,9 @@
     'IdfSerial',
     'IdfDut',
     'CaseTester',
     'LinuxSerial',
     'LinuxDut',
     'UnittestMenuCase',
 ]
+
+__version__ = '1.3.2'
```

### Comparing `pytest-embedded-idf-1.3.1/pytest_embedded_idf/app.py` & `pytest_embedded_idf-1.3.2/pytest_embedded_idf/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -188,30 +188,40 @@
     def _get_bin_file(self) -> Optional[str]:
         for fn in os.listdir(self.binary_path):
             if os.path.splitext(fn)[-1] == '.bin':
                 return os.path.realpath(os.path.join(self.binary_path, fn))
 
         return None
 
-    def _parse_flash_args(self) -> List[str]:
+    @property
+    def write_flash_args(self):
+        """
+        Returns:
+            list of flash args
+        """
         flash_args_filepath = None
         for fn in os.listdir(self.binary_path):
             if fn in [self.FLASH_PROJECT_ARGS_FILENAME, self.FLASH_ARGS_FILENAME]:
                 flash_args_filepath = os.path.realpath(os.path.join(self.binary_path, fn))
                 break
 
-        if not flash_args_filepath:
+        if flash_args_filepath:
+            with open(flash_args_filepath) as fr:
+                return shlex.split(fr.read().strip())
+
+        # generate it from flasher_args.json
+        if 'write_flash_args' in self.flash_args and 'flash_files' in self.flash_args:
+            return self.flash_args['write_flash_args'] + [
+                item for pair in self.flash_args['flash_files'].items() for item in pair
+            ]
+        else:
             raise ValueError(
-                f'{self.FLASH_PROJECT_ARGS_FILENAME} or {self.FLASH_ARGS_FILENAME} '
-                f'is not found under {self.binary_path}'
+                f'write_flash_args and flash_files fields are not found in {self.FLASH_ARGS_JSON_FILENAME}'
             )
 
-        with open(flash_args_filepath) as fr:
-            return shlex.split(fr.read().strip())
-
     def _parse_flash_args_json(
         self,
     ) -> Tuple[Dict[str, Any], List[FlashFile], Dict[str, str]]:
         flash_args_json_filepath = None
         for fn in os.listdir(self.binary_path):
             if fn == self.FLASH_ARGS_JSON_FILENAME:
                 flash_args_json_filepath = os.path.realpath(os.path.join(self.binary_path, fn))
```

### Comparing `pytest-embedded-idf-1.3.1/pytest_embedded_idf/dut.py` & `pytest_embedded_idf-1.3.2/pytest_embedded_idf/dut.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-idf-1.3.1/pytest_embedded_idf/linux.py` & `pytest_embedded_idf-1.3.2/pytest_embedded_idf/linux.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-idf-1.3.1/pytest_embedded_idf/serial.py` & `pytest_embedded_idf-1.3.2/pytest_embedded_idf/serial.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             live_print_call(
                 [
                     'esptool.py',
                     '--chip',
                     self.app.target,
                     'elf2image',
                     self.app.elf_file,
-                    *self.app._parse_flash_args(),
+                    *self.app.write_flash_args,
                 ],
                 msg_queue=self._q,
             )
             bin_file = self.app.elf_file.replace('.elf', '.bin')
 
         live_print_call(
             [
```

### Comparing `pytest-embedded-idf-1.3.1/pytest_embedded_idf/unity_tester.py` & `pytest_embedded_idf-1.3.2/pytest_embedded_idf/unity_tester.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,15 +318,15 @@
         else:
             self.testsuite.attrs['tests'] += 1
 
     @_record_single_unity_test_case
     def _run_normal_case(
         self,
         case: UnittestMenuCase,
-        reset: bool = False,
+        reset: bool = False,  # noqa
         timeout: float = 30,
     ) -> None:
         """
         Run a specific normal case
 
         Note:
             Will skip with a warning if the case type is not "normal"
@@ -343,15 +343,15 @@
         self.expect_exact(READY_PATTERN_LIST, timeout=timeout)
         self.confirm_write(case.index, expect_str=f'Running {case.name}...')
 
     @_record_single_unity_test_case
     def _run_multi_stage_case(
         self,
         case: UnittestMenuCase,
-        reset: bool = False,
+        reset: bool = False,  # noqa
         timeout: float = 30,
     ) -> None:
         """
         Run a specific multi_stage case
 
         Note:
             Will skip with a warning if the case type is not "multi_stage"
```

