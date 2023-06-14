# Comparing `tmp/test_kmn_456-0.0.1.tar.gz` & `tmp/test_kmn_456-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_kmn_456-0.0.1.tar", last modified: Wed Jun 14 14:41:10 2023, max compression
+gzip compressed data, was "test_kmn_456-0.1.3.tar", last modified: Wed Jun 14 18:04:02 2023, max compression
```

## Comparing `test_kmn_456-0.0.1.tar` & `test_kmn_456-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 madhukanoor   (501) staff       (20)        0 2023-06-14 14:41:10.166587 test_kmn_456-0.0.1/
--rw-r--r--   0 madhukanoor   (501) staff       (20)     1074 2023-06-14 13:48:18.000000 test_kmn_456-0.0.1/LICENSE
--rw-r--r--   0 madhukanoor   (501) staff       (20)     1291 2023-06-14 14:41:10.166342 test_kmn_456-0.0.1/PKG-INFO
--rw-r--r--   0 madhukanoor   (501) staff       (20)      783 2023-06-14 14:09:03.000000 test_kmn_456-0.0.1/README.md
--rw-r--r--   0 madhukanoor   (501) staff       (20)      582 2023-06-14 13:47:23.000000 test_kmn_456-0.0.1/pyproject.toml
--rw-r--r--   0 madhukanoor   (501) staff       (20)       38 2023-06-14 14:41:10.166650 test_kmn_456-0.0.1/setup.cfg
-drwxr-xr-x   0 madhukanoor   (501) staff       (20)        0 2023-06-14 14:41:10.164570 test_kmn_456-0.0.1/src/
-drwxr-xr-x   0 madhukanoor   (501) staff       (20)        0 2023-06-14 14:41:10.165370 test_kmn_456-0.0.1/src/test_kmn_456/
--rw-r--r--   0 madhukanoor   (501) staff       (20)        0 2023-06-14 13:44:30.000000 test_kmn_456-0.0.1/src/test_kmn_456/__init__.py
--rw-r--r--   0 madhukanoor   (501) staff       (20)       43 2023-06-14 13:45:08.000000 test_kmn_456-0.0.1/src/test_kmn_456/example.py
-drwxr-xr-x   0 madhukanoor   (501) staff       (20)        0 2023-06-14 14:41:10.166095 test_kmn_456-0.0.1/src/test_kmn_456.egg-info/
--rw-r--r--   0 madhukanoor   (501) staff       (20)     1291 2023-06-14 14:41:10.000000 test_kmn_456-0.0.1/src/test_kmn_456.egg-info/PKG-INFO
--rw-r--r--   0 madhukanoor   (501) staff       (20)      249 2023-06-14 14:41:10.000000 test_kmn_456-0.0.1/src/test_kmn_456.egg-info/SOURCES.txt
--rw-r--r--   0 madhukanoor   (501) staff       (20)        1 2023-06-14 14:41:10.000000 test_kmn_456-0.0.1/src/test_kmn_456.egg-info/dependency_links.txt
--rw-r--r--   0 madhukanoor   (501) staff       (20)       13 2023-06-14 14:41:10.000000 test_kmn_456-0.0.1/src/test_kmn_456.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:04:02.492271 test_kmn_456-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-14 18:03:46.000000 test_kmn_456-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-14 18:04:02.492271 test_kmn_456-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-14 18:03:46.000000 test_kmn_456-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-14 18:03:46.000000 test_kmn_456-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 18:04:02.492271 test_kmn_456-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:04:02.492271 test_kmn_456-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:04:02.492271 test_kmn_456-0.1.3/src/test_kmn_456/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:03:46.000000 test_kmn_456-0.1.3/src/test_kmn_456/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-14 18:03:46.000000 test_kmn_456-0.1.3/src/test_kmn_456/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:04:02.492271 test_kmn_456-0.1.3/src/test_kmn_456.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-14 18:04:02.000000 test_kmn_456-0.1.3/src/test_kmn_456.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-14 18:04:02.000000 test_kmn_456-0.1.3/src/test_kmn_456.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 18:04:02.000000 test_kmn_456-0.1.3/src/test_kmn_456.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 18:04:02.000000 test_kmn_456-0.1.3/src/test_kmn_456.egg-info/top_level.txt
```

### Comparing `test_kmn_456-0.0.1/LICENSE` & `test_kmn_456-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `test_kmn_456-0.0.1/PKG-INFO` & `test_kmn_456-0.1.3/src/test_kmn_456.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: test_kmn_456
-Version: 0.0.1
+Name: test-kmn-456
+Version: 0.1.3
 Summary: A small test example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,23 +15,23 @@
 # test_kmn_456
 # Example Package
 
 This is a simple example package. You can use
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
 to write your content.
 
-- Need pre-commit to run 
+- Need pre-commit to run
   commitlint which is written in node.js
 
-  commitlint can be installed using 
+  commitlint can be installed using
   https://github.com/conventional-changelog/commitlint/blob/master/docs/guides-local-setup.md
 
   Configure commit lint to use conventional config
 
   npm install --save-dev @commitlint/{cli,config-conventional}
   echo "module.exports = { extends: ['@commitlint/config-conventional'] };" > commitlint.config.js
 
 - pip install pre-commit
 - pre-commit install-hooks
 - pre-commit install --install-hooks --hook-type commit-msg
- OR
+OR
 - pre-commit install --install-hooks -t pre-commit -t commit-msg
```

### Comparing `test_kmn_456-0.0.1/README.md` & `test_kmn_456-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # test_kmn_456
 # Example Package
 
 This is a simple example package. You can use
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
 to write your content.
 
-- Need pre-commit to run 
+- Need pre-commit to run
   commitlint which is written in node.js
 
-  commitlint can be installed using 
+  commitlint can be installed using
   https://github.com/conventional-changelog/commitlint/blob/master/docs/guides-local-setup.md
 
   Configure commit lint to use conventional config
 
   npm install --save-dev @commitlint/{cli,config-conventional}
   echo "module.exports = { extends: ['@commitlint/config-conventional'] };" > commitlint.config.js
 
 - pip install pre-commit
 - pre-commit install-hooks
 - pre-commit install --install-hooks --hook-type commit-msg
- OR
+OR
 - pre-commit install --install-hooks -t pre-commit -t commit-msg
```

### Comparing `test_kmn_456-0.0.1/pyproject.toml` & `test_kmn_456-0.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "test_kmn_456"
-version = "0.0.1"
+version = "0.1.3"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small test example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `test_kmn_456-0.0.1/src/test_kmn_456.egg-info/PKG-INFO` & `test_kmn_456-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: test-kmn-456
-Version: 0.0.1
+Name: test_kmn_456
+Version: 0.1.3
 Summary: A small test example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,23 +15,23 @@
 # test_kmn_456
 # Example Package
 
 This is a simple example package. You can use
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
 to write your content.
 
-- Need pre-commit to run 
+- Need pre-commit to run
   commitlint which is written in node.js
 
-  commitlint can be installed using 
+  commitlint can be installed using
   https://github.com/conventional-changelog/commitlint/blob/master/docs/guides-local-setup.md
 
   Configure commit lint to use conventional config
 
   npm install --save-dev @commitlint/{cli,config-conventional}
   echo "module.exports = { extends: ['@commitlint/config-conventional'] };" > commitlint.config.js
 
 - pip install pre-commit
 - pre-commit install-hooks
 - pre-commit install --install-hooks --hook-type commit-msg
- OR
+OR
 - pre-commit install --install-hooks -t pre-commit -t commit-msg
```

