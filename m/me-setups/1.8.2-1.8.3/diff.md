# Comparing `tmp/me_setups-1.8.2.tar.gz` & `tmp/me_setups-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "me_setups-1.8.2.tar", last modified: Mon Jun 12 06:30:19 2023, max compression
+gzip compressed data, was "me_setups-1.8.3.tar", last modified: Wed Jun 14 13:56:25 2023, max compression
```

## Comparing `me_setups-1.8.2.tar` & `me_setups-1.8.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-12 06:30:19.323285 me_setups-1.8.2/
--rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-12 06:30:19.323332 me_setups-1.8.2/PKG-INFO
--rw-r--r--   0 idof     (12090585) develop   (1000)       19 2023-01-29 18:05:41.000000 me_setups-1.8.2/README.md
--rw-r--r--   0 idof     (12090585) develop   (1000)     1242 2023-06-12 06:30:19.326290 me_setups-1.8.2/setup.cfg
--rw-r--r--   0 idof     (12090585) develop   (1000)       74 2023-01-29 18:02:02.000000 me_setups-1.8.2/setup.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-12 06:30:19.263336 me_setups-1.8.2/src/
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-12 06:30:19.275775 me_setups-1.8.2/src/me_setups/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-29 21:40:13.000000 me_setups-1.8.2/src/me_setups/__init__.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-12 06:30:19.302761 me_setups-1.8.2/src/me_setups/boards/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-02-15 14:02:28.000000 me_setups-1.8.2/src/me_setups/boards/__init__.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      920 2023-03-12 12:03:35.000000 me_setups-1.8.2/src/me_setups/boards/default_boards.py
--rw-r--r--   0 idof     (12090585) develop   (1000)    11657 2023-06-04 13:52:01.000000 me_setups-1.8.2/src/me_setups/boards/gas52.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      119 2023-02-16 19:57:32.000000 me_setups-1.8.2/src/me_setups/boards/types.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-12 06:30:19.321291 me_setups-1.8.2/src/me_setups/components/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-30 07:57:12.000000 me_setups-1.8.2/src/me_setups/components/__init__.py
--rw-r--r--   0 idof     (12090585) develop   (1000)     8597 2023-06-06 17:26:44.000000 me_setups-1.8.2/src/me_setups/components/comp.py
--rw-r--r--   0 idof     (12090585) develop   (1000)    12933 2023-06-04 13:52:01.000000 me_setups-1.8.2/src/me_setups/components/eqs.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      198 2023-05-18 10:10:02.000000 me_setups-1.8.2/src/me_setups/components/mcs.py
--rw-r--r--   0 idof     (12090585) develop   (1000)     4187 2023-05-18 10:10:02.000000 me_setups-1.8.2/src/me_setups/components/mcu.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      488 2023-06-06 17:26:44.000000 me_setups-1.8.2/src/me_setups/utils.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-12 06:30:19.289737 me_setups-1.8.2/src/me_setups.egg-info/
--rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-12 06:30:19.000000 me_setups-1.8.2/src/me_setups.egg-info/PKG-INFO
--rw-r--r--   0 idof     (12090585) develop   (1000)      559 2023-06-12 06:30:19.000000 me_setups-1.8.2/src/me_setups.egg-info/SOURCES.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)        1 2023-06-12 06:30:19.000000 me_setups-1.8.2/src/me_setups.egg-info/dependency_links.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)       66 2023-06-12 06:30:19.000000 me_setups-1.8.2/src/me_setups.egg-info/requires.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)       10 2023-06-12 06:30:19.000000 me_setups-1.8.2/src/me_setups.egg-info/top_level.txt
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-14 13:56:25.292831 me_setups-1.8.3/
+-rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-14 13:56:25.293804 me_setups-1.8.3/PKG-INFO
+-rw-r--r--   0 idof     (12090585) develop   (1000)       19 2023-01-29 18:05:41.000000 me_setups-1.8.3/README.md
+-rw-r--r--   0 idof     (12090585) develop   (1000)     1242 2023-06-14 13:56:25.295799 me_setups-1.8.3/setup.cfg
+-rw-r--r--   0 idof     (12090585) develop   (1000)       74 2023-01-29 18:02:02.000000 me_setups-1.8.3/setup.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-14 13:56:25.251563 me_setups-1.8.3/src/
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-14 13:56:25.265060 me_setups-1.8.3/src/me_setups/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-29 21:40:13.000000 me_setups-1.8.3/src/me_setups/__init__.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-14 13:56:25.280834 me_setups-1.8.3/src/me_setups/boards/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-02-15 14:02:28.000000 me_setups-1.8.3/src/me_setups/boards/__init__.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      920 2023-03-12 12:03:35.000000 me_setups-1.8.3/src/me_setups/boards/default_boards.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)    11657 2023-06-04 13:52:01.000000 me_setups-1.8.3/src/me_setups/boards/gas52.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      119 2023-02-16 19:57:32.000000 me_setups-1.8.3/src/me_setups/boards/types.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-14 13:56:25.290520 me_setups-1.8.3/src/me_setups/components/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-30 07:57:12.000000 me_setups-1.8.3/src/me_setups/components/__init__.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)     8695 2023-06-14 13:55:31.000000 me_setups-1.8.3/src/me_setups/components/comp.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)    12933 2023-06-04 13:52:01.000000 me_setups-1.8.3/src/me_setups/components/eqs.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      198 2023-05-18 10:10:02.000000 me_setups-1.8.3/src/me_setups/components/mcs.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)     4187 2023-05-18 10:10:02.000000 me_setups-1.8.3/src/me_setups/components/mcu.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      488 2023-06-06 17:26:44.000000 me_setups-1.8.3/src/me_setups/utils.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-14 13:56:25.273059 me_setups-1.8.3/src/me_setups.egg-info/
+-rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-14 13:56:25.000000 me_setups-1.8.3/src/me_setups.egg-info/PKG-INFO
+-rw-r--r--   0 idof     (12090585) develop   (1000)      559 2023-06-14 13:56:25.000000 me_setups-1.8.3/src/me_setups.egg-info/SOURCES.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)        1 2023-06-14 13:56:25.000000 me_setups-1.8.3/src/me_setups.egg-info/dependency_links.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)       66 2023-06-14 13:56:25.000000 me_setups-1.8.3/src/me_setups.egg-info/requires.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)       10 2023-06-14 13:56:25.000000 me_setups-1.8.3/src/me_setups.egg-info/top_level.txt
```

### Comparing `me_setups-1.8.2/PKG-INFO` & `me_setups-1.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me_setups
-Version: 1.8.2
+Version: 1.8.3
 Summary: Abstraction for Mobileye setups.
 Home-page: http://gitlab.mobileye.com/idof/me-setups
 Author: Ido Frenkel
 Author-email: ido.frenkel@mobileye.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `me_setups-1.8.2/setup.cfg` & `me_setups-1.8.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = me_setups
-version = 1.8.2
+version = 1.8.3
 description = Abstraction for Mobileye setups.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = http://gitlab.mobileye.com/idof/me-setups
 author = Ido Frenkel
 author_email = ido.frenkel@mobileye.com
 classifiers =
```

### Comparing `me_setups-1.8.2/src/me_setups/boards/default_boards.py` & `me_setups-1.8.3/src/me_setups/boards/default_boards.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.8.2/src/me_setups/boards/gas52.py` & `me_setups-1.8.3/src/me_setups/boards/gas52.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.8.2/src/me_setups/components/comp.py` & `me_setups-1.8.3/src/me_setups/components/comp.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,16 @@
 
     def stop_sniffing(self) -> None:
         """\
             Stops the Sniffing thread
         """
         if self.sniff_thread.alive.is_set():  # pragma: no cover
             self.sniff_thread.stop()
+            if self.protocol.log_file is not None:
+                self.protocol.log_file.close()
 
         self.sniff_thread.join(10)
         if self.sniff_thread.is_alive():
             raise RuntimeError("stop sniffing fail!")  # pragma: no cover
 
     def config_sniffer(
         self,
```

### Comparing `me_setups-1.8.2/src/me_setups/components/eqs.py` & `me_setups-1.8.3/src/me_setups/components/eqs.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.8.2/src/me_setups/components/mcu.py` & `me_setups-1.8.3/src/me_setups/components/mcu.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.8.2/src/me_setups.egg-info/PKG-INFO` & `me_setups-1.8.3/src/me_setups.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me-setups
-Version: 1.8.2
+Version: 1.8.3
 Summary: Abstraction for Mobileye setups.
 Home-page: http://gitlab.mobileye.com/idof/me-setups
 Author: Ido Frenkel
 Author-email: ido.frenkel@mobileye.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `me_setups-1.8.2/src/me_setups.egg-info/SOURCES.txt` & `me_setups-1.8.3/src/me_setups.egg-info/SOURCES.txt`

 * *Files identical despite different names*

