# Comparing `tmp/via-0.0.2.tar.gz` & `tmp/via-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/via-0.0.2.tar", last modified: Wed Sep  5 08:37:48 2018, max compression
+gzip compressed data, was "via-0.1.1.tar", last modified: Wed Jun 14 12:01:01 2023, max compression
```

## Comparing `via-0.0.2.tar` & `via-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0 keming    (1000) keming    (1000)        0 2018-09-05 08:37:48.000000 via-0.0.2/
--rwxrwxrwx   0 keming    (1000) keming    (1000)     1369 2018-09-05 08:37:48.000000 via-0.0.2/PKG-INFO
--rwxrwxrwx   0 keming    (1000) keming    (1000)      680 2018-09-05 08:35:53.000000 via-0.0.2/README.md
--rwxrwxrwx   0 keming    (1000) keming    (1000)       38 2018-09-05 08:37:48.000000 via-0.0.2/setup.cfg
--rwxrwxrwx   0 keming    (1000) keming    (1000)      870 2018-09-05 08:36:03.000000 via-0.0.2/setup.py
-drwxrwxrwx   0 keming    (1000) keming    (1000)        0 2018-09-05 08:37:48.000000 via-0.0.2/via/
--rwxrwxrwx   0 keming    (1000) keming    (1000)     1189 2018-09-05 06:06:58.000000 via-0.0.2/via/ignore.py
--rwxrwxrwx   0 keming    (1000) keming    (1000)      990 2018-09-05 06:05:08.000000 via-0.0.2/via/license.py
--rwxrwxrwx   0 keming    (1000) keming    (1000)      443 2018-09-05 05:57:01.000000 via-0.0.2/via/utils.py
--rwxrwxrwx   0 keming    (1000) keming    (1000)      543 2018-09-05 08:33:12.000000 via-0.0.2/via/__init__.py
-drwxrwxrwx   0 keming    (1000) keming    (1000)        0 2018-09-05 08:37:48.000000 via-0.0.2/via.egg-info/
--rwxrwxrwx   0 keming    (1000) keming    (1000)        1 2018-09-05 08:37:48.000000 via-0.0.2/via.egg-info/dependency_links.txt
--rwxrwxrwx   0 keming    (1000) keming    (1000)       34 2018-09-05 08:37:48.000000 via-0.0.2/via.egg-info/entry_points.txt
--rwxrwxrwx   0 keming    (1000) keming    (1000)     1369 2018-09-05 08:37:48.000000 via-0.0.2/via.egg-info/PKG-INFO
--rwxrwxrwx   0 keming    (1000) keming    (1000)        9 2018-09-05 08:37:48.000000 via-0.0.2/via.egg-info/requires.txt
--rwxrwxrwx   0 keming    (1000) keming    (1000)      240 2018-09-05 08:37:48.000000 via-0.0.2/via.egg-info/SOURCES.txt
--rwxrwxrwx   0 keming    (1000) keming    (1000)        4 2018-09-05 08:37:48.000000 via-0.0.2/via.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:01:01.897400 via-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-14 12:00:48.000000 via-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-14 12:01:01.897400 via-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-14 12:00:48.000000 via-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 12:01:01.897400 via-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-14 12:00:48.000000 via-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:01:01.897400 via-0.1.1/via/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-14 12:00:48.000000 via-0.1.1/via/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-14 12:00:48.000000 via-0.1.1/via/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-14 12:00:48.000000 via-0.1.1/via/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-14 12:00:48.000000 via-0.1.1/via/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:01:01.897400 via-0.1.1/via.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-14 12:01:01.000000 via-0.1.1/via.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-14 12:01:01.000000 via-0.1.1/via.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 12:01:01.000000 via-0.1.1/via.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-14 12:01:01.000000 via-0.1.1/via.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 12:01:01.000000 via-0.1.1/via.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-14 12:01:01.000000 via-0.1.1/via.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `via-0.0.2/README.md` & `via-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 
 Initialize your repository.
 
 ## Feature
 
 - [x] `.gitignore`
 - [x] `License`
-- [x] args
 
-## Toturail
+## Tutorial
 
 ```sh
 # download python .gitignore file and MIT License
 # file will be saved to current dir
 via -i python -l mit
+# print to stdout
+via -i python --print
 ```
 
 ## Support
 
 ### Ignore
 
 All the files are downloaded from [github/gitignore](https://github.com/github/gitignore)
```

### Comparing `via-0.0.2/setup.py` & `via-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="via",
-    version="0.0.2",
+    version="0.1.1",
     author="Keming Yang",
     author_email="kemingy94@gmail.com",
     description="initialize your repos",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kemingy/via",
     packages=find_packages(),
```

### Comparing `via-0.0.2/via/__init__.py` & `via-0.1.1/via/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import argparse
 
-from .ignore import download_file
-from .license import download_license
+from via.ignore import download_ignore_file
+from via.license import download_license
+
 
 def main():
-    parser = argparse.ArgumentParser(description='via args parser')
-    parser.add_argument('-i', '--ignore', help='ignore language')
-    parser.add_argument('-l', '--license', help='license name')
+    parser = argparse.ArgumentParser(description="via args parser")
+    parser.add_argument("-i", "--ignore", help="ignore language")
+    parser.add_argument("-l", "--license", help="license name")
+    parser.add_argument("-p", "--print", help="print to stdout", action="store_true")
     args = parser.parse_args()
 
     if args.ignore:
-        download_file(args.ignore)
+        download_ignore_file(args.ignore, args.print)
 
     if args.license:
-        download_license(args.license)
+        download_license(args.license, args.print)
 
     if not (args.ignore or args.license):
-        print(parser.print_help())
+        print(parser.print_help())
```

