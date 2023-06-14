# Comparing `tmp/bdpyconsts-1.0.1.tar.gz` & `tmp/bdpyconsts-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdpyconsts-1.0.1.tar", last modified: Mon Aug  8 10:27:59 2022, max compression
+gzip compressed data, was "bdpyconsts-1.1.0.tar", last modified: Wed Jun 14 06:57:42 2023, max compression
```

## Comparing `bdpyconsts-1.0.1.tar` & `bdpyconsts-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-08-08 10:27:59.987906 bdpyconsts-1.0.1/
--rw-rw-rw-   0        0        0      701 2022-08-08 10:27:59.987906 bdpyconsts-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       82 2022-05-11 02:54:27.000000 bdpyconsts-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      843 2022-08-08 10:27:59.988814 bdpyconsts-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-08 10:27:59.972670 bdpyconsts-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2022-08-08 10:27:59.978343 bdpyconsts-1.0.1/src/bdpyconsts/
--rw-rw-rw-   0        0        0        0 2022-08-08 08:09:00.000000 bdpyconsts-1.0.1/src/bdpyconsts/__init__.py
--rw-rw-rw-   0        0        0      953 2022-08-08 10:27:17.000000 bdpyconsts-1.0.1/src/bdpyconsts/bdpyconsts.py
-drwxrwxrwx   0        0        0        0 2022-08-08 10:27:59.986902 bdpyconsts-1.0.1/src/bdpyconsts.egg-info/
--rw-rw-rw-   0        0        0      701 2022-08-08 10:27:59.000000 bdpyconsts-1.0.1/src/bdpyconsts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2022-08-08 10:27:59.000000 bdpyconsts-1.0.1/src/bdpyconsts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-08 10:27:59.000000 bdpyconsts-1.0.1/src/bdpyconsts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-08-08 10:27:59.000000 bdpyconsts-1.0.1/src/bdpyconsts.egg-info/top_level.txt
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-14 06:57:42.554695 bdpyconsts-1.1.0/
+-rw-r--r--   0 zhicheng   (501) staff       (20)     1056 2023-06-14 06:57:42.554785 bdpyconsts-1.1.0/PKG-INFO
+-rw-r--r--   0 zhicheng   (501) staff       (20)      368 2023-06-14 06:56:56.000000 bdpyconsts-1.1.0/README.md
+-rw-r--r--   0 zhicheng   (501) staff       (20)       80 2022-09-04 10:23:26.000000 bdpyconsts-1.1.0/pyproject.toml
+-rw-r--r--   0 zhicheng   (501) staff       (20)      812 2023-06-14 06:57:42.556569 bdpyconsts-1.1.0/setup.cfg
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-14 06:57:42.553134 bdpyconsts-1.1.0/src/
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-14 06:57:42.553718 bdpyconsts-1.1.0/src/bdpyconsts/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2022-09-04 10:23:26.000000 bdpyconsts-1.1.0/src/bdpyconsts/__init__.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     1438 2023-06-14 06:55:35.000000 bdpyconsts-1.1.0/src/bdpyconsts/bdpyconst.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-14 06:57:42.554590 bdpyconsts-1.1.0/src/bdpyconsts.egg-info/
+-rw-r--r--   0 zhicheng   (501) staff       (20)     1056 2023-06-14 06:57:42.000000 bdpyconsts-1.1.0/src/bdpyconsts.egg-info/PKG-INFO
+-rw-r--r--   0 zhicheng   (501) staff       (20)      241 2023-06-14 06:57:42.000000 bdpyconsts-1.1.0/src/bdpyconsts.egg-info/SOURCES.txt
+-rw-r--r--   0 zhicheng   (501) staff       (20)        1 2023-06-14 06:57:42.000000 bdpyconsts-1.1.0/src/bdpyconsts.egg-info/dependency_links.txt
+-rw-r--r--   0 zhicheng   (501) staff       (20)       11 2023-06-14 06:57:42.000000 bdpyconsts-1.1.0/src/bdpyconsts.egg-info/top_level.txt
```

### Comparing `bdpyconsts-1.0.1/PKG-INFO` & `bdpyconsts-1.1.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,31 @@
-Metadata-Version: 2.1
-Name: bdpyconsts
-Version: 1.0.1
-Summary: Implement python constant configuration and reading
-Home-page: https://github.com/biandoucheng/bd-py-const
-Author: biandoucheng
-Author-email: biandoucheng@outlook.com
-Project-URL: Bug Tracker, https://github.com/biandoucheng/bd-py-const/issues
-Project-URL: Use Example, https://github.com/biandoucheng/open-example/tree/main/bdpyconsts-example
-Classifier: Programming Language :: Python :: 3.5
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
+[metadata]
+name = bdpyconsts
+version = 1.1.0
+author = biandoucheng
+author_email = biandoucheng@outlook.com
+description = Implement python constant configuration and reading
+long_description = file: README.md
+long_description_content_type = text/markdown
+url = https://github.com/biandoucheng/bd-py-const
+project_urls = 
+	Bug Tracker = https://github.com/biandoucheng/bd-py-const/issues
+	Use Example = https://github.com/biandoucheng/open-example/tree/main/bdpyconsts-example
+classifiers = 
+	Programming Language :: Python :: 3.5
+	License :: OSI Approved :: Apache Software License
+	Operating System :: OS Independent
+	Development Status :: 5 - Production/Stable
+
+[options]
+package_dir = 
+	= src
+packages = find:
+python_requires = >=3.5
+
+[options.packages.find]
+where = src
+
+[egg_info]
+tag_build = 
+tag_date = 0
+
```

