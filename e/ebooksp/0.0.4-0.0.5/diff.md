# Comparing `tmp/ebooksp-0.0.4.tar.gz` & `tmp/ebooksp-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebooksp-0.0.4.tar", last modified: Wed Jun 14 02:30:03 2023, max compression
+gzip compressed data, was "ebooksp-0.0.5.tar", last modified: Wed Jun 14 02:35:48 2023, max compression
```

## Comparing `ebooksp-0.0.4.tar` & `ebooksp-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-14 02:30:03.048684 ebooksp-0.0.4/
--rw-r--r--   0 bo         (501) staff       (20)    11357 2023-06-13 11:17:27.000000 ebooksp-0.0.4/LICENSE
--rw-r--r--   0 bo         (501) staff       (20)     1025 2023-06-14 02:30:03.048561 ebooksp-0.0.4/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)      567 2023-06-13 11:19:50.000000 ebooksp-0.0.4/README.md
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-14 02:30:03.047897 ebooksp-0.0.4/ebooksp/
--rw-r--r--   0 bo         (501) staff       (20)      667 2023-06-13 11:19:50.000000 ebooksp-0.0.4/ebooksp/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     2023 2023-06-14 01:56:52.000000 ebooksp-0.0.4/ebooksp/ebook_convert_format.py
--rw-r--r--   0 bo         (501) staff       (20)     1309 2023-06-14 02:29:54.000000 ebooksp-0.0.4/ebooksp/ebook_to_text.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-14 02:30:03.048385 ebooksp-0.0.4/ebooksp.egg-info/
--rw-r--r--   0 bo         (501) staff       (20)     1025 2023-06-14 02:30:02.000000 ebooksp-0.0.4/ebooksp.egg-info/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)      257 2023-06-14 02:30:03.000000 ebooksp-0.0.4/ebooksp.egg-info/SOURCES.txt
--rw-r--r--   0 bo         (501) staff       (20)        1 2023-06-14 02:30:02.000000 ebooksp-0.0.4/ebooksp.egg-info/dependency_links.txt
--rw-r--r--   0 bo         (501) staff       (20)       13 2023-06-14 02:30:02.000000 ebooksp-0.0.4/ebooksp.egg-info/requires.txt
--rw-r--r--   0 bo         (501) staff       (20)        8 2023-06-14 02:30:02.000000 ebooksp-0.0.4/ebooksp.egg-info/top_level.txt
--rw-r--r--   0 bo         (501) staff       (20)       38 2023-06-14 02:30:03.048725 ebooksp-0.0.4/setup.cfg
--rw-r--r--   0 bo         (501) staff       (20)      791 2023-06-14 02:29:54.000000 ebooksp-0.0.4/setup.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-14 02:35:48.288675 ebooksp-0.0.5/
+-rw-r--r--   0 bo         (501) staff       (20)    11357 2023-06-13 11:17:27.000000 ebooksp-0.0.5/LICENSE
+-rw-r--r--   0 bo         (501) staff       (20)     1025 2023-06-14 02:35:48.288555 ebooksp-0.0.5/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)      567 2023-06-13 11:19:50.000000 ebooksp-0.0.5/README.md
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-14 02:35:48.287886 ebooksp-0.0.5/ebooksp/
+-rw-r--r--   0 bo         (501) staff       (20)      667 2023-06-13 11:19:50.000000 ebooksp-0.0.5/ebooksp/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     2023 2023-06-14 01:56:52.000000 ebooksp-0.0.5/ebooksp/ebook_convert_format.py
+-rw-r--r--   0 bo         (501) staff       (20)     1308 2023-06-14 02:35:36.000000 ebooksp-0.0.5/ebooksp/ebook_to_text.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-14 02:35:48.288403 ebooksp-0.0.5/ebooksp.egg-info/
+-rw-r--r--   0 bo         (501) staff       (20)     1025 2023-06-14 02:35:48.000000 ebooksp-0.0.5/ebooksp.egg-info/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)      257 2023-06-14 02:35:48.000000 ebooksp-0.0.5/ebooksp.egg-info/SOURCES.txt
+-rw-r--r--   0 bo         (501) staff       (20)        1 2023-06-14 02:35:48.000000 ebooksp-0.0.5/ebooksp.egg-info/dependency_links.txt
+-rw-r--r--   0 bo         (501) staff       (20)       13 2023-06-14 02:35:48.000000 ebooksp-0.0.5/ebooksp.egg-info/requires.txt
+-rw-r--r--   0 bo         (501) staff       (20)        8 2023-06-14 02:35:48.000000 ebooksp-0.0.5/ebooksp.egg-info/top_level.txt
+-rw-r--r--   0 bo         (501) staff       (20)       38 2023-06-14 02:35:48.288710 ebooksp-0.0.5/setup.cfg
+-rw-r--r--   0 bo         (501) staff       (20)      791 2023-06-14 02:35:36.000000 ebooksp-0.0.5/setup.py
```

### Comparing `ebooksp-0.0.4/LICENSE` & `ebooksp-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ebooksp-0.0.4/PKG-INFO` & `ebooksp-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebooksp
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Conversion Tool for e-book
 Home-page: https://gitee.com/maxbanana
 Author: hongbo liu
 Author-email: 782027465@qq.com
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ebooksp-0.0.4/README.md` & `ebooksp-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ebooksp-0.0.4/ebooksp/__init__.py` & `ebooksp-0.0.5/ebooksp/__init__.py`

 * *Files identical despite different names*

### Comparing `ebooksp-0.0.4/ebooksp/ebook_convert_format.py` & `ebooksp-0.0.5/ebooksp/ebook_convert_format.py`

 * *Files identical despite different names*

### Comparing `ebooksp-0.0.4/ebooksp/ebook_to_text.py` & `ebooksp-0.0.5/ebooksp/ebook_to_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     if delete:
         delete_epub(epub_book, timeout)
     return res
 
 
 def delete_epub(epub_path: str, timeout=60):
     """删除epub book"""
-    command = ['rm ', epub_path]
+    command = ['rm', epub_path]
     ret = subprocess.run(command, timeout=timeout)
     if ret.returncode == 0:
         print(f"success: delete {epub_path}")
     else:
         print(f"error: delete {epub_path}")
```

### Comparing `ebooksp-0.0.4/ebooksp.egg-info/PKG-INFO` & `ebooksp-0.0.5/ebooksp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebooksp
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Conversion Tool for e-book
 Home-page: https://gitee.com/maxbanana
 Author: hongbo liu
 Author-email: 782027465@qq.com
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ebooksp-0.0.4/setup.py` & `ebooksp-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='ebooksp',
-    version='0.0.4',
+    version='0.0.5',
     packages=setuptools.find_packages(),
     url='https://gitee.com/maxbanana',
     license='Apache',
     author='hongbo liu',
     author_email='782027465@qq.com',
     description='A Conversion Tool for e-book',
     long_description=long_description,
```

