# Comparing `tmp/license_tools-0.1.1.tar.gz` & `tmp/license_tools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "license_tools-0.1.1.tar", last modified: Tue Jun 13 14:49:14 2023, max compression
+gzip compressed data, was "license_tools-0.1.2.tar", last modified: Wed Jun 14 10:56:09 2023, max compression
```

## Comparing `license_tools-0.1.1.tar` & `license_tools-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-06-13 14:49:14.850900 license_tools-0.1.1/
--rw-r--r--   0 sdostal   (6000) users      (100)    11358 2022-05-16 19:23:11.000000 license_tools-0.1.1/LICENSE.txt
--rw-r--r--   0 sdostal   (6000) users      (100)     2397 2023-06-13 14:49:14.850900 license_tools-0.1.1/PKG-INFO
--rw-r--r--   0 sdostal   (6000) users      (100)     1618 2023-06-13 14:23:14.000000 license_tools-0.1.1/README.md
-drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-06-13 14:49:14.850900 license_tools-0.1.1/license_tools/
--rw-r--r--   0 sdostal   (6000) users      (100)        0 2021-01-11 15:34:09.000000 license_tools-0.1.1/license_tools/__init__.py
--rw-r--r--   0 sdostal   (6000) users      (100)     2422 2023-06-13 14:06:54.000000 license_tools-0.1.1/license_tools/__main__.py
--rw-r--r--   0 sdostal   (6000) users      (100)    10259 2023-06-13 14:20:04.000000 license_tools-0.1.1/license_tools/scancode_tools.py
-drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-06-13 14:49:14.850900 license_tools-0.1.1/license_tools.egg-info/
--rw-r--r--   0 sdostal   (6000) users      (100)     2397 2023-06-13 14:49:14.000000 license_tools-0.1.1/license_tools.egg-info/PKG-INFO
--rw-r--r--   0 sdostal   (6000) users      (100)      298 2023-06-13 14:49:14.000000 license_tools-0.1.1/license_tools.egg-info/SOURCES.txt
--rw-r--r--   0 sdostal   (6000) users      (100)        1 2023-06-13 14:49:14.000000 license_tools-0.1.1/license_tools.egg-info/dependency_links.txt
--rw-r--r--   0 sdostal   (6000) users      (100)       68 2023-06-13 14:49:14.000000 license_tools-0.1.1/license_tools.egg-info/requires.txt
--rw-r--r--   0 sdostal   (6000) users      (100)       14 2023-06-13 14:49:14.000000 license_tools-0.1.1/license_tools.egg-info/top_level.txt
--rw-r--r--   0 sdostal   (6000) users      (100)       38 2023-06-13 14:49:14.850900 license_tools-0.1.1/setup.cfg
--rw-r--r--   0 sdostal   (6000) users      (100)     1423 2023-06-13 14:49:04.000000 license_tools-0.1.1/setup.py
+drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-06-14 10:56:09.185801 license_tools-0.1.2/
+-rw-r--r--   0 sdostal   (6000) users      (100)    11358 2022-05-16 19:23:11.000000 license_tools-0.1.2/LICENSE.txt
+-rw-r--r--   0 sdostal   (6000) users      (100)     2397 2023-06-14 10:56:09.185801 license_tools-0.1.2/PKG-INFO
+-rw-r--r--   0 sdostal   (6000) users      (100)     1618 2023-06-13 14:23:14.000000 license_tools-0.1.2/README.md
+drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-06-14 10:56:09.185801 license_tools-0.1.2/license_tools/
+-rw-r--r--   0 sdostal   (6000) users      (100)        0 2021-01-11 15:34:09.000000 license_tools-0.1.2/license_tools/__init__.py
+-rw-r--r--   0 sdostal   (6000) users      (100)     2427 2023-06-14 10:37:12.000000 license_tools-0.1.2/license_tools/__main__.py
+-rw-r--r--   0 sdostal   (6000) users      (100)    10036 2023-06-14 10:55:20.000000 license_tools-0.1.2/license_tools/scancode_tools.py
+drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-06-14 10:56:09.185801 license_tools-0.1.2/license_tools.egg-info/
+-rw-r--r--   0 sdostal   (6000) users      (100)     2397 2023-06-14 10:56:09.000000 license_tools-0.1.2/license_tools.egg-info/PKG-INFO
+-rw-r--r--   0 sdostal   (6000) users      (100)      298 2023-06-14 10:56:09.000000 license_tools-0.1.2/license_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 sdostal   (6000) users      (100)        1 2023-06-14 10:56:09.000000 license_tools-0.1.2/license_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 sdostal   (6000) users      (100)       68 2023-06-14 10:56:09.000000 license_tools-0.1.2/license_tools.egg-info/requires.txt
+-rw-r--r--   0 sdostal   (6000) users      (100)       14 2023-06-14 10:56:09.000000 license_tools-0.1.2/license_tools.egg-info/top_level.txt
+-rw-r--r--   0 sdostal   (6000) users      (100)       38 2023-06-14 10:56:09.185801 license_tools-0.1.2/setup.cfg
+-rw-r--r--   0 sdostal   (6000) users      (100)     1423 2023-06-14 10:52:34.000000 license_tools-0.1.2/setup.py
```

### Comparing `license_tools-0.1.1/LICENSE.txt` & `license_tools-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `license_tools-0.1.1/PKG-INFO` & `license_tools-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: license_tools
-Version: 0.1.1
+Version: 0.1.2
 Summary: Collection of tools for working with Open Source licenses
 Home-page: https://github.com/stefan6419846/license_tools
 Author: stefan6419846
 License: Apache-2.0
 Keywords: open source,license,package,dependency,licensing
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `license_tools-0.1.1/README.md` & `license_tools-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `license_tools-0.1.1/license_tools/__main__.py` & `license_tools-0.1.2/license_tools/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,27 +24,27 @@
         '--index-url', action='store', type=str, required=False, default='', help='PyPI index URL to use.'
     )
     parser.add_argument(
         '--jobs', action='store', type=int, required=False, default=4, help='Parallel jobs to use.'
     )
 
     parser.add_argument(
-        '--retrieve-copyrights', action='store_true', required=False, default=True, help='Retrieve copyrights.'
+        '--retrieve-copyrights', action='store_true', required=False, default=False, help='Retrieve copyrights.'
     )
     parser.add_argument(
-        '--retrieve-emails', action='store_true', required=False, default=True, help='Retrieve e-mails.'
+        '--retrieve-emails', action='store_true', required=False, default=False, help='Retrieve e-mails.'
     )
     parser.add_argument(
-        '--retrieve-file-info', action='store_true', required=False, default=True, help='Retrieve file information.'
+        '--retrieve-file-info', action='store_true', required=False, default=False, help='Retrieve file information.'
     )
     parser.add_argument(
-        '--retrieve-urls', action='store_true', required=False, default=True, help='Retrieve URLs.'
+        '--retrieve-urls', action='store_true', required=False, default=False, help='Retrieve URLs.'
     )
     parser.add_argument(
-        '--retrieve-ldd-data', action='store_true', required=False, default=True, help='Retrieve shared object linking data.'
+        '--retrieve-ldd-data', action='store_true', required=False, default=False, help='Retrieve shared object linking data.'
     )
 
     arguments = parser.parse_args()
 
     scancode_tools.run(
         directory=arguments.directory,
         file_path=arguments.file,
```

### Comparing `license_tools-0.1.1/license_tools/scancode_tools.py` & `license_tools-0.1.2/license_tools/scancode_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,18 +177,14 @@
         if self.retrieve_licenses:
             self.licenses = Licenses(**api.get_licenses(path_str))
         if self.retrieve_file_info:
             self.file_info = FileInfo(**api.get_file_info(path_str))
 
 
 def check_shared_objects(path: Path, short_path: str) -> str:
-    # https://opensource.stackexchange.com/questions/13060/linking-closed-source-with-linux-vdso-so-1
-    # https://github.com/torvalds/linux/blob/master/LICENSES/exceptions/Linux-syscall-note
-    # https://github.com/torvalds/linux/blob/master/COPYING
-    # https://www.kernel.org/doc/html/v4.18/process/license-rules.html
     if path.suffix != '.so' and not (path.suffixes and path.suffixes[0] == '.so'):
         return
     output = subprocess.check_output(['ldd', path], stderr=subprocess.PIPE)
     return output.decode('UTF-8')
 
 
 def run_on_file(
@@ -197,16 +193,18 @@
         retrieve_copyrights: bool = False,
         retrieve_emails: bool = False,
         retrieve_file_info: bool = False,
         retrieve_urls: bool = False,
         retrieve_ldd_data: bool = False,
 ) -> FileResults:
     if retrieve_ldd_data:
-        print(short_path)
-        print(check_shared_objects(path=path, short_path=short_path))
+        results = check_shared_objects(path=path, short_path=short_path)
+        if results:
+            print(short_path)
+            print(check_shared_objects(path=path, short_path=short_path))
     return FileResults(
         path=path,
         short_path=short_path,
         retrieve_copyrights=retrieve_copyrights,
         retrieve_emails=retrieve_emails,
         retrieve_file_info=retrieve_file_info,
         retrieve_urls=retrieve_urls,
```

### Comparing `license_tools-0.1.1/license_tools.egg-info/PKG-INFO` & `license_tools-0.1.2/license_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: license-tools
-Version: 0.1.1
+Version: 0.1.2
 Summary: Collection of tools for working with Open Source licenses
 Home-page: https://github.com/stefan6419846/license_tools
 Author: stefan6419846
 License: Apache-2.0
 Keywords: open source,license,package,dependency,licensing
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `license_tools-0.1.1/setup.py` & `license_tools-0.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 ROOT_DIRECTORY = Path(__file__).parent.resolve()
 
 
 setuptools.setup(
     name='license_tools',
     description='Collection of tools for working with Open Source licenses',
-    version='0.1.1',
+    version='0.1.2',
     license='Apache-2.0',
     long_description=Path(ROOT_DIRECTORY / 'README.md').read_text(encoding='UTF-8'),
     long_description_content_type='text/markdown',
     author='stefan6419846',
     url='https://github.com/stefan6419846/license_tools',
     packages=setuptools.find_packages(),
     include_package_data=True,
```

