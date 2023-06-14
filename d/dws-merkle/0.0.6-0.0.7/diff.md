# Comparing `tmp/dws-merkle-0.0.6.tar.gz` & `tmp/dws-merkle-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dws-merkle-0.0.6.tar", last modified: Sun Dec 25 09:59:53 2022, max compression
+gzip compressed data, was "dws-merkle-0.0.7.tar", last modified: Wed Jun 14 09:46:42 2023, max compression
```

## Comparing `dws-merkle-0.0.6.tar` & `dws-merkle-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2022-12-25 09:59:53.200528 dws-merkle-0.0.6/
--rw-r--r--   0 nivshitrit   (501) staff       (20)     1073 2022-10-09 08:58:27.000000 dws-merkle-0.0.6/LICENSE.rst
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6728 2022-12-25 09:59:53.200604 dws-merkle-0.0.6/PKG-INFO
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6211 2022-10-09 08:58:27.000000 dws-merkle-0.0.6/README.md
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2022-12-25 09:59:53.199733 dws-merkle-0.0.6/dws_merkle/
--rw-r--r--   0 nivshitrit   (501) staff       (20)      814 2022-12-25 09:57:39.000000 dws-merkle-0.0.6/dws_merkle/Base.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)       94 2022-12-01 11:25:58.000000 dws-merkle-0.0.6/dws_merkle/__init__.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)       58 2022-12-25 09:59:49.000000 dws-merkle-0.0.6/dws_merkle/common.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     2746 2022-12-25 09:57:39.000000 dws-merkle-0.0.6/dws_merkle/merkleTree.py
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2022-12-25 09:59:53.200418 dws-merkle-0.0.6/dws_merkle.egg-info/
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6728 2022-12-25 09:59:52.000000 dws-merkle-0.0.6/dws_merkle.egg-info/PKG-INFO
--rw-r--r--   0 nivshitrit   (501) staff       (20)      297 2022-12-25 09:59:53.000000 dws-merkle-0.0.6/dws_merkle.egg-info/SOURCES.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)        1 2022-12-25 09:59:52.000000 dws-merkle-0.0.6/dws_merkle.egg-info/dependency_links.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)        9 2022-12-25 09:59:53.000000 dws-merkle-0.0.6/dws_merkle.egg-info/requires.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)       11 2022-12-25 09:59:53.000000 dws-merkle-0.0.6/dws_merkle.egg-info/top_level.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)      107 2022-12-25 09:59:53.200844 dws-merkle-0.0.6/setup.cfg
--rw-r--r--   0 nivshitrit   (501) staff       (20)     1146 2022-12-01 11:26:41.000000 dws-merkle-0.0.6/setup.py
+drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-14 09:46:42.816842 dws-merkle-0.0.7/
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     1073 2023-06-14 09:10:53.000000 dws-merkle-0.0.7/LICENSE.rst
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     6767 2023-06-14 09:46:42.816918 dws-merkle-0.0.7/PKG-INFO
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     6211 2023-06-14 09:10:53.000000 dws-merkle-0.0.7/README.md
+drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-14 09:46:42.816109 dws-merkle-0.0.7/dws_merkle/
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      640 2023-06-14 09:33:16.000000 dws-merkle-0.0.7/dws_merkle/Base.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)       94 2023-06-14 09:10:53.000000 dws-merkle-0.0.7/dws_merkle/__init__.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)       58 2023-06-14 09:46:11.000000 dws-merkle-0.0.7/dws_merkle/common.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     2746 2023-06-14 09:10:53.000000 dws-merkle-0.0.7/dws_merkle/merkleTree.py
+drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-14 09:46:42.816721 dws-merkle-0.0.7/dws_merkle.egg-info/
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     6767 2023-06-14 09:46:42.000000 dws-merkle-0.0.7/dws_merkle.egg-info/PKG-INFO
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      297 2023-06-14 09:46:42.000000 dws-merkle-0.0.7/dws_merkle.egg-info/SOURCES.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)        1 2023-06-14 09:46:42.000000 dws-merkle-0.0.7/dws_merkle.egg-info/dependency_links.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)        9 2023-06-14 09:46:42.000000 dws-merkle-0.0.7/dws_merkle.egg-info/requires.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)       11 2023-06-14 09:46:42.000000 dws-merkle-0.0.7/dws_merkle.egg-info/top_level.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      107 2023-06-14 09:46:42.817154 dws-merkle-0.0.7/setup.cfg
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     1146 2023-06-14 09:10:53.000000 dws-merkle-0.0.7/setup.py
```

### Comparing `dws-merkle-0.0.6/LICENSE.rst` & `dws-merkle-0.0.7/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dws-merkle-0.0.6/PKG-INFO` & `dws-merkle-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: dws-merkle
-Version: 0.0.6
+Version: 0.0.7
 Summary: dws-merkle
+Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
+Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -103,7 +105,9 @@
 Show your appreciation to those who have contributed to the project.
 
 ## License
 For open source projects, say how it is licensed.
 
 ## Project status
 If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
+
+
```

### Comparing `dws-merkle-0.0.6/README.md` & `dws-merkle-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dws-merkle-0.0.6/dws_merkle/Base.py` & `dws-merkle-0.0.7/dws_merkle/Base.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,12 +13,8 @@
             self.headers = {"Authorization": username + "," + key}
             self.url = "https://test-api.dcentralab.com/"
         if stage == 'staging':
             self.headers = {"Authorization": username + "," + key}
             self.url = "https://staging.dcentralab.com/"
         if stage == 'main':
             self.headers = {"Authorization": username + "," + key}
-            self.url = "https://api.dcentralab.com/"
-
-        response = requests.get(self.url, headers=self.headers)
-        if response.status_code != 200:
-            raise "Unauthorized, MerkleTree instance cannot be used"
+            self.url = "https://api.dcentralab.com/"
```

### Comparing `dws-merkle-0.0.6/dws_merkle/merkleTree.py` & `dws-merkle-0.0.7/dws_merkle/merkleTree.py`

 * *Files identical despite different names*

### Comparing `dws-merkle-0.0.6/dws_merkle.egg-info/PKG-INFO` & `dws-merkle-0.0.7/dws_merkle.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: dws-merkle
-Version: 0.0.6
+Version: 0.0.7
 Summary: dws-merkle
+Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
+Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -103,7 +105,9 @@
 Show your appreciation to those who have contributed to the project.
 
 ## License
 For open source projects, say how it is licensed.
 
 ## Project status
 If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
+
+
```

### Comparing `dws-merkle-0.0.6/setup.py` & `dws-merkle-0.0.7/setup.py`

 * *Files identical despite different names*

