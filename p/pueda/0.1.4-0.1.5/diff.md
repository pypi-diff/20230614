# Comparing `tmp/pueda-0.1.4.tar.gz` & `tmp/pueda-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pueda-0.1.4.tar", last modified: Tue Jun 13 22:11:45 2023, max compression
+gzip compressed data, was "pueda-0.1.5.tar", last modified: Wed Jun 14 20:15:21 2023, max compression
```

## Comparing `pueda-0.1.4.tar` & `pueda-0.1.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-13 22:11:45.014708 pueda-0.1.4/
--rwxrwxrwx   0 marco     (1000) marco     (1000)    11357 2022-12-10 01:01:26.000000 pueda-0.1.4/LICENSE
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2267 2023-06-13 22:11:45.015048 pueda-0.1.4/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1923 2023-02-27 23:28:27.000000 pueda-0.1.4/README.md
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-13 22:11:44.973543 pueda-0.1.4/data/
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-13 22:11:44.974622 pueda-0.1.4/data/icarus/
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-13 22:11:44.985142 pueda-0.1.4/data/icarus/inc/
--rwxrwxrwx   0 marco     (1000) marco     (1000)       88 2023-02-26 23:04:23.000000 pueda-0.1.4/data/icarus/inc/dump.vh
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-13 22:11:44.987107 pueda-0.1.4/data/icarus/src/
--rwxrwxrwx   0 marco     (1000) marco     (1000)      296 2023-02-26 23:04:23.000000 pueda-0.1.4/data/icarus/src/dump.v
--rwxrwxrwx   0 marco     (1000) marco     (1000)      103 2023-06-13 22:11:45.016189 pueda-0.1.4/setup.cfg
--rwxrwxrwx   0 marco     (1000) marco     (1000)      963 2023-06-13 22:08:10.000000 pueda-0.1.4/setup.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-13 22:11:44.976151 pueda-0.1.4/src/
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-13 22:11:45.002618 pueda-0.1.4/src/pueda/
--rwxrwxrwx   0 marco     (1000) marco     (1000)      150 2023-03-15 01:01:16.000000 pueda-0.1.4/src/pueda/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3092 2023-03-15 01:37:00.000000 pueda-0.1.4/src/pueda/common.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     7433 2023-03-26 15:13:03.000000 pueda-0.1.4/src/pueda/edalize.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      866 2023-02-27 22:13:51.000000 pueda-0.1.4/src/pueda/gtkw.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2924 2023-03-15 02:15:01.000000 pueda-0.1.4/src/pueda/icarus.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     4934 2023-03-15 01:37:22.000000 pueda-0.1.4/src/pueda/myhdl.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1709 2023-06-13 22:07:38.000000 pueda-0.1.4/src/pueda/pyverilator.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1688 2023-03-15 01:49:00.000000 pueda-0.1.4/src/pueda/vcd.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      325 2023-01-22 17:37:49.000000 pueda-0.1.4/src/pueda/veriloggen.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1376 2023-02-28 20:52:57.000000 pueda-0.1.4/src/pueda/yosys.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-13 22:11:45.009014 pueda-0.1.4/src/pueda.egg-info/
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2267 2023-06-13 22:11:44.000000 pueda-0.1.4/src/pueda.egg-info/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)      558 2023-06-13 22:11:44.000000 pueda-0.1.4/src/pueda.egg-info/SOURCES.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2023-06-13 22:11:44.000000 pueda-0.1.4/src/pueda.egg-info/dependency_links.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)       69 2023-06-13 22:11:44.000000 pueda-0.1.4/src/pueda.egg-info/requires.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)        6 2023-06-13 22:11:44.000000 pueda-0.1.4/src/pueda.egg-info/top_level.txt
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-13 22:11:45.013587 pueda-0.1.4/test/
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1370 2023-06-13 22:10:13.000000 pueda-0.1.4/test/test.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1162 2023-02-27 20:41:20.000000 pueda-0.1.4/test/test_myhdl_counter.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      463 2023-02-27 20:41:20.000000 pueda-0.1.4/test/test_verilated_dpi_counter.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      454 2023-02-27 20:41:20.000000 pueda-0.1.4/test/test_verilator_counter.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-14 20:15:21.824193 pueda-0.1.5/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)    11357 2022-12-10 01:01:26.000000 pueda-0.1.5/LICENSE
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2267 2023-06-14 20:15:21.824432 pueda-0.1.5/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1923 2023-02-27 23:28:27.000000 pueda-0.1.5/README.md
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-14 20:15:21.759828 pueda-0.1.5/data/
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-14 20:15:21.761004 pueda-0.1.5/data/icarus/
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-14 20:15:21.771894 pueda-0.1.5/data/icarus/inc/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       88 2023-02-26 23:04:23.000000 pueda-0.1.5/data/icarus/inc/dump.vh
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-14 20:15:21.774094 pueda-0.1.5/data/icarus/src/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      296 2023-02-26 23:04:23.000000 pueda-0.1.5/data/icarus/src/dump.v
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      103 2023-06-14 20:15:21.825369 pueda-0.1.5/setup.cfg
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      963 2023-06-14 20:12:57.000000 pueda-0.1.5/setup.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-14 20:15:21.762571 pueda-0.1.5/src/
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-14 20:15:21.812516 pueda-0.1.5/src/pueda/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      150 2023-03-15 01:01:16.000000 pueda-0.1.5/src/pueda/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3092 2023-03-15 01:37:00.000000 pueda-0.1.5/src/pueda/common.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     7433 2023-03-26 15:13:03.000000 pueda-0.1.5/src/pueda/edalize.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      866 2023-02-27 22:13:51.000000 pueda-0.1.5/src/pueda/gtkw.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2924 2023-03-15 02:15:01.000000 pueda-0.1.5/src/pueda/icarus.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     4934 2023-03-15 01:37:22.000000 pueda-0.1.5/src/pueda/myhdl.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1795 2023-06-14 20:12:34.000000 pueda-0.1.5/src/pueda/pyverilator.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1688 2023-03-15 01:49:00.000000 pueda-0.1.5/src/pueda/vcd.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      325 2023-01-22 17:37:49.000000 pueda-0.1.5/src/pueda/veriloggen.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1376 2023-02-28 20:52:57.000000 pueda-0.1.5/src/pueda/yosys.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-14 20:15:21.819027 pueda-0.1.5/src/pueda.egg-info/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2267 2023-06-14 20:15:21.000000 pueda-0.1.5/src/pueda.egg-info/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      558 2023-06-14 20:15:21.000000 pueda-0.1.5/src/pueda.egg-info/SOURCES.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2023-06-14 20:15:21.000000 pueda-0.1.5/src/pueda.egg-info/dependency_links.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       69 2023-06-14 20:15:21.000000 pueda-0.1.5/src/pueda.egg-info/requires.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        6 2023-06-14 20:15:21.000000 pueda-0.1.5/src/pueda.egg-info/top_level.txt
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-14 20:15:21.823204 pueda-0.1.5/test/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1384 2023-06-14 20:13:34.000000 pueda-0.1.5/test/test.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1162 2023-02-27 20:41:20.000000 pueda-0.1.5/test/test_myhdl_counter.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      463 2023-02-27 20:41:20.000000 pueda-0.1.5/test/test_verilated_dpi_counter.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      454 2023-02-27 20:41:20.000000 pueda-0.1.5/test/test_verilator_counter.py
```

### Comparing `pueda-0.1.4/LICENSE` & `pueda-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pueda-0.1.4/PKG-INFO` & `pueda-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pueda
-Version: 0.1.4
+Version: 0.1.5
 Summary: Collection of python for micro-Electronic Design Automation
 Home-page: https://github.com/bat52/pueda
 Author: Marco Merlin
 Author-email: marcomerli@gmail.com
 License: Apache 2.0
 Keywords: python EDA CAD
 Platform: UNKNOWN
```

### Comparing `pueda-0.1.4/README.md` & `pueda-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pueda-0.1.4/setup.py` & `pueda-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     for d, folders, files in os.walk(datadir)]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pueda',
-    version='0.1.4',
+    version='0.1.5',
     license='Apache 2.0',
     author="Marco Merlin",
     author_email='marcomerli@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     description="Collection of python for micro-Electronic Design Automation",
     long_description=long_description,
```

### Comparing `pueda-0.1.4/src/pueda/common.py` & `pueda-0.1.5/src/pueda/common.py`

 * *Files identical despite different names*

### Comparing `pueda-0.1.4/src/pueda/edalize.py` & `pueda-0.1.5/src/pueda/edalize.py`

 * *Files identical despite different names*

### Comparing `pueda-0.1.4/src/pueda/gtkw.py` & `pueda-0.1.5/src/pueda/gtkw.py`

 * *Files identical despite different names*

### Comparing `pueda-0.1.4/src/pueda/icarus.py` & `pueda-0.1.5/src/pueda/icarus.py`

 * *Files identical despite different names*

### Comparing `pueda-0.1.4/src/pueda/myhdl.py` & `pueda-0.1.5/src/pueda/myhdl.py`

 * *Files identical despite different names*

### Comparing `pueda-0.1.4/src/pueda/pyverilator.py` & `pueda-0.1.5/src/pueda/pyverilator.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pueda.vcd import vcd_view
 
 class pyverilator_wrapper(object):
     sim = None
     dump_filename = ''
 
     def __init__(self, fname='', src_dirs=[], command_args = [],
-                 dump_en = False, dump_fst = False, dump_filename = 'dump'):
+                 dump_en = False, dump_fst = False, dump_filename = 'dump', dump_level=0):
 
         # rename to .v, if .sv
         if not os.path.isfile(fname):
             assert False, f'File {fname} does not exist!'
 
         base,ext = os.path.splitext(fname)
         # print(ext)
@@ -26,15 +26,16 @@
         else:
             ofname = fname
         print(ofname)
 
         self.sim = pyverilator.PyVerilator.build(ofname,
                                                  verilog_path=src_dirs,
                                                  args=command_args,
-                                                 dump_fst=dump_fst)
+                                                 dump_fst=dump_fst,
+                                                 dump_level=dump_level)
         if dump_en:
             if dump_fst:
                 dump_ext = '.fst'
             else:
                 dump_ext = '.vcd'
             self.dump_filename = dump_filename + dump_ext
             # start gtkwave to view the waveforms as they are made
```

### Comparing `pueda-0.1.4/src/pueda/vcd.py` & `pueda-0.1.5/src/pueda/vcd.py`

 * *Files identical despite different names*

### Comparing `pueda-0.1.4/src/pueda/yosys.py` & `pueda-0.1.5/src/pueda/yosys.py`

 * *Files identical despite different names*

### Comparing `pueda-0.1.4/src/pueda.egg-info/PKG-INFO` & `pueda-0.1.5/src/pueda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pueda
-Version: 0.1.4
+Version: 0.1.5
 Summary: Collection of python for micro-Electronic Design Automation
 Home-page: https://github.com/bat52/pueda
 Author: Marco Merlin
 Author-email: marcomerli@gmail.com
 License: Apache 2.0
 Keywords: python EDA CAD
 Platform: UNKNOWN
```

### Comparing `pueda-0.1.4/src/pueda.egg-info/SOURCES.txt` & `pueda-0.1.5/src/pueda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pueda-0.1.4/test/test.py` & `pueda-0.1.5/test/test.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def test_edalize_icarus_counter(self):
        from pueda.edalize import icarus
        icarus(simname='counter', top='counter_tb', src_dirs = ['./counter/rtl','./counter/tb'], iverilog_options=['-g2005-sv'])
        # self.assertEqual('foo'.upper(), 'FOO')
 
     def test_pyverilator_counter(self):
         from pueda.pyverilator import pyverilator_wrapper
-        pv = pyverilator_wrapper(fname='./counter/rtl/counter.v', src_dirs=['./counter/rtl'], command_args = [], dump_en = True)
+        pv = pyverilator_wrapper(fname='./counter/rtl/counter.v', src_dirs=['./counter/rtl'], command_args = [], dump_en = True, dump_level=1)
 
         for _ in range(16):
             pv.sim.clock.tick()
             print('count = %d' % pv.sim.io.count)
         assert pv.sim.io.count == 0
         # pv.view_waves() this may hold the test, so skip it
```

### Comparing `pueda-0.1.4/test/test_myhdl_counter.py` & `pueda-0.1.5/test/test_myhdl_counter.py`

 * *Files identical despite different names*

