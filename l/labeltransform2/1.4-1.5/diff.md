# Comparing `tmp/labeltransform2-1.4.tar.gz` & `tmp/labeltransform2-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labeltransform2-1.4.tar", last modified: Wed Jun 14 08:59:48 2023, max compression
+gzip compressed data, was "labeltransform2-1.5.tar", last modified: Wed Jun 14 09:13:14 2023, max compression
```

## Comparing `labeltransform2-1.4.tar` & `labeltransform2-1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 08:59:48.653375 labeltransform2-1.4/
--rw-rw-rw-   0        0        0    11558 2023-06-14 02:18:41.000000 labeltransform2-1.4/LICENSE
--rw-rw-rw-   0        0        0      179 2023-06-14 08:59:48.652383 labeltransform2-1.4/PKG-INFO
--rw-rw-rw-   0        0        0      961 2023-06-14 02:18:41.000000 labeltransform2-1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 08:59:48.639378 labeltransform2-1.4/labeltransform2/
--rw-rw-rw-   0        0        0       34 2023-06-14 07:41:09.000000 labeltransform2-1.4/labeltransform2/__init__.py
--rw-rw-rw-   0        0        0     4071 2023-06-14 08:56:53.000000 labeltransform2-1.4/labeltransform2/generate_voc.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:59:48.651381 labeltransform2-1.4/labeltransform2.egg-info/
--rw-rw-rw-   0        0        0      179 2023-06-14 08:59:48.000000 labeltransform2-1.4/labeltransform2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-06-14 08:59:48.000000 labeltransform2-1.4/labeltransform2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 08:59:48.000000 labeltransform2-1.4/labeltransform2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-14 08:59:48.000000 labeltransform2-1.4/labeltransform2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-14 08:59:48.000000 labeltransform2-1.4/labeltransform2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 08:59:48.653375 labeltransform2-1.4/setup.cfg
--rw-rw-rw-   0        0        0      302 2023-06-14 08:59:27.000000 labeltransform2-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:13:14.004530 labeltransform2-1.5/
+-rw-rw-rw-   0        0        0    11558 2023-06-14 02:18:41.000000 labeltransform2-1.5/LICENSE
+-rw-rw-rw-   0        0        0      225 2023-06-14 09:13:14.003531 labeltransform2-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      961 2023-06-14 02:18:41.000000 labeltransform2-1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 09:13:13.997533 labeltransform2-1.5/labeltransform2/
+-rw-rw-rw-   0        0        0       34 2023-06-14 07:41:09.000000 labeltransform2-1.5/labeltransform2/__init__.py
+-rw-rw-rw-   0        0        0     4345 2023-06-14 09:13:09.000000 labeltransform2-1.5/labeltransform2/generate_voc.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:13:14.002531 labeltransform2-1.5/labeltransform2.egg-info/
+-rw-rw-rw-   0        0        0      225 2023-06-14 09:13:13.000000 labeltransform2-1.5/labeltransform2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-06-14 09:13:13.000000 labeltransform2-1.5/labeltransform2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 09:13:13.000000 labeltransform2-1.5/labeltransform2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-14 09:13:13.000000 labeltransform2-1.5/labeltransform2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-14 09:13:13.000000 labeltransform2-1.5/labeltransform2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 09:13:14.004530 labeltransform2-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      348 2023-06-14 09:10:09.000000 labeltransform2-1.5/setup.py
```

### Comparing `labeltransform2-1.4/LICENSE` & `labeltransform2-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `labeltransform2-1.4/README.md` & `labeltransform2-1.5/README.md`

 * *Files identical despite different names*

### Comparing `labeltransform2-1.4/labeltransform2/generate_voc.py` & `labeltransform2-1.5/labeltransform2/generate_voc.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,22 @@
         name.text, xmin.text, ymin.text, xmax.text, ymax.text = bbox[1:]
         return obj
 
     def voc_2_yolo(self):
         self.names = self.names & [i.stem for i in self.img_dir.glob("*.jpg") if \
             self.img_dir.joinpath(i.stem + ".xml").exists()]
         assert len(self.names) > 0
-        for name in self.names:
+        n = len(self.names) // 5
+        name_list = [self.names[i*n:(i+1)*n if i<4 else -1] for i in range(5)]
+        for names in name_list:
+            task = Process(target=self.voc_2_yolo_, args=(names, ))
+            task.start()
+
+    def voc_2_yolo_(self, names):
+        for name in names:
             bboxes = self.parse(name)
             with open(self.img_dir.joinpath(name + ".txt"), "w")as f:
                 f.writelines(bboxes)
 
     def parse(self, name):
         anno = self.img_dir.joinpath(name + ".xml")
         tree = ET.parse(anno)
```

