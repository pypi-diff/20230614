# Comparing `tmp/bmw-lobster-core-0.9.4.tar.gz` & `tmp/bmw-lobster-core-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-core-0.9.4.tar", last modified: Tue Jun 13 09:18:56 2023, max compression
+gzip compressed data, was "bmw-lobster-core-0.9.5.tar", last modified: Wed Jun 14 14:03:19 2023, max compression
```

## Comparing `bmw-lobster-core-0.9.4.tar` & `bmw-lobster-core-0.9.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.189235 bmw-lobster-core-0.9.4/
--rw-r--r--   0 florian   (1000) florian   (1000)     2695 2023-06-13 09:18:56.189235 bmw-lobster-core-0.9.4/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     1735 2023-06-13 09:17:37.000000 bmw-lobster-core-0.9.4/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.185235 bmw-lobster-core-0.9.4/bmw_lobster_core.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     2695 2023-06-13 09:18:56.000000 bmw-lobster-core-0.9.4/bmw_lobster_core.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      679 2023-06-13 09:18:56.000000 bmw-lobster-core-0.9.4/bmw_lobster_core.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-13 09:18:56.000000 bmw-lobster-core-0.9.4/bmw_lobster_core.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)      240 2023-06-13 09:18:56.000000 bmw-lobster-core-0.9.4/bmw_lobster_core.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-06-13 09:18:56.000000 bmw-lobster-core-0.9.4/bmw_lobster_core.egg-info/top_level.txt
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.189235 bmw-lobster-core-0.9.4/lobster/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/__init__.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.189235 bmw-lobster-core-0.9.4/lobster/config/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/config/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)     4161 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/config/lexer.py
--rw-r--r--   0 florian   (1000) florian   (1000)     9087 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/config/parser.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2501 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/errors.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1244 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/exceptions.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.189235 bmw-lobster-core-0.9.4/lobster/html/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/html/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2682 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/html/assets.py
--rw-r--r--   0 florian   (1000) florian   (1000)     9667 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/html/htmldoc.py
--rw-r--r--   0 florian   (1000) florian   (1000)     4402 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/io.py
--rw-r--r--   0 florian   (1000) florian   (1000)    11205 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/items.py
--rw-r--r--   0 florian   (1000) florian   (1000)     7162 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/location.py
--rw-r--r--   0 florian   (1000) florian   (1000)     8158 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/report.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.185235 bmw-lobster-core-0.9.4/lobster/tools/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.189235 bmw-lobster-core-0.9.4/lobster/tools/core/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/tools/core/__init__.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     1917 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/tools/core/ci_report.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)    15951 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/tools/core/html_report.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     3707 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/tools/core/online_report.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     1818 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/tools/core/report.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1026 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/version.py
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-13 09:18:56.189235 bmw-lobster-core-0.9.4/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2514 2023-06-13 09:17:37.000000 bmw-lobster-core-0.9.4/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:19.117634 bmw-lobster-core-0.9.5/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2695 2023-06-14 14:03:19.117634 bmw-lobster-core-0.9.5/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     1735 2023-06-13 09:17:37.000000 bmw-lobster-core-0.9.5/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:19.113634 bmw-lobster-core-0.9.5/bmw_lobster_core.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2695 2023-06-14 14:03:19.000000 bmw-lobster-core-0.9.5/bmw_lobster_core.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      679 2023-06-14 14:03:19.000000 bmw-lobster-core-0.9.5/bmw_lobster_core.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-14 14:03:19.000000 bmw-lobster-core-0.9.5/bmw_lobster_core.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)      240 2023-06-14 14:03:19.000000 bmw-lobster-core-0.9.5/bmw_lobster_core.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-06-14 14:03:19.000000 bmw-lobster-core-0.9.5/bmw_lobster_core.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:19.113634 bmw-lobster-core-0.9.5/lobster/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:18.000000 bmw-lobster-core-0.9.5/lobster/__init__.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:19.113634 bmw-lobster-core-0.9.5/lobster/config/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:18.000000 bmw-lobster-core-0.9.5/lobster/config/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     4161 2023-06-14 14:03:18.000000 bmw-lobster-core-0.9.5/lobster/config/lexer.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     9087 2023-06-14 14:03:18.000000 bmw-lobster-core-0.9.5/lobster/config/parser.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2501 2023-06-14 14:03:18.000000 bmw-lobster-core-0.9.5/lobster/errors.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1244 2023-06-14 14:03:18.000000 bmw-lobster-core-0.9.5/lobster/exceptions.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:19.117634 bmw-lobster-core-0.9.5/lobster/html/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:18.000000 bmw-lobster-core-0.9.5/lobster/html/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2682 2023-06-14 14:03:18.000000 bmw-lobster-core-0.9.5/lobster/html/assets.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     9667 2023-06-14 14:03:18.000000 bmw-lobster-core-0.9.5/lobster/html/htmldoc.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     4402 2023-06-14 14:03:18.000000 bmw-lobster-core-0.9.5/lobster/io.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    11205 2023-06-14 14:03:18.000000 bmw-lobster-core-0.9.5/lobster/items.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     7684 2023-06-14 14:03:18.000000 bmw-lobster-core-0.9.5/lobster/location.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     8158 2023-06-14 14:03:18.000000 bmw-lobster-core-0.9.5/lobster/report.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:19.113634 bmw-lobster-core-0.9.5/lobster/tools/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:19.117634 bmw-lobster-core-0.9.5/lobster/tools/core/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:18.000000 bmw-lobster-core-0.9.5/lobster/tools/core/__init__.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     1917 2023-06-14 14:03:18.000000 bmw-lobster-core-0.9.5/lobster/tools/core/ci_report.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)    15951 2023-06-14 14:03:18.000000 bmw-lobster-core-0.9.5/lobster/tools/core/html_report.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     3707 2023-06-14 14:03:18.000000 bmw-lobster-core-0.9.5/lobster/tools/core/online_report.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     1818 2023-06-14 14:03:18.000000 bmw-lobster-core-0.9.5/lobster/tools/core/report.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1026 2023-06-14 14:03:18.000000 bmw-lobster-core-0.9.5/lobster/version.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-14 14:03:19.117634 bmw-lobster-core-0.9.5/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2514 2023-06-13 09:17:37.000000 bmw-lobster-core-0.9.5/setup.py
```

### Comparing `bmw-lobster-core-0.9.4/PKG-INFO` & `bmw-lobster-core-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-core
-Version: 0.9.4
+Version: 0.9.5
 Summary: Lightweight Open BMW Software Traceability Evidence Report
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-core-0.9.4/README.md` & `bmw-lobster-core-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.4/bmw_lobster_core.egg-info/PKG-INFO` & `bmw-lobster-core-0.9.5/bmw_lobster_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-core
-Version: 0.9.4
+Version: 0.9.5
 Summary: Lightweight Open BMW Software Traceability Evidence Report
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-core-0.9.4/bmw_lobster_core.egg-info/SOURCES.txt` & `bmw-lobster-core-0.9.5/bmw_lobster_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.4/lobster/config/lexer.py` & `bmw-lobster-core-0.9.5/lobster/config/lexer.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.4/lobster/config/parser.py` & `bmw-lobster-core-0.9.5/lobster/config/parser.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.4/lobster/errors.py` & `bmw-lobster-core-0.9.5/lobster/errors.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.4/lobster/exceptions.py` & `bmw-lobster-core-0.9.5/lobster/exceptions.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.4/lobster/html/assets.py` & `bmw-lobster-core-0.9.5/lobster/html/assets.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.4/lobster/html/htmldoc.py` & `bmw-lobster-core-0.9.5/lobster/html/htmldoc.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.4/lobster/io.py` & `bmw-lobster-core-0.9.5/lobster/io.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.4/lobster/items.py` & `bmw-lobster-core-0.9.5/lobster/items.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.4/lobster/location.py` & `bmw-lobster-core-0.9.5/lobster/location.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 #
 # You should have received a copy of the GNU Affero General Public
 # License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
 from abc import ABCMeta, abstractmethod
 
+import html
+
 from lobster.exceptions import LOBSTER_Exception
 
 
 class Location(metaclass=ABCMeta):
     @abstractmethod
     def to_string(self):
         pass
@@ -47,27 +49,49 @@
         try:
             if json["kind"] == "file":
                 return File_Reference.from_json(json)
             elif json["kind"] == "github":
                 return Github_Reference.from_json(json)
             elif json["kind"] == "codebeamer":
                 return Codebeamer_Reference.from_json(json)
+            elif json["kind"] == "void":
+                return Void_Reference.from_json(json)
             else:
                 raise LOBSTER_Exception("unknown location kind %s" %
                                         json["kind"])
         except KeyError as err:
             raise LOBSTER_Exception(
                 "malformed location data, missing %s" % err.args[0],
                 json) from err
         except AssertionError:
             raise LOBSTER_Exception(
                 "malformed %s location data" % json["kind"],
                 json) from err
 
 
+class Void_Reference(Location):
+    def __init__(self):
+        pass
+
+    def to_string(self):
+        return "<unknown location>"
+
+    def to_html(self):
+        return html.escape(self.to_string())
+
+    def to_json(self):
+        return {"kind": "void"}
+
+    @classmethod
+    def from_json(cls, json):
+        assert isinstance(json, dict)
+        assert json["kind"] == "void"
+        return Void_Reference()
+
+
 class File_Reference(Location):
     def __init__(self, filename, line=None, column=None):
         assert isinstance(filename, str)
         assert line is None or (isinstance(line, int) and
                                 line >= 1)
         assert column is None or (line is not None and
                                   isinstance(column, int) and
```

### Comparing `bmw-lobster-core-0.9.4/lobster/report.py` & `bmw-lobster-core-0.9.5/lobster/report.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.4/lobster/tools/core/ci_report.py` & `bmw-lobster-core-0.9.5/lobster/tools/core/ci_report.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.4/lobster/tools/core/html_report.py` & `bmw-lobster-core-0.9.5/lobster/tools/core/html_report.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.4/lobster/tools/core/online_report.py` & `bmw-lobster-core-0.9.5/lobster/tools/core/online_report.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.4/lobster/tools/core/report.py` & `bmw-lobster-core-0.9.5/lobster/tools/core/report.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.4/lobster/version.py` & `bmw-lobster-core-0.9.5/lobster/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public
 # License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
-VERSION_TUPLE = (0, 9, 4)
+VERSION_TUPLE = (0, 9, 5)
 VERSION_SUFFIX = ""
 
 LOBSTER_VERSION = ("%u.%u.%u" % VERSION_TUPLE) + \
     ("-%s" % VERSION_SUFFIX if VERSION_SUFFIX else "")
 
 FULL_NAME = "LOBSTER %s" % LOBSTER_VERSION
```

### Comparing `bmw-lobster-core-0.9.4/setup.py` & `bmw-lobster-core-0.9.5/setup.py`

 * *Files identical despite different names*

