# Comparing `tmp/git-dummy-0.0.7.tar.gz` & `tmp/git-dummy-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-dummy-0.0.7.tar", last modified: Thu Mar 23 18:59:39 2023, max compression
+gzip compressed data, was "git-dummy-0.0.8.tar", last modified: Wed Jun 14 06:23:49 2023, max compression
```

## Comparing `git-dummy-0.0.7.tar` & `git-dummy-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-23 18:59:39.545029 git-dummy-0.0.7/
--rw-rw-rw-   0        0        0    18431 2023-03-23 15:27:25.000000 git-dummy-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     5653 2023-03-23 18:59:39.545029 git-dummy-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     4941 2023-03-23 15:27:25.000000 git-dummy-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-03-23 18:59:39.536027 git-dummy-0.0.7/git_dummy/
--rw-rw-rw-   0        0        0        0 2023-03-23 15:27:25.000000 git-dummy-0.0.7/git_dummy/__init__.py
--rw-rw-rw-   0        0        0     4068 2023-03-23 15:27:25.000000 git-dummy-0.0.7/git_dummy/__main__.py
--rw-rw-rw-   0        0        0      319 2023-03-23 15:27:25.000000 git-dummy-0.0.7/git_dummy/settings.py
-drwxrwxrwx   0        0        0        0 2023-03-23 18:59:39.545029 git-dummy-0.0.7/git_dummy.egg-info/
--rw-rw-rw-   0        0        0     5653 2023-03-23 18:59:39.000000 git-dummy-0.0.7/git_dummy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-03-23 18:59:39.000000 git-dummy-0.0.7/git_dummy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-23 18:59:39.000000 git-dummy-0.0.7/git_dummy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-03-23 18:59:39.000000 git-dummy-0.0.7/git_dummy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       25 2023-03-23 18:59:39.000000 git-dummy-0.0.7/git_dummy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-23 18:59:39.000000 git-dummy-0.0.7/git_dummy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-23 18:59:39.545029 git-dummy-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1214 2023-03-23 18:52:35.000000 git-dummy-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:23:49.824033 git-dummy-0.0.8/
+-rw-rw-rw-   0        0        0    18431 2023-03-23 15:27:25.000000 git-dummy-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     5804 2023-06-14 06:23:49.824033 git-dummy-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5092 2023-06-14 06:01:15.000000 git-dummy-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 06:23:49.816033 git-dummy-0.0.8/git_dummy/
+-rw-rw-rw-   0        0        0        0 2023-03-23 15:27:25.000000 git-dummy-0.0.8/git_dummy/__init__.py
+-rw-rw-rw-   0        0        0     5146 2023-06-14 06:17:47.000000 git-dummy-0.0.8/git_dummy/__main__.py
+-rw-rw-rw-   0        0        0      345 2023-06-14 05:53:40.000000 git-dummy-0.0.8/git_dummy/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:23:49.824033 git-dummy-0.0.8/git_dummy.egg-info/
+-rw-rw-rw-   0        0        0     5804 2023-06-14 06:23:49.000000 git-dummy-0.0.8/git_dummy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-06-14 06:23:49.000000 git-dummy-0.0.8/git_dummy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 06:23:49.000000 git-dummy-0.0.8/git_dummy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-14 06:23:49.000000 git-dummy-0.0.8/git_dummy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       25 2023-06-14 06:23:49.000000 git-dummy-0.0.8/git_dummy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-14 06:23:49.000000 git-dummy-0.0.8/git_dummy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 06:23:49.824033 git-dummy-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1214 2023-06-14 06:22:50.000000 git-dummy-0.0.8/setup.py
```

### Comparing `git-dummy-0.0.7/LICENSE` & `git-dummy-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `git-dummy-0.0.7/PKG-INFO` & `git-dummy-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-dummy
-Version: 0.0.7
+Version: 0.0.8
 Summary: Generate dummy Git repositories populated with the desired number of commits, branches, and structure.
 Home-page: https://initialcommit.com/tools/git-dummy
 Author: Jacob Stopak
 Author-email: jacob@initialcommit.io
 Project-URL: Homepage, https://initialcommit.com/tools/git-dummy
 Project-URL: Source, https://github.com/initialcommit-com/git-dummy
 Keywords: git dummy generate populate repo repository
@@ -77,16 +77,17 @@
 Available options and flags include:
 
 `--name`: The name of the dummy Git repo, defaults to "dummy".  
 `--commits`: The number of commits to populate in the dummy Git repo, defaults to 5.  
 `--branches`: The number of branches to generate in the dummy Git repo, defaults to 1.  
 `--diverge-at`: The commit number at which branches diverge from `main`.  
 `--merge`: A comma separated list of branch postfix ids to merge back into `main`.  
-`--git-dir`: The path at which to store the dummy Git repo, defaults to current directory.
-`--no-subdir`: Initialize the dummy Git repo in the current directory instead of in a subdirectory.
+`--git-dir`: The path at which to store the dummy Git repo, defaults to current directory.  
+`--no-subdir`: Initialize the dummy Git repo in the current directory instead of in a subdirectory.  
+`--constant_sha`: Use constant values for commit author, email, and commit date parameters to yield consistent sha1 values across git-dummy runs.
 
 ## Command examples
 Generate a dummy Git repo called "cheese" on your Desktop, with 2 branches and 10 commits on each branch:
 
 ```console
 $ git-dummy --name=cheese --branches=2 --commits=10 --git-dir=~/Desktop
 ```
```

### Comparing `git-dummy-0.0.7/README.md` & `git-dummy-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,16 +60,17 @@
 Available options and flags include:
 
 `--name`: The name of the dummy Git repo, defaults to "dummy".  
 `--commits`: The number of commits to populate in the dummy Git repo, defaults to 5.  
 `--branches`: The number of branches to generate in the dummy Git repo, defaults to 1.  
 `--diverge-at`: The commit number at which branches diverge from `main`.  
 `--merge`: A comma separated list of branch postfix ids to merge back into `main`.  
-`--git-dir`: The path at which to store the dummy Git repo, defaults to current directory.
-`--no-subdir`: Initialize the dummy Git repo in the current directory instead of in a subdirectory.
+`--git-dir`: The path at which to store the dummy Git repo, defaults to current directory.  
+`--no-subdir`: Initialize the dummy Git repo in the current directory instead of in a subdirectory.  
+`--constant_sha`: Use constant values for commit author, email, and commit date parameters to yield consistent sha1 values across git-dummy runs.
 
 ## Command examples
 Generate a dummy Git repo called "cheese" on your Desktop, with 2 branches and 10 commits on each branch:
 
 ```console
 $ git-dummy --name=cheese --branches=2 --commits=10 --git-dir=~/Desktop
 ```
```

### Comparing `git-dummy-0.0.7/git_dummy.egg-info/PKG-INFO` & `git-dummy-0.0.8/git_dummy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-dummy
-Version: 0.0.7
+Version: 0.0.8
 Summary: Generate dummy Git repositories populated with the desired number of commits, branches, and structure.
 Home-page: https://initialcommit.com/tools/git-dummy
 Author: Jacob Stopak
 Author-email: jacob@initialcommit.io
 Project-URL: Homepage, https://initialcommit.com/tools/git-dummy
 Project-URL: Source, https://github.com/initialcommit-com/git-dummy
 Keywords: git dummy generate populate repo repository
@@ -77,16 +77,17 @@
 Available options and flags include:
 
 `--name`: The name of the dummy Git repo, defaults to "dummy".  
 `--commits`: The number of commits to populate in the dummy Git repo, defaults to 5.  
 `--branches`: The number of branches to generate in the dummy Git repo, defaults to 1.  
 `--diverge-at`: The commit number at which branches diverge from `main`.  
 `--merge`: A comma separated list of branch postfix ids to merge back into `main`.  
-`--git-dir`: The path at which to store the dummy Git repo, defaults to current directory.
-`--no-subdir`: Initialize the dummy Git repo in the current directory instead of in a subdirectory.
+`--git-dir`: The path at which to store the dummy Git repo, defaults to current directory.  
+`--no-subdir`: Initialize the dummy Git repo in the current directory instead of in a subdirectory.  
+`--constant_sha`: Use constant values for commit author, email, and commit date parameters to yield consistent sha1 values across git-dummy runs.
 
 ## Command examples
 Generate a dummy Git repo called "cheese" on your Desktop, with 2 branches and 10 commits on each branch:
 
 ```console
 $ git-dummy --name=cheese --branches=2 --commits=10 --git-dir=~/Desktop
 ```
```

### Comparing `git-dummy-0.0.7/setup.py` & `git-dummy-0.0.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="git-dummy",
-    version="0.0.7",
+    version="0.0.8",
     author="Jacob Stopak",
     author_email="jacob@initialcommit.io",
     description="Generate dummy Git repositories populated with the desired number of commits, branches, and structure.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://initialcommit.com/tools/git-dummy",
     packages=setuptools.find_packages(),
```

