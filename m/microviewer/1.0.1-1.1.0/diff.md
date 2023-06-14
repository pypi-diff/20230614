# Comparing `tmp/microviewer-1.0.1.tar.gz` & `tmp/microviewer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microviewer-1.0.1.tar", last modified: Wed Jun  7 02:03:41 2023, max compression
+gzip compressed data, was "microviewer-1.1.0.tar", last modified: Wed Jun 14 17:27:26 2023, max compression
```

## Comparing `microviewer-1.0.1.tar` & `microviewer-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-07 02:03:41.140790 microviewer-1.0.1/
--rw-r--r--   0 wms        (501) staff       (20)       52 2023-06-07 02:03:41.000000 microviewer-1.0.1/AUTHORS
--rw-r--r--   0 wms        (501) staff       (20)      495 2023-06-07 02:03:41.000000 microviewer-1.0.1/ChangeLog
--rw-r--r--   0 wms        (501) staff       (20)    26526 2023-06-05 21:07:17.000000 microviewer-1.0.1/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)     2372 2023-06-07 02:03:41.140973 microviewer-1.0.1/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)     1358 2023-06-06 15:00:16.000000 microviewer-1.0.1/README.md
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-07 02:03:41.138120 microviewer-1.0.1/microviewer/
--rw-r--r--   0 wms        (501) staff       (20)     5037 2023-06-06 05:31:02.000000 microviewer-1.0.1/microviewer/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)    34702 2023-06-06 19:11:19.000000 microviewer-1.0.1/microviewer/datacube.js
--rw-r--r--   0 wms        (501) staff       (20)     1911 2023-06-05 21:09:00.000000 microviewer-1.0.1/microviewer/favicon.ico
--rw-r--r--   0 wms        (501) staff       (20)    18826 2023-06-06 15:06:58.000000 microviewer-1.0.1/microviewer/index.html
--rw-r--r--   0 wms        (501) staff       (20)    87462 2023-06-06 04:26:20.000000 microviewer-1.0.1/microviewer/jquery-3.7.0.min.js
--rw-r--r--   0 wms        (501) staff       (20)       11 2023-06-06 04:58:06.000000 microviewer-1.0.1/microviewer/requirements.txt
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-07 02:03:41.139957 microviewer-1.0.1/microviewer.egg-info/
--rw-r--r--   0 wms        (501) staff       (20)     2372 2023-06-07 02:03:41.000000 microviewer-1.0.1/microviewer.egg-info/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)      516 2023-06-07 02:03:41.000000 microviewer-1.0.1/microviewer.egg-info/SOURCES.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-07 02:03:41.000000 microviewer-1.0.1/microviewer.egg-info/dependency_links.txt
--rw-r--r--   0 wms        (501) staff       (20)       47 2023-06-07 02:03:41.000000 microviewer-1.0.1/microviewer.egg-info/entry_points.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-06 04:24:32.000000 microviewer-1.0.1/microviewer.egg-info/not-zip-safe
--rw-r--r--   0 wms        (501) staff       (20)       46 2023-06-07 02:03:41.000000 microviewer-1.0.1/microviewer.egg-info/pbr.json
--rw-r--r--   0 wms        (501) staff       (20)       28 2023-06-07 02:03:41.000000 microviewer-1.0.1/microviewer.egg-info/top_level.txt
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-07 02:03:41.140493 microviewer-1.0.1/microviewer_cli/
--rw-r--r--   0 wms        (501) staff       (20)       18 2023-06-06 04:44:54.000000 microviewer-1.0.1/microviewer_cli/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     1088 2023-06-06 05:02:43.000000 microviewer-1.0.1/microviewer_cli/cli.py
--rw-r--r--   0 wms        (501) staff       (20)   220312 2023-06-06 07:35:34.000000 microviewer-1.0.1/seg-demo.png
--rw-r--r--   0 wms        (501) staff       (20)     1032 2023-06-07 02:03:41.141623 microviewer-1.0.1/setup.cfg
--rw-r--r--   0 wms        (501) staff       (20)      225 2023-06-06 04:44:08.000000 microviewer-1.0.1/setup.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-14 17:27:26.025618 microviewer-1.1.0/
+-rw-r--r--   0 wms        (501) staff       (20)       52 2023-06-14 17:27:25.000000 microviewer-1.1.0/AUTHORS
+-rw-r--r--   0 wms        (501) staff       (20)      664 2023-06-14 17:27:25.000000 microviewer-1.1.0/ChangeLog
+-rw-r--r--   0 wms        (501) staff       (20)    26526 2023-06-05 21:07:17.000000 microviewer-1.1.0/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)     2423 2023-06-14 17:27:26.025750 microviewer-1.1.0/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)     1409 2023-06-14 17:26:48.000000 microviewer-1.1.0/README.md
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-14 17:27:26.023379 microviewer-1.1.0/microviewer/
+-rw-r--r--   0 wms        (501) staff       (20)     5049 2023-06-14 17:22:52.000000 microviewer-1.1.0/microviewer/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)    34702 2023-06-14 17:25:16.000000 microviewer-1.1.0/microviewer/datacube.js
+-rw-r--r--   0 wms        (501) staff       (20)     1911 2023-06-05 21:09:00.000000 microviewer-1.1.0/microviewer/favicon.ico
+-rw-r--r--   0 wms        (501) staff       (20)    18826 2023-06-06 15:06:58.000000 microviewer-1.1.0/microviewer/index.html
+-rw-r--r--   0 wms        (501) staff       (20)    87462 2023-06-06 04:26:20.000000 microviewer-1.1.0/microviewer/jquery-3.7.0.min.js
+-rw-r--r--   0 wms        (501) staff       (20)       11 2023-06-06 04:58:06.000000 microviewer-1.1.0/microviewer/requirements.txt
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-14 17:27:26.024893 microviewer-1.1.0/microviewer.egg-info/
+-rw-r--r--   0 wms        (501) staff       (20)     2423 2023-06-14 17:27:25.000000 microviewer-1.1.0/microviewer.egg-info/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)      516 2023-06-14 17:27:26.000000 microviewer-1.1.0/microviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-14 17:27:25.000000 microviewer-1.1.0/microviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 wms        (501) staff       (20)       47 2023-06-14 17:27:25.000000 microviewer-1.1.0/microviewer.egg-info/entry_points.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-06 04:24:32.000000 microviewer-1.1.0/microviewer.egg-info/not-zip-safe
+-rw-r--r--   0 wms        (501) staff       (20)       46 2023-06-14 17:27:25.000000 microviewer-1.1.0/microviewer.egg-info/pbr.json
+-rw-r--r--   0 wms        (501) staff       (20)       28 2023-06-14 17:27:25.000000 microviewer-1.1.0/microviewer.egg-info/top_level.txt
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-14 17:27:26.025439 microviewer-1.1.0/microviewer_cli/
+-rw-r--r--   0 wms        (501) staff       (20)       18 2023-06-06 04:44:54.000000 microviewer-1.1.0/microviewer_cli/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     1911 2023-06-14 17:24:30.000000 microviewer-1.1.0/microviewer_cli/cli.py
+-rw-r--r--   0 wms        (501) staff       (20)   220312 2023-06-06 07:35:34.000000 microviewer-1.1.0/seg-demo.png
+-rw-r--r--   0 wms        (501) staff       (20)     1032 2023-06-14 17:27:26.026211 microviewer-1.1.0/setup.cfg
+-rw-r--r--   0 wms        (501) staff       (20)      225 2023-06-06 04:44:08.000000 microviewer-1.1.0/setup.py
```

### Comparing `microviewer-1.0.1/LICENSE` & `microviewer-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `microviewer-1.0.1/PKG-INFO` & `microviewer-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microviewer
-Version: 1.0.1
+Version: 1.1.0
 Summary: Visualize 3D numpy arrays in the browser.
 Home-page: https://github.com/seung-lab/microviewer/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
@@ -49,14 +49,15 @@
 ## Supports
 
 - 8-bit grayscale 3D images
 - color images (including 3 channel 3D images)
 - floating point images
 - boolean images
 - segmentation labels
+- .npy or .nii format (must install nibabel first)
 
 ## Installation
 
 ```bash
 pip install microviewer
 ```
```

### Comparing `microviewer-1.0.1/README.md` & `microviewer-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 ## Supports
 
 - 8-bit grayscale 3D images
 - color images (including 3 channel 3D images)
 - floating point images
 - boolean images
 - segmentation labels
+- .npy or .nii format (must install nibabel first)
 
 ## Installation
 
 ```bash
 pip install microviewer
 ```
```

### Comparing `microviewer-1.0.1/microviewer/__init__.py` & `microviewer-1.1.0/microviewer/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,27 +39,27 @@
 
   assert np.all(img.shape[:3] == seg.shape[:3])
 
   img_data = {
     "img": img,
     "cloudpath": cloudpath,
     "resolution": resolution,
-    "layer_type": ('segmentation' if seg else 'image'),
+    "layer_type": 'image',
     "offset": offset,
   }
 
   seg_data = {
     "img": seg,
     "cloudpath": cloudpath,
     "resolution": resolution,
-    "layer_type": ('segmentation' if seg else 'image'),
+    "layer_type": 'segmentation',
     "offset": offset,
   }
 
-  return run([ img, seg ], hostname=hostname, port=port, browser=browser)
+  return run([ img_data, seg_data ], hostname=hostname, port=port, browser=browser)
 
 def view(
   img:np.ndarray, 
   seg:bool = False, 
   resolution:Optional[np.ndarray] = np.ones((3,), dtype=int), 
   offset:Optional[np.ndarray] = np.zeros((3,), dtype=int),
   cloudpath:str = "IN MEMORY", 
@@ -90,16 +90,15 @@
 
   if browser:
     webbrowser.open(url, new=2)
 
   try:
     myServer.serve_forever()
   except KeyboardInterrupt:
-    # extra \n to prevent display of "^CContinuing"
-    print("\nContinuing program execution...")
+    print("")
   finally:
     myServer.server_close()
 
 class ViewerServerHandler(BaseHTTPRequestHandler):
   def __init__(self, cutouts, *args):
     self.cutouts = cutouts
     BaseHTTPRequestHandler.__init__(self, *args)
@@ -154,18 +153,18 @@
     else:
       img, seg = self.cutouts
       msg = json.dumps({
         'viewtype': 'hyper',
         'cloudpath': [ img['cloudpath'], seg['cloudpath'] ],
         'bounds': bounds,
         'resolution': [ int(x) for x in cutout['resolution'] ],
-        'data_types': [ str(img.dtype), str(seg.dtype) ],
+        'data_types': [ str(img["img"].dtype), str(seg["img"].dtype) ],
         'data_bytes': [ 
-          np.dtype(img.dtype).itemsize,
-          np.dtype(seg.dtype).itemsize
+          np.dtype(img["img"].dtype).itemsize,
+          np.dtype(seg["img"].dtype).itemsize
         ],
       })
     self.wfile.write(msg.encode('utf-8'))
 
   def serve_file(self):
     self.send_header('Content-type', 'text/html')
     self.end_headers()
@@ -175,7 +174,12 @@
     if path == '':
       path = 'index.html'
 
     dirname = os.path.dirname(__file__)
     filepath = os.path.join(dirname, './' + path)
     with open(filepath, 'rb') as f:
       self.wfile.write(f.read())  
+
+  # silent, no need to print that it's serving html and js
+  def log_message(self, format, *args):
+    pass
+
```

### Comparing `microviewer-1.0.1/microviewer/datacube.js` & `microviewer-1.1.0/microviewer/datacube.js`

 * *Files identical despite different names*

### Comparing `microviewer-1.0.1/microviewer/favicon.ico` & `microviewer-1.1.0/microviewer/favicon.ico`

 * *Files identical despite different names*

### Comparing `microviewer-1.0.1/microviewer/index.html` & `microviewer-1.1.0/microviewer/index.html`

 * *Files identical despite different names*

### Comparing `microviewer-1.0.1/microviewer/jquery-3.7.0.min.js` & `microviewer-1.1.0/microviewer/jquery-3.7.0.min.js`

 * *Files identical despite different names*

### Comparing `microviewer-1.0.1/microviewer.egg-info/PKG-INFO` & `microviewer-1.1.0/microviewer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microviewer
-Version: 1.0.1
+Version: 1.1.0
 Summary: Visualize 3D numpy arrays in the browser.
 Home-page: https://github.com/seung-lab/microviewer/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
@@ -49,14 +49,15 @@
 ## Supports
 
 - 8-bit grayscale 3D images
 - color images (including 3 channel 3D images)
 - floating point images
 - boolean images
 - segmentation labels
+- .npy or .nii format (must install nibabel first)
 
 ## Installation
 
 ```bash
 pip install microviewer
 ```
```

### Comparing `microviewer-1.0.1/microviewer.egg-info/SOURCES.txt` & `microviewer-1.1.0/microviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microviewer-1.0.1/seg-demo.png` & `microviewer-1.1.0/seg-demo.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.0.1/setup.cfg` & `microviewer-1.1.0/setup.cfg`

 * *Files identical despite different names*

