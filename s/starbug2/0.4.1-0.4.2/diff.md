# Comparing `tmp/starbug2-0.4.1.tar.gz` & `tmp/starbug2-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starbug2-0.4.1.tar", last modified: Mon Jun 12 19:16:12 2023, max compression
+gzip compressed data, was "starbug2-0.4.2.tar", last modified: Wed Jun 14 16:14:37 2023, max compression
```

## Comparing `starbug2-0.4.1.tar` & `starbug2-0.4.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:12.101716 starbug2-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-12 19:15:57.000000 starbug2-0.4.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-12 19:15:57.000000 starbug2-0.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-12 19:15:57.000000 starbug2-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-06-12 19:16:12.101716 starbug2-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-06-12 19:15:57.000000 starbug2-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:12.097716 starbug2-0.4.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    13797 2023-06-12 19:15:57.000000 starbug2-0.4.1/bin/starbug2
--rwxr-xr-x   0 runner    (1001) docker     (123)     5629 2023-06-12 19:15:57.000000 starbug2-0.4.1/bin/starbug2-match
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:12.097716 starbug2-0.4.1/extras/
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-12 19:15:57.000000 starbug2-0.4.1/extras/starbug2.completion
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-12 19:15:57.000000 starbug2-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-12 19:16:12.101716 starbug2-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-12 19:15:57.000000 starbug2-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:12.097716 starbug2-0.4.1/starbug2/
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-12 19:15:57.000000 starbug2-0.4.1/starbug2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-12 19:15:57.000000 starbug2-0.4.1/starbug2/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)    15640 2023-06-12 19:15:57.000000 starbug2-0.4.1/starbug2/matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-06-12 19:15:57.000000 starbug2-0.4.1/starbug2/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:12.101716 starbug2-0.4.1/starbug2/param/
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-12 19:15:57.000000 starbug2-0.4.1/starbug2/param/default.param
--rw-r--r--   0 runner    (1001) docker     (123)    28598 2023-06-12 19:15:57.000000 starbug2-0.4.1/starbug2/routines.py
--rw-r--r--   0 runner    (1001) docker     (123)    31810 2023-06-12 19:15:57.000000 starbug2-0.4.1/starbug2/starbug.py
--rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-06-12 19:15:57.000000 starbug2-0.4.1/starbug2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:12.101716 starbug2-0.4.1/starbug2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-06-12 19:16:12.000000 starbug2-0.4.1/starbug2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-12 19:16:12.000000 starbug2-0.4.1/starbug2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:16:12.000000 starbug2-0.4.1/starbug2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-12 19:16:12.000000 starbug2-0.4.1/starbug2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 19:16:12.000000 starbug2-0.4.1/starbug2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:12.101716 starbug2-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-12 19:15:57.000000 starbug2-0.4.1/tests/test_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-12 19:15:57.000000 starbug2-0.4.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:14:37.595449 starbug2-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-14 16:14:17.000000 starbug2-0.4.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 16:14:17.000000 starbug2-0.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-14 16:14:17.000000 starbug2-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-14 16:14:37.595449 starbug2-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-14 16:14:17.000000 starbug2-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:14:37.591449 starbug2-0.4.2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13797 2023-06-14 16:14:17.000000 starbug2-0.4.2/bin/starbug2
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7374 2023-06-14 16:14:17.000000 starbug2-0.4.2/bin/starbug2-match
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:14:37.591449 starbug2-0.4.2/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-14 16:14:17.000000 starbug2-0.4.2/extras/starbug2.completion
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-14 16:14:17.000000 starbug2-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-14 16:14:37.595449 starbug2-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-14 16:14:17.000000 starbug2-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:14:37.591449 starbug2-0.4.2/starbug2/
+-rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-06-14 16:14:17.000000 starbug2-0.4.2/starbug2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-14 16:14:17.000000 starbug2-0.4.2/starbug2/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15392 2023-06-14 16:14:17.000000 starbug2-0.4.2/starbug2/matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-06-14 16:14:17.000000 starbug2-0.4.2/starbug2/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:14:37.595449 starbug2-0.4.2/starbug2/param/
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-06-14 16:14:17.000000 starbug2-0.4.2/starbug2/param/default.param
+-rw-r--r--   0 runner    (1001) docker     (123)    28598 2023-06-14 16:14:17.000000 starbug2-0.4.2/starbug2/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31810 2023-06-14 16:14:17.000000 starbug2-0.4.2/starbug2/starbug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-06-14 16:14:17.000000 starbug2-0.4.2/starbug2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:14:37.595449 starbug2-0.4.2/starbug2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-14 16:14:37.000000 starbug2-0.4.2/starbug2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-14 16:14:37.000000 starbug2-0.4.2/starbug2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:14:37.000000 starbug2-0.4.2/starbug2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-14 16:14:37.000000 starbug2-0.4.2/starbug2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 16:14:37.000000 starbug2-0.4.2/starbug2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:14:37.595449 starbug2-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-14 16:14:17.000000 starbug2-0.4.2/tests/test_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-14 16:14:17.000000 starbug2-0.4.2/tests/test_utils.py
```

### Comparing `starbug2-0.4.1/LICENSE.txt` & `starbug2-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.1/PKG-INFO` & `starbug2-0.4.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,11 @@
-Metadata-Version: 2.1
-Name: starbug2
-Version: 0.4.1
-Summary: JWST PSF photometry in complex crowded fields.
-Author: Conor Nally
-Author-email: conor.nally@ed.ac.uk
-License: GNU General Public License v3.0
-Description-Content-Type: text/markdown
-
 # StarBugII
 
 JWST PSF photometry in dusty crowded fields.
-Last updated: v0.4.1
+Last updated: v0.4.2
 
 [![Python application](https://github.com/conornally/starbug2/actions/workflows/python-app.yml/badge.svg)](https://github.com/conornally/starbug2/actions/workflows/python-app.yml)
 [![PyPI version fury.io](https://badge.fury.io/py/starbug2.svg)](https://pypi.python.org/pypi/starbug2/)
 [![Latest release](https://badgen.net/github/release/conornally/starbug2)](https://github.com/conornally/starbug2/releases)
 
 
 ## Installation
@@ -80,28 +71,26 @@
        --apply-zeropint    a.fits : Apply a zeropoint (-s ZEROPOINT=1.0) to a.fits
        --calc-instr-zp     a.fits : Calculate and apply an instrumental zero point onto a.fits
 
    --> typical runs
       $~ starbug2 -vD -p file.param image.fits      //Source detect on image with a parameter file
       $~ starbug2 -vDM -n4 images*.fits             //Source detect and match outputs of a list of images
       $~ starbug2 -vd image-ap.fits -BP image.fits  //PSF photometry on an image with a source file (image-ap.fits)
-
-
+```
+```bash
 StarbugII Matching 
 usage: starbug2-match [-BGfhv] [-o output] [-p file.param] [-s KEY=VAL] table.fits ...
     -B  --band               : match in "BAND" mode (does not preserve a column for every frame)
     -D  --dither             : match in "DITHER" mode (preserves a column for every frame)
     -f  --full               : export full catalogue
     -G  --generic            : match in "GENERIC" mode
     -h  --help               : show help message
     -o  --output  file.fits  : output matched catalogue
     -p  --param   file.param : load starbug parameter file
     -s  --set     option     : set value in parameter file at runtime (-s MATCH_THRESH=1)
+
+    --> typical runs
+       $~ starbug2-match -Gfo outfile.fits tab1.fits tab2.fits
+       $~ starbug2-match -sMATCH_THRESH=0.2 -sBRIDGE_COL=F444W -Bo out.fits F*W.fits
 ```
 
 See [starbug-manual](https://github.com/conornally/starbug2/blob/main/docs/starbug-manual.md) for more detailed instructions.
-
-## TODO
-
-* Need to really figure out setup.cfg to include the extras files
-* MIRI Background masking
-* psf dither match dropping apMag
```

### Comparing `starbug2-0.4.1/README.md` & `starbug2-0.4.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,20 @@
+Metadata-Version: 2.1
+Name: starbug2
+Version: 0.4.2
+Summary: JWST PSF photometry in complex crowded fields.
+Author: Conor Nally
+Author-email: conor.nally@ed.ac.uk
+License: GNU General Public License v3.0
+Description-Content-Type: text/markdown
+
 # StarBugII
 
 JWST PSF photometry in dusty crowded fields.
-Last updated: v0.4.1
+Last updated: v0.4.2
 
 [![Python application](https://github.com/conornally/starbug2/actions/workflows/python-app.yml/badge.svg)](https://github.com/conornally/starbug2/actions/workflows/python-app.yml)
 [![PyPI version fury.io](https://badge.fury.io/py/starbug2.svg)](https://pypi.python.org/pypi/starbug2/)
 [![Latest release](https://badgen.net/github/release/conornally/starbug2)](https://github.com/conornally/starbug2/releases)
 
 
 ## Installation
@@ -71,28 +80,26 @@
        --apply-zeropint    a.fits : Apply a zeropoint (-s ZEROPOINT=1.0) to a.fits
        --calc-instr-zp     a.fits : Calculate and apply an instrumental zero point onto a.fits
 
    --> typical runs
       $~ starbug2 -vD -p file.param image.fits      //Source detect on image with a parameter file
       $~ starbug2 -vDM -n4 images*.fits             //Source detect and match outputs of a list of images
       $~ starbug2 -vd image-ap.fits -BP image.fits  //PSF photometry on an image with a source file (image-ap.fits)
-
-
+```
+```bash
 StarbugII Matching 
 usage: starbug2-match [-BGfhv] [-o output] [-p file.param] [-s KEY=VAL] table.fits ...
     -B  --band               : match in "BAND" mode (does not preserve a column for every frame)
     -D  --dither             : match in "DITHER" mode (preserves a column for every frame)
     -f  --full               : export full catalogue
     -G  --generic            : match in "GENERIC" mode
     -h  --help               : show help message
     -o  --output  file.fits  : output matched catalogue
     -p  --param   file.param : load starbug parameter file
     -s  --set     option     : set value in parameter file at runtime (-s MATCH_THRESH=1)
+
+    --> typical runs
+       $~ starbug2-match -Gfo outfile.fits tab1.fits tab2.fits
+       $~ starbug2-match -sMATCH_THRESH=0.2 -sBRIDGE_COL=F444W -Bo out.fits F*W.fits
 ```
 
 See [starbug-manual](https://github.com/conornally/starbug2/blob/main/docs/starbug-manual.md) for more detailed instructions.
-
-## TODO
-
-* Need to really figure out setup.cfg to include the extras files
-* MIRI Background masking
-* psf dither match dropping apMag
```

### Comparing `starbug2-0.4.1/bin/starbug2` & `starbug2-0.4.2/bin/starbug2`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.1/extras/starbug2.completion` & `starbug2-0.4.2/extras/starbug2.completion`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.1/starbug2/__init__.py` & `starbug2-0.4.2/starbug2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
  JWST photometry in       ./=== \  \.     \      * 
  complex crowded fields   | (O)  |  |     |           *
                            \._._/ ./    _(\)   *   
  conor.nally@ed.ac.uk     /   ~--\ ----~   \      *
                         ---      ___       ---      
  > %s"""
 
-motd="RM_MATCH will be removed very soon, it will be replaced with NEXP_THRESH"
+motd="Match NIRCam and MIRI: $~ starbug2-match -sBRIDGE_COL=F444W -sMATCH_THRESH -Bo outfile.fits F*W.fits ..."
 
 from os import getenv
 _=getenv("STARBUG_DATDIR") 
 DATDIR=_ if _ else "%s/.local/share/starbug"%(getenv("HOME"))
 
 
 ## HASHDEFS
```

### Comparing `starbug2-0.4.1/starbug2/mask.py` & `starbug2-0.4.2/starbug2/mask.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,24 +22,27 @@
     def from_file(fname):
         with open(fname) as fp:
             return Mask.from_string(fp.readline())
     @staticmethod
     def from_string(string):
         """
         String Format:
-            [-x XCOL] [-y YCOL] [-l Label] x1 y1 x2 y2 x3 y3 ...
+            [-x XCOL] [-y YCOL] [-l Label] : x1 y1 x2 y2 x3 y3 ...
         """
         label=None
         keys=[None,None]
-        opts,args=getopt.getopt(string.split(' '), "l:x:y:")
+        _opts,_coords=string.split(':')
+        opts,args=getopt.getopt(_opts.split(' '), "l:x:y:")
         for opt,optarg in opts:
             if opt=="-x": keys[0]=optarg
             if opt=="-y": keys[1]=optarg
             if opt=="-l": label=optarg
-        points=np.array(args, dtype=float).reshape((int(len(args)/2),2))
+        coords=_coords.strip().rstrip().split(' ')
+        print(coords)
+        points=np.array(coords, dtype=float).reshape((int(len(coords)/2),2))
         return Mask(points,keys,label=label)
 
     def plot(self, ax, **kwargs):
         patch=Polygon(self.path._vertices, label=self.label, **kwargs)
         ax.add_patch(patch)
```

### Comparing `starbug2-0.4.1/starbug2/matching.py` & `starbug2-0.4.2/starbug2/matching.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,21 +196,14 @@
                     else: 
                         tmp.add_row(src[colnames]) ##i can purely use add_row to simplifiy the code
         tmp.rename_columns(colnames, list("%s_%d"%(name,n) for name in colnames))
         base=hcascade((base,tmp), colnames=colnames)
     base=Table(base,dtype=[float]*len(base.colnames)).filled(np.nan)
     return finish_matching(base, colnames)
 
-def nircam_miri_match(nircam, miri, nircam_lockcol="F444W", miri_lockcol=None):
-    """
-    Matching between a nircam catalogue and a miri catalogue
-    It optionally requires a source to be present in one column in each catalougue
-    """
-    pass
-
 def band_match(catalogues, colnames=("RA","DEC")):
     """
     Given a list of catalogues (with filter names in the meta data), match them
     in order of decreasing astrometric accuracy. 
     If F115W, F444W, F770W are input, the F115W centroid positions will be 
     taken as "correct". If a source is not resolved in this band, the next most 
     astrometrically accurate position is taken, i.e. F444W
@@ -258,15 +251,15 @@
             if f_id >= list(starbug2.filters.keys()).index("F277W"): separation=0.10
             if f_id >= list(starbug2.filters.keys()).index("F560W"): separation=0.15
             if f_id >= list(starbug2.filters.keys()).index("F1000W"): separation=0.20
             if f_id >= list(starbug2.filters.keys()).index("F1500W"): separation=0.25
 
 
             for ii,(src,IDX,sep) in enumerate(zip(tab,idx,d2d)):
-                load.msg="matching:%s(%.2g)"%(fltr,separation)
+                load.msg="matching:%s(%.2g\")"%(fltr,separation)
                 load();load.show()
                 if (sep<=separation*u.arcsec) and (sep==min(d2d[idx==IDX])):
                     for name in _colnames: tmp[IDX][name]=src[name]
                 else:
                     tmp.add_row(src[_colnames])
             #tmp=generic_match((base,tab), threshold=threshold, add_src=True, load=load)
```

### Comparing `starbug2-0.4.1/starbug2/misc.py` & `starbug2-0.4.2/starbug2/misc.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.1/starbug2/param/default.param` & `starbug2-0.4.2/starbug2/param/default.param`

 * *Files 10% similar despite different names*

```diff
@@ -46,18 +46,20 @@
 PSF_SIZE    = -1         //Set fit size of psf (>0) or -1 to take PSF file dimensions
 GEN_RESIDUAL= 0          //generate a residual image
 
 ## SOURCE STATS
 CALC_CROWD  = 1          //Run crowding metric calculation (execution time scales N^2)
 
 ## CATALOGUE MATCHING
-MATCH_THRESH= 0.1        //when combining background subtraction catalogue, minimum separation (arcsec) of centroids to be considered separate sources
+MATCH_THRESH= 0.1        // when combining background subtraction catalogue, minimum separation (arcsec) of centroids to be considered separate sources
 MATCH_COLS  =            // EXTRA columns to include in output matched table i.e sharpness
 RM_MATCH    = -1         // [REMOVING THIS SOON] Remove any sources with less matches than N-RM_MATCH. (if -1, keep everything) 
 NEXP_THRESH = -1         // Keep sources that appear in NUM >= NEXP_THRESH (if -1 keep everything)
+SN_THRESH   = -1         // Remove sources with SN ratio < SN_THRESH before matching (default -1 to not apply this cut)
+BRIDGE_COL  =            // Bridge --band matching NIRCam and MIRI catalogues by ensuring NIRCam catalogue has a match in BRIDGE_COL
 
 ## ARTIFICAL STARS
 NUMBER_ARTIFICIAL_STARS= 500 //number of individual stars to test
 SUBIMAGE_SIZE= 500       //number of pixels ? to crop around artificial star
 MIN_FLUX    = 10         //minimun flux for artificial star
 MAX_FLUX    = 10000      //maximum flux for artificial star
 SEPARATION_THRESH= 2     //number pixels above which the separation is too high and the artifical star failed to be detected
```

### Comparing `starbug2-0.4.1/starbug2/routines.py` & `starbug2-0.4.2/starbug2/routines.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.1/starbug2/starbug.py` & `starbug2-0.4.2/starbug2/starbug.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.1/starbug2/utils.py` & `starbug2-0.4.2/starbug2/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -163,14 +163,37 @@
 
 
 def export_table(table, fname=None, header=None):
     if table:
         if not fname: fname="/tmp/starbug.fits"
         fits.BinTableHDU(data=reindex(table), header=header).writeto(fname, overwrite=True)
 
+def import_table(fname):
+    """
+    """
+    tab=None
+    if os.path.exists(fname):
+        if os.path.splitext(fname)[1]==".fits":
+            tab=Table.read(fname,format="fits")
+            tmp=Table()
+            
+            if "flag" in tab.colnames:
+                tmp.add_column(tab["flag"])
+                tab.remove_columns("flag")
+            if "NUM" in tab.colnames:
+                tmp.add_column(tab["NUM"])
+                tab.remove_columns("NUM")
+            tab=tab.filled(np.nan)
+            if tmp: tab=hstack((tab,tmp))
+
+        else: perror("Table must fits format\n")
+    else: perror("Unable to locate \"%s\"\n"%fname)
+    return tab
+
+
 def find_colnames(tab, basename):
     """
     find substring (basename) within the table colnames
     """
     return [colname for colname in tab.colnames if colname[:len(basename)]==basename]
 
 def combine_fnames(fnames, ntrys=10):
```

### Comparing `starbug2-0.4.1/starbug2.egg-info/PKG-INFO` & `starbug2-0.4.2/starbug2.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: starbug2
-Version: 0.4.1
+Version: 0.4.2
 Summary: JWST PSF photometry in complex crowded fields.
 Author: Conor Nally
 Author-email: conor.nally@ed.ac.uk
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 
 # StarBugII
 
 JWST PSF photometry in dusty crowded fields.
-Last updated: v0.4.1
+Last updated: v0.4.2
 
 [![Python application](https://github.com/conornally/starbug2/actions/workflows/python-app.yml/badge.svg)](https://github.com/conornally/starbug2/actions/workflows/python-app.yml)
 [![PyPI version fury.io](https://badge.fury.io/py/starbug2.svg)](https://pypi.python.org/pypi/starbug2/)
 [![Latest release](https://badgen.net/github/release/conornally/starbug2)](https://github.com/conornally/starbug2/releases)
 
 
 ## Installation
@@ -80,28 +80,26 @@
        --apply-zeropint    a.fits : Apply a zeropoint (-s ZEROPOINT=1.0) to a.fits
        --calc-instr-zp     a.fits : Calculate and apply an instrumental zero point onto a.fits
 
    --> typical runs
       $~ starbug2 -vD -p file.param image.fits      //Source detect on image with a parameter file
       $~ starbug2 -vDM -n4 images*.fits             //Source detect and match outputs of a list of images
       $~ starbug2 -vd image-ap.fits -BP image.fits  //PSF photometry on an image with a source file (image-ap.fits)
-
-
+```
+```bash
 StarbugII Matching 
 usage: starbug2-match [-BGfhv] [-o output] [-p file.param] [-s KEY=VAL] table.fits ...
     -B  --band               : match in "BAND" mode (does not preserve a column for every frame)
     -D  --dither             : match in "DITHER" mode (preserves a column for every frame)
     -f  --full               : export full catalogue
     -G  --generic            : match in "GENERIC" mode
     -h  --help               : show help message
     -o  --output  file.fits  : output matched catalogue
     -p  --param   file.param : load starbug parameter file
     -s  --set     option     : set value in parameter file at runtime (-s MATCH_THRESH=1)
+
+    --> typical runs
+       $~ starbug2-match -Gfo outfile.fits tab1.fits tab2.fits
+       $~ starbug2-match -sMATCH_THRESH=0.2 -sBRIDGE_COL=F444W -Bo out.fits F*W.fits
 ```
 
 See [starbug-manual](https://github.com/conornally/starbug2/blob/main/docs/starbug-manual.md) for more detailed instructions.
-
-## TODO
-
-* Need to really figure out setup.cfg to include the extras files
-* MIRI Background masking
-* psf dither match dropping apMag
```

### Comparing `starbug2-0.4.1/tests/test_routines.py` & `starbug2-0.4.2/tests/test_routines.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.1/tests/test_utils.py` & `starbug2-0.4.2/tests/test_utils.py`

 * *Files identical despite different names*

