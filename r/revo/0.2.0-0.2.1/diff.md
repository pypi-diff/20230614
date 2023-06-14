# Comparing `tmp/revo-0.2.0-py3-none-any.whl.zip` & `tmp/revo-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6476 bytes, number of entries: 7
+Zip file size: 6509 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       24 b- defN 23-May-29 11:26 revo/__init__.py
--rw-r--r--  2.0 unx     5476 b- defN 23-May-30 05:57 revo/_revo.py
--rw-r--r--  2.0 unx     1068 b- defN 23-May-30 07:02 revo-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     6600 b- defN 23-May-30 07:02 revo-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-30 07:02 revo-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-May-30 07:02 revo-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      511 b- defN 23-May-30 07:02 revo-0.2.0.dist-info/RECORD
-7 files, 13776 bytes uncompressed, 5576 bytes compressed:  59.5%
+-rw-r--r--  2.0 unx     5479 b- defN 23-Jun-14 05:36 revo/_revo.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jun-14 05:41 revo-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6672 b- defN 23-Jun-14 05:41 revo-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-14 05:41 revo-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-14 05:41 revo-0.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      511 b- defN 23-Jun-14 05:41 revo-0.2.1.dist-info/RECORD
+7 files, 13851 bytes uncompressed, 5609 bytes compressed:  59.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: revo/__init__.py
 Comment: 
 
 Filename: revo/_revo.py
 Comment: 
 
-Filename: revo-0.2.0.dist-info/LICENSE
+Filename: revo-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: revo-0.2.0.dist-info/METADATA
+Filename: revo-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: revo-0.2.0.dist-info/WHEEL
+Filename: revo-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: revo-0.2.0.dist-info/top_level.txt
+Filename: revo-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: revo-0.2.0.dist-info/RECORD
+Filename: revo-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## revo/_revo.py

```diff
@@ -150,15 +150,15 @@
             del self[key]
 
         # mercy on unresolved or illegal references?
         if not self.mercy:
             for key, val in self.melt():
                 if '$(' not in str(val):
                     continue
-                mo = re.search(r'(\$\(.+\))', val)
+                mo = re.search(r'(\$\([^)]+\))', val)
                 if not mo:
                     err = f'illegal reference "{val}" (from {key})'
                 else:
                     err = f'reference {mo.group(1)} unresolved (from {key})'
                 raise ValueError(err)
 
         return self
```

## Comparing `revo-0.2.0.dist-info/LICENSE` & `revo-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `revo-0.2.0.dist-info/METADATA` & `revo-0.2.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revo
-Version: 0.2.0
+Version: 0.2.1
 Summary: Referenced Values in Objects.
 Author-email: Sun Yijiang <sunyijiang@gmail.com>
 Project-URL: Homepage, https://github.com/sunyj/revo
 Project-URL: Bug Tracker, https://github.com/sunyj/revo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Revo – *Re*ferenced *V*alues in *O*bjects
 
 **Revo** is a non-intrusive variable substitution solution for config files.
 
+**Revo** is [listed on PyPI](https://pypi.org/project/revo/).
+
 **Revo** casts a Python built-in `dict` or `list` into a mutable tree, where the
 value of each tree node is either a string or a number, while any node can
 reference any other node in the tree with GNU make style `$(var)` variable
 syntax.
 
 Although a tiny (under 200 lines of code) library, **revo** provides some
 level of programmability to plain old Python objects and thus great
@@ -29,15 +31,15 @@
 variable substitution to it.
 
 
 # Design ideas
 
 **Revo** treats a Python built-in object as a tree of data, like an XML
 doc. The top-level object must be `dict` or `list`. Values on tree nodes must
-be either `str` or built-in number (`int` or `float`).
+be either `str`, `bool`, or built-in number (`int` or `float`).
 
 In order to reference *any* node in an object tree, we need to design a path
 mechanism. Yes, the idea is like [XPath](https://en.wikipedia.org/wiki/XPath)
 for Python objects, but much simpler.
 
 In fact, we can almost simply borrow the design of UNIX path: slash-separated
 string, with only a small adaptation: path segments in integer literals are
```

