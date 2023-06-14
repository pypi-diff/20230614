# Comparing `tmp/docmaptools-0.8.0.tar.gz` & `tmp/docmaptools-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmaptools-0.8.0.tar", last modified: Wed Jun  7 16:32:50 2023, max compression
+gzip compressed data, was "docmaptools-0.9.0.tar", last modified: Fri Jun  9 01:59:17 2023, max compression
```

## Comparing `docmaptools-0.8.0.tar` & `docmaptools-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-07 16:32:50.566735 docmaptools-0.8.0/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     1088 2023-06-07 16:32:18.000000 docmaptools-0.8.0/LICENSE
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       24 2023-06-07 16:32:18.000000 docmaptools-0.8.0/MANIFEST.in
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      643 2023-06-07 16:32:50.566735 docmaptools-0.8.0/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       90 2023-06-07 16:32:18.000000 docmaptools-0.8.0/README.md
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-07 16:32:50.566735 docmaptools-0.8.0/docmaptools/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      543 2023-06-07 16:32:18.000000 docmaptools-0.8.0/docmaptools/__init__.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     4796 2023-06-07 16:32:18.000000 docmaptools-0.8.0/docmaptools/convert.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     8585 2023-06-07 16:32:18.000000 docmaptools-0.8.0/docmaptools/parse.py
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-07 16:32:50.566735 docmaptools-0.8.0/docmaptools.egg-info/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      643 2023-06-07 16:32:50.000000 docmaptools-0.8.0/docmaptools.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      358 2023-06-07 16:32:50.000000 docmaptools-0.8.0/docmaptools.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)        1 2023-06-07 16:32:50.000000 docmaptools-0.8.0/docmaptools.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       20 2023-06-07 16:32:50.000000 docmaptools-0.8.0/docmaptools.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       12 2023-06-07 16:32:50.000000 docmaptools-0.8.0/docmaptools.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       78 2023-06-07 16:32:18.000000 docmaptools-0.8.0/requirements.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       38 2023-06-07 16:32:50.566735 docmaptools-0.8.0/setup.cfg
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      840 2023-06-07 16:32:18.000000 docmaptools-0.8.0/setup.py
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-07 16:32:50.566735 docmaptools-0.8.0/tests/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     8341 2023-06-07 16:32:18.000000 docmaptools-0.8.0/tests/test_convert.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      710 2023-06-07 16:32:18.000000 docmaptools-0.8.0/tests/test_init.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)    33743 2023-06-07 16:32:18.000000 docmaptools-0.8.0/tests/test_parse.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-09 01:59:17.421592 docmaptools-0.9.0/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     1088 2023-06-09 01:58:48.000000 docmaptools-0.9.0/LICENSE
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       24 2023-06-09 01:58:48.000000 docmaptools-0.9.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      643 2023-06-09 01:59:17.421592 docmaptools-0.9.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       90 2023-06-09 01:58:48.000000 docmaptools-0.9.0/README.md
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-09 01:59:17.421592 docmaptools-0.9.0/docmaptools/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      543 2023-06-09 01:58:48.000000 docmaptools-0.9.0/docmaptools/__init__.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     5318 2023-06-09 01:58:48.000000 docmaptools-0.9.0/docmaptools/convert.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     8585 2023-06-09 01:58:48.000000 docmaptools-0.9.0/docmaptools/parse.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-09 01:59:17.421592 docmaptools-0.9.0/docmaptools.egg-info/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      643 2023-06-09 01:59:17.000000 docmaptools-0.9.0/docmaptools.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      358 2023-06-09 01:59:17.000000 docmaptools-0.9.0/docmaptools.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)        1 2023-06-09 01:59:17.000000 docmaptools-0.9.0/docmaptools.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       20 2023-06-09 01:59:17.000000 docmaptools-0.9.0/docmaptools.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       12 2023-06-09 01:59:17.000000 docmaptools-0.9.0/docmaptools.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       78 2023-06-09 01:58:48.000000 docmaptools-0.9.0/requirements.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       38 2023-06-09 01:59:17.421592 docmaptools-0.9.0/setup.cfg
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      840 2023-06-09 01:58:48.000000 docmaptools-0.9.0/setup.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-09 01:59:17.421592 docmaptools-0.9.0/tests/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     8477 2023-06-09 01:58:48.000000 docmaptools-0.9.0/tests/test_convert.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      710 2023-06-09 01:58:48.000000 docmaptools-0.9.0/tests/test_init.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)    33743 2023-06-09 01:58:48.000000 docmaptools-0.9.0/tests/test_parse.py
```

### Comparing `docmaptools-0.8.0/LICENSE` & `docmaptools-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `docmaptools-0.8.0/PKG-INFO` & `docmaptools-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docmaptools
-Version: 0.8.0
+Version: 0.9.0
 Summary: Use DocMap content, generate JATS XML from it, and other utility functions.
 Home-page: https://github.com/elifesciences/docmap-tools
 Maintainer: eLife Sciences Publications Ltd.
 Maintainer-email: tech-team@elifesciences.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `docmaptools-0.8.0/docmaptools/__init__.py` & `docmaptools-0.9.0/docmaptools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 
 LOGGER = logging.getLogger(__name__)
 LOGGER.addHandler(logging.NullHandler())
 
 
 def configure_logging(filename, level=logging.INFO, format_string=None):
```

### Comparing `docmaptools-0.8.0/docmaptools/convert.py` & `docmaptools-0.9.0/docmaptools/convert.py`

 * *Files 16% similar despite different names*

```diff
@@ -72,14 +72,29 @@
             elem.set("{http://www.w3.org/1999/xlink}href", elem.get("src"))
             del elem.attrib["src"]
         # remove title attribute
         if elem.get("title"):
             del elem.attrib["title"]
     for elem in root.findall(".//li"):
         elem.tag = "list-item"
+        # copy the contnet to a p tag
+        p_tag = Element("p")
+        p_tag.text = elem.text
+        p_tag.tail = elem.tail
+        # remove old tag content
+        elem.text = None
+        elem.tail = None
+        # copy the tags to the p tag
+        for tag_index, child_tag in enumerate(elem.iterfind("*")):
+            # insert into the new tag
+            p_tag.insert(tag_index, child_tag)
+            # remove old tag
+            elem.remove(child_tag)
+        # insert the p tag
+        elem.insert(0, p_tag)
     for elem in root.findall(".//ol"):
         elem.tag = "list"
         elem.set("list-type", "order")
     for elem in root.findall(".//ul"):
         elem.tag = "list"
         elem.set("list-type", "bullet")
```

### Comparing `docmaptools-0.8.0/docmaptools/parse.py` & `docmaptools-0.9.0/docmaptools/parse.py`

 * *Files identical despite different names*

### Comparing `docmaptools-0.8.0/docmaptools.egg-info/PKG-INFO` & `docmaptools-0.9.0/docmaptools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docmaptools
-Version: 0.8.0
+Version: 0.9.0
 Summary: Use DocMap content, generate JATS XML from it, and other utility functions.
 Home-page: https://github.com/elifesciences/docmap-tools
 Maintainer: eLife Sciences Publications Ltd.
 Maintainer-email: tech-team@elifesciences.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `docmaptools-0.8.0/setup.py` & `docmaptools-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `docmaptools-0.8.0/tests/test_convert.py` & `docmaptools-0.9.0/tests/test_convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,23 +19,27 @@
         content = convert.convert_html_string(string)
         self.assertEqual(content, expected)
 
     def test_html_to_xml_edge_case(self):
         string = (
             b"<p>"
             b"<em><strong>Test</strong></em>"
-            b"<ul><li><em>dot</em></li></ul>"
+            b"<ul><li>Text <em><strong>dot</strong></em> tail</li></ul>"
             b"</p>"
         )
         expected = (
             b"<root>"
             b"<body>"
             b"<p>"
             b"<italic><bold>Test</bold></italic>"
-            b'<list list-type="bullet"><list-item><italic>dot</italic></list-item></list>'
+            b'<list list-type="bullet">'
+            b"<list-item>"
+            b"<p>Text <italic><bold>dot</bold></italic> tail</p>"
+            b"</list-item>"
+            b"</list>"
             b"</p></body>"
             b"</root>"
         )
         content = convert.convert_html_string(string)
         self.assertEqual(content, expected)
 
 
@@ -189,15 +193,15 @@
     def test_replace_tags_img(self):
         xml_string = b"<root><img/></root>"
         expected = b"<root><inline-graphic /></root>"
         self.assertEqual(invoke_module_function(xml_string, "replace_tags"), expected)
 
     def test_replace_tags_li(self):
         xml_string = b"<root><li/></root>"
-        expected = b"<root><list-item /></root>"
+        expected = b"<root><list-item><p /></list-item></root>"
         self.assertEqual(invoke_module_function(xml_string, "replace_tags"), expected)
 
     def test_replace_tags_ol(self):
         xml_string = b"<root><ol/></root>"
         expected = b'<root><list list-type="order" /></root>'
         self.assertEqual(invoke_module_function(xml_string, "replace_tags"), expected)
```

### Comparing `docmaptools-0.8.0/tests/test_init.py` & `docmaptools-0.9.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `docmaptools-0.8.0/tests/test_parse.py` & `docmaptools-0.9.0/tests/test_parse.py`

 * *Files identical despite different names*

