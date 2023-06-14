# Comparing `tmp/jiffyCodec-0.1.0.tar.gz` & `tmp/jiffyCodec-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiffyCodec-0.1.0.tar", last modified: Wed Jun 14 03:04:46 2023, max compression
+gzip compressed data, was "jiffyCodec-0.3.1.tar", last modified: Tue Jun 13 19:03:06 2023, max compression
```

## Comparing `jiffyCodec-0.1.0.tar` & `jiffyCodec-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-06-14 03:04:46.318483 jiffyCodec-0.1.0/
--rw-r--r--   0 jeff       (501) staff       (20)    11365 2023-05-10 15:52:49.000000 jiffyCodec-0.1.0/LICENSE
--rw-r--r--   0 jeff       (501) staff       (20)    13431 2023-06-14 03:04:46.318041 jiffyCodec-0.1.0/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)    12905 2023-06-14 03:00:42.000000 jiffyCodec-0.1.0/README.md
--rw-r--r--   0 jeff       (501) staff       (20)      752 2023-06-14 03:04:05.000000 jiffyCodec-0.1.0/pyproject.toml
--rw-r--r--   0 jeff       (501) staff       (20)       38 2023-06-14 03:04:46.318630 jiffyCodec-0.1.0/setup.cfg
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-06-14 03:04:46.314993 jiffyCodec-0.1.0/src/
--rw-r--r--   0 jeff       (501) staff       (20)        1 2023-06-14 02:57:08.000000 jiffyCodec-0.1.0/src/__init__.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-06-14 03:04:46.317101 jiffyCodec-0.1.0/src/jiffyCodec.egg-info/
--rw-r--r--   0 jeff       (501) staff       (20)    13431 2023-06-14 03:04:46.000000 jiffyCodec-0.1.0/src/jiffyCodec.egg-info/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)      269 2023-06-14 03:04:46.000000 jiffyCodec-0.1.0/src/jiffyCodec.egg-info/SOURCES.txt
--rw-r--r--   0 jeff       (501) staff       (20)        1 2023-06-14 03:04:46.000000 jiffyCodec-0.1.0/src/jiffyCodec.egg-info/dependency_links.txt
--rw-r--r--   0 jeff       (501) staff       (20)       89 2023-06-14 03:04:46.000000 jiffyCodec-0.1.0/src/jiffyCodec.egg-info/requires.txt
--rw-r--r--   0 jeff       (501) staff       (20)       20 2023-06-14 03:04:46.000000 jiffyCodec-0.1.0/src/jiffyCodec.egg-info/top_level.txt
--rw-r--r--   0 jeff       (501) staff       (20)    48699 2023-06-14 02:57:08.000000 jiffyCodec-0.1.0/src/jiffyCodec.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-06-14 03:04:46.317453 jiffyCodec-0.1.0/tests/
--rwxr-xr-x   0 jeff       (501) staff       (20)     3493 2023-06-14 03:00:42.000000 jiffyCodec-0.1.0/tests/test.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-06-13 19:03:06.265383 jiffyCodec-0.3.1/
+-rw-r--r--   0 jeff       (501) staff       (20)    11365 2023-05-10 15:52:49.000000 jiffyCodec-0.3.1/LICENSE
+-rw-r--r--   0 jeff       (501) staff       (20)    13431 2023-06-13 19:03:06.264903 jiffyCodec-0.3.1/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)    12905 2023-06-13 18:59:22.000000 jiffyCodec-0.3.1/README.md
+-rw-r--r--   0 jeff       (501) staff       (20)      752 2023-06-13 18:59:22.000000 jiffyCodec-0.3.1/pyproject.toml
+-rw-r--r--   0 jeff       (501) staff       (20)       38 2023-06-13 19:03:06.265498 jiffyCodec-0.3.1/setup.cfg
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-06-13 19:03:06.259028 jiffyCodec-0.3.1/src/
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-06-13 19:03:06.261656 jiffyCodec-0.3.1/src/jiffyCodec/
+-rw-r--r--   0 jeff       (501) staff       (20)        1 2023-05-17 16:31:34.000000 jiffyCodec-0.3.1/src/jiffyCodec/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)    48699 2023-06-13 18:47:04.000000 jiffyCodec-0.3.1/src/jiffyCodec/jiffyCodec.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-06-13 19:03:06.263880 jiffyCodec-0.3.1/src/jiffyCodec.egg-info/
+-rw-r--r--   0 jeff       (501) staff       (20)    13431 2023-06-13 19:03:06.000000 jiffyCodec-0.3.1/src/jiffyCodec.egg-info/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)      291 2023-06-13 19:03:06.000000 jiffyCodec-0.3.1/src/jiffyCodec.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        1 2023-06-13 19:03:06.000000 jiffyCodec-0.3.1/src/jiffyCodec.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       89 2023-06-13 19:03:06.000000 jiffyCodec-0.3.1/src/jiffyCodec.egg-info/requires.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       11 2023-06-13 19:03:06.000000 jiffyCodec-0.3.1/src/jiffyCodec.egg-info/top_level.txt
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-06-13 19:03:06.264289 jiffyCodec-0.3.1/tests/
+-rwxr-xr-x   0 jeff       (501) staff       (20)     3422 2023-06-13 18:59:22.000000 jiffyCodec-0.3.1/tests/test.py
```

### Comparing `jiffyCodec-0.1.0/LICENSE` & `jiffyCodec-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jiffyCodec-0.1.0/PKG-INFO` & `jiffyCodec-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiffyCodec
-Version: 0.1.0
+Version: 0.3.1
 Summary: jiffyCodec: a fast, lossless SIMD compression codec for LiDAR streams
 Author-email: Jeff Ford <jsford64@gmail.com>, Jordan Ford <jsford94@gmail.com>
 Project-URL: Homepage, https://github.com/jsford64/jiffy-compression
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `jiffyCodec-0.1.0/README.md` & `jiffyCodec-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `jiffyCodec-0.1.0/pyproject.toml` & `jiffyCodec-0.3.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jiffyCodec"
-version = "0.1.0"
+version = "0.3.1"
 authors = [
   { name="Jeff Ford", email="jsford64@gmail.com" },
   { name="Jordan Ford", email="jsford94@gmail.com" },
 ]
 description = "jiffyCodec: a fast, lossless SIMD compression codec for LiDAR streams"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `jiffyCodec-0.1.0/src/jiffyCodec.egg-info/PKG-INFO` & `jiffyCodec-0.3.1/src/jiffyCodec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiffyCodec
-Version: 0.1.0
+Version: 0.3.1
 Summary: jiffyCodec: a fast, lossless SIMD compression codec for LiDAR streams
 Author-email: Jeff Ford <jsford64@gmail.com>, Jordan Ford <jsford94@gmail.com>
 Project-URL: Homepage, https://github.com/jsford64/jiffy-compression
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `jiffyCodec-0.1.0/src/jiffyCodec.py` & `jiffyCodec-0.3.1/src/jiffyCodec/jiffyCodec.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 '''
 
 VERSION_MAJOR = 0
-VERSION_MINOR = 3
+VERSION_MINOR = 4
 VERSION = np.uint16(VERSION_MAJOR * 256 + VERSION_MINOR)
 MAGIC = b'JFFY'
 
 ############################### ByteStream Class ###############################
 
 class ByteStream(BufferedRandom):
     '''
```

### Comparing `jiffyCodec-0.1.0/tests/test.py` & `jiffyCodec-0.3.1/tests/test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 import sys
 import path
-sys.path.append(str(path.Path(__file__).abspath().parent)+'/examples')
 from encode_to_file import get_frames
 
 import jiffyCodec as jf
 import numpy as np
 
 '''
     Copyright 2023 Jeff S. Ford and Jordan S. Ford
```

