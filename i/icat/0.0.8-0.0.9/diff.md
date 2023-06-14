# Comparing `tmp/icat-0.0.8.tar.gz` & `tmp/icat-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/gretchen/Dropbox/Projects/python/icat/dist/tmpaf0fm7bn/icat-0.0.8.tar", last modified: Tue Mar  2 20:54:38 2021, max compression
+gzip compressed data, was "/home/gretchen/Dropbox/Projects/python/icat/dist/tmpbm9pq3ef/icat-0.0.9.tar", last modified: Wed Mar  3 04:36:39 2021, max compression
```

## Comparing `icat-0.0.8.tar` & `icat-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 gretchen  (1000) gretchen  (1000)        0 2021-03-02 20:54:38.191934 icat-0.0.8/
--rw-rw-r--   0 gretchen  (1000) gretchen  (1000)      693 2021-03-02 20:54:38.191934 icat-0.0.8/PKG-INFO
--rw-rw-r--   0 gretchen  (1000) gretchen  (1000)      138 2021-03-02 14:06:21.000000 icat-0.0.8/README.md
-drwxrwxr-x   0 gretchen  (1000) gretchen  (1000)        0 2021-03-02 20:54:38.187934 icat-0.0.8/bin/
--rw-rw-r--   0 gretchen  (1000) gretchen  (1000)        0 2021-03-02 15:03:27.000000 icat-0.0.8/bin/__init__.py
--rwxrwxr-x   0 gretchen  (1000) gretchen  (1000)     9376 2021-03-02 20:53:09.000000 icat-0.0.8/bin/__main__.py
--rwxrwxr-x   0 gretchen  (1000) gretchen  (1000)     9308 2021-03-02 15:39:55.000000 icat-0.0.8/bin/icat
-drwxrwxr-x   0 gretchen  (1000) gretchen  (1000)        0 2021-03-02 20:54:38.191934 icat-0.0.8/icat.egg-info/
--rw-rw-r--   0 gretchen  (1000) gretchen  (1000)      693 2021-03-02 20:54:38.000000 icat-0.0.8/icat.egg-info/PKG-INFO
--rw-rw-r--   0 gretchen  (1000) gretchen  (1000)      196 2021-03-02 20:54:38.000000 icat-0.0.8/icat.egg-info/SOURCES.txt
--rw-rw-r--   0 gretchen  (1000) gretchen  (1000)        1 2021-03-02 20:54:38.000000 icat-0.0.8/icat.egg-info/dependency_links.txt
--rw-rw-r--   0 gretchen  (1000) gretchen  (1000)        4 2021-03-02 20:54:38.000000 icat-0.0.8/icat.egg-info/top_level.txt
--rw-rw-r--   0 gretchen  (1000) gretchen  (1000)      137 2021-03-02 14:01:34.000000 icat-0.0.8/pyproject.toml
--rw-rw-r--   0 gretchen  (1000) gretchen  (1000)      563 2021-03-02 20:54:38.191934 icat-0.0.8/setup.cfg
--rwxrwxr-x   0 gretchen  (1000) gretchen  (1000)       77 2021-03-02 15:51:39.000000 icat-0.0.8/setup.py
+drwxrwxr-x   0 gretchen  (1000) gretchen  (1000)        0 2021-03-03 04:36:39.836053 icat-0.0.9/
+-rw-rw-r--   0 gretchen  (1000) gretchen  (1000)      693 2021-03-03 04:36:39.836053 icat-0.0.9/PKG-INFO
+-rw-rw-r--   0 gretchen  (1000) gretchen  (1000)      138 2021-03-02 14:06:21.000000 icat-0.0.9/README.md
+drwxrwxr-x   0 gretchen  (1000) gretchen  (1000)        0 2021-03-03 04:36:39.836053 icat-0.0.9/bin/
+-rw-rw-r--   0 gretchen  (1000) gretchen  (1000)        0 2021-03-02 15:03:27.000000 icat-0.0.9/bin/__init__.py
+-rwxrwxr-x   0 gretchen  (1000) gretchen  (1000)     9435 2021-03-03 04:28:03.000000 icat-0.0.9/bin/__main__.py
+-rwxrwxr-x   0 gretchen  (1000) gretchen  (1000)     9435 2021-03-03 04:28:54.000000 icat-0.0.9/bin/icat
+drwxrwxr-x   0 gretchen  (1000) gretchen  (1000)        0 2021-03-03 04:36:39.836053 icat-0.0.9/icat.egg-info/
+-rw-rw-r--   0 gretchen  (1000) gretchen  (1000)      693 2021-03-03 04:36:39.000000 icat-0.0.9/icat.egg-info/PKG-INFO
+-rw-rw-r--   0 gretchen  (1000) gretchen  (1000)      196 2021-03-03 04:36:39.000000 icat-0.0.9/icat.egg-info/SOURCES.txt
+-rw-rw-r--   0 gretchen  (1000) gretchen  (1000)        1 2021-03-03 04:36:39.000000 icat-0.0.9/icat.egg-info/dependency_links.txt
+-rw-rw-r--   0 gretchen  (1000) gretchen  (1000)        4 2021-03-03 04:36:39.000000 icat-0.0.9/icat.egg-info/top_level.txt
+-rw-rw-r--   0 gretchen  (1000) gretchen  (1000)      137 2021-03-02 14:01:34.000000 icat-0.0.9/pyproject.toml
+-rw-rw-r--   0 gretchen  (1000) gretchen  (1000)      563 2021-03-03 04:36:39.836053 icat-0.0.9/setup.cfg
+-rwxrwxr-x   0 gretchen  (1000) gretchen  (1000)       77 2021-03-02 15:51:39.000000 icat-0.0.9/setup.py
```

### Comparing `icat-0.0.8/PKG-INFO` & `icat-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icat
-Version: 0.0.8
+Version: 0.0.9
 Summary: displays images on the terminal using  ANSI graphics
 Home-page: https://github.com/gretchycat/icat
 Author: Gretchen Maculo
 Author-email: gretchen.maculo@gmail.com
 License: UNKNOWN
 Description: # icat displays images on the terminal using ansi graphics
         # supports monochrome, 8 color, 16 color, 256 color and 24-bit color terminals
```

### Comparing `icat-0.0.8/bin/__main__.py` & `icat-0.0.9/bin/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,8 +328,9 @@
             help="Character set: utf8 | dos | ascii")
     (options, args)=parser.parse_args()
     if len(args)==0:
         parser.print_help()
     for imagefile in args:
         docat(imagefile, options.mode, int(options.width), options.half, options.charset)
 
-
+if __name__ == "__main__" or __name__ == "icat":
+    main()
```

### Comparing `icat-0.0.8/bin/icat` & `icat-0.0.9/bin/icat`

 * *Files 1% similar despite different names*

```diff
@@ -312,23 +312,25 @@
         c0=0
         if mode!='1bit' and mode!='bw':
             print("\x1b[0m")
         else:
             print('')
     img.close()
 
-parser=OptionParser(usage="usage: %prog [options] filelist")
-parser.add_option("-m", "--mode", dest="mode", default="24bit", 
-        help="Color mode: 24bit | 8bit | 8bitgrey | 4bit | 4bitgrey | 3bit | bw")
-parser.add_option("-w", "--width", dest="width", default="0",
-        help="0=auto, w>0 constrains image to the width")
-parser.add_option("-H", "--halfblock", dest="half", default="yes",
-        help="Use half-blocks: no | yes")
-parser.add_option("-c", "--charset", dest="charset", default="utf8",
-        help="Character set: utf8 | dos | ascii")
-(options, args)=parser.parse_args()
-if len(args)==0:
-    parser.print_help()
-for imagefile in args:
-    docat(imagefile, options.mode, int(options.width), options.half, options.charset)
-
+def main():
+    parser=OptionParser(usage="usage: %prog [options] filelist")
+    parser.add_option("-m", "--mode", dest="mode", default="24bit", 
+            help="Color mode: 24bit | 8bit | 8bitgrey | 4bit | 4bitgrey | 3bit | bw")
+    parser.add_option("-w", "--width", dest="width", default="0",
+            help="0=auto, w>0 constrains image to the width")
+    parser.add_option("-H", "--halfblock", dest="half", default="yes",
+            help="Use half-blocks: no | yes")
+    parser.add_option("-c", "--charset", dest="charset", default="utf8",
+            help="Character set: utf8 | dos | ascii")
+    (options, args)=parser.parse_args()
+    if len(args)==0:
+        parser.print_help()
+    for imagefile in args:
+        docat(imagefile, options.mode, int(options.width), options.half, options.charset)
 
+if __name__ == "__main__" or __name__ == "icat":
+    main()
```

### Comparing `icat-0.0.8/icat.egg-info/PKG-INFO` & `icat-0.0.9/icat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icat
-Version: 0.0.8
+Version: 0.0.9
 Summary: displays images on the terminal using  ANSI graphics
 Home-page: https://github.com/gretchycat/icat
 Author: Gretchen Maculo
 Author-email: gretchen.maculo@gmail.com
 License: UNKNOWN
 Description: # icat displays images on the terminal using ansi graphics
         # supports monochrome, 8 color, 16 color, 256 color and 24-bit color terminals
```

### Comparing `icat-0.0.8/setup.cfg` & `icat-0.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = icat
-version = 0.0.8
+version = 0.0.9
 url = https://github.com/gretchycat/icat
 author = Gretchen Maculo
 author_email = gretchen.maculo@gmail.com
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Operating System :: OS Independent
```

