# Comparing `tmp/circuitpython-build-tools-1.8.6.tar.gz` & `tmp/circuitpython-build-tools-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/circuitpython-build-tools-1.8.6.tar", last modified: Tue Sep 14 18:48:09 2021, max compression
+gzip compressed data, was "dist/circuitpython-build-tools-1.9.0.tar", last modified: Tue Dec 14 17:33:12 2021, max compression
```

## Comparing `circuitpython-build-tools-1.8.6.tar` & `circuitpython-build-tools-1.9.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 18:48:09.000000 circuitpython-build-tools-1.8.6/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 18:48:09.000000 circuitpython-build-tools-1.8.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 18:48:09.000000 circuitpython-build-tools-1.8.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1789 2021-09-14 18:47:59.000000 circuitpython-build-tools-1.8.6/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      764 2021-09-14 18:47:59.000000 circuitpython-build-tools-1.8.6/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      128 2021-09-14 18:47:59.000000 circuitpython-build-tools-1.8.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     3228 2021-09-14 18:47:59.000000 circuitpython-build-tools-1.8.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2021-09-14 18:47:59.000000 circuitpython-build-tools-1.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      285 2021-09-14 18:48:09.000000 circuitpython-build-tools-1.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3964 2021-09-14 18:47:59.000000 circuitpython-build-tools-1.8.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 18:48:09.000000 circuitpython-build-tools-1.8.6/circuitpython_build_tools/
--rw-r--r--   0 runner    (1001) docker     (121)    12992 2021-09-14 18:47:59.000000 circuitpython-build-tools-1.8.6/circuitpython_build_tools/build.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 18:48:09.000000 circuitpython-build-tools-1.8.6/circuitpython_build_tools/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)    11937 2021-09-14 18:47:59.000000 circuitpython-build-tools-1.8.6/circuitpython_build_tools/scripts/build_bundles.py
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2021-09-14 18:47:59.000000 circuitpython-build-tools-1.8.6/circuitpython_build_tools/scripts/build_mpy_cross.py
--rw-r--r--   0 runner    (1001) docker     (121)     1396 2021-09-14 18:47:59.000000 circuitpython-build-tools-1.8.6/circuitpython_build_tools/target_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 18:48:09.000000 circuitpython-build-tools-1.8.6/circuitpython_build_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2021-09-14 18:48:09.000000 circuitpython-build-tools-1.8.6/circuitpython_build_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      659 2021-09-14 18:48:09.000000 circuitpython-build-tools-1.8.6/circuitpython_build_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-14 18:48:09.000000 circuitpython-build-tools-1.8.6/circuitpython_build_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      131 2021-09-14 18:48:09.000000 circuitpython-build-tools-1.8.6/circuitpython_build_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-14 18:48:09.000000 circuitpython-build-tools-1.8.6/circuitpython_build_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-09-14 18:48:09.000000 circuitpython-build-tools-1.8.6/circuitpython_build_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-09-14 18:48:09.000000 circuitpython-build-tools-1.8.6/circuitpython_build_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2021-09-14 18:47:59.000000 circuitpython-build-tools-1.8.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-14 18:48:09.000000 circuitpython-build-tools-1.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      774 2021-09-14 18:47:59.000000 circuitpython-build-tools-1.8.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 17:33:12.000000 circuitpython-build-tools-1.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 17:33:12.000000 circuitpython-build-tools-1.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 17:33:12.000000 circuitpython-build-tools-1.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1789 2021-12-14 17:33:01.000000 circuitpython-build-tools-1.9.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      764 2021-12-14 17:33:01.000000 circuitpython-build-tools-1.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2021-12-14 17:33:01.000000 circuitpython-build-tools-1.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     3228 2021-12-14 17:33:01.000000 circuitpython-build-tools-1.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1096 2021-12-14 17:33:01.000000 circuitpython-build-tools-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2021-12-14 17:33:12.000000 circuitpython-build-tools-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3964 2021-12-14 17:33:01.000000 circuitpython-build-tools-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 17:33:12.000000 circuitpython-build-tools-1.9.0/circuitpython_build_tools/
+-rw-r--r--   0 runner    (1001) docker     (121)    12992 2021-12-14 17:33:01.000000 circuitpython-build-tools-1.9.0/circuitpython_build_tools/build.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 17:33:12.000000 circuitpython-build-tools-1.9.0/circuitpython_build_tools/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    11937 2021-12-14 17:33:01.000000 circuitpython-build-tools-1.9.0/circuitpython_build_tools/scripts/build_bundles.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1568 2021-12-14 17:33:01.000000 circuitpython-build-tools-1.9.0/circuitpython_build_tools/scripts/build_mpy_cross.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1351 2021-12-14 17:33:01.000000 circuitpython-build-tools-1.9.0/circuitpython_build_tools/target_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 17:33:12.000000 circuitpython-build-tools-1.9.0/circuitpython_build_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2021-12-14 17:33:12.000000 circuitpython-build-tools-1.9.0/circuitpython_build_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      659 2021-12-14 17:33:12.000000 circuitpython-build-tools-1.9.0/circuitpython_build_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-14 17:33:12.000000 circuitpython-build-tools-1.9.0/circuitpython_build_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      131 2021-12-14 17:33:12.000000 circuitpython-build-tools-1.9.0/circuitpython_build_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-14 17:33:12.000000 circuitpython-build-tools-1.9.0/circuitpython_build_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-12-14 17:33:12.000000 circuitpython-build-tools-1.9.0/circuitpython_build_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2021-12-14 17:33:12.000000 circuitpython-build-tools-1.9.0/circuitpython_build_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2021-12-14 17:33:01.000000 circuitpython-build-tools-1.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-14 17:33:12.000000 circuitpython-build-tools-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      774 2021-12-14 17:33:01.000000 circuitpython-build-tools-1.9.0/setup.py
```

### Comparing `circuitpython-build-tools-1.8.6/.github/workflows/build.yml` & `circuitpython-build-tools-1.9.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-build-tools-1.8.6/.github/workflows/release.yml` & `circuitpython-build-tools-1.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-build-tools-1.8.6/CODE_OF_CONDUCT.md` & `circuitpython-build-tools-1.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-build-tools-1.8.6/LICENSE` & `circuitpython-build-tools-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-build-tools-1.8.6/README.md` & `circuitpython-build-tools-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `circuitpython-build-tools-1.8.6/circuitpython_build_tools/build.py` & `circuitpython-build-tools-1.9.0/circuitpython_build_tools/build.py`

 * *Files identical despite different names*

### Comparing `circuitpython-build-tools-1.8.6/circuitpython_build_tools/scripts/build_bundles.py` & `circuitpython-build-tools-1.9.0/circuitpython_build_tools/scripts/build_bundles.py`

 * *Files identical despite different names*

### Comparing `circuitpython-build-tools-1.8.6/circuitpython_build_tools/scripts/build_mpy_cross.py` & `circuitpython-build-tools-1.9.0/circuitpython_build_tools/scripts/build_mpy_cross.py`

 * *Files identical despite different names*

### Comparing `circuitpython-build-tools-1.8.6/circuitpython_build_tools/target_versions.py` & `circuitpython-build-tools-1.9.0/circuitpython_build_tools/target_versions.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,10 +21,9 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 # The tag specifies which version of CircuitPython to use for mpy-cross.
 # The name is used when constructing the zip file names.
 VERSIONS = [
-    {"tag": "6.3.0", "name": "6.x"},
-    {"tag": "7.0.0-alpha.3", "name": "7.x"},
+    {"tag": "7.0.0", "name": "7.x"},
 ]
```

### Comparing `circuitpython-build-tools-1.8.6/circuitpython_build_tools.egg-info/SOURCES.txt` & `circuitpython-build-tools-1.9.0/circuitpython_build_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-build-tools-1.8.6/setup.py` & `circuitpython-build-tools-1.9.0/setup.py`

 * *Files identical despite different names*

