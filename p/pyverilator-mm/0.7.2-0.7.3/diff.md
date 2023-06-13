# Comparing `tmp/pyverilator-mm-0.7.2.tar.gz` & `tmp/pyverilator-mm-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyverilator-mm-0.7.2.tar", last modified: Tue Jun 13 21:00:08 2023, max compression
+gzip compressed data, was "pyverilator-mm-0.7.3.tar", last modified: Tue Jun 13 21:58:52 2023, max compression
```

## Comparing `pyverilator-mm-0.7.2.tar` & `pyverilator-mm-0.7.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-13 21:00:08.050223 pyverilator-mm-0.7.2/
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1086 2022-12-26 22:28:03.000000 pyverilator-mm-0.7.2/LICENSE.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)     4419 2023-06-13 21:00:08.049692 pyverilator-mm-0.7.2/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3625 2023-05-24 20:52:32.000000 pyverilator-mm-0.7.2/README.rst
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-13 21:00:08.041449 pyverilator-mm-0.7.2/pyverilator/
--rwxrwxrwx   0 marco     (1000) marco     (1000)      128 2022-12-26 22:28:03.000000 pyverilator-mm-0.7.2/pyverilator/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      435 2022-12-26 22:28:03.000000 pyverilator-mm-0.7.2/pyverilator/__main__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)    38127 2023-06-13 20:41:33.000000 pyverilator-mm-0.7.2/pyverilator/pyverilator.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      565 2023-05-23 21:21:28.000000 pyverilator-mm-0.7.2/pyverilator/verilator_tools.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     6892 2023-06-13 19:27:06.000000 pyverilator-mm-0.7.2/pyverilator/verilatorcpp.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-13 21:00:08.045807 pyverilator-mm-0.7.2/pyverilator_mm.egg-info/
--rwxrwxrwx   0 marco     (1000) marco     (1000)     4419 2023-06-13 21:00:07.000000 pyverilator-mm-0.7.2/pyverilator_mm.egg-info/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)      317 2023-06-13 21:00:07.000000 pyverilator-mm-0.7.2/pyverilator_mm.egg-info/SOURCES.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2023-06-13 21:00:07.000000 pyverilator-mm-0.7.2/pyverilator_mm.egg-info/dependency_links.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)       12 2023-06-13 21:00:07.000000 pyverilator-mm-0.7.2/pyverilator_mm.egg-info/top_level.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)       38 2023-06-13 21:00:08.050411 pyverilator-mm-0.7.2/setup.cfg
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1556 2023-06-13 20:56:38.000000 pyverilator-mm-0.7.2/setup.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-13 21:58:52.804522 pyverilator-mm-0.7.3/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1086 2022-12-26 22:28:03.000000 pyverilator-mm-0.7.3/LICENSE.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     4464 2023-06-13 21:58:52.801864 pyverilator-mm-0.7.3/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3670 2023-06-13 21:11:02.000000 pyverilator-mm-0.7.3/README.rst
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-13 21:58:52.787312 pyverilator-mm-0.7.3/pyverilator/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      128 2022-12-26 22:28:03.000000 pyverilator-mm-0.7.3/pyverilator/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      435 2022-12-26 22:28:03.000000 pyverilator-mm-0.7.3/pyverilator/__main__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)    38157 2023-06-13 21:55:20.000000 pyverilator-mm-0.7.3/pyverilator/pyverilator.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      565 2023-05-23 21:21:28.000000 pyverilator-mm-0.7.3/pyverilator/verilator_tools.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     6892 2023-06-13 19:27:06.000000 pyverilator-mm-0.7.3/pyverilator/verilatorcpp.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-13 21:58:52.799456 pyverilator-mm-0.7.3/pyverilator_mm.egg-info/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     4464 2023-06-13 21:58:52.000000 pyverilator-mm-0.7.3/pyverilator_mm.egg-info/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      317 2023-06-13 21:58:52.000000 pyverilator-mm-0.7.3/pyverilator_mm.egg-info/SOURCES.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2023-06-13 21:58:52.000000 pyverilator-mm-0.7.3/pyverilator_mm.egg-info/dependency_links.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       12 2023-06-13 21:58:52.000000 pyverilator-mm-0.7.3/pyverilator_mm.egg-info/top_level.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       38 2023-06-13 21:58:52.805096 pyverilator-mm-0.7.3/setup.cfg
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1556 2023-06-13 21:57:41.000000 pyverilator-mm-0.7.3/setup.py
```

### Comparing `pyverilator-mm-0.7.2/LICENSE.txt` & `pyverilator-mm-0.7.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyverilator-mm-0.7.2/PKG-INFO` & `pyverilator-mm-0.7.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyverilator-mm
-Version: 0.7.2
+Version: 0.7.3
 Summary: Python interface to Verilator models
 Home-page: https://github.com/bat52/pyverilator
 Author: CSAIL CSG, Marco Merlin
 Author-email: acwright@mit.edu, bthom@mit.edu
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bat52/pyverilator/issues
 Project-URL: Source, https://github.com/bat52/pyverilator
@@ -64,33 +64,33 @@
         wire [7:0] next_count_reg;
         assign next_count_reg = (en == 1) ? count_reg + 1 : count_reg;
         assign out = next_count_reg;
         always @(posedge clk) begin
             if (rst == 1) count_reg <= 0;
             else          count_reg <= next_count_reg;
         end
-    endmodule'''
+    endmodule
 
 Then you can use ``pyverilator`` to simulate this module using verilator in
 python.
 
 .. code:: python
 
     sim = pyverilator.PyVerilator.build('counter.v')
 
     # start gtkwave to view the waveforms as they are made
     sim.start_gtkwave()
 
     # add all the io and internal signals to gtkwave
     sim.send_signals_to_gtkwave(sim.io)
-    sim.send_signals_to_gtkwave(sim.internals)
+    # sim.send_signals_to_gtkwave(sim.internals) # not working anymore
 
     # add all the io and internal signals to gtkwave
     sim.send_to_gtkwave(sim.io)
-    sim.send_to_gtkwave(sim.internals)
+    # sim.send_to_gtkwave(sim.internals) # not working anymore
 
     # tick the automatically detected clock
     sim.clock.tick()
 
     # set rst back to 0
     sim.io.rst = 0
```

### Comparing `pyverilator-mm-0.7.2/README.rst` & `pyverilator-mm-0.7.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -43,33 +43,33 @@
         wire [7:0] next_count_reg;
         assign next_count_reg = (en == 1) ? count_reg + 1 : count_reg;
         assign out = next_count_reg;
         always @(posedge clk) begin
             if (rst == 1) count_reg <= 0;
             else          count_reg <= next_count_reg;
         end
-    endmodule'''
+    endmodule
 
 Then you can use ``pyverilator`` to simulate this module using verilator in
 python.
 
 .. code:: python
 
     sim = pyverilator.PyVerilator.build('counter.v')
 
     # start gtkwave to view the waveforms as they are made
     sim.start_gtkwave()
 
     # add all the io and internal signals to gtkwave
     sim.send_signals_to_gtkwave(sim.io)
-    sim.send_signals_to_gtkwave(sim.internals)
+    # sim.send_signals_to_gtkwave(sim.internals) # not working anymore
 
     # add all the io and internal signals to gtkwave
     sim.send_to_gtkwave(sim.io)
-    sim.send_to_gtkwave(sim.internals)
+    # sim.send_to_gtkwave(sim.internals) # not working anymore
 
     # tick the automatically detected clock
     sim.clock.tick()
 
     # set rst back to 0
     sim.io.rst = 0
```

### Comparing `pyverilator-mm-0.7.2/pyverilator/pyverilator.py` & `pyverilator-mm-0.7.3/pyverilator/pyverilator.py`

 * *Files 0% similar despite different names*

```diff
@@ -721,14 +721,15 @@
         for name, _ in self.inputs + self.outputs + self.internal_signals:
             if name == signal_name:
                 return True
         return False
 
     @property
     def finished(self):
+        self.stop_vcd_trace()
         return self.lib.get_finished() & 1
 
     @finished.setter
     def finished(self, b):
         return self.lib.set_finished(b)
 
     def set_vl_finish_callback(self, cb):
```

### Comparing `pyverilator-mm-0.7.2/pyverilator/verilator_tools.py` & `pyverilator-mm-0.7.3/pyverilator/verilator_tools.py`

 * *Files identical despite different names*

### Comparing `pyverilator-mm-0.7.2/pyverilator/verilatorcpp.py` & `pyverilator-mm-0.7.3/pyverilator/verilatorcpp.py`

 * *Files identical despite different names*

### Comparing `pyverilator-mm-0.7.2/pyverilator_mm.egg-info/PKG-INFO` & `pyverilator-mm-0.7.3/pyverilator_mm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyverilator-mm
-Version: 0.7.2
+Version: 0.7.3
 Summary: Python interface to Verilator models
 Home-page: https://github.com/bat52/pyverilator
 Author: CSAIL CSG, Marco Merlin
 Author-email: acwright@mit.edu, bthom@mit.edu
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bat52/pyverilator/issues
 Project-URL: Source, https://github.com/bat52/pyverilator
@@ -64,33 +64,33 @@
         wire [7:0] next_count_reg;
         assign next_count_reg = (en == 1) ? count_reg + 1 : count_reg;
         assign out = next_count_reg;
         always @(posedge clk) begin
             if (rst == 1) count_reg <= 0;
             else          count_reg <= next_count_reg;
         end
-    endmodule'''
+    endmodule
 
 Then you can use ``pyverilator`` to simulate this module using verilator in
 python.
 
 .. code:: python
 
     sim = pyverilator.PyVerilator.build('counter.v')
 
     # start gtkwave to view the waveforms as they are made
     sim.start_gtkwave()
 
     # add all the io and internal signals to gtkwave
     sim.send_signals_to_gtkwave(sim.io)
-    sim.send_signals_to_gtkwave(sim.internals)
+    # sim.send_signals_to_gtkwave(sim.internals) # not working anymore
 
     # add all the io and internal signals to gtkwave
     sim.send_to_gtkwave(sim.io)
-    sim.send_to_gtkwave(sim.internals)
+    # sim.send_to_gtkwave(sim.internals) # not working anymore
 
     # tick the automatically detected clock
     sim.clock.tick()
 
     # set rst back to 0
     sim.io.rst = 0
```

### Comparing `pyverilator-mm-0.7.2/setup.py` & `pyverilator-mm-0.7.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pyverilator-mm',
-    version='0.7.2',
+    version='0.7.3',
     description='Python interface to Verilator models',
     long_description=long_description,
     url='https://github.com/bat52/pyverilator',
     author='CSAIL CSG, Marco Merlin',
     author_email='acwright@mit.edu, bthom@mit.edu',
     # https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
```

