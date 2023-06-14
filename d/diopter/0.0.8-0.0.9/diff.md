# Comparing `tmp/diopter-0.0.8.tar.gz` & `tmp/diopter-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diopter-0.0.8.tar", last modified: Tue Jan 10 11:51:25 2023, max compression
+gzip compressed data, was "diopter-0.0.9.tar", last modified: Wed Jan 11 15:52:37 2023, max compression
```

## Comparing `diopter-0.0.8.tar` & `diopter-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-01-10 11:51:25.056536 diopter-0.0.8/
--rw-r--r--   0 theo      (1000) theo      (1000)      575 2022-05-18 10:01:28.000000 diopter-0.0.8/LICENSE
--rw-r--r--   0 theo      (1000) theo      (1000)       25 2022-07-18 12:13:14.000000 diopter-0.0.8/MANIFEST.in
--rw-r--r--   0 theo      (1000) theo      (1000)      449 2023-01-10 11:51:25.056536 diopter-0.0.8/PKG-INFO
--rw-r--r--   0 theo      (1000) theo      (1000)       44 2022-07-18 12:13:14.000000 diopter-0.0.8/README.md
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-01-10 11:51:25.056536 diopter-0.0.8/diopter/
--rw-r--r--   0 theo      (1000) theo      (1000)      194 2022-12-06 15:13:04.000000 diopter-0.0.8/diopter/__init__.py
--rw-r--r--   0 theo      (1000) theo      (1000)     8905 2022-12-30 10:48:35.000000 diopter-0.0.8/diopter/bisector.py
--rw-r--r--   0 theo      (1000) theo      (1000)    29476 2023-01-10 11:50:59.000000 diopter-0.0.8/diopter/compiler.py
--rw-r--r--   0 theo      (1000) theo      (1000)     5799 2023-01-10 11:50:59.000000 diopter-0.0.8/diopter/generator.py
--rw-r--r--   0 theo      (1000) theo      (1000)     3144 2022-12-06 15:13:04.000000 diopter-0.0.8/diopter/preprocessor.py
--rw-r--r--   0 theo      (1000) theo      (1000)        0 2022-07-18 12:13:14.000000 diopter-0.0.8/diopter/py.typed
--rw-r--r--   0 theo      (1000) theo      (1000)     5034 2022-12-07 19:34:25.000000 diopter-0.0.8/diopter/reducer.py
--rw-r--r--   0 theo      (1000) theo      (1000)    13675 2022-12-06 15:13:04.000000 diopter-0.0.8/diopter/sanitizer.py
--rw-r--r--   0 theo      (1000) theo      (1000)     2589 2022-12-23 12:51:08.000000 diopter-0.0.8/diopter/utils.py
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-01-10 11:51:25.056536 diopter-0.0.8/diopter.egg-info/
--rw-r--r--   0 theo      (1000) theo      (1000)      449 2023-01-10 11:51:25.000000 diopter-0.0.8/diopter.egg-info/PKG-INFO
--rw-r--r--   0 theo      (1000) theo      (1000)      516 2023-01-10 11:51:25.000000 diopter-0.0.8/diopter.egg-info/SOURCES.txt
--rw-r--r--   0 theo      (1000) theo      (1000)        1 2023-01-10 11:51:25.000000 diopter-0.0.8/diopter.egg-info/dependency_links.txt
--rw-r--r--   0 theo      (1000) theo      (1000)       17 2023-01-10 11:51:25.000000 diopter-0.0.8/diopter.egg-info/requires.txt
--rw-r--r--   0 theo      (1000) theo      (1000)       14 2023-01-10 11:51:25.000000 diopter-0.0.8/diopter.egg-info/top_level.txt
--rw-r--r--   0 theo      (1000) theo      (1000)      196 2022-12-06 15:13:04.000000 diopter-0.0.8/pyproject.toml
--rw-r--r--   0 theo      (1000) theo      (1000)      610 2023-01-10 11:51:25.056536 diopter-0.0.8/setup.cfg
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-01-10 11:51:25.056536 diopter-0.0.8/tests/
--rw-r--r--   0 theo      (1000) theo      (1000)        0 2022-12-06 15:13:04.000000 diopter-0.0.8/tests/__init__.py
--rw-r--r--   0 theo      (1000) theo      (1000)     3150 2022-12-23 12:51:08.000000 diopter-0.0.8/tests/compilation_command_parsing_test.py
--rw-r--r--   0 theo      (1000) theo      (1000)     3722 2022-12-23 12:51:08.000000 diopter-0.0.8/tests/compiler_test.py
--rw-r--r--   0 theo      (1000) theo      (1000)      471 2022-12-06 15:13:04.000000 diopter-0.0.8/tests/reducer_test.py
--rwxr-xr-x   0 theo      (1000) theo      (1000)     1394 2022-12-06 17:15:49.000000 diopter-0.0.8/tests/sanitizer_test.py
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-01-11 15:52:37.813498 diopter-0.0.9/
+-rw-r--r--   0 theo      (1000) theo      (1000)      575 2022-05-17 12:37:35.000000 diopter-0.0.9/LICENSE
+-rw-r--r--   0 theo      (1000) theo      (1000)       25 2022-08-04 09:52:06.000000 diopter-0.0.9/MANIFEST.in
+-rw-r--r--   0 theo      (1000) theo      (1000)      449 2023-01-11 15:52:37.813498 diopter-0.0.9/PKG-INFO
+-rw-r--r--   0 theo      (1000) theo      (1000)       44 2022-08-04 09:52:06.000000 diopter-0.0.9/README.md
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-01-11 15:52:37.813498 diopter-0.0.9/diopter/
+-rw-r--r--   0 theo      (1000) theo      (1000)      194 2022-12-02 08:53:24.000000 diopter-0.0.9/diopter/__init__.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     8905 2022-12-02 08:53:24.000000 diopter-0.0.9/diopter/bisector.py
+-rw-r--r--   0 theo      (1000) theo      (1000)    29476 2023-01-11 15:50:47.000000 diopter-0.0.9/diopter/compiler.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     5799 2023-01-11 15:50:47.000000 diopter-0.0.9/diopter/generator.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     3144 2022-12-02 08:53:24.000000 diopter-0.0.9/diopter/preprocessor.py
+-rw-r--r--   0 theo      (1000) theo      (1000)        0 2022-08-04 09:52:06.000000 diopter-0.0.9/diopter/py.typed
+-rw-r--r--   0 theo      (1000) theo      (1000)     7796 2023-01-11 15:50:47.000000 diopter-0.0.9/diopter/reducer.py
+-rw-r--r--   0 theo      (1000) theo      (1000)    13871 2023-01-11 15:50:47.000000 diopter-0.0.9/diopter/sanitizer.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     2589 2022-12-09 11:01:55.000000 diopter-0.0.9/diopter/utils.py
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-01-11 15:52:37.813498 diopter-0.0.9/diopter.egg-info/
+-rw-r--r--   0 theo      (1000) theo      (1000)      449 2023-01-11 15:52:37.000000 diopter-0.0.9/diopter.egg-info/PKG-INFO
+-rw-r--r--   0 theo      (1000) theo      (1000)      516 2023-01-11 15:52:37.000000 diopter-0.0.9/diopter.egg-info/SOURCES.txt
+-rw-r--r--   0 theo      (1000) theo      (1000)        1 2023-01-11 15:52:37.000000 diopter-0.0.9/diopter.egg-info/dependency_links.txt
+-rw-r--r--   0 theo      (1000) theo      (1000)       17 2023-01-11 15:52:37.000000 diopter-0.0.9/diopter.egg-info/requires.txt
+-rw-r--r--   0 theo      (1000) theo      (1000)       14 2023-01-11 15:52:37.000000 diopter-0.0.9/diopter.egg-info/top_level.txt
+-rw-r--r--   0 theo      (1000) theo      (1000)      196 2022-12-02 08:53:24.000000 diopter-0.0.9/pyproject.toml
+-rw-r--r--   0 theo      (1000) theo      (1000)      610 2023-01-11 15:52:37.813498 diopter-0.0.9/setup.cfg
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-01-11 15:52:37.813498 diopter-0.0.9/tests/
+-rw-r--r--   0 theo      (1000) theo      (1000)        0 2022-12-02 08:53:24.000000 diopter-0.0.9/tests/__init__.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     3150 2022-12-09 11:01:55.000000 diopter-0.0.9/tests/compilation_command_parsing_test.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     3722 2023-01-11 15:50:47.000000 diopter-0.0.9/tests/compiler_test.py
+-rw-r--r--   0 theo      (1000) theo      (1000)      605 2023-01-11 15:50:47.000000 diopter-0.0.9/tests/reducer_test.py
+-rwxr-xr-x   0 theo      (1000) theo      (1000)     1394 2022-12-09 09:19:22.000000 diopter-0.0.9/tests/sanitizer_test.py
```

### Comparing `diopter-0.0.8/LICENSE` & `diopter-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `diopter-0.0.8/diopter/bisector.py` & `diopter-0.0.9/diopter/bisector.py`

 * *Files identical despite different names*

### Comparing `diopter-0.0.8/diopter/compiler.py` & `diopter-0.0.9/diopter/compiler.py`

 * *Files identical despite different names*

### Comparing `diopter-0.0.8/diopter/generator.py` & `diopter-0.0.9/diopter/generator.py`

 * *Files identical despite different names*

### Comparing `diopter-0.0.8/diopter/preprocessor.py` & `diopter-0.0.9/diopter/preprocessor.py`

 * *Files identical despite different names*

### Comparing `diopter-0.0.8/diopter/sanitizer.py` & `diopter-0.0.9/diopter/sanitizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,16 +76,18 @@
             clang used for checking compiler warnings and ub/address sanitizers result
         ccomp (Optional[CComp]):
             CompCert used for validating the program
         checked_warnings (Optional[tuple[str,...]]):
             the warnings whose presence to check
         use_ub_address_sanitizer (bool):
             whether Sanitizer.sanitize should use clang's ub and address sanitizers
-        check_warnings_and_sanitizer_opt_level (OptLevel):
-            optimization level used when checking for warnings and running sanitizers
+        check_warnings_opt_level (OptLevel):
+            optimization level used when checking for warnings
+        sanitizer_opt_level (OptLevel):
+            optimization level used when running sanitizers
         compilation_timeout (int):
             seconds to wait before aborting when compiling the program
         execution_timeout (int):
             seconds to wait before aborting when executing the program (ub/asan)
         ccomp_timeout  (int):
             seconds to wait before aborting when interpreting the program with ccomp
     """
@@ -124,26 +126,28 @@
         "pointer from integer",
         "incompatible implicit",
         "excess elements in struct initializer",
         "comparison between pointer and integer",
         "return type of ‘main’ is not ‘int’",
         "past the end of the array",
         "no return statement in function returning non-void",
+        "undefined behavior",
     )
 
     def __init__(
         self,
         *,
         check_warnings: bool = True,
         use_ub_address_sanitizer: bool = True,
         use_ccomp_if_available: bool = True,
         gcc: Optional[CompilerExe] = None,
         clang: Optional[CompilerExe] = None,
         ccomp: Optional[CComp] = None,
-        check_warnings_and_sanitizer_opt_level: OptLevel = OptLevel.O3,
+        check_warnings_opt_level: OptLevel = OptLevel.O3,
+        sanitizer_opt_level: OptLevel = OptLevel.O0,
         checked_warnings: Optional[tuple[str, ...]] = None,
         compilation_timeout: int = 8,
         execution_timeout: int = 4,
         ccomp_timeout: int = 16,
     ):
         """
         Args:
@@ -159,17 +163,20 @@
                 CompilerExe.get_system_gcc will be used
             clang (Optional[CompilerExe]):
                 the clang executable to use, if not provided
                 CompilerExe.get_system_clang will be used
             ccomp (Optional[CComp]:
                 the ccomp executable to use, if not provided and use_ccomp
                 is True CComp.get_system_ccomp will be used if available
-            check_warnings_and_sanitizer_opt_level (OptLevel):
-                which optimization level to use when checking for compiler
-                warnings and ub/address sanitizer issues
+            check_warnings_opt_level (OptLevel):
+                which optimization level to use when checking
+                for compiler warnings
+            sanitizer_opt_level (OptLevel):
+                which optimization level to use when checking
+                for ub/address sanitizer issues
             checked_warnings (Optional[tuple[str,...]]):
                 if not None implies check_warnings = True and will
                 be used instead of Sanitizer.default_warnings
             compilation_timeout (int):
                 after how many seconds to abort a compilation and fail
             execution_timeout (int):
                 after how many seconds to abort an execution and fail
@@ -183,17 +190,16 @@
         if use_ccomp_if_available and not self.ccomp:
             self.ccomp = CComp.get_system_ccomp()
         if checked_warnings:
             self.checked_warnings = checked_warnings
         elif check_warnings:
             self.checked_warnings = Sanitizer.default_warnings
         self.use_ub_address_sanitizer = use_ub_address_sanitizer
-        self.check_warnings_and_sanitizer_opt_level = (
-            check_warnings_and_sanitizer_opt_level
-        )
+        self.check_warnings_opt_level = check_warnings_opt_level
+        self.sanitizer_opt_level = sanitizer_opt_level
         self.compilation_timeout = compilation_timeout
         self.execution_timeout = execution_timeout
         self.ccomp_timeout = ccomp_timeout
 
     def check_for_compiler_warnings(self, program: SourceProgram) -> SanitizationResult:
         """Checks the program for compiler warnings.
 
@@ -234,24 +240,24 @@
             return SanitizationResult()
 
         with TempDirEnv():
             if not (
                 gcc_result := check_warnings_impl(
                     CompilationSetting(
                         compiler=self.gcc,
-                        opt_level=self.check_warnings_and_sanitizer_opt_level,
+                        opt_level=self.check_warnings_opt_level,
                     )
                 )
             ):
                 return gcc_result
             if not (
                 clang_result := check_warnings_impl(
                     CompilationSetting(
                         compiler=self.clang,
-                        opt_level=self.check_warnings_and_sanitizer_opt_level,
+                        opt_level=self.check_warnings_opt_level,
                     )
                 )
             ):
                 return clang_result
 
         return SanitizationResult()
 
@@ -277,15 +283,15 @@
             exe = tempfile.NamedTemporaryFile(suffix=".exe", delete=False)
             exe.close()
             os.chmod(exe.name, 0o777)
             # Compile program with -fsanitize=...
             try:
                 CompilationSetting(
                     compiler=self.clang,
-                    opt_level=self.check_warnings_and_sanitizer_opt_level,
+                    opt_level=self.sanitizer_opt_level,
                 ).compile_program_to_executable(
                     program,
                     Path(exe.name),
                     (
                         "-Wall",
                         "-Wextra",
                         "-Wpedantic",
```

### Comparing `diopter-0.0.8/diopter/utils.py` & `diopter-0.0.9/diopter/utils.py`

 * *Files identical despite different names*

### Comparing `diopter-0.0.8/diopter.egg-info/SOURCES.txt` & `diopter-0.0.9/diopter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diopter-0.0.8/setup.cfg` & `diopter-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = diopter
-version = 0.0.8
+version = 0.0.9
 author = Theodoros Theodoridis, Yann Girsberger
 author_email = theodort@inf.ethz.ch
 description = A library for building differential tests
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache License 2.0
 url = https://github.com/DeadCodeProductions/diopter
```

### Comparing `diopter-0.0.8/tests/compilation_command_parsing_test.py` & `diopter-0.0.9/tests/compilation_command_parsing_test.py`

 * *Files identical despite different names*

### Comparing `diopter-0.0.8/tests/compiler_test.py` & `diopter-0.0.9/tests/compiler_test.py`

 * *Files identical despite different names*

### Comparing `diopter-0.0.8/tests/sanitizer_test.py` & `diopter-0.0.9/tests/sanitizer_test.py`

 * *Files identical despite different names*

