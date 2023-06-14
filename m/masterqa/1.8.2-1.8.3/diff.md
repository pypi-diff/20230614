# Comparing `tmp/masterqa-1.8.2.tar.gz` & `tmp/masterqa-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masterqa-1.8.2.tar", last modified: Fri Apr 21 19:37:46 2023, max compression
+gzip compressed data, was "masterqa-1.8.3.tar", last modified: Wed Jun 14 00:35:52 2023, max compression
```

## Comparing `masterqa-1.8.2.tar` & `masterqa-1.8.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-21 19:37:46.187779 masterqa-1.8.2/
--rw-r--r--   0 michael    (501) staff       (20)     1682 2022-12-06 03:15:26.000000 masterqa-1.8.2/.gitignore
--rw-r--r--   0 michael    (501) staff       (20)     1080 2022-12-06 03:15:26.000000 masterqa-1.8.2/LICENSE
--rw-r--r--   0 michael    (501) staff       (20)      100 2022-12-06 03:15:26.000000 masterqa-1.8.2/MANIFEST.in
--rw-r--r--   0 michael    (501) staff       (20)     3015 2023-04-21 19:37:46.187828 masterqa-1.8.2/PKG-INFO
--rwxr-xr-x   0 michael    (501) staff       (20)     2616 2023-01-24 04:43:53.000000 masterqa-1.8.2/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-21 19:37:46.187153 masterqa-1.8.2/masterqa/
--rwxr-xr-x   0 michael    (501) staff       (20)       48 2022-12-06 03:15:26.000000 masterqa-1.8.2/masterqa/__init__.py
--rwxr-xr-x   0 michael    (501) staff       (20)    17697 2023-04-21 19:32:04.000000 masterqa-1.8.2/masterqa/master_qa.py
--rwxr-xr-x   0 michael    (501) staff       (20)      718 2022-12-06 03:15:26.000000 masterqa-1.8.2/masterqa/settings.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-21 19:37:46.187679 masterqa-1.8.2/masterqa.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     3015 2023-04-21 19:37:46.000000 masterqa-1.8.2/masterqa.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      310 2023-04-21 19:37:46.000000 masterqa-1.8.2/masterqa.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-21 19:37:46.000000 masterqa-1.8.2/masterqa.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       77 2023-04-21 19:37:46.000000 masterqa-1.8.2/masterqa.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        9 2023-04-21 19:37:46.000000 masterqa-1.8.2/masterqa.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)     1440 2023-04-21 19:32:04.000000 masterqa-1.8.2/pytest.ini
--rwxr-xr-x   0 michael    (501) staff       (20)       82 2023-04-21 19:32:04.000000 masterqa-1.8.2/requirements.txt
--rwxr-xr-x   0 michael    (501) staff       (20)      188 2023-04-21 19:37:46.188017 masterqa-1.8.2/setup.cfg
--rwxr-xr-x   0 michael    (501) staff       (20)     3481 2023-04-21 19:32:04.000000 masterqa-1.8.2/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-14 00:35:52.376828 masterqa-1.8.3/
+-rw-r--r--   0 michael    (501) staff       (20)     1682 2022-12-06 03:15:26.000000 masterqa-1.8.3/.gitignore
+-rw-r--r--   0 michael    (501) staff       (20)     1080 2022-12-06 03:15:26.000000 masterqa-1.8.3/LICENSE
+-rw-r--r--   0 michael    (501) staff       (20)      100 2022-12-06 03:15:26.000000 masterqa-1.8.3/MANIFEST.in
+-rw-r--r--   0 michael    (501) staff       (20)     3015 2023-06-14 00:35:52.376898 masterqa-1.8.3/PKG-INFO
+-rwxr-xr-x   0 michael    (501) staff       (20)     2616 2023-01-24 04:43:53.000000 masterqa-1.8.3/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-14 00:35:52.375926 masterqa-1.8.3/masterqa/
+-rwxr-xr-x   0 michael    (501) staff       (20)       48 2022-12-06 03:15:26.000000 masterqa-1.8.3/masterqa/__init__.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    17697 2023-04-21 19:32:04.000000 masterqa-1.8.3/masterqa/master_qa.py
+-rwxr-xr-x   0 michael    (501) staff       (20)      718 2022-12-06 03:15:26.000000 masterqa-1.8.3/masterqa/settings.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-14 00:35:52.376696 masterqa-1.8.3/masterqa.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     3015 2023-06-14 00:35:52.000000 masterqa-1.8.3/masterqa.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      310 2023-06-14 00:35:52.000000 masterqa-1.8.3/masterqa.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-14 00:35:52.000000 masterqa-1.8.3/masterqa.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       77 2023-06-14 00:35:52.000000 masterqa-1.8.3/masterqa.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        9 2023-06-14 00:35:52.000000 masterqa-1.8.3/masterqa.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)     1440 2023-04-21 19:32:04.000000 masterqa-1.8.3/pytest.ini
+-rwxr-xr-x   0 michael    (501) staff       (20)       82 2023-06-14 00:32:16.000000 masterqa-1.8.3/requirements.txt
+-rwxr-xr-x   0 michael    (501) staff       (20)      188 2023-06-14 00:35:52.377138 masterqa-1.8.3/setup.cfg
+-rwxr-xr-x   0 michael    (501) staff       (20)     3481 2023-06-14 00:32:16.000000 masterqa-1.8.3/setup.py
```

### Comparing `masterqa-1.8.2/.gitignore` & `masterqa-1.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `masterqa-1.8.2/LICENSE` & `masterqa-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `masterqa-1.8.2/PKG-INFO` & `masterqa-1.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masterqa
-Version: 1.8.2
+Version: 1.8.3
 Summary: Automation-Assisted Manual Testing - https://masterqa.com
 Home-page: https://github.com/masterqa/MasterQA
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Platform: Windows
```

### Comparing `masterqa-1.8.2/README.md` & `masterqa-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `masterqa-1.8.2/masterqa/master_qa.py` & `masterqa-1.8.3/masterqa/master_qa.py`

 * *Files identical despite different names*

### Comparing `masterqa-1.8.2/masterqa/settings.py` & `masterqa-1.8.3/masterqa/settings.py`

 * *Files identical despite different names*

### Comparing `masterqa-1.8.2/masterqa.egg-info/PKG-INFO` & `masterqa-1.8.3/masterqa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masterqa
-Version: 1.8.2
+Version: 1.8.3
 Summary: Automation-Assisted Manual Testing - https://masterqa.com
 Home-page: https://github.com/masterqa/MasterQA
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Platform: Windows
```

### Comparing `masterqa-1.8.2/pytest.ini` & `masterqa-1.8.3/pytest.ini`

 * *Files identical despite different names*

### Comparing `masterqa-1.8.2/setup.py` & `masterqa-1.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,28 +57,28 @@
         print("\n*** The Release was PUBLISHED SUCCESSFULLY to PyPI! :) ***\n")
     else:
         print("\n>>> The Release was NOT PUBLISHED to PyPI! <<<\n")
     sys.exit()
 
 setup(
     name="masterqa",
-    version="1.8.2",
+    version="1.8.3",
     description="Automation-Assisted Manual Testing - https://masterqa.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     platforms=["Windows", "Linux", "Mac OS-X"],
     url="https://github.com/masterqa/MasterQA",
     author="Michael Mintz",
     author_email="mdmintz@gmail.com",
     maintainer="Michael Mintz",
     license="MIT",
     python_requires=">=3.6",
     install_requires=[
-        "seleniumbase>=4.14.1",
-        "pdbp>=1.3.1",
+        "seleniumbase>=4.15.3",
+        "pdbp>=1.4.0",
         "tabcompleter>=1.2.0",
         "sbvirtualdisplay>=1.2.0",
     ],
     packages=["masterqa"],
     entry_points={
         "nose.plugins": []
     }
```

