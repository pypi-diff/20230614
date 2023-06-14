# Comparing `tmp/ratr0_utils-0.1.6.tar.gz` & `tmp/ratr0_utils-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ratr0_utils-0.1.6.tar", last modified: Sat Apr 17 19:48:12 2021, max compression
+gzip compressed data, was "ratr0_utils-0.1.7.tar", last modified: Tue Apr 25 16:55:55 2023, max compression
```

## Comparing `ratr0_utils-0.1.6.tar` & `ratr0_utils-0.1.7.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxr-x   0 weiju     (1000) weiju     (1000)        0 2021-04-17 19:48:12.518763 ratr0_utils-0.1.6/
--rw-rw-r--   0 weiju     (1000) weiju     (1000)      989 2021-04-17 19:48:12.518763 ratr0_utils-0.1.6/PKG-INFO
--rw-r--r--   0 weiju     (1000) weiju     (1000)      714 2017-11-09 18:54:53.000000 ratr0_utils-0.1.6/README.md
-drwxrwxr-x   0 weiju     (1000) weiju     (1000)        0 2021-04-17 19:48:12.454804 ratr0_utils-0.1.6/bin/
--rwxrwxr-x   0 weiju     (1000) weiju     (1000)     1728 2021-04-17 19:46:56.000000 ratr0_utils-0.1.6/bin/ratr0-converttiled
--rwxr--r--   0 weiju     (1000) weiju     (1000)      581 2018-02-26 18:40:53.000000 ratr0_utils-0.1.6/bin/ratr0-file
--rwxrwxr-x   0 weiju     (1000) weiju     (1000)      800 2020-11-03 20:38:17.000000 ratr0_utils-0.1.6/bin/ratr0-makelevel
--rwxrwxr-x   0 weiju     (1000) weiju     (1000)      956 2020-11-03 20:38:17.000000 ratr0_utils-0.1.6/bin/ratr0-makesprites
--rwxrwxr-x   0 weiju     (1000) weiju     (1000)     2316 2021-04-17 19:46:56.000000 ratr0_utils-0.1.6/bin/ratr0-maketiles
--rwxrwxr-x   0 weiju     (1000) weiju     (1000)      566 2020-11-03 20:38:17.000000 ratr0_utils-0.1.6/bin/ratr0-wav2raw8
-drwxrwxr-x   0 weiju     (1000) weiju     (1000)        0 2021-04-17 19:48:12.414830 ratr0_utils-0.1.6/ratr0/
-drwxrwxr-x   0 weiju     (1000) weiju     (1000)        0 2021-04-17 19:48:12.478789 ratr0_utils-0.1.6/ratr0/util/
--rw-r--r--   0 weiju     (1000) weiju     (1000)        0 2017-10-18 03:22:33.000000 ratr0_utils-0.1.6/ratr0/util/__init__.py
--rw-rw-r--   0 weiju     (1000) weiju     (1000)      558 2020-11-03 20:38:17.000000 ratr0_utils-0.1.6/ratr0/util/compute_lf.py
--rw-rw-r--   0 weiju     (1000) weiju     (1000)     2074 2021-04-17 19:46:56.000000 ratr0_utils-0.1.6/ratr0/util/file_info.py
--rw-rw-r--   0 weiju     (1000) weiju     (1000)     1594 2021-04-17 19:46:56.000000 ratr0_utils-0.1.6/ratr0/util/levels.py
--rw-rw-r--   0 weiju     (1000) weiju     (1000)     3647 2020-11-03 20:38:17.000000 ratr0_utils-0.1.6/ratr0/util/png_util.py
--rw-rw-r--   0 weiju     (1000) weiju     (1000)     8218 2020-11-03 20:38:17.000000 ratr0_utils-0.1.6/ratr0/util/sprites.py
--rw-rw-r--   0 weiju     (1000) weiju     (1000)     1455 2021-04-17 19:46:56.000000 ratr0_utils-0.1.6/ratr0/util/tiled.py
--rw-rw-r--   0 weiju     (1000) weiju     (1000)     9424 2021-04-17 19:46:56.000000 ratr0_utils-0.1.6/ratr0/util/tiles.py
--rw-rw-r--   0 weiju     (1000) weiju     (1000)       62 2020-09-08 21:16:51.000000 ratr0_utils-0.1.6/ratr0/util/tiles2png.py
-drwxrwxr-x   0 weiju     (1000) weiju     (1000)        0 2021-04-17 19:48:12.518763 ratr0_utils-0.1.6/ratr0_utils.egg-info/
--rw-r--r--   0 weiju     (1000) weiju     (1000)      989 2021-04-17 19:48:12.000000 ratr0_utils-0.1.6/ratr0_utils.egg-info/PKG-INFO
--rw-r--r--   0 weiju     (1000) weiju     (1000)      557 2021-04-17 19:48:12.000000 ratr0_utils-0.1.6/ratr0_utils.egg-info/SOURCES.txt
--rw-r--r--   0 weiju     (1000) weiju     (1000)        1 2021-04-17 19:48:12.000000 ratr0_utils-0.1.6/ratr0_utils.egg-info/dependency_links.txt
--rw-r--r--   0 weiju     (1000) weiju     (1000)        1 2017-10-18 18:01:39.000000 ratr0_utils-0.1.6/ratr0_utils.egg-info/not-zip-safe
--rw-r--r--   0 weiju     (1000) weiju     (1000)        7 2021-04-17 19:48:12.000000 ratr0_utils-0.1.6/ratr0_utils.egg-info/requires.txt
--rw-r--r--   0 weiju     (1000) weiju     (1000)        6 2021-04-17 19:48:12.000000 ratr0_utils-0.1.6/ratr0_utils.egg-info/top_level.txt
--rw-r--r--   0 weiju     (1000) weiju     (1000)       67 2021-04-17 19:48:12.518763 ratr0_utils-0.1.6/setup.cfg
--rw-rw-r--   0 weiju     (1000) weiju     (1000)     1870 2021-04-17 19:46:56.000000 ratr0_utils-0.1.6/setup.py
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-25 16:55:55.181780 ratr0_utils-0.1.7/
+-rw-r--r--   0 weiju      (501) staff       (20)    35147 2020-12-11 22:44:23.000000 ratr0_utils-0.1.7/LICENSE
+-rw-r--r--   0 weiju      (501) staff       (20)      972 2023-04-25 16:55:55.181845 ratr0_utils-0.1.7/PKG-INFO
+-rw-r--r--   0 weiju      (501) staff       (20)      904 2023-04-07 17:46:49.000000 ratr0_utils-0.1.7/README.md
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-25 16:55:55.179077 ratr0_utils-0.1.7/bin/
+-rwxr-xr-x   0 weiju      (501) staff       (20)     1728 2021-04-17 19:35:49.000000 ratr0_utils-0.1.7/bin/ratr0-converttiled
+-rwxr-xr-x   0 weiju      (501) staff       (20)      581 2020-12-11 22:44:23.000000 ratr0_utils-0.1.7/bin/ratr0-file
+-rwxr-xr-x   0 weiju      (501) staff       (20)      800 2020-12-11 22:44:23.000000 ratr0_utils-0.1.7/bin/ratr0-makelevel
+-rwxr-xr-x   0 weiju      (501) staff       (20)     1287 2023-04-07 20:12:30.000000 ratr0_utils-0.1.7/bin/ratr0-makeplanes
+-rwxr-xr-x   0 weiju      (501) staff       (20)      956 2020-12-11 22:44:23.000000 ratr0_utils-0.1.7/bin/ratr0-makesprites
+-rwxr-xr-x   0 weiju      (501) staff       (20)     2364 2023-04-23 21:19:04.000000 ratr0_utils-0.1.7/bin/ratr0-maketiles
+-rwxr-xr-x   0 weiju      (501) staff       (20)      566 2020-12-11 22:44:23.000000 ratr0_utils-0.1.7/bin/ratr0-wav2raw8
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-25 16:55:55.175907 ratr0_utils-0.1.7/ratr0/
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-25 16:55:55.180709 ratr0_utils-0.1.7/ratr0/util/
+-rw-r--r--   0 weiju      (501) staff       (20)        0 2020-12-11 22:44:23.000000 ratr0_utils-0.1.7/ratr0/util/__init__.py
+-rw-r--r--   0 weiju      (501) staff       (20)      558 2020-12-11 22:44:23.000000 ratr0_utils-0.1.7/ratr0/util/compute_lf.py
+-rw-r--r--   0 weiju      (501) staff       (20)     2074 2021-04-17 19:35:49.000000 ratr0_utils-0.1.7/ratr0/util/file_info.py
+-rw-r--r--   0 weiju      (501) staff       (20)     1594 2021-04-17 19:35:49.000000 ratr0_utils-0.1.7/ratr0/util/levels.py
+-rw-r--r--   0 weiju      (501) staff       (20)     3647 2023-04-07 17:33:33.000000 ratr0_utils-0.1.7/ratr0/util/png_util.py
+-rw-r--r--   0 weiju      (501) staff       (20)     8218 2020-12-11 22:44:23.000000 ratr0_utils-0.1.7/ratr0/util/sprites.py
+-rw-r--r--   0 weiju      (501) staff       (20)     1455 2021-04-17 19:35:49.000000 ratr0_utils-0.1.7/ratr0/util/tiled.py
+-rw-r--r--   0 weiju      (501) staff       (20)    11359 2023-04-24 03:59:32.000000 ratr0_utils-0.1.7/ratr0/util/tiles.py
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-25 16:55:55.181674 ratr0_utils-0.1.7/ratr0_utils.egg-info/
+-rw-r--r--   0 weiju      (501) staff       (20)      972 2023-04-25 16:55:55.000000 ratr0_utils-0.1.7/ratr0_utils.egg-info/PKG-INFO
+-rw-r--r--   0 weiju      (501) staff       (20)      562 2023-04-25 16:55:55.000000 ratr0_utils-0.1.7/ratr0_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 weiju      (501) staff       (20)        1 2023-04-25 16:55:55.000000 ratr0_utils-0.1.7/ratr0_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 weiju      (501) staff       (20)        1 2021-04-06 23:18:12.000000 ratr0_utils-0.1.7/ratr0_utils.egg-info/not-zip-safe
+-rw-r--r--   0 weiju      (501) staff       (20)        7 2023-04-25 16:55:55.000000 ratr0_utils-0.1.7/ratr0_utils.egg-info/requires.txt
+-rw-r--r--   0 weiju      (501) staff       (20)        6 2023-04-25 16:55:55.000000 ratr0_utils-0.1.7/ratr0_utils.egg-info/top_level.txt
+-rw-r--r--   0 weiju      (501) staff       (20)       67 2023-04-25 16:55:55.182043 ratr0_utils-0.1.7/setup.cfg
+-rw-r--r--   0 weiju      (501) staff       (20)     1913 2023-04-25 16:54:51.000000 ratr0_utils-0.1.7/setup.py
```

### Comparing `ratr0_utils-0.1.6/PKG-INFO` & `ratr0_utils-0.1.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: ratr0_utils
-Version: 0.1.6
+Version: 0.1.7
 Summary: ratr0-utils is a collection of utilities for game development using the RATR0 engine
 Home-page: https://github.com/weiju/ratr0-utils
 Author: Wei-ju Wu
 Author-email: weiju.wu@gmail.com
 Maintainer: Wei-ju Wu
 Maintainer-email: weiju.wu@gmail.com
 License: GPL V3
-Description: UNKNOWN
 Keywords: ratr0,amiga,game,development,classic,ecs,aga
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
```

### Comparing `ratr0_utils-0.1.6/README.md` & `ratr0_utils-0.1.7/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -20,7 +20,13 @@
 is using underscore
 
 python3 setup.py sdist bdist_wheel
 
 ## Uploading to pypi
 
 twine upload -r pypi dist/ratr0_utils-<version>*
+
+## Known pitfalls
+
+Image conversion can fail when the PNG is not in indexed format.
+Modern image editors often save PNG in 24bit format, so make sure
+that the PNG is in the format you need
```

### Comparing `ratr0_utils-0.1.6/bin/ratr0-converttiled` & `ratr0_utils-0.1.7/bin/ratr0-converttiled`

 * *Files identical despite different names*

### Comparing `ratr0_utils-0.1.6/bin/ratr0-file` & `ratr0_utils-0.1.7/bin/ratr0-file`

 * *Files identical despite different names*

### Comparing `ratr0_utils-0.1.6/bin/ratr0-makelevel` & `ratr0_utils-0.1.7/bin/ratr0-makelevel`

 * *Files identical despite different names*

### Comparing `ratr0_utils-0.1.6/bin/ratr0-makesprites` & `ratr0_utils-0.1.7/bin/ratr0-makesprites`

 * *Files identical despite different names*

### Comparing `ratr0_utils-0.1.6/bin/ratr0-maketiles` & `ratr0_utils-0.1.7/bin/ratr0-maketiles`

 * *Files 10% similar despite different names*

```diff
@@ -38,12 +38,13 @@
     tiles.write_tiles(im, args.outfile, tile_size, colors,
                       palette24=args.palette24,
                       non_interleaved=args.non_interleaved,
                       create_mask=args.create_mask,
                       verbose=args.verbose)
 
     if args.mask_file is not None:
-        tiles.write_mask(args.mask_file, im, tile_size, 1,
+        depth = int(math.log2(len(colors)))
+        tiles.write_mask(args.mask_file, im, tile_size, depth,
                          palette24=args.palette24,
                          non_interleaved=args.non_interleaved,
                          verbose=args.verbose)
```

### Comparing `ratr0_utils-0.1.6/bin/ratr0-wav2raw8` & `ratr0_utils-0.1.7/bin/ratr0-wav2raw8`

 * *Files identical despite different names*

### Comparing `ratr0_utils-0.1.6/ratr0/util/compute_lf.py` & `ratr0_utils-0.1.7/ratr0/util/compute_lf.py`

 * *Files identical despite different names*

### Comparing `ratr0_utils-0.1.6/ratr0/util/file_info.py` & `ratr0_utils-0.1.7/ratr0/util/file_info.py`

 * *Files identical despite different names*

### Comparing `ratr0_utils-0.1.6/ratr0/util/levels.py` & `ratr0_utils-0.1.7/ratr0/util/levels.py`

 * *Files identical despite different names*

### Comparing `ratr0_utils-0.1.6/ratr0/util/png_util.py` & `ratr0_utils-0.1.7/ratr0/util/png_util.py`

 * *Files identical despite different names*

### Comparing `ratr0_utils-0.1.6/ratr0/util/sprites.py` & `ratr0_utils-0.1.7/ratr0/util/sprites.py`

 * *Files identical despite different names*

### Comparing `ratr0_utils-0.1.6/ratr0/util/tiled.py` & `ratr0_utils-0.1.7/ratr0/util/tiled.py`

 * *Files identical despite different names*

### Comparing `ratr0_utils-0.1.6/ratr0/util/tiles.py` & `ratr0_utils-0.1.7/ratr0/util/tiles.py`

 * *Files 22% similar despite different names*

```diff
@@ -164,14 +164,39 @@
 
     return TilesInfo(version, flags, depth, width, height,
                      tile_size_h, tile_size_v, num_tiles_h, num_tiles_v,
                      palette_size, imgdata_size, checksum,
                      palette)
 
 
+def write_planes_to_c(im, outfile, colors, non_interleaved, verbose, indent=4):
+    """write tile file using the specifications"""
+    depth = int(math.log2(len(colors)))
+    planes, map_words_per_row = png_util.extract_planes(im, depth, verbose)
+    print("#Planes: %d map words per row: %d" % (len(planes), map_words_per_row))
+    with open(outfile, 'w') as out:
+        out.write("UINT16 data[] = {\n")
+        out_data = []
+        if non_interleaved:
+            for plane in planes:
+                for word in plane:
+                    out_data.append("0x%04x" % word)
+        else:
+            interleaved_data = png_util.interleave_planes(planes, map_words_per_row)
+            for row in interleaved_data:
+                for word in row:
+                    out_data.append("0x%04x" % word)
+        out_rows = png_util.chunks(out_data, map_words_per_row)
+        for row in out_rows:
+            out.write(" " * indent)
+            out.write(", ".join(row))
+            out.write(",\n")
+        out.write("\n};\n")
+
+
 def write_tiles(im, outfile, tile_size, colors, palette24,
                 non_interleaved, create_mask, verbose):
     """write tile file using the specifications"""
     depth = int(math.log2(len(colors)))
     planes, map_words_per_row = png_util.extract_planes(im, depth, verbose)
     write_tile_file(outfile, im, tile_size, planes, colors, map_words_per_row,
                     palette24, non_interleaved, create_mask, verbose)
@@ -187,67 +212,87 @@
         flags |= 2
     else:
         # convert colors by or'ing them into a 12 bit value
         # this changes colors from a list of triples into a flat list
         colors = [(((r >> 4) & 0x0f) << 8) | (((g >> 4) & 0x0f) << 4) | ((b >> 4) & 0x0f)
                   for r, g, b in colors]
         #print(['%03x' % c for c in colors])
-    if create_mask:
-        flags |= 8
-        mask_depth = 1
 
     palette_size = len(colors)
     depth = int(math.log2(palette_size))
+
+    if create_mask:
+        flags |= 8
+        # if interleaved, mask depth is same as image depth
+        mask_depth = 1 if non_interleaved else depth
+
+
     imgdata_size = map_words_per_row * 2 * im.height * (depth + mask_depth)
     tile_sheet_dim = (int(im.width / tile_size[0]), int(im.height / tile_size[1]))
     if verbose:
         print('tile size h: %d v: %d' % (tile_size[0], tile_size[1]))
         print('tile sheet width: %d height: %d' % (tile_sheet_dim[0], tile_sheet_dim[1]))
 
     # add an additional plane that merges down the 1 bits of the planes list
     if create_mask:
         mask_plane = [0] * len(planes[0])
         for i in range(len(mask_plane)):
             w = 0
             for plane in planes:
                 w |= plane[i]
             mask_plane[i] = w
-        planes.append(mask_plane)
 
     with open(outfile, 'wb') as out:
         tiles_info = TilesInfo(FILE_FORMAT_VERSION, flags,
                                depth, im.width, im.height,
                                tile_size[0], tile_size[1],
                                tile_sheet_dim[0], tile_sheet_dim[1],
                                palette_size, imgdata_size, checksum,
                                colors)
         tiles_info.write(out)
         if non_interleaved:
+            planes.append(mask_plane)
             for plane in planes:
                 for word in plane:
                     out.write(struct.pack(">H", word))
         else:
             interleaved_data = png_util.interleave_planes(planes, map_words_per_row)
             for row in interleaved_data:
                 for word in row:
                     out.write(struct.pack(">H", word))
+            if create_mask:
+                # interleaved mask
+                # we need to multiply the mask plane data
+                mask_planes = [mask_plane for i in range(depth)]
+                interleaved_mask = png_util.interleave_planes(mask_planes, map_words_per_row)
+                for row in interleaved_mask:
+                    for word in row:
+                        out.write(struct.pack(">H", word))
 
 
 def setornot(v):
     return 1 if v > 0 else 0
 
 
 def write_mask(outfile, im, tile_size, depth,
                palette24,
                non_interleaved, verbose):
-    colors = [setornot(c) for c in im.getdata()]
-    mask_img = Image.new(mode="1", size=im.size)
-    mask_img.putdata(colors)
-
-    # write a debug PNG file as visual control
-    mask_img.save(outfile)
-    """
-    mask_img.save("tmp_mask.png")
-    #mask_img = Image.open('tmp_mask.png')
-    mask_colors = png_util.make_colors(mask_img, depth, verbose)
-    write_tiles(mask_img, outfile, tile_size, mask_colors,
-                palette24=palette24, non_interleaved=non_interleaved, verbose=verbose)"""
+    """Write a preview mask in png format, as a quick visual control"""
+    # Non-interleaved: just write one bitplane at the end
+    if non_interleaved:
+        colors = [setornot(c) for c in im.getdata()]
+        mask_img = Image.new(mode="1", size=im.size)
+        mask_img.putdata(colors)
+        # write a debug PNG file as visual control
+        mask_img.save(outfile)
+    else:
+        # interleaved: duplicate each row times the depth
+        colors = [setornot(c) for c in im.getdata()]
+        color_rows = list(png_util.chunks(colors, im.width))
+        final_colors = []
+        for row in color_rows:
+            new_row = row * depth
+            final_colors.extend(row * depth)
+        mask_img = Image.new(mode="1", size=(im.width, im.height * depth))
+        mask_img.putdata(final_colors)
+        # write a debug PNG file as visual control
+        mask_img.save(outfile)
```

### Comparing `ratr0_utils-0.1.6/ratr0_utils.egg-info/PKG-INFO` & `ratr0_utils-0.1.7/ratr0_utils.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: ratr0-utils
-Version: 0.1.6
+Version: 0.1.7
 Summary: ratr0-utils is a collection of utilities for game development using the RATR0 engine
 Home-page: https://github.com/weiju/ratr0-utils
 Author: Wei-ju Wu
 Author-email: weiju.wu@gmail.com
 Maintainer: Wei-ju Wu
 Maintainer-email: weiju.wu@gmail.com
 License: GPL V3
-Description: UNKNOWN
 Keywords: ratr0,amiga,game,development,classic,ecs,aga
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
```

### Comparing `ratr0_utils-0.1.6/ratr0_utils.egg-info/SOURCES.txt` & `ratr0_utils-0.1.7/ratr0_utils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 bin/ratr0-converttiled
 bin/ratr0-file
 bin/ratr0-makelevel
+bin/ratr0-makeplanes
 bin/ratr0-makesprites
 bin/ratr0-maketiles
 bin/ratr0-wav2raw8
 ratr0/util/__init__.py
 ratr0/util/compute_lf.py
 ratr0/util/file_info.py
 ratr0/util/levels.py
 ratr0/util/png_util.py
 ratr0/util/sprites.py
 ratr0/util/tiled.py
 ratr0/util/tiles.py
-ratr0/util/tiles2png.py
 ratr0_utils.egg-info/PKG-INFO
 ratr0_utils.egg-info/SOURCES.txt
 ratr0_utils.egg-info/dependency_links.txt
 ratr0_utils.egg-info/not-zip-safe
 ratr0_utils.egg-info/requires.txt
 ratr0_utils.egg-info/top_level.txt
```

### Comparing `ratr0_utils-0.1.6/setup.py` & `ratr0_utils-0.1.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 NAME = 'ratr0_utils'
 PACKAGES = ['ratr0.util']
 DESCRIPTION = 'ratr0-utils is a collection of utilities for game development using the RATR0 engine'
 LICENSE = 'GPL V3'
 URI = 'https://github.com/weiju/ratr0-utils'
 AUTHOR = 'Wei-ju Wu'
-VERSION = '0.1.6'
+VERSION = '0.1.7'
 
 KEYWORDS = ['ratr0', 'amiga', 'game', 'development', 'classic', 'ecs', 'aga']
 
 # See trove classifiers
 # https://testpypi.python.org/pypi?%3Aaction=list_classifiers
 
 CLASSIFIERS = [
@@ -49,10 +49,11 @@
           zip_safe=False,
           classifiers=CLASSIFIERS,
           install_requires=INSTALL_REQUIRES,
           include_package_data=True, package_data=PACKAGE_DATA,
           scripts=['bin/ratr0-maketiles',
                    'bin/ratr0-makesprites',
                    'bin/ratr0-makelevel',
+                   'bin/ratr0-makeplanes',
                    'bin/ratr0-converttiled',
                    'bin/ratr0-file',
                    'bin/ratr0-wav2raw8'])
```

