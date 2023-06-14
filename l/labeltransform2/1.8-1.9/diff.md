# Comparing `tmp/labeltransform2-1.8.tar.gz` & `tmp/labeltransform2-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labeltransform2-1.8.tar", last modified: Wed Jun 14 09:41:05 2023, max compression
+gzip compressed data, was "labeltransform2-1.9.tar", last modified: Wed Jun 14 09:45:26 2023, max compression
```

## Comparing `labeltransform2-1.8.tar` & `labeltransform2-1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 09:41:05.466852 labeltransform2-1.8/
--rw-rw-rw-   0        0        0    11558 2023-06-14 02:18:41.000000 labeltransform2-1.8/LICENSE
--rw-rw-rw-   0        0        0      225 2023-06-14 09:41:05.465843 labeltransform2-1.8/PKG-INFO
--rw-rw-rw-   0        0        0      961 2023-06-14 02:18:41.000000 labeltransform2-1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 09:41:05.459874 labeltransform2-1.8/labeltransform2/
--rw-rw-rw-   0        0        0       34 2023-06-14 07:41:09.000000 labeltransform2-1.8/labeltransform2/__init__.py
--rw-rw-rw-   0        0        0     4405 2023-06-14 09:40:50.000000 labeltransform2-1.8/labeltransform2/generate_voc.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:41:05.464845 labeltransform2-1.8/labeltransform2.egg-info/
--rw-rw-rw-   0        0        0      225 2023-06-14 09:41:05.000000 labeltransform2-1.8/labeltransform2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-06-14 09:41:05.000000 labeltransform2-1.8/labeltransform2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 09:41:05.000000 labeltransform2-1.8/labeltransform2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-14 09:41:05.000000 labeltransform2-1.8/labeltransform2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-14 09:41:05.000000 labeltransform2-1.8/labeltransform2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 09:41:05.466852 labeltransform2-1.8/setup.cfg
--rw-rw-rw-   0        0        0      348 2023-06-14 09:41:01.000000 labeltransform2-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:45:26.143720 labeltransform2-1.9/
+-rw-rw-rw-   0        0        0    11558 2023-06-14 02:18:41.000000 labeltransform2-1.9/LICENSE
+-rw-rw-rw-   0        0        0      225 2023-06-14 09:45:26.143720 labeltransform2-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      961 2023-06-14 02:18:41.000000 labeltransform2-1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 09:45:26.138717 labeltransform2-1.9/labeltransform2/
+-rw-rw-rw-   0        0        0       34 2023-06-14 07:41:09.000000 labeltransform2-1.9/labeltransform2/__init__.py
+-rw-rw-rw-   0        0        0     4410 2023-06-14 09:45:11.000000 labeltransform2-1.9/labeltransform2/generate_voc.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:45:26.142718 labeltransform2-1.9/labeltransform2.egg-info/
+-rw-rw-rw-   0        0        0      225 2023-06-14 09:45:26.000000 labeltransform2-1.9/labeltransform2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-06-14 09:45:26.000000 labeltransform2-1.9/labeltransform2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 09:45:26.000000 labeltransform2-1.9/labeltransform2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-14 09:45:26.000000 labeltransform2-1.9/labeltransform2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-14 09:45:26.000000 labeltransform2-1.9/labeltransform2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 09:45:26.143720 labeltransform2-1.9/setup.cfg
+-rw-rw-rw-   0        0        0      348 2023-06-14 09:42:41.000000 labeltransform2-1.9/setup.py
```

### Comparing `labeltransform2-1.8/LICENSE` & `labeltransform2-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `labeltransform2-1.8/README.md` & `labeltransform2-1.9/README.md`

 * *Files identical despite different names*

### Comparing `labeltransform2-1.8/labeltransform2/generate_voc.py` & `labeltransform2-1.9/labeltransform2/generate_voc.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         size = root.find("size")
         width = int(eval(size.find("width").text))
         height = int(eval(size.find("height").text))
         objs = root.findall("object")
         bboxes = []
 
         for obj in objs:
-            cls = obj.find("name")
+            cls = obj.find("name").text
             if cls in self.cls_names:
                 cls = self.cls_names[cls]
             else:
                 self.cls_names[cls] = len(self.cls_names)
                 cls = self.cls_names[cls]
             bndbox = obj.find("bndbox")
             x1 = int(eval(bndbox.find("xmin").text))
```

