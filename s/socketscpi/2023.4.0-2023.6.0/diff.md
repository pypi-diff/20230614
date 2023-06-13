# Comparing `tmp/socketscpi-2023.4.0.tar.gz` & `tmp/socketscpi-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketscpi-2023.4.0.tar", last modified: Mon Apr 17 20:25:38 2023, max compression
+gzip compressed data, was "socketscpi-2023.6.0.tar", last modified: Tue Jun 13 23:07:19 2023, max compression
```

## Comparing `socketscpi-2023.4.0.tar` & `socketscpi-2023.6.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 20:25:38.463078 socketscpi-2023.4.0/
--rw-rw-rw-   0        0        0      179 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3718 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1080 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/LICENSE
--rw-rw-rw-   0        0        0      273 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2020 2023-04-17 20:25:38.464077 socketscpi-2023.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1171 2023-04-17 20:14:12.000000 socketscpi-2023.4.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-17 20:25:38.415079 socketscpi-2023.4.0/docs/
--rw-rw-rw-   0        0        0      631 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-04-17 20:25:38.352080 socketscpi-2023.4.0/docs/_build/
-drwxrwxrwx   0        0        0        0 2023-04-17 20:25:38.353077 socketscpi-2023.4.0/docs/_build/html/
-drwxrwxrwx   0        0        0        0 2023-04-17 20:25:38.426083 socketscpi-2023.4.0/docs/_build/html/_static/
--rw-rw-rw-   0        0        0      286 2022-08-11 20:34:12.000000 socketscpi-2023.4.0/docs/_build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2022-08-11 20:34:12.000000 socketscpi-2023.4.0/docs/_build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2022-08-11 20:34:12.000000 socketscpi-2023.4.0/docs/_build/html/_static/plus.png
--rw-rw-rw-   0        0        0       29 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/docs/authors.rst
--rw-rw-rw-   0        0        0     5020 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/docs/contributing.rst
--rw-rw-rw-   0        0        0     1063 2023-04-17 20:11:11.000000 socketscpi-2023.4.0/docs/history.rst
--rw-rw-rw-   0        0        0      315 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/docs/index.rst
--rw-rw-rw-   0        0        0     1229 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/docs/installation.rst
--rwxrwxrwx   0        0        0      808 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/docs/make.bat
--rw-rw-rw-   0        0        0       28 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/docs/readme.rst
--rw-rw-rw-   0        0        0     4599 2023-04-17 20:12:40.000000 socketscpi-2023.4.0/docs/usage.rst
--rw-rw-rw-   0        0        0       95 2021-07-09 19:46:58.000000 socketscpi-2023.4.0/pyproject.toml
--rw-rw-rw-   0        0        0     1297 2023-04-17 20:25:38.466079 socketscpi-2023.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 20:25:38.434079 socketscpi-2023.4.0/socketscpi/
--rw-rw-rw-   0        0        0      163 2023-04-17 20:13:17.000000 socketscpi-2023.4.0/socketscpi/__init__.py
--rw-rw-rw-   0        0        0    13293 2023-04-17 19:18:11.000000 socketscpi-2023.4.0/socketscpi/socketscpi.py
-drwxrwxrwx   0        0        0        0 2023-04-17 20:25:38.452091 socketscpi-2023.4.0/socketscpi.egg-info/
--rw-rw-rw-   0        0        0     2020 2023-04-17 20:25:38.000000 socketscpi-2023.4.0/socketscpi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      612 2023-04-17 20:25:38.000000 socketscpi-2023.4.0/socketscpi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 20:25:38.000000 socketscpi-2023.4.0/socketscpi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-17 20:25:38.000000 socketscpi-2023.4.0/socketscpi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-17 20:25:38.000000 socketscpi-2023.4.0/socketscpi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 20:25:38.460079 socketscpi-2023.4.0/tests/
--rw-rw-rw-   0        0        0       68 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/tests/__init__.py
--rw-rw-rw-   0        0        0      887 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/tests/test_socketscpi.py
+drwxrwxrwx   0        0        0        0 2023-06-13 23:07:19.055423 socketscpi-2023.6.0/
+-rw-rw-rw-   0        0        0      179 2021-05-06 23:00:54.000000 socketscpi-2023.6.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3718 2021-05-06 23:00:54.000000 socketscpi-2023.6.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1080 2021-05-06 23:00:54.000000 socketscpi-2023.6.0/LICENSE
+-rw-rw-rw-   0        0        0      273 2021-05-06 23:00:54.000000 socketscpi-2023.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2020 2023-06-13 23:07:19.056428 socketscpi-2023.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1171 2023-04-17 20:14:12.000000 socketscpi-2023.6.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-13 23:07:19.005425 socketscpi-2023.6.0/docs/
+-rw-rw-rw-   0        0        0      631 2021-05-06 23:00:54.000000 socketscpi-2023.6.0/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-06-13 23:07:18.928423 socketscpi-2023.6.0/docs/_build/
+drwxrwxrwx   0        0        0        0 2023-06-13 23:07:18.928423 socketscpi-2023.6.0/docs/_build/html/
+drwxrwxrwx   0        0        0        0 2023-06-13 23:07:19.017428 socketscpi-2023.6.0/docs/_build/html/_static/
+-rw-rw-rw-   0        0        0      286 2022-08-11 20:34:12.000000 socketscpi-2023.6.0/docs/_build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2022-08-11 20:34:12.000000 socketscpi-2023.6.0/docs/_build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2022-08-11 20:34:12.000000 socketscpi-2023.6.0/docs/_build/html/_static/plus.png
+-rw-rw-rw-   0        0        0       29 2021-05-06 23:00:54.000000 socketscpi-2023.6.0/docs/authors.rst
+-rw-rw-rw-   0        0        0     5020 2023-06-13 22:50:44.000000 socketscpi-2023.6.0/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2021-05-06 23:00:54.000000 socketscpi-2023.6.0/docs/contributing.rst
+-rw-rw-rw-   0        0        0     1244 2023-06-13 22:44:15.000000 socketscpi-2023.6.0/docs/history.rst
+-rw-rw-rw-   0        0        0      315 2021-05-06 23:00:54.000000 socketscpi-2023.6.0/docs/index.rst
+-rw-rw-rw-   0        0        0     1229 2021-05-06 23:00:54.000000 socketscpi-2023.6.0/docs/installation.rst
+-rwxrwxrwx   0        0        0      808 2021-05-06 23:00:54.000000 socketscpi-2023.6.0/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2021-05-06 23:00:54.000000 socketscpi-2023.6.0/docs/readme.rst
+-rw-rw-rw-   0        0        0     4599 2023-04-17 20:12:40.000000 socketscpi-2023.6.0/docs/usage.rst
+-rw-rw-rw-   0        0        0       95 2021-07-09 19:46:58.000000 socketscpi-2023.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1297 2023-06-13 23:07:19.058424 socketscpi-2023.6.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 23:07:19.024424 socketscpi-2023.6.0/socketscpi/
+-rw-rw-rw-   0        0        0      163 2023-06-13 22:36:24.000000 socketscpi-2023.6.0/socketscpi/__init__.py
+-rw-rw-rw-   0        0        0    13568 2023-06-13 20:01:54.000000 socketscpi-2023.6.0/socketscpi/socketscpi.py
+drwxrwxrwx   0        0        0        0 2023-06-13 23:07:19.043423 socketscpi-2023.6.0/socketscpi.egg-info/
+-rw-rw-rw-   0        0        0     2020 2023-06-13 23:07:18.000000 socketscpi-2023.6.0/socketscpi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      612 2023-06-13 23:07:18.000000 socketscpi-2023.6.0/socketscpi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 23:07:18.000000 socketscpi-2023.6.0/socketscpi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-13 23:07:18.000000 socketscpi-2023.6.0/socketscpi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-13 23:07:18.000000 socketscpi-2023.6.0/socketscpi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 23:07:19.052431 socketscpi-2023.6.0/tests/
+-rw-rw-rw-   0        0        0       68 2021-05-06 23:00:54.000000 socketscpi-2023.6.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      887 2021-05-06 23:00:54.000000 socketscpi-2023.6.0/tests/test_socketscpi.py
```

### Comparing `socketscpi-2023.4.0/CONTRIBUTING.rst` & `socketscpi-2023.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `socketscpi-2023.4.0/LICENSE` & `socketscpi-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `socketscpi-2023.4.0/PKG-INFO` & `socketscpi-2023.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketscpi
-Version: 2023.4.0
+Version: 2023.6.0
 Summary: socketscpi provides a robust SCPI interface to electronic test and measurement equipment via raw socket protocol, removing the requirement for VISA and improving data transfer speed over VXI-11.
 Home-page: https://github.com/morgan-at-keysight/socketscpi
 Author: Morgan Allison
 Author-email: morgan.allison@keysight.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `socketscpi-2023.4.0/README.rst` & `socketscpi-2023.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `socketscpi-2023.4.0/docs/Makefile` & `socketscpi-2023.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `socketscpi-2023.4.0/docs/conf.py` & `socketscpi-2023.6.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 source_suffix = '.rst'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = u'socketscpi'
-copyright = u"2019-2020, Morgan Allison"
+copyright = u"2019-2023, Morgan Allison"
 author = u"Morgan Allison"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
@@ -61,15 +61,15 @@
 release = socketscpi.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `socketscpi-2023.4.0/docs/history.rst` & `socketscpi-2023.6.0/docs/history.rst`

 * *Files 16% similar despite different names*

```diff
@@ -26,8 +26,14 @@
 ----------------------
 
 * Renamed ``binblockwrite()``, ``binblockread()``, and ``disconnect()`` to ``write_binary_values()``, ``read_binary_values()``, and ``close()``, respectively, to match the function calls in PyVISA.
 
 2023.04.0 (2023-04-17)
 ----------------------
 
-* Added error checking syntax for UXR scopes. Added an argument in the ``SocketInstrument`` constructor to allow user to decide if verbose error checking will be attempted.
+* Added error checking syntax for UXR scopes. Added an argument in the ``SocketInstrument`` constructor to allow user to decide if verbose error checking will be attempted.
+
+2023.06.0 (2023-06-13)
+----------------------
+
+* Relaxed error checking to account for different "No error" responses from different instrument vendors. Updated comments.
+
```

### Comparing `socketscpi-2023.4.0/docs/installation.rst` & `socketscpi-2023.6.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `socketscpi-2023.4.0/docs/make.bat` & `socketscpi-2023.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `socketscpi-2023.4.0/docs/usage.rst` & `socketscpi-2023.6.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `socketscpi-2023.4.0/setup.cfg` & `socketscpi-2023.6.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [bumpversion]
-current_version = 2023.04.0
+current_version = 2023.06.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
 
 [bumpversion:file:socketscpi/__init__.py]
 search = __version__ = '{current_version}'
 replace = __version__ = '{new_version}'
 
 [metadata]
 name = socketscpi
-version = 2023.04.0
+version = 2023.06.0
 author = Morgan Allison
 author_email = morgan.allison@keysight.com
 description = socketscpi provides a robust SCPI interface to electronic test and measurement equipment via raw socket protocol, removing the requirement for VISA and improving data transfer speed over VXI-11.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/morgan-at-keysight/socketscpi
 classifiers =
```

### Comparing `socketscpi-2023.4.0/socketscpi/socketscpi.py` & `socketscpi-2023.6.0/socketscpi/socketscpi.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                 self.err_check()
             except SockInstError:
                 pass
 
     def disconnect(self):
         """DEPRECATED. THIS IS A PASS-THROUGH FUNCTION ONLY."""
 
-        warnings.warn("socketscpi.binblockread() is deprecated. Use socketscpi.query_binary_values() instead.")
+        warnings.warn("socketscpi.disconnect() is deprecated. Use socketscpi.close() instead.")
 
         return self.close()
 
     def close(self):
         """Gracefully close socket connection."""
         self.socket.shutdown(socket.SHUT_RDWR)
         self.socket.close()
@@ -132,24 +132,25 @@
         return result
 
     def err_check(self):
         """Prints out all errors and clears error queue. Raises SockInstError with the info of the error encountered."""
 
         err = []
 
-        # syst:err? response format varies between instruments, so remove whitespace and extra characters before checking
-        if 'mso' in self.instId.lower() or 'dso' in self.instId.lower():
+        # syst:err? syntax varies between instruments, so adjust syntax for Keysight oscilloscopes
+        if 'mso' in self.instId.lower() or 'dso' in self.instId.lower() or 'uxr' in self.instId.lower():
             cmd = 'SYST:ERR? string'
         else:
             cmd = 'SYST:ERR?'
 
-        # Strip out extra characters
+        # syst:err? response format varies between instrument families, so remove whitespace and extra characters before checking
         temp = self.query(cmd, errCheck=False).strip().replace('+', '').replace('-', '')
-        # Read all errors until none are left
-        while temp != '0,"No error"':
+
+        # Read all errors until none are left. Generally, instruments return a message that begins with the string '0,"No error'.
+        while '0,"No error' not in temp:
             # Build list of errors
             err.append(temp)
             temp = self.query(cmd, errCheck=False).strip().replace('+', '').replace('-', '')
         if err:
             raise SockInstError(err)
 
     def binblockread(self, cmd, datatype='b', debug=False, errCheck=True):
@@ -281,15 +282,15 @@
     def binblockwrite(self, cmd, data, debug=False, errCheck=True):
         """DEPRECATED. THIS IS A PASS-THROUGH FUNCTION ONLY."""
 
         warnings.warn("socketscpi.binblockwrite() is deprecated. Use socketscpi.write_binary_values() instead.")
 
         return self.write_binary_values(cmd, data, debug=debug, errCheck=errCheck)
 
-    def write_binary_values(self, cmd, data, debug=False, errCheck=True):
+    def write_binary_values(self, cmd, data, debug=False, errCheck=True, *args, **kwargs):
         """
         Sends a command and payload data with IEEE 488.2 binary block format
 
         The data is formatted as:
         #<x><yyy><data><newline>, where:
         <x> is the number of y bytes. For example, if <yyy>=500, then <x>=3.
         NOTE: <x> is a hexadecimal number.
@@ -298,14 +299,16 @@
         <newline> is a single byte new line character at the end of the data.
 
         Args:
             cmd (string): SCPI command used to send data to instrument as a binary block.
             data (NumPy ndarray): NumPy array containing data to load into the instrument.
             debug (bool): Turns debug mode on or off.
             errCheck (bool): Local error check flag. Auto error checking will only be done if both global and local error checking is enabled.
+        
+        *args and **kwargs added to allow for pyvisa syntax compatibility
        """
 
         # Generate binary block header from data
         header = self.binblock_header(data)
 
         # Send message, header, data, and termination
         self.socket.send(cmd.encode('latin_1'))
@@ -319,14 +322,13 @@
             print(f'header: {header}')
         
         if errCheck and self.globalErrCheck:
             print(f'BINBLOCKWRITE - local: {errCheck}, global: {self.globalErrCheck}')
             self.err_check()
 
 
-
 class SockInstError(Exception):
     pass
 
 
 class BinblockError(Exception):
     pass
```

### Comparing `socketscpi-2023.4.0/socketscpi.egg-info/PKG-INFO` & `socketscpi-2023.6.0/socketscpi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketscpi
-Version: 2023.4.0
+Version: 2023.6.0
 Summary: socketscpi provides a robust SCPI interface to electronic test and measurement equipment via raw socket protocol, removing the requirement for VISA and improving data transfer speed over VXI-11.
 Home-page: https://github.com/morgan-at-keysight/socketscpi
 Author: Morgan Allison
 Author-email: morgan.allison@keysight.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `socketscpi-2023.4.0/socketscpi.egg-info/SOURCES.txt` & `socketscpi-2023.6.0/socketscpi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `socketscpi-2023.4.0/tests/test_socketscpi.py` & `socketscpi-2023.6.0/tests/test_socketscpi.py`

 * *Files identical despite different names*

