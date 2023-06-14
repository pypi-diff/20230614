# Comparing `tmp/pianogen-0.0.3.tar.gz` & `tmp/pianogen-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pianogen-0.0.3.tar", last modified: Fri Jun  9 13:23:01 2023, max compression
+gzip compressed data, was "pianogen-0.0.4.tar", last modified: Tue Jun 13 09:26:00 2023, max compression
```

## Comparing `pianogen-0.0.3.tar` & `pianogen-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:01.355190 pianogen-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-05-24 11:02:52.000000 pianogen-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2759 2023-06-09 13:23:01.355190 pianogen-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2055 2023-05-24 12:21:29.000000 pianogen-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:01.323027 pianogen-0.0.3/pianogen/
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:01.343136 pianogen-0.0.3/pianogen/pianogen/
--rw-rw-rw-   0        0        0      150 2023-05-24 11:15:01.000000 pianogen-0.0.3/pianogen/pianogen/__init__.py
--rw-rw-rw-   0        0        0     1718 2023-06-09 13:10:11.000000 pianogen-0.0.3/pianogen/pianogen/commonTracks.py
--rw-rw-rw-   0        0        0     3135 2023-06-09 13:20:37.000000 pianogen-0.0.3/pianogen/pianogen/parse_to_npy.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:01.355190 pianogen-0.0.3/pianogen/pianogen.egg-info/
--rw-rw-rw-   0        0        0     2759 2023-06-09 13:23:01.000000 pianogen-0.0.3/pianogen/pianogen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-06-09 13:23:01.000000 pianogen-0.0.3/pianogen/pianogen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 13:23:01.000000 pianogen-0.0.3/pianogen/pianogen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-09 13:23:01.000000 pianogen-0.0.3/pianogen/pianogen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-09 13:23:01.000000 pianogen-0.0.3/pianogen/pianogen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-22 07:26:14.000000 pianogen-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      868 2023-06-09 13:23:01.355190 pianogen-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 09:26:00.212584 pianogen-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-05-24 11:02:52.000000 pianogen-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2759 2023-06-13 09:26:00.212584 pianogen-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2055 2023-05-24 12:21:29.000000 pianogen-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 09:26:00.186330 pianogen-0.0.4/pianogen/
+drwxrwxrwx   0        0        0        0 2023-06-13 09:26:00.199471 pianogen-0.0.4/pianogen/pianogen/
+-rw-rw-rw-   0        0        0      150 2023-05-24 11:15:01.000000 pianogen-0.0.4/pianogen/pianogen/__init__.py
+-rw-rw-rw-   0        0        0     1978 2023-06-13 09:20:01.000000 pianogen-0.0.4/pianogen/pianogen/commonTracks.py
+-rw-rw-rw-   0        0        0     3288 2023-06-13 09:13:34.000000 pianogen-0.0.4/pianogen/pianogen/parse_to_npy.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:26:00.212584 pianogen-0.0.4/pianogen/pianogen.egg-info/
+-rw-rw-rw-   0        0        0     2759 2023-06-13 09:26:00.000000 pianogen-0.0.4/pianogen/pianogen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-06-13 09:26:00.000000 pianogen-0.0.4/pianogen/pianogen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 09:26:00.000000 pianogen-0.0.4/pianogen/pianogen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-13 09:26:00.000000 pianogen-0.0.4/pianogen/pianogen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 09:26:00.000000 pianogen-0.0.4/pianogen/pianogen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-22 07:26:14.000000 pianogen-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      868 2023-06-13 09:26:00.213586 pianogen-0.0.4/setup.cfg
```

### Comparing `pianogen-0.0.3/LICENSE` & `pianogen-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pianogen-0.0.3/PKG-INFO` & `pianogen-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pianogen
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pianoroll-generator A package to generate pianoroll (NPZ) datasets
 Home-page: https://github.com/cliffordkleinsr/pianoroll-generator
 Author: Clifford Njoroge
 Author-email: cnjoroge@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pianogen-0.0.3/README.md` & `pianogen-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pianogen-0.0.3/pianogen/pianogen/commonTracks.py` & `pianogen-0.0.4/pianogen/pianogen/commonTracks.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     ) -> None:
         self.fldr = fldr # the folder where your midis are saved
         #self.savez = savez
 
     def get_items(
         self,
     ) -> None:
-        files = glob.glob(join(self.fldr, '*mid'))
+        files = glob.glob(join(self.fldr, '*[mM][iI][dD]'))
         str_files, clean_files = [], []
         print("Cleaning Files ...............\ ")
         for f in files:
             try:
                 gud_f =Multitrack(f)
                 len(gud_f.tracks)
                 str_files +=[f]
@@ -30,30 +30,39 @@
         
     def most_common(
         self,
         lst,
     ) -> None:
         return max(set(lst), key=lst.count)
     
+    
     def get_listItems(
         self,
     ) -> None:
         #os.makedirs(self.savez, exist_ok=True)
         str_files, clean_files = self.get_items()
               
         tracks = [len(f.tracks) for f in clean_files]
         mc = self.most_common(tracks)
-
+        
+        cocon = "The most common have {} tracks".format(mc)
         '''loop'''
         common = []
         for f, c in zip(str_files, clean_files):
             if len(c.tracks) == mc:
                 common +=[f]
                 #print('moving:', f, 'with no. of tracks ', len(m.tracks))
                 #shutil.move(f, self.savez)
-        with open('common_files.json', 'w') as outfile:
-            json.dump(common, outfile)      
+        os.makedirs('utilities', exist_ok=True)
+
+        
+        with open('utilities/common_files.json', 'w') as outfile:
+            json.dump(common, outfile)
+        
+         
+        with open('utilities/mc.txt', 'w') as mc_file:
+            mc_file.write(cocon)
```

### Comparing `pianogen-0.0.3/pianogen/pianogen/parse_to_npy.py` & `pianogen-0.0.4/pianogen/pianogen/parse_to_npy.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self.results = []
         
     def get_items(
         self,
     ) -> None:
         
         #all_files = glob.glob(join(self.fldr, '*mid'))
-        with open('common_files.json','r') as opfile:
+        with open('utilities/common_files.json','r') as opfile:
             common_files = json.load(opfile)   
         return common_files
 
     def parse(
         self,
     ) -> None:
         N_TRACKS = [len(Multitrack(f).tracks) for f in self.get_items()][0]
@@ -64,20 +64,21 @@
             if pianoroll.shape[0] < 4 * 4 * self.BEAT_RESOLUTION:
                 continue
 
             # Keep only the mid-range pitches
             pianoroll = pianoroll[:, 24:108]
 
             # Reshape and get the phrase pianorolls
+            #Original shape: (num_time_steps, 4 * num_beats, num_pitches, num_tracks)
             pianoroll = pianoroll.reshape(-1, 4 * self.BEAT_RESOLUTION, 84, N_TRACKS)
             self.results.append(np.concatenate(
                 [pianoroll[:-3], pianoroll[1:-2], pianoroll[2:-1], pianoroll[3:]], 1))
 
             result = np.concatenate(self.results, 0)
-            
+            #New shape: (-1, 4 * num_beats, num_pitches, num_tracks)
             #print('Original shape: ', result.shape)
             
             result = result.reshape(-1, RESHAPE_PARAMS['num_bar'], RESHAPE_PARAMS['num_timestep'],
                         RESHAPE_PARAMS['num_pitch'], RESHAPE_PARAMS['num_track'])
 
             #print('New shape: ', result.shape)
```

### Comparing `pianogen-0.0.3/pianogen/pianogen.egg-info/PKG-INFO` & `pianogen-0.0.4/pianogen/pianogen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pianogen
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pianoroll-generator A package to generate pianoroll (NPZ) datasets
 Home-page: https://github.com/cliffordkleinsr/pianoroll-generator
 Author: Clifford Njoroge
 Author-email: cnjoroge@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pianogen-0.0.3/setup.cfg` & `pianogen-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6961 6e6f 6765 6e0d 0a76 6572   = pianogen..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e33 0d0a 6175  sion = 0.0.3..au
+00000020: 7369 6f6e 203d 2030 2e30 2e34 0d0a 6175  sion = 0.0.4..au
 00000030: 7468 6f72 203d 2043 6c69 6666 6f72 6420  thor = Clifford 
 00000040: 4e6a 6f72 6f67 650d 0a61 7574 686f 725f  Njoroge..author_
 00000050: 656d 6169 6c20 3d20 636e 6a6f 726f 6765  email = cnjoroge
 00000060: 4067 6d61 696c 2e63 6f6d 0d0a 6465 7363  @gmail.com..desc
 00000070: 7269 7074 696f 6e20 3d20 5069 616e 6f72  ription = Pianor
 00000080: 6f6c 6c2d 6765 6e65 7261 746f 7220 4120  oll-generator A 
 00000090: 7061 636b 6167 6520 746f 2067 656e 6572  package to gener
```

