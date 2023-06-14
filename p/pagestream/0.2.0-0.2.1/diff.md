# Comparing `tmp/pagestream-0.2.0.tar.gz` & `tmp/pagestream-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pagestream-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pagestream-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pagestream-0.2.0.tar` & `pagestream-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       18 2023-01-10 15:37:06.079380 pagestream-0.2.0/.gitignore
--rw-r--r--   0        0        0     1080 2023-01-10 14:58:19.027912 pagestream-0.2.0/LICENSE
--rw-r--r--   0        0        0      624 2023-01-10 15:22:41.920947 pagestream-0.2.0/README.md
--rw-r--r--   0        0        0      487 2023-06-07 12:59:31.135307 pagestream-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2367 2023-06-07 14:50:42.907363 pagestream-0.2.0/src/pagestream/__init__.py
--rwxr-xr-x   0        0        0      700 2023-06-07 14:48:44.058259 pagestream-0.2.0/src/pagestream/cli.py
--rw-r--r--   0        0        0      993 1970-01-01 00:00:00.000000 pagestream-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       18 2023-01-10 15:37:06.079380 pagestream-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1080 2023-01-10 14:58:19.027912 pagestream-0.2.1/LICENSE
+-rw-r--r--   0        0        0      528 2023-06-07 14:55:50.163659 pagestream-0.2.1/README.md
+-rw-r--r--   0        0        0      487 2023-06-07 12:59:31.135307 pagestream-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2268 2023-06-14 09:44:24.392923 pagestream-0.2.1/src/pagestream/__init__.py
+-rwxr-xr-x   0        0        0      700 2023-06-13 12:23:09.526221 pagestream-0.2.1/src/pagestream/cli.py
+-rw-r--r--   0        0        0      897 1970-01-01 00:00:00.000000 pagestream-0.2.1/PKG-INFO
```

### Comparing `pagestream-0.2.0/LICENSE` & `pagestream-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pagestream-0.2.0/README.md` & `pagestream-0.2.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,11 @@
 This module was created to split these FOIA requests by outline. As an
 investigative journalism platform, we encounter different kinds of pagestreams
 in the wild. The intent for this module is to be a place where we collect
 different functionality regarding these streams.
 
 Example usage:
 ```
-stream = PDFPageStream("/path/to.pdf")
-
-if stream.can_extract_by_outline():
-    stream.extract_to("/output/path")
+pagestream --help
 ```
```

### Comparing `pagestream-0.2.0/src/pagestream/__init__.py` & `pagestream-0.2.1/src/pagestream/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from re import search
 from sys import setrecursionlimit
 from logging import info
 from pathlib import Path
 from pikepdf._qpdf import Pdf, Page
 
-__version__ = "v0.2.0"
+__version__ = "v0.2.1"
 
 # flatten function can recurse a lot, python limits this by default to not
 # cause overflows in the CPython implementation
 setrecursionlimit(1024 * 1024)
 
 class PDFPageStream:
     """Represents a PDF file that consists of a stream of merged PDF documents"""
@@ -24,36 +24,35 @@
             for item in outline.root:
                 item = item.to_dictionary_object(self.pdf)
 
                 # Could this be an actual embedded document?
                 title = item.get('/Title')
                 if title is None:
                     continue
-                # TODO - Intent here is to not extract single pages that are
-                # just named something like "page <x>", there's better ways to do this
-                regex = "|".join(['Pagina\s?\d+', 'Page\s?\d+', '_Pagina_'])
-                is_literal_page = search(regex, str(title)) is not None
-                is_single_page = item.get('/Count') is None
-                if is_literal_page and is_single_page:
-                    continue
 
-                # Create new PDF & append from src
-                pdf = Pdf.new()
-                with pdf.open_metadata() as meta:
-                    meta['dc:title'] = str(title)
-
-                if not is_single_page:
-                    next = item.get('/First')
-                    while next is not None:
-                        pdf.pages.append(Page(next.get('/Dest')[0]))
-                        next = next.get('/Next')
-                else:
-                    pdf.pages.append(Page(item.get('/A').get('/D')[0]))
+                # Some outlines are broken and dont have destination set
+                destination = item.get('/A').get('/D')[0]
+
+                if destination is not None:
+                    # First page
+                    first = Page(destination).index
+
+                    # last page is either the destination of the next outline item, or the last page of the document
+                    next = self.pdf.pages[-1].index
+                    if item.get('/Next') is not None and item.get('/Next').get('/A').get('/D')[0] is not None:
+                        next = Page(item.get('/Next').get('/A').get('/D')[0]).index
+
+                    pdf = Pdf.new()
+                    with pdf.open_metadata() as meta:
+                        meta['dc:title'] = str(title)
+
+                    for page in self.pdf.pages[first:next]:
+                        pdf.pages.append(page)
 
-                yield pdf
+                    yield pdf
 
     def extract_to(self, output_path):
         """Output split files into path"""
         if not output_path.exists():
             output_path.mkdir(parents=True)
 
         for pdf in self.get_embedded_documents():
```

### Comparing `pagestream-0.2.0/src/pagestream/cli.py` & `pagestream-0.2.1/src/pagestream/cli.py`

 * *Files identical despite different names*

### Comparing `pagestream-0.2.0/PKG-INFO` & `pagestream-0.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pagestream
-Version: 0.2.0
+Version: 0.2.1
 Summary: Handle PDF pagestreams with PikePDF and split them by outline
 Author-email: Johan Schuijt <johan@ftm.nl>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pikepdf
 Requires-Dist: click
 Project-URL: Home, https://github.com/followthemoney/pagestream
@@ -19,15 +19,12 @@
 This module was created to split these FOIA requests by outline. As an
 investigative journalism platform, we encounter different kinds of pagestreams
 in the wild. The intent for this module is to be a place where we collect
 different functionality regarding these streams.
 
 Example usage:
 ```
-stream = PDFPageStream("/path/to.pdf")
-
-if stream.can_extract_by_outline():
-    stream.extract_to("/output/path")
+pagestream --help
 ```
```

