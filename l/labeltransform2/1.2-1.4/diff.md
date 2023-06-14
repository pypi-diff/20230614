# Comparing `tmp/labeltransform2-1.2.tar.gz` & `tmp/labeltransform2-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labeltransform2-1.2.tar", last modified: Wed Jun 14 08:34:10 2023, max compression
+gzip compressed data, was "labeltransform2-1.4.tar", last modified: Wed Jun 14 08:59:48 2023, max compression
```

## Comparing `labeltransform2-1.2.tar` & `labeltransform2-1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 08:34:10.272167 labeltransform2-1.2/
--rw-rw-rw-   0        0        0    11558 2023-06-14 02:18:41.000000 labeltransform2-1.2/LICENSE
--rw-rw-rw-   0        0        0      179 2023-06-14 08:34:10.271166 labeltransform2-1.2/PKG-INFO
--rw-rw-rw-   0        0        0      961 2023-06-14 02:18:41.000000 labeltransform2-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 08:34:10.265168 labeltransform2-1.2/labeltransform2/
--rw-rw-rw-   0        0        0       34 2023-06-14 07:41:09.000000 labeltransform2-1.2/labeltransform2/__init__.py
--rw-rw-rw-   0        0        0     3622 2023-06-14 08:33:30.000000 labeltransform2-1.2/labeltransform2/generate_voc.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:34:10.270169 labeltransform2-1.2/labeltransform2.egg-info/
--rw-rw-rw-   0        0        0      179 2023-06-14 08:34:10.000000 labeltransform2-1.2/labeltransform2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-06-14 08:34:10.000000 labeltransform2-1.2/labeltransform2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 08:34:10.000000 labeltransform2-1.2/labeltransform2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-14 08:34:10.000000 labeltransform2-1.2/labeltransform2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-14 08:34:10.000000 labeltransform2-1.2/labeltransform2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 08:34:10.272167 labeltransform2-1.2/setup.cfg
--rw-rw-rw-   0        0        0      302 2023-06-14 08:34:05.000000 labeltransform2-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:59:48.653375 labeltransform2-1.4/
+-rw-rw-rw-   0        0        0    11558 2023-06-14 02:18:41.000000 labeltransform2-1.4/LICENSE
+-rw-rw-rw-   0        0        0      179 2023-06-14 08:59:48.652383 labeltransform2-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      961 2023-06-14 02:18:41.000000 labeltransform2-1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 08:59:48.639378 labeltransform2-1.4/labeltransform2/
+-rw-rw-rw-   0        0        0       34 2023-06-14 07:41:09.000000 labeltransform2-1.4/labeltransform2/__init__.py
+-rw-rw-rw-   0        0        0     4071 2023-06-14 08:56:53.000000 labeltransform2-1.4/labeltransform2/generate_voc.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:59:48.651381 labeltransform2-1.4/labeltransform2.egg-info/
+-rw-rw-rw-   0        0        0      179 2023-06-14 08:59:48.000000 labeltransform2-1.4/labeltransform2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-06-14 08:59:48.000000 labeltransform2-1.4/labeltransform2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 08:59:48.000000 labeltransform2-1.4/labeltransform2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-14 08:59:48.000000 labeltransform2-1.4/labeltransform2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-14 08:59:48.000000 labeltransform2-1.4/labeltransform2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 08:59:48.653375 labeltransform2-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      302 2023-06-14 08:59:27.000000 labeltransform2-1.4/setup.py
```

### Comparing `labeltransform2-1.2/LICENSE` & `labeltransform2-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `labeltransform2-1.2/README.md` & `labeltransform2-1.4/README.md`

 * *Files identical despite different names*

### Comparing `labeltransform2-1.2/labeltransform2/generate_voc.py` & `labeltransform2-1.4/labeltransform2/generate_voc.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,28 +12,34 @@
         self.img_dir = Path(img_dir)
         self.data = data
         self.data.columns = ["name", "cls", "x1", "y1", "x2", "y2"]
         self.names = list(set(self.data["name"].to_list()))
         self.cls_names = {}
     
 
-    def write(self):
-        for name in self.names:
-            print(name)
+    def write(self, names):
+        for name in names:
             tree, root, filename, width, height, depth, obj = self.style()
             img = self.img_dir.joinpath(name + ".jpg")
             filename.text = img.name
             cv_img = cv2.imread(img.__str__())
             h, w, c = cv_img.shape
             width.text, height.text, depth.text = str(w), str(h), str(c)
             bboxes = self.data[self.data["name"]==name].to_numpy()
             for bbox in bboxes:
                 obj_ = self.new_obj(obj, bbox)
                 root.append(obj_)
             tree.write(self.img_dir.joinpath(name + ".xml"))
+    
+    def to_voc(self):
+        n = len(self.names) // 5
+        name_list = [self.names[i*n:(i+1)*n if i<4 else -1] for i in range(5)]
+        for names in name_list:
+            task = Process(target=self.write, args=(names, ))
+            task.start()
                 
     def style(self):
         tree0 = ET.parse("./xml/voc.xml")
         tree = deepcopy(tree0)
         root = tree.getroot()
         filename = root.find("filename")
         size = root.find("size")
@@ -92,7 +98,16 @@
             w = x2 - x1
             h = y2 - y1
             bbox = [cx / width, cy / height, w / width, h / height]
             bbox = f"{cls} " + " ".join(list(map(lambda x: str(x), bbox))) + "\n"
             bboxes.append(bbox)
         
         return bboxes
+
+
+if __name__ == "__main__":
+    
+    names = list(range(1989))
+    n = len(names) // 5
+    name_list = [names[i*n:(i+1)*n if i<4 else -1] for i in range(5)]
+
+    print([len(i) for i in name_list])
```

