# Comparing `tmp/microviewer-1.1.0.tar.gz` & `tmp/microviewer-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microviewer-1.1.0.tar", last modified: Wed Jun 14 17:27:26 2023, max compression
+gzip compressed data, was "microviewer-1.1.1.tar", last modified: Wed Jun 14 17:41:56 2023, max compression
```

## Comparing `microviewer-1.1.0.tar` & `microviewer-1.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-14 17:27:26.025618 microviewer-1.1.0/
--rw-r--r--   0 wms        (501) staff       (20)       52 2023-06-14 17:27:25.000000 microviewer-1.1.0/AUTHORS
--rw-r--r--   0 wms        (501) staff       (20)      664 2023-06-14 17:27:25.000000 microviewer-1.1.0/ChangeLog
--rw-r--r--   0 wms        (501) staff       (20)    26526 2023-06-05 21:07:17.000000 microviewer-1.1.0/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)     2423 2023-06-14 17:27:26.025750 microviewer-1.1.0/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)     1409 2023-06-14 17:26:48.000000 microviewer-1.1.0/README.md
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-14 17:27:26.023379 microviewer-1.1.0/microviewer/
--rw-r--r--   0 wms        (501) staff       (20)     5049 2023-06-14 17:22:52.000000 microviewer-1.1.0/microviewer/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)    34702 2023-06-14 17:25:16.000000 microviewer-1.1.0/microviewer/datacube.js
--rw-r--r--   0 wms        (501) staff       (20)     1911 2023-06-05 21:09:00.000000 microviewer-1.1.0/microviewer/favicon.ico
--rw-r--r--   0 wms        (501) staff       (20)    18826 2023-06-06 15:06:58.000000 microviewer-1.1.0/microviewer/index.html
--rw-r--r--   0 wms        (501) staff       (20)    87462 2023-06-06 04:26:20.000000 microviewer-1.1.0/microviewer/jquery-3.7.0.min.js
--rw-r--r--   0 wms        (501) staff       (20)       11 2023-06-06 04:58:06.000000 microviewer-1.1.0/microviewer/requirements.txt
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-14 17:27:26.024893 microviewer-1.1.0/microviewer.egg-info/
--rw-r--r--   0 wms        (501) staff       (20)     2423 2023-06-14 17:27:25.000000 microviewer-1.1.0/microviewer.egg-info/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)      516 2023-06-14 17:27:26.000000 microviewer-1.1.0/microviewer.egg-info/SOURCES.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-14 17:27:25.000000 microviewer-1.1.0/microviewer.egg-info/dependency_links.txt
--rw-r--r--   0 wms        (501) staff       (20)       47 2023-06-14 17:27:25.000000 microviewer-1.1.0/microviewer.egg-info/entry_points.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-06 04:24:32.000000 microviewer-1.1.0/microviewer.egg-info/not-zip-safe
--rw-r--r--   0 wms        (501) staff       (20)       46 2023-06-14 17:27:25.000000 microviewer-1.1.0/microviewer.egg-info/pbr.json
--rw-r--r--   0 wms        (501) staff       (20)       28 2023-06-14 17:27:25.000000 microviewer-1.1.0/microviewer.egg-info/top_level.txt
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-14 17:27:26.025439 microviewer-1.1.0/microviewer_cli/
--rw-r--r--   0 wms        (501) staff       (20)       18 2023-06-06 04:44:54.000000 microviewer-1.1.0/microviewer_cli/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     1911 2023-06-14 17:24:30.000000 microviewer-1.1.0/microviewer_cli/cli.py
--rw-r--r--   0 wms        (501) staff       (20)   220312 2023-06-06 07:35:34.000000 microviewer-1.1.0/seg-demo.png
--rw-r--r--   0 wms        (501) staff       (20)     1032 2023-06-14 17:27:26.026211 microviewer-1.1.0/setup.cfg
--rw-r--r--   0 wms        (501) staff       (20)      225 2023-06-06 04:44:08.000000 microviewer-1.1.0/setup.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-14 17:41:56.541316 microviewer-1.1.1/
+-rw-r--r--   0 wms        (501) staff       (20)       52 2023-06-14 17:41:56.000000 microviewer-1.1.1/AUTHORS
+-rw-r--r--   0 wms        (501) staff       (20)      711 2023-06-14 17:41:56.000000 microviewer-1.1.1/ChangeLog
+-rw-r--r--   0 wms        (501) staff       (20)    26526 2023-06-05 21:07:17.000000 microviewer-1.1.1/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)     2423 2023-06-14 17:41:56.541438 microviewer-1.1.1/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)     1409 2023-06-14 17:26:48.000000 microviewer-1.1.1/README.md
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-14 17:41:56.539102 microviewer-1.1.1/microviewer/
+-rw-r--r--   0 wms        (501) staff       (20)     5201 2023-06-14 17:36:31.000000 microviewer-1.1.1/microviewer/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)    34702 2023-06-14 17:25:16.000000 microviewer-1.1.1/microviewer/datacube.js
+-rw-r--r--   0 wms        (501) staff       (20)     1911 2023-06-05 21:09:00.000000 microviewer-1.1.1/microviewer/favicon.ico
+-rw-r--r--   0 wms        (501) staff       (20)    18700 2023-06-14 17:40:54.000000 microviewer-1.1.1/microviewer/index.html
+-rw-r--r--   0 wms        (501) staff       (20)    87462 2023-06-06 04:26:20.000000 microviewer-1.1.1/microviewer/jquery-3.7.0.min.js
+-rw-r--r--   0 wms        (501) staff       (20)       11 2023-06-06 04:58:06.000000 microviewer-1.1.1/microviewer/requirements.txt
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-14 17:41:56.540699 microviewer-1.1.1/microviewer.egg-info/
+-rw-r--r--   0 wms        (501) staff       (20)     2423 2023-06-14 17:41:56.000000 microviewer-1.1.1/microviewer.egg-info/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)      516 2023-06-14 17:41:56.000000 microviewer-1.1.1/microviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-14 17:41:56.000000 microviewer-1.1.1/microviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 wms        (501) staff       (20)       47 2023-06-14 17:41:56.000000 microviewer-1.1.1/microviewer.egg-info/entry_points.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-06 04:24:32.000000 microviewer-1.1.1/microviewer.egg-info/not-zip-safe
+-rw-r--r--   0 wms        (501) staff       (20)       46 2023-06-14 17:41:56.000000 microviewer-1.1.1/microviewer.egg-info/pbr.json
+-rw-r--r--   0 wms        (501) staff       (20)       28 2023-06-14 17:41:56.000000 microviewer-1.1.1/microviewer.egg-info/top_level.txt
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-14 17:41:56.541175 microviewer-1.1.1/microviewer_cli/
+-rw-r--r--   0 wms        (501) staff       (20)       18 2023-06-06 04:44:54.000000 microviewer-1.1.1/microviewer_cli/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     2024 2023-06-14 17:34:58.000000 microviewer-1.1.1/microviewer_cli/cli.py
+-rw-r--r--   0 wms        (501) staff       (20)   220312 2023-06-06 07:35:34.000000 microviewer-1.1.1/seg-demo.png
+-rw-r--r--   0 wms        (501) staff       (20)     1032 2023-06-14 17:41:56.541876 microviewer-1.1.1/setup.cfg
+-rw-r--r--   0 wms        (501) staff       (20)      225 2023-06-06 04:44:08.000000 microviewer-1.1.1/setup.py
```

### Comparing `microviewer-1.1.0/ChangeLog` & `microviewer-1.1.1/ChangeLog`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+1.1.1
+-----
+
+* fix: better filenames in title
+
 1.1.0
 -----
 
 * docs: note that nii is supported
 * fix: hyperview working, supported in CLI
 * feat: support NIFTI images if nibabel is installed
 * feat: silence logging
```

### Comparing `microviewer-1.1.0/LICENSE` & `microviewer-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `microviewer-1.1.0/PKG-INFO` & `microviewer-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microviewer
-Version: 1.1.0
+Version: 1.1.1
 Summary: Visualize 3D numpy arrays in the browser.
 Home-page: https://github.com/seung-lab/microviewer/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `microviewer-1.1.0/README.md` & `microviewer-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `microviewer-1.1.0/microviewer/__init__.py` & `microviewer-1.1.1/microviewer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,25 +35,30 @@
 ):
 
   img = to3d(img)
   seg = to3d(seg)
 
   assert np.all(img.shape[:3] == seg.shape[:3])
 
+  if isinstance(cloudpath, list):
+    cloudpath_img, cloudpath_seg = cloudpath
+  else:
+    cloudpath_img, cloudpath_seg = cloudpath, cloudpath
+
   img_data = {
     "img": img,
-    "cloudpath": cloudpath,
+    "cloudpath": cloudpath_img,
     "resolution": resolution,
     "layer_type": 'image',
     "offset": offset,
   }
 
   seg_data = {
     "img": seg,
-    "cloudpath": cloudpath,
+    "cloudpath": cloudpath_seg,
     "resolution": resolution,
     "layer_type": 'segmentation',
     "offset": offset,
   }
 
   return run([ img_data, seg_data ], hostname=hostname, port=port, browser=browser)
```

### Comparing `microviewer-1.1.0/microviewer/datacube.js` & `microviewer-1.1.1/microviewer/datacube.js`

 * *Files identical despite different names*

### Comparing `microviewer-1.1.0/microviewer/favicon.ico` & `microviewer-1.1.1/microviewer/favicon.ico`

 * *Files identical despite different names*

### Comparing `microviewer-1.1.0/microviewer/index.html` & `microviewer-1.1.1/microviewer/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -477,18 +477,15 @@
         let hyper = (PARAMETERS.viewtype === 'hyper') ? 'Hyper ' : '';
         let firstlayer = PARAMETERS.cloudpath[0];
 
         if (firstlayer === 'IN MEMORY') {
           document.title = `MEMORY - ${hyper}μViewer`;
         }
         else if (firstlayer) {
-          let layername = firstlayer.split('/');
-          layername = layername[ layername.length - 2 ] + '/' + layername[ layername.length - 1 ];
-
-          document.title = `${layername} - ${hyper}μViewer`;
+          document.title = `${PARAMETERS.cloudpath.join(" ; ")} - ${hyper}μViewer`;
         }
 
         elems.channel.css('width', SIZE.x + 'px').css('height', SIZE.y + 'px');
 
         let b = PARAMETERS.bounds;
         elems.cloudpath.text( PARAMETERS.cloudpath.join("; ") );
         elems.bounds.text(
```

### Comparing `microviewer-1.1.0/microviewer/jquery-3.7.0.min.js` & `microviewer-1.1.1/microviewer/jquery-3.7.0.min.js`

 * *Files identical despite different names*

### Comparing `microviewer-1.1.0/microviewer.egg-info/PKG-INFO` & `microviewer-1.1.1/microviewer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microviewer
-Version: 1.1.0
+Version: 1.1.1
 Summary: Visualize 3D numpy arrays in the browser.
 Home-page: https://github.com/seung-lab/microviewer/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `microviewer-1.1.0/microviewer.egg-info/SOURCES.txt` & `microviewer-1.1.1/microviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microviewer-1.1.0/microviewer_cli/cli.py` & `microviewer-1.1.1/microviewer_cli/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -59,21 +59,28 @@
 @click.option('--seg', is_flag=True, default=False, help="Display image as segmentation.", show_default=True)
 @click.option('--browser/--no-browser', default=True, is_flag=True, help="Open the dataset in the system's default web browser.", show_default=True)
 def main(image, segmentation, seg, browser):
   """
   View 3D images in the browser.
   """
   try:
-    image = load(image)
+    image_np = load(image)
     if segmentation:
-      segmentation = load(segmentation)
+      segmentation_np = load(segmentation)
   except ValueError:
     print("Data type not supported.")
     return
 
   if segmentation is not None:
-    microviewer.hyperview(image, segmentation, browser=browser)
+    microviewer.hyperview(
+      image_np, segmentation_np, 
+      browser=browser, 
+      cloudpath=[ image, segmentation ],
+    )
   else:
-    microviewer.view(image, seg=seg, browser=browser)
+    microviewer.view(
+      image_np, seg=seg, 
+      browser=browser, cloudpath=image
+    )
```

### Comparing `microviewer-1.1.0/seg-demo.png` & `microviewer-1.1.1/seg-demo.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.1.0/setup.cfg` & `microviewer-1.1.1/setup.cfg`

 * *Files identical despite different names*

