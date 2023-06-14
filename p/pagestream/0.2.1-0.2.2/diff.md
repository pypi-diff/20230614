# Comparing `tmp/pagestream-0.2.1.tar.gz` & `tmp/pagestream-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pagestream-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pagestream-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pagestream-0.2.1.tar` & `pagestream-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       18 2023-01-10 15:37:06.079380 pagestream-0.2.1/.gitignore
--rw-r--r--   0        0        0     1080 2023-01-10 14:58:19.027912 pagestream-0.2.1/LICENSE
--rw-r--r--   0        0        0      528 2023-06-07 14:55:50.163659 pagestream-0.2.1/README.md
--rw-r--r--   0        0        0      487 2023-06-07 12:59:31.135307 pagestream-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2268 2023-06-14 09:44:24.392923 pagestream-0.2.1/src/pagestream/__init__.py
--rwxr-xr-x   0        0        0      700 2023-06-13 12:23:09.526221 pagestream-0.2.1/src/pagestream/cli.py
--rw-r--r--   0        0        0      897 1970-01-01 00:00:00.000000 pagestream-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       18 2023-01-10 15:37:06.079380 pagestream-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1080 2023-01-10 14:58:19.027912 pagestream-0.2.2/LICENSE
+-rw-r--r--   0        0        0      528 2023-06-07 14:55:50.163659 pagestream-0.2.2/README.md
+-rw-r--r--   0        0        0      487 2023-06-07 12:59:31.135307 pagestream-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3053 2023-06-14 10:21:43.933785 pagestream-0.2.2/src/pagestream/__init__.py
+-rwxr-xr-x   0        0        0      700 2023-06-13 12:23:09.526221 pagestream-0.2.2/src/pagestream/cli.py
+-rw-r--r--   0        0        0      897 1970-01-01 00:00:00.000000 pagestream-0.2.2/PKG-INFO
```

### Comparing `pagestream-0.2.1/LICENSE` & `pagestream-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pagestream-0.2.1/README.md` & `pagestream-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pagestream-0.2.1/src/pagestream/__init__.py` & `pagestream-0.2.2/src/pagestream/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,46 +4,65 @@
 
 from re import search
 from sys import setrecursionlimit
 from logging import info
 from pathlib import Path
 from pikepdf._qpdf import Pdf, Page
 
-__version__ = "v0.2.1"
+__version__ = "v0.2.2"
 
 # flatten function can recurse a lot, python limits this by default to not
 # cause overflows in the CPython implementation
 setrecursionlimit(1024 * 1024)
 
 class PDFPageStream:
     """Represents a PDF file that consists of a stream of merged PDF documents"""
     def __init__(self, path: Path):
         self.pdf = Pdf.open(path)
 
+    @staticmethod
+    def get_destination(item):
+        if item.get('/Dest') is not None:
+            return item.get('/Dest')[0]
+        elif item.get('/A') is not None and item.get('/A').get('/D') is not None:
+            return item.get('/A').get('/D')[0]
+        else:
+            raise Exception('Outline item has no destination')
+
     def get_embedded_documents(self):
         with self.pdf.open_outline() as outline:
             for item in outline.root:
                 item = item.to_dictionary_object(self.pdf)
 
                 # Could this be an actual embedded document?
                 title = item.get('/Title')
                 if title is None:
                     continue
 
-                # Some outlines are broken and dont have destination set
-                destination = item.get('/A').get('/D')[0]
+                destination = PDFPageStream.get_destination(item)
 
+                # Some outlines are broken and don't have destination target set
                 if destination is not None:
                     # First page
                     first = Page(destination).index
 
                     # last page is either the destination of the next outline item, or the last page of the document
-                    next = self.pdf.pages[-1].index
-                    if item.get('/Next') is not None and item.get('/Next').get('/A').get('/D')[0] is not None:
-                        next = Page(item.get('/Next').get('/A').get('/D')[0]).index
+                    next = len(self.pdf.pages)
+                    if item.get('/Next') is not None:
+                        next_destination = PDFPageStream.get_destination(item.get('/Next'))
+                        if next_destination is not None:
+                            next = Page(next_destination).index
+
+                    # Is this just a "Page .." reference?
+                    regex = "|".join(['Pagina\s?\d+', 'Page\s?\d+', '_Pagina_'])
+                    is_literal_page = search(regex, str(title)) is not None
+                    is_single_page = next - first == 1
+
+                    if is_literal_page and is_single_page:
+                        continue
 
                     pdf = Pdf.new()
                     with pdf.open_metadata() as meta:
                         meta['dc:title'] = str(title)
 
                     for page in self.pdf.pages[first:next]:
                         pdf.pages.append(page)
```

### Comparing `pagestream-0.2.1/src/pagestream/cli.py` & `pagestream-0.2.2/src/pagestream/cli.py`

 * *Files identical despite different names*

### Comparing `pagestream-0.2.1/PKG-INFO` & `pagestream-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pagestream
-Version: 0.2.1
+Version: 0.2.2
 Summary: Handle PDF pagestreams with PikePDF and split them by outline
 Author-email: Johan Schuijt <johan@ftm.nl>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pikepdf
 Requires-Dist: click
 Project-URL: Home, https://github.com/followthemoney/pagestream
```

