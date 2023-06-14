# Comparing `tmp/pyverilator-mm-0.7.3.tar.gz` & `tmp/pyverilator-mm-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyverilator-mm-0.7.3.tar", last modified: Tue Jun 13 21:58:52 2023, max compression
+gzip compressed data, was "pyverilator-mm-0.7.5.tar", last modified: Wed Jun 14 20:08:51 2023, max compression
```

## Comparing `pyverilator-mm-0.7.3.tar` & `pyverilator-mm-0.7.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-13 21:58:52.804522 pyverilator-mm-0.7.3/
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1086 2022-12-26 22:28:03.000000 pyverilator-mm-0.7.3/LICENSE.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)     4464 2023-06-13 21:58:52.801864 pyverilator-mm-0.7.3/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3670 2023-06-13 21:11:02.000000 pyverilator-mm-0.7.3/README.rst
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-13 21:58:52.787312 pyverilator-mm-0.7.3/pyverilator/
--rwxrwxrwx   0 marco     (1000) marco     (1000)      128 2022-12-26 22:28:03.000000 pyverilator-mm-0.7.3/pyverilator/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      435 2022-12-26 22:28:03.000000 pyverilator-mm-0.7.3/pyverilator/__main__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)    38157 2023-06-13 21:55:20.000000 pyverilator-mm-0.7.3/pyverilator/pyverilator.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      565 2023-05-23 21:21:28.000000 pyverilator-mm-0.7.3/pyverilator/verilator_tools.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     6892 2023-06-13 19:27:06.000000 pyverilator-mm-0.7.3/pyverilator/verilatorcpp.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-13 21:58:52.799456 pyverilator-mm-0.7.3/pyverilator_mm.egg-info/
--rwxrwxrwx   0 marco     (1000) marco     (1000)     4464 2023-06-13 21:58:52.000000 pyverilator-mm-0.7.3/pyverilator_mm.egg-info/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)      317 2023-06-13 21:58:52.000000 pyverilator-mm-0.7.3/pyverilator_mm.egg-info/SOURCES.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2023-06-13 21:58:52.000000 pyverilator-mm-0.7.3/pyverilator_mm.egg-info/dependency_links.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)       12 2023-06-13 21:58:52.000000 pyverilator-mm-0.7.3/pyverilator_mm.egg-info/top_level.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)       38 2023-06-13 21:58:52.805096 pyverilator-mm-0.7.3/setup.cfg
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1556 2023-06-13 21:57:41.000000 pyverilator-mm-0.7.3/setup.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-14 20:08:51.078061 pyverilator-mm-0.7.5/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1086 2022-12-26 22:28:03.000000 pyverilator-mm-0.7.5/LICENSE.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     4464 2023-06-14 20:08:51.076321 pyverilator-mm-0.7.5/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3670 2023-06-13 21:11:02.000000 pyverilator-mm-0.7.5/README.rst
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-14 20:08:51.069603 pyverilator-mm-0.7.5/pyverilator/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      128 2022-12-26 22:28:03.000000 pyverilator-mm-0.7.5/pyverilator/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      435 2022-12-26 22:28:03.000000 pyverilator-mm-0.7.5/pyverilator/__main__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)    38303 2023-06-14 20:06:33.000000 pyverilator-mm-0.7.5/pyverilator/pyverilator.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      565 2023-05-23 21:21:28.000000 pyverilator-mm-0.7.5/pyverilator/verilator_tools.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     6893 2023-06-14 07:21:06.000000 pyverilator-mm-0.7.5/pyverilator/verilatorcpp.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-14 20:08:51.075193 pyverilator-mm-0.7.5/pyverilator_mm.egg-info/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     4464 2023-06-14 20:08:51.000000 pyverilator-mm-0.7.5/pyverilator_mm.egg-info/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      317 2023-06-14 20:08:51.000000 pyverilator-mm-0.7.5/pyverilator_mm.egg-info/SOURCES.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2023-06-14 20:08:51.000000 pyverilator-mm-0.7.5/pyverilator_mm.egg-info/dependency_links.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       12 2023-06-14 20:08:51.000000 pyverilator-mm-0.7.5/pyverilator_mm.egg-info/top_level.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       38 2023-06-14 20:08:51.078442 pyverilator-mm-0.7.5/setup.cfg
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1556 2023-06-14 20:07:23.000000 pyverilator-mm-0.7.5/setup.py
```

### Comparing `pyverilator-mm-0.7.3/LICENSE.txt` & `pyverilator-mm-0.7.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyverilator-mm-0.7.3/PKG-INFO` & `pyverilator-mm-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyverilator-mm
-Version: 0.7.3
+Version: 0.7.5
 Summary: Python interface to Verilator models
 Home-page: https://github.com/bat52/pyverilator
 Author: CSAIL CSG, Marco Merlin
 Author-email: acwright@mit.edu, bthom@mit.edu
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bat52/pyverilator/issues
 Project-URL: Source, https://github.com/bat52/pyverilator
```

### Comparing `pyverilator-mm-0.7.3/README.rst` & `pyverilator-mm-0.7.5/README.rst`

 * *Files identical despite different names*

### Comparing `pyverilator-mm-0.7.3/pyverilator/pyverilator.py` & `pyverilator-mm-0.7.5/pyverilator/pyverilator.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,15 +366,16 @@
 
     default_vcd_filename = 'gtkwave.vcd'
 
     @classmethod
     def build(cls, top_verilog_file, preceding_files='', verilog_path = [],
             build_dir = 'obj_dir',
             json_data = None, gen_only = False, quiet=False,
-            command_args=(), verilog_defines=(), args=[], cargs='', dump_fst = False,
+            command_args=(), verilog_defines=(), args=[], cargs='', 
+            dump_en = True, dump_fst = False, dump_level=0
         ):
         """Build an object file from verilog and load it into python.
 
         Creates a folder build_dir in which it puts all the files necessary to create
         a model of top_verilog_file using verilator and the C compiler. All the files are created in build_dir.
 
         If the project is made of more than one verilog file, all the files used by the top_verilog_file will be searched
@@ -425,30 +426,33 @@
         # Old versions of Verilator are interpreted as a perl script by the shell,
         # while more recent versions are interpreted as a bash script that calls perl on itself
         which_verilator = shutil.which('verilator')
         if which_verilator is None:
             raise Exception("'verilator' executable not found")
         verilog_defines = ["+define+" + x for x in verilog_defines]
         cflags = '-fPIC -shared --std=c++11 -DVL_USER_FINISH ' + cargs
-        if dump_fst:
-            cflags += '-DDUMP_FST'
+        
+        if dump_en:
+            cflags += ' -DDUMP_LEVEL=%d' % dump_level
+            if dump_fst:
+                cflags += ' -DDUMP_FST'
 
         vargs = ['-CFLAGS',
                 cflags,
                 '--trace', # tracing (--trace) is required in order to see internal signals
                 '--cc',
                 preceding_files,
                 top_verilog_file,
                 # '--top',
                 # verilog_module_name,
                 '--exe',
                 verilator_cpp_wrapper_path,
                 ]
 
-        if dump_fst:
+        if dump_en and dump_fst:
             vargs += ['--trace-fst'] # allow fst saving that is faster
 
         verilator_args = ['perl', which_verilator, '-Wno-fatal', '-Mdir', build_dir] \
                          + args \
                          + verilog_path_args \
                          + verilog_defines \
                          + vargs
```

### Comparing `pyverilator-mm-0.7.3/pyverilator/verilator_tools.py` & `pyverilator-mm-0.7.5/pyverilator/verilator_tools.py`

 * *Files identical despite different names*

### Comparing `pyverilator-mm-0.7.3/pyverilator/verilatorcpp.py` & `pyverilator-mm-0.7.5/pyverilator/verilatorcpp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pyverilator.verilator_tools import verilator_flushcall_ok
 
 def header_cpp(top_module):
     return f"""#include <cstddef>
     #include "verilated.h"
     #if VM_TRACE
-        #ifndef DUMPLEVEL
+        #ifndef DUMP_LEVEL
             #define DUMP_LEVEL 0
         #endif
         #ifdef DUMP_FST
             #include <verilated_fst_c.h>
             #define DUMP_TYPE VerilatedFstC
             // #define DUMP_FILE "dump.fst"
         #else
```

### Comparing `pyverilator-mm-0.7.3/pyverilator_mm.egg-info/PKG-INFO` & `pyverilator-mm-0.7.5/pyverilator_mm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyverilator-mm
-Version: 0.7.3
+Version: 0.7.5
 Summary: Python interface to Verilator models
 Home-page: https://github.com/bat52/pyverilator
 Author: CSAIL CSG, Marco Merlin
 Author-email: acwright@mit.edu, bthom@mit.edu
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bat52/pyverilator/issues
 Project-URL: Source, https://github.com/bat52/pyverilator
```

### Comparing `pyverilator-mm-0.7.3/setup.py` & `pyverilator-mm-0.7.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pyverilator-mm',
-    version='0.7.3',
+    version='0.7.5',
     description='Python interface to Verilator models',
     long_description=long_description,
     url='https://github.com/bat52/pyverilator',
     author='CSAIL CSG, Marco Merlin',
     author_email='acwright@mit.edu, bthom@mit.edu',
     # https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
```

