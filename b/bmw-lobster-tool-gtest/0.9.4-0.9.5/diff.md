# Comparing `tmp/bmw-lobster-tool-gtest-0.9.4.tar.gz` & `tmp/bmw-lobster-tool-gtest-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-tool-gtest-0.9.4.tar", last modified: Tue Jun 13 09:18:57 2023, max compression
+gzip compressed data, was "bmw-lobster-tool-gtest-0.9.5.tar", last modified: Wed Jun 14 14:03:20 2023, max compression
```

## Comparing `bmw-lobster-tool-gtest-0.9.4.tar` & `bmw-lobster-tool-gtest-0.9.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:57.477253 bmw-lobster-tool-gtest-0.9.4/
--rw-r--r--   0 florian   (1000) florian   (1000)     1825 2023-06-13 09:18:57.477253 bmw-lobster-tool-gtest-0.9.4/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      828 2023-06-13 09:17:37.000000 bmw-lobster-tool-gtest-0.9.4/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:57.477253 bmw-lobster-tool-gtest-0.9.4/bmw_lobster_tool_gtest.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     1825 2023-06-13 09:18:57.000000 bmw-lobster-tool-gtest-0.9.4/bmw_lobster_tool_gtest.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      357 2023-06-13 09:18:57.000000 bmw-lobster-tool-gtest-0.9.4/bmw_lobster_tool_gtest.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-13 09:18:57.000000 bmw-lobster-tool-gtest-0.9.4/bmw_lobster_tool_gtest.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       65 2023-06-13 09:18:57.000000 bmw-lobster-tool-gtest-0.9.4/bmw_lobster_tool_gtest.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       24 2023-06-13 09:18:57.000000 bmw-lobster-tool-gtest-0.9.4/bmw_lobster_tool_gtest.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-06-13 09:18:57.000000 bmw-lobster-tool-gtest-0.9.4/bmw_lobster_tool_gtest.egg-info/top_level.txt
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:57.477253 bmw-lobster-tool-gtest-0.9.4/lobster/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:57.477253 bmw-lobster-tool-gtest-0.9.4/lobster/tools/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:57.477253 bmw-lobster-tool-gtest-0.9.4/lobster/tools/gtest/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:57.000000 bmw-lobster-tool-gtest-0.9.4/lobster/tools/gtest/__init__.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     5529 2023-06-13 09:18:57.000000 bmw-lobster-tool-gtest-0.9.4/lobster/tools/gtest/gtest.py
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-13 09:18:57.477253 bmw-lobster-tool-gtest-0.9.4/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2231 2023-05-08 15:03:18.000000 bmw-lobster-tool-gtest-0.9.4/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:20.365656 bmw-lobster-tool-gtest-0.9.5/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1825 2023-06-14 14:03:20.365656 bmw-lobster-tool-gtest-0.9.5/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      828 2023-06-13 09:17:37.000000 bmw-lobster-tool-gtest-0.9.5/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:20.365656 bmw-lobster-tool-gtest-0.9.5/bmw_lobster_tool_gtest.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1825 2023-06-14 14:03:20.000000 bmw-lobster-tool-gtest-0.9.5/bmw_lobster_tool_gtest.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      357 2023-06-14 14:03:20.000000 bmw-lobster-tool-gtest-0.9.5/bmw_lobster_tool_gtest.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-14 14:03:20.000000 bmw-lobster-tool-gtest-0.9.5/bmw_lobster_tool_gtest.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       65 2023-06-14 14:03:20.000000 bmw-lobster-tool-gtest-0.9.5/bmw_lobster_tool_gtest.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       24 2023-06-14 14:03:20.000000 bmw-lobster-tool-gtest-0.9.5/bmw_lobster_tool_gtest.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-06-14 14:03:20.000000 bmw-lobster-tool-gtest-0.9.5/bmw_lobster_tool_gtest.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:20.361656 bmw-lobster-tool-gtest-0.9.5/lobster/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:20.361656 bmw-lobster-tool-gtest-0.9.5/lobster/tools/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:20.365656 bmw-lobster-tool-gtest-0.9.5/lobster/tools/gtest/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:20.000000 bmw-lobster-tool-gtest-0.9.5/lobster/tools/gtest/__init__.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     5739 2023-06-14 14:03:20.000000 bmw-lobster-tool-gtest-0.9.5/lobster/tools/gtest/gtest.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-14 14:03:20.365656 bmw-lobster-tool-gtest-0.9.5/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2231 2023-05-08 15:03:18.000000 bmw-lobster-tool-gtest-0.9.5/setup.py
```

### Comparing `bmw-lobster-tool-gtest-0.9.4/PKG-INFO` & `bmw-lobster-tool-gtest-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-gtest
-Version: 0.9.4
+Version: 0.9.5
 Summary: LOBSTER Tool for GoogleTest
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-tool-gtest-0.9.4/README.md` & `bmw-lobster-tool-gtest-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `bmw-lobster-tool-gtest-0.9.4/bmw_lobster_tool_gtest.egg-info/PKG-INFO` & `bmw-lobster-tool-gtest-0.9.5/bmw_lobster_tool_gtest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-gtest
-Version: 0.9.4
+Version: 0.9.5
 Summary: LOBSTER Tool for GoogleTest
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-tool-gtest-0.9.4/lobster/tools/gtest/gtest.py` & `bmw-lobster-tool-gtest-0.9.5/lobster/tools/gtest/gtest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 import sys
 import argparse
 import os.path
 import xml.etree.ElementTree as ET
 
 from lobster.items import Tracing_Tag, Activity
-from lobster.location import File_Reference
+from lobster.location import Void_Reference, File_Reference
 from lobster.io import lobster_write
 
 
 def main():
     ap = argparse.ArgumentParser()
     ap.add_argument("files",
                     nargs="+",
@@ -76,16 +76,18 @@
             suite_name = suite.attrib["name"]
             for testcase in suite:
                 assert testcase.tag == "testcase"
                 test_name     = testcase.attrib["name"]
                 test_executed = testcase.attrib["status"] == "run"
                 test_ok       = True
                 test_tags     = []
-                source_file   = testcase.attrib["file"]
-                source_line   = int(testcase.attrib["line"])
+                source_file   = testcase.attrib.get("file", None)
+                source_line   = int(testcase.attrib["line"]) \
+                    if "line" in testcase.attrib \
+                    else None
                 for props in testcase:
                     if props.tag == "failure":
                         test_ok = False
                     elif props.tag == "properties":
                         for prop in props:
                             assert prop.tag == "property"
                             if prop.attrib["name"] == "lobster-tracing":
@@ -98,14 +100,16 @@
                                 source_line = int(prop.attrib["value"])
 
                 if source_file in c_files_rel and \
                    len(c_files_rel[source_file]) == 1:
                     test_source = File_Reference(
                         filename = list(c_files_rel[source_file])[0],
                         line     = source_line)
+                elif source_file is None:
+                    test_source = Void_Reference()
                 else:
                     test_source = File_Reference(
                         filename = source_file,
                         line     = source_line)
 
                 uid = "%s:%s" % (suite_name, test_name)
                 if test_executed:
@@ -129,13 +133,13 @@
 
     if options.out:
         with open(options.out, "w", encoding="UTF-8") as fd:
             lobster_write(fd, Activity, "lobster_gtest", items)
         print("Written output for %u items to %s" % (len(items),
                                                      options.out))
     else:
-        lobster_write(fd, Activity, "lobster_gtest", items)
+        lobster_write(sys.stdout, Activity, "lobster_gtest", items)
         print()
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `bmw-lobster-tool-gtest-0.9.4/setup.py` & `bmw-lobster-tool-gtest-0.9.5/setup.py`

 * *Files identical despite different names*

