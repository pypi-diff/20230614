# Comparing `tmp/pyarbtools-2022.11.2.tar.gz` & `tmp/pyarbtools-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyarbtools-2022.11.2.tar", last modified: Thu Nov 10 23:14:59 2022, max compression
+gzip compressed data, was "pyarbtools-2023.6.1.tar", last modified: Wed Jun 14 00:15:14 2023, max compression
```

## Comparing `pyarbtools-2022.11.2.tar` & `pyarbtools-2023.6.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-11-10 23:14:59.217226 pyarbtools-2022.11.2/
--rw-rw-rw-   0        0        0     2011 2021-05-06 23:00:16.000000 pyarbtools-2022.11.2/LICENSE
--rw-rw-rw-   0        0        0      135 2021-05-06 23:00:16.000000 pyarbtools-2022.11.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2961 2022-11-10 23:14:59.217226 pyarbtools-2022.11.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-11-10 23:14:59.214226 pyarbtools-2022.11.2/PyArbTools.egg-info/
--rw-rw-rw-   0        0        0     2961 2022-11-10 23:14:59.000000 pyarbtools-2022.11.2/PyArbTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2022-11-10 23:14:59.000000 pyarbtools-2022.11.2/PyArbTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-10 23:14:59.000000 pyarbtools-2022.11.2/PyArbTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2022-11-10 23:14:59.000000 pyarbtools-2022.11.2/PyArbTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-11-10 23:14:59.000000 pyarbtools-2022.11.2/PyArbTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2220 2022-11-10 19:31:09.000000 pyarbtools-2022.11.2/README.rst
-drwxrwxrwx   0        0        0        0 2022-11-10 23:14:59.209226 pyarbtools-2022.11.2/pyarbtools/
--rw-rw-rw-   0        0        0      465 2022-11-10 23:13:39.000000 pyarbtools-2022.11.2/pyarbtools/__init__.py
--rw-rw-rw-   0        0        0      898 2022-11-04 17:37:42.000000 pyarbtools-2022.11.2/pyarbtools/error.py
--rw-rw-rw-   0        0        0    22382 2021-05-06 23:00:16.000000 pyarbtools-2022.11.2/pyarbtools/favicon.ico
--rw-rw-rw-   0        0        0    57547 2022-11-04 17:39:02.000000 pyarbtools-2022.11.2/pyarbtools/gui.py
--rw-rw-rw-   0        0        0    97348 2022-11-10 23:07:53.000000 pyarbtools-2022.11.2/pyarbtools/instruments.py
--rw-rw-rw-   0        0        0    44714 2022-11-10 17:46:41.000000 pyarbtools-2022.11.2/pyarbtools/vsaControl.py
--rw-rw-rw-   0        0        0    88284 2021-05-06 23:00:16.000000 pyarbtools-2022.11.2/pyarbtools/wfmBuilder.py
--rw-rw-rw-   0        0        0       95 2021-11-01 21:39:33.000000 pyarbtools-2022.11.2/pyproject.toml
--rw-rw-rw-   0        0        0     1004 2022-11-10 23:14:59.219226 pyarbtools-2022.11.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-14 00:15:14.173838 pyarbtools-2023.6.1/
+-rw-rw-rw-   0        0        0     2011 2021-05-06 23:00:16.000000 pyarbtools-2023.6.1/LICENSE
+-rw-rw-rw-   0        0        0      135 2021-05-06 23:00:16.000000 pyarbtools-2023.6.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2960 2023-06-14 00:15:14.173838 pyarbtools-2023.6.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 00:15:14.169840 pyarbtools-2023.6.1/PyArbTools.egg-info/
+-rw-rw-rw-   0        0        0     2960 2023-06-14 00:15:14.000000 pyarbtools-2023.6.1/PyArbTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-06-14 00:15:14.000000 pyarbtools-2023.6.1/PyArbTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 00:15:14.000000 pyarbtools-2023.6.1/PyArbTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-14 00:15:14.000000 pyarbtools-2023.6.1/PyArbTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-14 00:15:14.000000 pyarbtools-2023.6.1/PyArbTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2220 2023-05-11 19:23:31.000000 pyarbtools-2023.6.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-14 00:15:14.157836 pyarbtools-2023.6.1/pyarbtools/
+-rw-rw-rw-   0        0        0      465 2023-06-14 00:14:02.000000 pyarbtools-2023.6.1/pyarbtools/__init__.py
+-rw-rw-rw-   0        0        0      473 2023-05-11 19:43:24.000000 pyarbtools-2023.6.1/pyarbtools/error.py
+-rw-rw-rw-   0        0        0    22382 2021-05-06 23:00:16.000000 pyarbtools-2023.6.1/pyarbtools/favicon.ico
+-rw-rw-rw-   0        0        0    57547 2023-05-11 19:23:31.000000 pyarbtools-2023.6.1/pyarbtools/gui.py
+-rw-rw-rw-   0        0        0    97994 2023-06-13 23:42:45.000000 pyarbtools-2023.6.1/pyarbtools/instruments.py
+-rw-rw-rw-   0        0        0    44714 2023-05-11 19:23:31.000000 pyarbtools-2023.6.1/pyarbtools/vsaControl.py
+-rw-rw-rw-   0        0        0    88284 2021-05-06 23:00:16.000000 pyarbtools-2023.6.1/pyarbtools/wfmBuilder.py
+-rw-rw-rw-   0        0        0       95 2021-11-01 21:39:33.000000 pyarbtools-2023.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1003 2023-06-14 00:15:14.176848 pyarbtools-2023.6.1/setup.cfg
```

### Comparing `pyarbtools-2022.11.2/LICENSE` & `pyarbtools-2023.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyarbtools-2022.11.2/PKG-INFO` & `pyarbtools-2023.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarbtools
-Version: 2022.11.2
+Version: 2023.6.1
 Summary: PyArbTools provides waveform creation and remote instrument control capabilities for Keysight signal generators.
 Home-page: https://github.com/morgan-at-keysight/pyarbtools
 Author: Morgan Allison
 Author-email: morgan.allison@keysight.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyarbtools-2022.11.2/PyArbTools.egg-info/PKG-INFO` & `pyarbtools-2023.6.1/PyArbTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarbtools
-Version: 2022.11.2
+Version: 2023.6.1
 Summary: PyArbTools provides waveform creation and remote instrument control capabilities for Keysight signal generators.
 Home-page: https://github.com/morgan-at-keysight/pyarbtools
 Author: Morgan Allison
 Author-email: morgan.allison@keysight.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyarbtools-2022.11.2/PyArbTools.egg-info/SOURCES.txt` & `pyarbtools-2023.6.1/PyArbTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyarbtools-2022.11.2/README.rst` & `pyarbtools-2023.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyarbtools-2022.11.2/pyarbtools/favicon.ico` & `pyarbtools-2023.6.1/pyarbtools/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyarbtools-2022.11.2/pyarbtools/gui.py` & `pyarbtools-2023.6.1/pyarbtools/gui.py`

 * *Files identical despite different names*

### Comparing `pyarbtools-2022.11.2/pyarbtools/instruments.py` & `pyarbtools-2023.6.1/pyarbtools/instruments.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,26 @@
 Builds instrument specific classes for each signal generator.
 The classes include minimum waveform length/granularity checks, binary
 waveform formatting, sequencer length/granularity checks, sample rate
 checks, etc. per instrument.
 Tested on M8190A, M8195A, M8196A, N5182B, E8257D, M9383A, N5193A, N5194A
 """
 
-from socket import socket
 import numpy as np
 import socketscpi
 import pyvisa
 
 from pyarbtools import error
 
 """
 TODO:
+* PyVISA Socket doesn't work
+* Check M9381/3A error class in VSG.download_wfm()
 * Add a function for IQ adjustments in VSG class
 * Add multithreading for waveform download and wfmBuilder
-* DONE -- Separate out configure() into individual methods that update class attributes
-* Add a check for PDW length (600k limit?)
 * Add a multi-binblockwrite feature for download_wfm in the case of
     waveform size > 1 GB
 """
 
 
 def wraparound_calc(length, gran, minLen):
     """
@@ -83,40 +82,45 @@
                     self.instance = socketscpi.SocketInstrument(ipAddress, port=5025, timeout=timeout, noDelay=True)
             elif self.apiType == "pyvisa":
                 if protocol.lower() == "vxi11":
                     self.instance = pyvisa.ResourceManager().open_resource(f"tcpip::{ipAddress}::inst{port}::instr")
                 elif protocol.lower() == "hislip":
                     self.instance = pyvisa.ResourceManager().open_resource(f"tcpip::{ipAddress}::hislip{port}::instr")
                 elif protocol.lower() == "socket":
-                    self.instance = pyvisa.ResourceManager().open_resource(f"tcpip::{ipAddress}::{port}::socket")
+                    raise error.InstrumentError(f'socket protocol in PyVISA is not currently working, use "hislip" or "vxi11"')
+                    # self.instance = pyvisa.ResourceManager().open_resource(f"tcpip0::{ipAddress}::{port}::socket")
                 else:
                     raise ValueError('Invalid protocol selection. Use "vxi11", "hislip", or "socket".')
-                self.instId = self.query("*idn?")
             else:
                 raise ValueError(f'"{self.apiType}" is not a valid apiType, use "socketscpi" or "pyvisa".')
+            
+            self.instId = self.instance.query("*idn?")
 
     def __getattr__(self, __name: str):
         """This is a passthrough method that allows the base class to access attributes from the parent class.
         See the accepted answer at
         https://stackoverflow.com/questions/65754399/conditional-inheritance-based-on-arguments-in-python"""
         return self.instance.__getattribute__(__name)
         
     def err_check(self):
         """Prints out all errors and clears error queue. Raises InstrumentError with the info of the error encountered."""
 
         err = []
         cmd = 'SYST:ERR?'
 
         # Strip out extra characters
-        temp = self.query(cmd).strip().replace('+', '').replace('-', '')
+        temp = self.query(cmd)
+        temp = temp.strip().replace('+', '').replace('-', '')
         # Read all errors until none are left
         while temp != '0,"No error"':
             # Build list of errors
+            print(temp)
             err.append(temp)
-            temp = self.query(cmd).strip().replace('+', '').replace('-', '')
+            temp = self.query(cmd)
+            temp = temp.strip().replace('+', '').replace('-', '')
         if err:
             raise error.InstrumentError(err)
 
 class M8190A(SignalGeneratorBase):
     """Generic class for controlling a Keysight M8190A AWG.
 
     Attributes:
@@ -335,15 +339,15 @@
             ch (int): Channel to be configured
             cf (float): Carrier frequency of channel
         """
 
         if not isinstance(ch, int) or ch < 1 or ch > 2:
             raise ValueError("'ch' must be 1 or 2.")
         if not isinstance(cf, float) or cf <= 0:
-            raise socketscpi.SockInstError("Carrier frequency must be a positive floating point value.")
+            raise ValueError("Carrier frequency must be a positive floating point value.")
         self.write(f"carrier{ch}:freq {cf}")
         if ch == 1:
             self.cf1 = float(self.query(f"carrier{ch}:freq?").strip().split(",")[0])
         else:
             self.cf2 = float(self.query(f"carrier{ch}:freq?").strip().split(",")[0])
 
     def set_refSrc(self, refSrc):
@@ -492,15 +496,15 @@
             # Sync marker occupies the second least significant bit in the waveform data
             syncMkrData[syncMkr : syncMkr + syncMkrLength] = 1 << 1
 
             # Combine sample and sync markers into single binary value and add to waveform data
             markerData = sampleMkrData + syncMkrData
             wfm += markerData
         else:
-            raise socketscpi.SockInstError('Invalid wfmFormat chosen. Use "iq" or "real".')
+            raise ValueError('Invalid wfmFormat chosen. Use "iq" or "real".')
 
         # Initialize waveform segment, populate it with data, and provide a name
         segment = int(self.query(f"trace{ch}:catalog?").strip().split(",")[-2]) + 1
         self.write(f"trace{ch}:def {segment}, {length}")
         self.write_binary_values(f"trace{ch}:data {segment}, 0, ", wfm, datatype='h')
         self.write(f'trace{ch}:name {segment},"{name}_{segment}"')
 
@@ -564,15 +568,15 @@
         self.check_resolution()
 
         # If waveform length doesn't meet granularity or minimum length requirements, repeat the waveform until it does
         repeats = wraparound_calc(len(wfm), self.gran, self.minLen)
         wfm = np.tile(wfm, repeats)
         rl = len(wfm)
         if rl < self.minLen:
-            raise error.AWGError(f"Waveform length: {rl}, must be at least {self.minLen}.")
+            raise error.InstrumentError(f"Waveform length: {rl}, must be at least {self.minLen}.")
         rem = rl % self.gran
         if rem != 0:
             raise error.GranularityError(f"Waveform must have a granularity of {self.gran}. Extra samples: {rem}")
 
         # Apply the binary multiplier, cast to int16, and shift samples over if required
         return np.array(self.binMult * wfm, dtype=np.int16) << self.binShift
 
@@ -582,17 +586,17 @@
         Args:
             wfmID (int): Waveform identifier, used to select waveform to be deleted.
             ch (int): AWG channel from which the segment will be deleted.
         """
 
         # Argument checking
         if type(wfmID) != int or wfmID < 1:
-            raise socketscpi.SockInstError("Segment ID must be a positive integer.")
+            raise error.InstrumentError("Segment ID must be a positive integer.")
         if ch not in [1, 2]:
-            raise socketscpi.SockInstError("Channel must be 1 or 2.")
+            raise error.InstrumentError("Channel must be 1 or 2.")
         self.write("abort")
         self.write(f"trace{ch}:delete {wfmID}")
 
     def clear_all_wfm(self):
         """Clears all segments from segment memory."""
         self.write("abort")
         self.write("trace1:delete:all")
@@ -811,15 +815,15 @@
         # Populate the sequence index with an idle segment
         self.write(f"stable1:data {seqIndex}, {controlEntry}, 1, 0, {idleSample}, {idleDelay}, 0")
 
         self.err_check()
 
 
 # noinspection PyUnusedLocal,PyUnusedLocal
-class M8195A(socketscpi.SocketInstrument):
+class M8195A(SignalGeneratorBase):
     """
     Generic class for controlling Keysight M8195A AWG.
 
     Attributes:
         dacMode (str): DAC operation mode. ('single', 'dual', 'four', 'marker', 'dcd', 'dcmarker')
         memDiv (int): Clock/memory divider rate. (1, 2, 4)
         fs (float): AWG sample rate.
@@ -828,19 +832,21 @@
         amp1/2/3/4 (float): Output amplitude in volts pk-pk. (min=75 mV, max=1 V)
         func (str): AWG mode, either arb or sequencing. ('arb', 'sts', 'stsc')
 
     TODO
         Add check to ensure that the correct instrument is connected
     """
 
-    def __init__(self, host, port=5025, timeout=10, reset=False):
-        super().__init__(host, port, timeout)
+    def __init__(self, ipAddress, apiType="socketscpi", timeout=10, reset=False, **kwargs):
+        super().__init__(ipAddress, apiType=apiType, timeout=timeout, **kwargs)
+        
         if reset:
             self.write("*rst")
             self.query("*opc?")
+            self.write("abort")
 
         # Query all settings from AWG and store them as class attributes
         self.dacMode = self.query("inst:dacm?").strip()
         self.memDiv = 1
         self.fs = float(self.query("frequency:raster?").strip())
         self.effFs = self.fs / self.memDiv
         self.func = self.query("func:mode?").strip()
@@ -980,19 +986,19 @@
         """
         Sets and reads the output voltage amplitude (pk-pk) for specified channels using SCPI commands.
         Args:
             amplitude (float): Output amplitude in Volts pk-pk.
             channel (int): Channel to change. (1, 2, 3, or 4).
         """
         if channel not in [1, 2, 3, 4]:
-            raise error.AWGError("'channel' must be 1, 2, 3, or 4.")
+            raise error.InstrumentError("'channel' must be 1, 2, 3, or 4.")
         if not isinstance(amplitude, float) and not isinstance(amplitude, int):
-            raise error.AWGError("'amplitude' must be a floating point value.")
+            raise error.InstrumentError("'amplitude' must be a floating point value.")
         if amplitude < 75e-3 or amplitude > 1:
-            raise error.AWGError("'amplitude' must be between 75 mV and 1 V.")
+            raise error.InstrumentError("'amplitude' must be between 75 mV and 1 V.")
 
         self.write(f"voltage{channel} {amplitude}")
         # This is a neat use of Python's exec() function, which takes a "program" in as a string and executes it
         # Very useful if you need to dynamically decide which variable names to call
         exec(f"self.amp{channel} = float(self.query('voltage{channel}?'))")
 
     def sanity_check(self):
@@ -1027,42 +1033,42 @@
         self.write("abort")
         wfm = self.check_wfm(wfmData)
         length = len(wfmData)
 
         # Initialize waveform segment, populate it with data, and provide a name
         segment = int(self.query(f"trace{ch}:catalog?").strip().split(",")[-2]) + 1
         self.write(f"trace{ch}:def {segment}, {length}")
-        self.write_binary_values(f"trace{ch}:data {segment}, 0, ", wfm)
+        self.write_binary_values(f"trace{ch}:data {segment}, 0, ", wfm, datatype='b')
         self.write(f'trace{ch}:name {segment},"{name}_{segment}"')
 
         # Use 'segment' as the waveform identifier for the .play() method.
         return segment
 
     def check_wfm(self, wfmData):
         """
         HELPER FUNCTION
         Checks minimum size and granularity and returns waveform with
         appropriate binary formatting.
 
-        See pages 273-274 in Keysight M8195A User's Guide (Edition 13.0,
-        October 2017) for more info.
+        See page 253 in Keysight M8195A User's Guide Rev 2 (Edition 7.0,
+        March 2019) for more info.
         Args:
             wfmData (NumPy array): Unscaled/unformatted waveform data.
 
         Returns:
             (NumPy array): Waveform data that has been scaled and
                 formatted appropriately for download to AWG
         """
 
         # If waveform length doesn't meet granularity or minimum length requirements, repeat the waveform until it does
         repeats = wraparound_calc(len(wfmData), self.gran, self.minLen)
         wfm = np.tile(wfmData, repeats)
         rl = len(wfm)
         if rl < self.minLen:
-            raise error.AWGError(f"Waveform length: {rl}, must be at least {self.minLen}.")
+            raise error.InstrumentError(f"Waveform length: {rl}, must be at least {self.minLen}.")
         if rl % self.gran != 0:
             raise error.GranularityError(f"Waveform must have a granularity of {self.gran}.")
 
         # Apply the binary multiplier, cast to int16, and shift samples over if required
         return np.array(self.binMult * wfm, dtype=np.int8) << self.binShift
 
     def delete_segment(self, wfmID=1, ch=1):
@@ -1071,17 +1077,17 @@
         Args:
             wfmID (int): Waveform identifier, used to select waveform to be deleted.
             ch (int): AWG channel from which the segment will be deleted.
         """
 
         # Argument checking
         if type(wfmID) != int or wfmID < 1:
-            raise socketscpi.SockInstError("Segment ID must be a positive integer.")
+            raise ValueError("Segment ID must be a positive integer.")
         if ch not in [1, 2, 3, 4]:
-            raise socketscpi.SockInstError("Channel must be 1, 2, 3, or 4.")
+            raise ValueError("Channel must be 1, 2, 3, or 4.")
         self.write("abort")
         self.write(f"trace{ch}:del {wfmID}")
 
     def clear_all_wfm(self):
         """Clears all segments from segment memory."""
         self.write("abort")
         for ch in range(1, 5):
@@ -1108,33 +1114,35 @@
         """
 
         self.write(f"output{ch} off")
         self.write("abort")
 
 
 # noinspection PyUnusedLocal,PyUnusedLocal
-class M8196A(socketscpi.SocketInstrument):
+class M8196A(SignalGeneratorBase):
     """
     Generic class for controlling Keysight M8196A AWG.
 
     Attributes:
         dacMode (str): DAC operation mode. ('single', 'dual', 'four', 'marker', 'dcmarker')
         fs (float): AWG sample rate.
         refSrc (str): Reference clock source. ('axi', 'int', 'ext')
         refFreq (float): Reference clock frequency.
 
     TODO
         Add check to ensure that the correct instrument is connected
     """
 
-    def __init__(self, host, port=5025, timeout=10, reset=False):
-        super().__init__(host, port, timeout)
+    def __init__(self, ipAddress, apiType="socketscpi", timeout=10, reset=False, **kwargs):
+        super().__init__(ipAddress, apiType=apiType, timeout=timeout, **kwargs)
+        
         if reset:
             self.write("*rst")
             self.query("*opc?")
+            self.write("abort")
 
         # Query all settings from AWG and store them as class attributes
         self.dacMode = self.query("inst:dacm?").strip()
         self.fs = float(self.query("frequency:raster?").strip())
         self.amp = float(self.query("voltage?").strip())
         self.refSrc = self.query("roscillator:source?").strip()
         self.refFreq = float(self.query("roscillator:frequency?").strip())
@@ -1217,37 +1225,37 @@
         Sets and reads reference frequency using SCPI commands.
         Args:
             refFreq (float): Reference clock frequency.
         """
 
         # Check for valid refSrc arguments and assign
         if self.refSrc.lower() not in ["int", "ext", "axi"]:
-            raise error.AWGError("Invalid reference source selection.")
+            raise error.InstrumentError("Invalid reference source selection.")
         self.write(f"roscillator:source {self.refSrc}")
         self.refSrc = self.query("roscillator:source?").strip().lower()
 
         # Check for presence of external ref signal
         srcAvailable = self.query(f"roscillator:source:check? {self.refSrc}").strip()
         if not srcAvailable:
-            raise error.AWGError("No signal at selected reference source.")
+            raise error.InstrumentError("No signal at selected reference source.")
 
         # Only set ref frequency if using ext ref, int/axi is always 100 MHz
         if self.refSrc == "ext":
             # Seamlessly manage external clock range selection based on ref freq.
             # Precision clock source
             if 2.3125e9 <= refFreq <= 3e9:
                 self.write("roscillator:range rang3")
             # Standard external clock source
             elif 10e6 <= refFreq <= 300e6:
                 self.write("roscillator:range rang1")
             # Wide external clock source
             elif 162e6 <= refFreq <= 17e9:
                 self.write("roscillator:range rang2")
             else:
-                raise error.AWGError("Selected reference clock frequency outside allowable range.")
+                raise error.InstrumentError("Selected reference clock frequency outside allowable range.")
             self.write(f"roscillator:frequency {refFreq}")
         self.refFreq = float(self.query("roscillator:frequency?").strip())
 
     def sanity_check(self):
         """Prints out user-accessible class attributes."""
 
         print("Sample rate:", self.fs)
@@ -1275,15 +1283,15 @@
         self.clear_all_wfm()
         wfm = self.check_wfm(wfmData)
         length = len(wfm)
 
         # Initialize waveform segment, populate it with data, and provide a name
         segment = 1
         self.write(f"trace{ch}:def {segment}, {length}")
-        self.write_binary_values(f"trace{ch}:data {segment}, 0, ", wfm)
+        self.write_binary_values(f"trace{ch}:data {segment}, 0, ", wfm, datatype='b')
         self.write(f'trace{ch}:name {segment},"{name}_{segment}"')
 
         # Use 'segment' as the waveform identifier for the .play() method.
         return segment
 
     def check_wfm(self, wfmData):
         """
@@ -1302,17 +1310,17 @@
         """
 
         # If waveform length doesn't meet granularity or minimum length requirements, repeat the waveform until it does
         repeats = wraparound_calc(len(wfmData), self.gran, self.minLen)
         wfm = np.tile(wfmData, repeats)
         rl = len(wfm)
         if rl < self.minLen:
-            raise error.AWGError(f"Waveform length: {rl}, must be at least {self.minLen}.")
+            raise error.InstrumentError(f"Waveform length: {rl}, must be at least {self.minLen}.")
         if rl > self.maxLen:
-            raise error.AWGError(f"Waveform length: {rl}, must be shorter than {self.maxLen}.")
+            raise error.InstrumentError(f"Waveform length: {rl}, must be shorter than {self.maxLen}.")
         if rl % self.gran != 0:
             raise error.GranularityError(f"Waveform must have a granularity of {self.gran}.")
 
         # Apply the binary multiplier, cast to int16, and shift samples over if required
         return np.array(self.binMult * wfm, dtype=np.int8) << self.binShift
 
     def delete_segment(self):
@@ -1386,17 +1394,17 @@
             self.refFreq = 10e6
         elif "ext" in self.refSrc.lower():
             self.refFreq = float(self.query("roscillator:frequency:external?").strip())
         elif "bbg" in self.refSrc.lower():
             if "M938" not in self.instId:
                 self.refFreq = float(self.query("roscillator:frequency:bbg?").strip())
             else:
-                raise error.VSGError("Invalid reference source chosen, select 'int' or 'ext'.")
+                raise error.InstrumentError("Invalid reference source chosen, select 'int' or 'ext'.")
         else:
-            raise error.VSGError("Unknown refSrc selected.")
+            raise error.InstrumentError("Unknown refSrc selected.")
 
         # Initialize waveform format constants and populate them with check_resolution()
         self.minLen = 60
         self.binMult = 32767
         if "M938" not in self.instId:
             self.iqScale = float(self.query("radio:arb:rscaling?").strip())
             self.gran = 2
@@ -1571,15 +1579,15 @@
         if "int" in self.refSrc.lower():
             self.refFreq = 10e6
         elif "ext" in self.refSrc.lower():
             self.refFreq = float(self.query("roscillator:frequency:external?").strip())
         elif "bbg" in self.refSrc.lower():
             self.refFreq = float(self.query("roscillator:frequency:bbg?").strip())
         else:
-            raise error.VSGError("Unknown refSrc selected.")
+            raise error.InstrumentError("Unknown refSrc selected.")
 
     def sanity_check(self):
         """Prints out user-accessible class attributes."""
         print("RF State:", self.rfState)
         print("Modulation State:", self.modState)
         print("Center Frequency:", self.cf)
         print("Output Amplitude:", self.amp)
@@ -1602,15 +1610,15 @@
             (str): Useful waveform identifier/name. Use this as the waveform identifier for the .play() method.
         """
 
         # Stop output before doing anything else
         self.set_modState(0)
         self.set_arbState(0)
 
-        # Adjust endianness for M9381/3A
+        # # Adjust endianness for M9381/3A
         if "M938" in self.instId:
             bigEndian = False
         else:
             bigEndian = True
 
         # Data type checking
         if not isinstance(wfmData, np.ndarray):
@@ -1632,20 +1640,20 @@
                 self.query("*opc?")
                 self.write(f'mmemory:delete "C:\\Temp\\{wfmID}"')
                 self.query("*opc?")
                 self.err_check()
             except socketscpi.SockInstError:
                 # print('Waveform doesn\'t exist, skipping delete operation.')
                 pass
-            self.write_binary_values(f'mmemory:data "C:\\Temp\\{wfmID}",', wfm)
+            self.write_binary_values(f'mmemory:data "C:\\Temp\\{wfmID}",', wfm, datatype='h')
             self.write(f'memory:copy "C:\\Temp\\{wfmID}","{wfmID}"')
 
         # EXG/MXG/PSG download procedure
         else:
-            self.write_binary_values(f'mmemory:data "WFM1:{wfmID}", ', wfm)
+            self.write_binary_values(f'mmemory:data "WFM1:{wfmID}",', wfm, datatype='h')
             self.write(f'radio:arb:waveform "WFM1:{wfmID}"')
 
         # Use 'wfmID' as the waveform identifier for the .play() method.
         return wfmID
 
     @staticmethod
     def iq_wfm_combiner(i, q):
@@ -1684,15 +1692,15 @@
         """
 
         # If waveform length doesn't meet granularity or minimum length requirements, repeat the waveform until it does
         repeats = wraparound_calc(len(wfm), self.gran, self.minLen)
         wfm = np.tile(wfm, repeats)
         rl = len(wfm)
         if rl < self.minLen:
-            raise error.VSGError(f"Waveform length: {rl}, must be at least {self.minLen}.")
+            raise error.InstrumentError(f"Waveform length: {rl}, must be at least {self.minLen}.")
         if rl % self.gran != 0:
             raise error.GranularityError(f"Waveform must have a granularity of {self.gran}.")
 
         if bigEndian:
             return np.array(self.binMult * wfm, dtype=np.int16).byteswap()
         else:
             return np.array(self.binMult * wfm, dtype=np.int16)
@@ -1744,16 +1752,18 @@
 
         self.set_rfState(0)
         self.set_modState(0)
         self.set_arbState(0)
 
 
 # noinspection PyAttributeOutsideInit,PyUnresolvedReferences,PyUnresolvedReferences,PyUnresolvedReferences,PyUnresolvedReferences,PyUnresolvedReferences,PyUnresolvedReferences,PyUnresolvedReferences,PyUnresolvedReferences
-class VXG(socketscpi.SocketInstrument):
-    def __init__(self, host, port=5025, timeout=10, reset=False):
+class VXG(SignalGeneratorBase):
+    # def __init__(self, host, port=5025, timeout=10, reset=False):
+    def __init__(self, ipAddress, apiType="socketscpi", timeout=10, reset=False, **kwargs):
+
         """
         Generic class for controlling the M9384B VXG signal generator.
 
         Attributes:
             rf1State (int): Turns the RF output on or off. (1, 0)
             modState (int): Turns the baseband modulator on or off. (1, 0)
             cf (float): Sets the generator's carrier frequency.
@@ -1763,15 +1773,16 @@
             refSrc (str): Sets the reference clock source. ('int', 'ext', 'bbg')
             fs (float): Sets the sample rate of the baseband generator.
 
         TODO
             Add check to ensure that the correct instrument is connected
         """
 
-        super().__init__(host, port, timeout)
+        # super().__init__(host, port, timeout)
+        super().__init__(ipAddress, apiType=apiType, timeout=timeout, **kwargs)
         if reset:
             self.write("*rst")
             self.query("*opc?")
 
         # Query the options on the VXG to see how many channels it has
         optionString = self.query("*opt?")
 
@@ -1805,25 +1816,25 @@
         self.refSrc = self.query("roscillator:source?").strip()
 
         if "int" in self.refSrc.lower():
             self.refFreq = 10e6
         elif "ext" in self.refSrc.lower():
             self.refFreq = float(self.query("roscillator:frequency:external?").strip())
         else:
-            raise error.VXGError("Unknown refSrc selected.")
+            raise error.InstrumentError("Unknown refSrc selected.")
 
         # Initialize waveform format constants and populate them with check_resolution()
         self.minLen = 512
         self.binMult = 32767
         self.gran = 8
 
     # def configure(self, rfState=1, modState=1, cf=1e9, amp=-20, alcState=0, iqScale=70, refSrc='int', fs=200e6):
     def configure(self, **kwargs):
         """
-        Sets basic configuration for VSG and populates class attributes accordingly.
+        Sets basic configuration for VXG and populates class attributes accordingly.
         Keyword Arguments:
             rfState1|2 (int): Turns the RF output on or off. (1, 0)
             modState1|2 (int): Turns the baseband modulator on or off. (1, 0)
             cf1|2 (float): Sets the generator's carrier frequency.
             amp1|2 (int/float): Sets the generator's RF output power.
             alcState (int): Turns the ALC (automatic level control) on or off. (1, 0)
             iqScale (int): Scales the IQ modulator. Default/safe value is 70
@@ -2078,15 +2089,15 @@
         if "int" in self.refSrc.lower():
             self.refFreq = 10e6
         elif "ext" in self.refSrc.lower():
             self.refFreq = float(self.query("roscillator:frequency:external?").strip())
         elif "bbg" in self.refSrc.lower():
             self.refFreq = float(self.query("roscillator:frequency:bbg?").strip())
         else:
-            raise error.VSGError("Unknown refSrc selected.")
+            raise error.InstrumentError("Unknown refSrc selected.")
 
     def sanity_check(self):
         """Prints out initialized values."""
         print("RF State 1:", self.rfState1)
         print("Modulation State 1:", self.modState1)
         print("Center Frequency 1:", self.cf1)
         print("Output Amplitude 1:", self.amp1)
@@ -2150,17 +2161,17 @@
         # self.write_binary_values(
         #     f'mmemory:data "D:\\Users\\Instrument\\Documents\\Keysight\\PathWave\\SignalGenerator\\Waveforms\\{wfmID}.bin",',
         #     wfm,
         # )
 
         # Save waveform to specified location on hard drive.
         if sim:
-            self.write_binary_values(f'mmemory:data "C:\\Temp\\{wfmID}.bin",', wfm)
+            self.write_binary_values(f'mmemory:data "C:\\Temp\\{wfmID}.bin",', wfm, datatype='h')
         else:
-            self.write_binary_values(f'mmemory:data "D:\\Users\\Instrument\\Documents\\Keysight\\PathWave\\SignalGenerator\\Waveforms\\{wfmID}.bin",', wfm)
+            self.write_binary_values(f'mmemory:data "D:\\Users\\Instrument\\Documents\\Keysight\\PathWave\\SignalGenerator\\Waveforms\\{wfmID}.bin",', wfm, datatype='h')
             
         return wfmID
 
     @staticmethod
     def iq_wfm_combiner(i, q):
         """
         Combines i and q wfms into a single interleaved wfm for download to generator.
@@ -2195,15 +2206,15 @@
         """
 
         # If waveform length doesn't meet granularity or minimum length requirements, repeat the waveform until it does
         repeats = wraparound_calc(len(wfm), self.gran, self.minLen)
         wfm = np.tile(wfm, repeats)
         rl = len(wfm)
         if rl < self.minLen:
-            raise error.VSGError(f"Waveform length: {rl}, must be at least {self.minLen}.")
+            raise error.InstrumentError(f"Waveform length: {rl}, must be at least {self.minLen}.")
         if rl % self.gran != 0:
             raise error.GranularityError(f"Waveform must have a granularity of {self.gran}.")
 
         return np.array(self.binMult * wfm, dtype=np.int16).byteswap()
 
     def delete_wfm(self, wfmID):
         """
```

### Comparing `pyarbtools-2022.11.2/pyarbtools/vsaControl.py` & `pyarbtools-2023.6.1/pyarbtools/vsaControl.py`

 * *Files identical despite different names*

### Comparing `pyarbtools-2022.11.2/pyarbtools/wfmBuilder.py` & `pyarbtools-2023.6.1/pyarbtools/wfmBuilder.py`

 * *Files identical despite different names*

### Comparing `pyarbtools-2022.11.2/setup.cfg` & `pyarbtools-2023.6.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7961 7262 746f 6f6c 730d 0a76   = pyarbtools..v
-00000020: 6572 7369 6f6e 203d 2032 3032 322e 3131  ersion = 2022.11
-00000030: 2e30 320d 0a61 7574 686f 7220 3d20 4d6f  .02..author = Mo
-00000040: 7267 616e 2041 6c6c 6973 6f6e 0d0a 6175  rgan Allison..au
-00000050: 7468 6f72 5f65 6d61 696c 203d 206d 6f72  thor_email = mor
-00000060: 6761 6e2e 616c 6c69 736f 6e40 6b65 7973  gan.allison@keys
-00000070: 6967 6874 2e63 6f6d 0d0a 6465 7363 7269  ight.com..descri
-00000080: 7074 696f 6e20 3d20 5079 4172 6254 6f6f  ption = PyArbToo
-00000090: 6c73 2070 726f 7669 6465 7320 7761 7665  ls provides wave
-000000a0: 666f 726d 2063 7265 6174 696f 6e20 616e  form creation an
-000000b0: 6420 7265 6d6f 7465 2069 6e73 7472 756d  d remote instrum
-000000c0: 656e 7420 636f 6e74 726f 6c20 6361 7061  ent control capa
-000000d0: 6269 6c69 7469 6573 2066 6f72 204b 6579  bilities for Key
-000000e0: 7369 6768 7420 7369 676e 616c 2067 656e  sight signal gen
-000000f0: 6572 6174 6f72 732e 0d0a 6c6f 6e67 5f64  erators...long_d
-00000100: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
-00000110: 653a 2052 4541 444d 452e 7273 740d 0a6c  e: README.rst..l
-00000120: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
-00000130: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
-00000140: 6578 742f 782d 7273 740d 0a75 726c 203d  ext/x-rst..url =
-00000150: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000160: 636f 6d2f 6d6f 7267 616e 2d61 742d 6b65  com/morgan-at-ke
-00000170: 7973 6967 6874 2f70 7961 7262 746f 6f6c  ysight/pyarbtool
-00000180: 730d 0a63 6c61 7373 6966 6965 7273 203d  s..classifiers =
-00000190: 200d 0a09 4465 7665 6c6f 706d 656e 7420   ...Development 
-000001a0: 5374 6174 7573 203a 3a20 3420 2d20 4265  Status :: 4 - Be
-000001b0: 7461 0d0a 0949 6e74 656e 6465 6420 4175  ta...Intended Au
-000001c0: 6469 656e 6365 203a 3a20 4465 7665 6c6f  dience :: Develo
-000001d0: 7065 7273 0d0a 0950 726f 6772 616d 6d69  pers...Programmi
-000001e0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000001f0: 7974 686f 6e20 3a3a 2033 0d0a 0950 726f  ython :: 3...Pro
-00000200: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000210: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000220: 2e36 0d0a 0950 726f 6772 616d 6d69 6e67  .6...Programming
-00000230: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000240: 686f 6e20 3a3a 2033 2e37 0d0a 0950 726f  hon :: 3.7...Pro
-00000250: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000260: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000270: 2e38 0d0a 0950 726f 6772 616d 6d69 6e67  .8...Programming
-00000280: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000290: 686f 6e20 3a3a 2033 2e39 0d0a 0d0a 5b6f  hon :: 3.9....[o
-000002a0: 7074 696f 6e73 5d0d 0a70 6163 6b61 6765  ptions]..package
-000002b0: 5f64 6972 203d 200d 0a70 6163 6b61 6765  _dir = ..package
-000002c0: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
-000002d0: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-000002e0: 2e36 0d0a 696e 7374 616c 6c5f 7265 7175  .6..install_requ
-000002f0: 6972 6573 203d 200d 0a09 6e75 6d70 790d  ires = ...numpy.
-00000300: 0a09 7363 6970 790d 0a09 736f 636b 6574  ..scipy...socket
-00000310: 7363 7069 0d0a 096d 6174 706c 6f74 6c69  scpi...matplotli
-00000320: 620d 0a09 7079 7669 7361 0d0a 0d0a 5b6f  b...pyvisa....[o
-00000330: 7074 696f 6e73 2e70 6163 6b61 6765 5f64  ptions.package_d
-00000340: 6174 615d 0d0a 7079 6172 6274 6f6f 6c73  ata]..pyarbtools
-00000350: 203d 2066 6176 6963 6f6e 2e69 636f 0d0a   = favicon.ico..
-00000360: 0d0a 5b62 6469 7374 5f77 6865 656c 5d0d  ..[bdist_wheel].
-00000370: 0a75 6e69 7665 7273 616c 203d 2031 0d0a  .universal = 1..
-00000380: 0d0a 5b66 6c61 6b65 385d 0d0a 6578 636c  ..[flake8]..excl
-00000390: 7564 6520 3d20 646f 6373 2c20 2e67 6974  ude = docs, .git
-000003a0: 2c20 5f5f 7079 6361 6368 655f 5f2c 2062  , __pycache__, b
-000003b0: 7569 6c64 2c20 7365 7475 702e 7079 0d0a  uild, setup.py..
-000003c0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-000003d0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-000003e0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000020: 6572 7369 6f6e 203d 2032 3032 332e 3036  ersion = 2023.06
+00000030: 2e31 0d0a 6175 7468 6f72 203d 204d 6f72  .1..author = Mor
+00000040: 6761 6e20 416c 6c69 736f 6e0d 0a61 7574  gan Allison..aut
+00000050: 686f 725f 656d 6169 6c20 3d20 6d6f 7267  hor_email = morg
+00000060: 616e 2e61 6c6c 6973 6f6e 406b 6579 7369  an.allison@keysi
+00000070: 6768 742e 636f 6d0d 0a64 6573 6372 6970  ght.com..descrip
+00000080: 7469 6f6e 203d 2050 7941 7262 546f 6f6c  tion = PyArbTool
+00000090: 7320 7072 6f76 6964 6573 2077 6176 6566  s provides wavef
+000000a0: 6f72 6d20 6372 6561 7469 6f6e 2061 6e64  orm creation and
+000000b0: 2072 656d 6f74 6520 696e 7374 7275 6d65   remote instrume
+000000c0: 6e74 2063 6f6e 7472 6f6c 2063 6170 6162  nt control capab
+000000d0: 696c 6974 6965 7320 666f 7220 4b65 7973  ilities for Keys
+000000e0: 6967 6874 2073 6967 6e61 6c20 6765 6e65  ight signal gene
+000000f0: 7261 746f 7273 2e0d 0a6c 6f6e 675f 6465  rators...long_de
+00000100: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
+00000110: 3a20 5245 4144 4d45 2e72 7374 0d0a 6c6f  : README.rst..lo
+00000120: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
+00000130: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
+00000140: 7874 2f78 2d72 7374 0d0a 7572 6c20 3d20  xt/x-rst..url = 
+00000150: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000160: 6f6d 2f6d 6f72 6761 6e2d 6174 2d6b 6579  om/morgan-at-key
+00000170: 7369 6768 742f 7079 6172 6274 6f6f 6c73  sight/pyarbtools
+00000180: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
+00000190: 0d0a 0944 6576 656c 6f70 6d65 6e74 2053  ...Development S
+000001a0: 7461 7475 7320 3a3a 2034 202d 2042 6574  tatus :: 4 - Bet
+000001b0: 610d 0a09 496e 7465 6e64 6564 2041 7564  a...Intended Aud
+000001c0: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
+000001d0: 6572 730d 0a09 5072 6f67 7261 6d6d 696e  ers...Programmin
+000001e0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000001f0: 7468 6f6e 203a 3a20 330d 0a09 5072 6f67  thon :: 3...Prog
+00000200: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000210: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000220: 360d 0a09 5072 6f67 7261 6d6d 696e 6720  6...Programming 
+00000230: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000240: 6f6e 203a 3a20 332e 370d 0a09 5072 6f67  on :: 3.7...Prog
+00000250: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000260: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000270: 380d 0a09 5072 6f67 7261 6d6d 696e 6720  8...Programming 
+00000280: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000290: 6f6e 203a 3a20 332e 390d 0a0d 0a5b 6f70  on :: 3.9....[op
+000002a0: 7469 6f6e 735d 0d0a 7061 636b 6167 655f  tions]..package_
+000002b0: 6469 7220 3d20 0d0a 7061 636b 6167 6573  dir = ..packages
+000002c0: 203d 2066 696e 643a 0d0a 7079 7468 6f6e   = find:..python
+000002d0: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
+000002e0: 360d 0a69 6e73 7461 6c6c 5f72 6571 7569  6..install_requi
+000002f0: 7265 7320 3d20 0d0a 096e 756d 7079 0d0a  res = ...numpy..
+00000300: 0973 6369 7079 0d0a 0973 6f63 6b65 7473  .scipy...sockets
+00000310: 6370 690d 0a09 6d61 7470 6c6f 746c 6962  cpi...matplotlib
+00000320: 0d0a 0970 7976 6973 610d 0a0d 0a5b 6f70  ...pyvisa....[op
+00000330: 7469 6f6e 732e 7061 636b 6167 655f 6461  tions.package_da
+00000340: 7461 5d0d 0a70 7961 7262 746f 6f6c 7320  ta]..pyarbtools 
+00000350: 3d20 6661 7669 636f 6e2e 6963 6f0d 0a0d  = favicon.ico...
+00000360: 0a5b 6264 6973 745f 7768 6565 6c5d 0d0a  .[bdist_wheel]..
+00000370: 756e 6976 6572 7361 6c20 3d20 310d 0a0d  universal = 1...
+00000380: 0a5b 666c 616b 6538 5d0d 0a65 7863 6c75  .[flake8]..exclu
+00000390: 6465 203d 2064 6f63 732c 202e 6769 742c  de = docs, .git,
+000003a0: 205f 5f70 7963 6163 6865 5f5f 2c20 6275   __pycache__, bu
+000003b0: 696c 642c 2073 6574 7570 2e70 790d 0a0d  ild, setup.py...
+000003c0: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
+000003d0: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
+000003e0: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
```

