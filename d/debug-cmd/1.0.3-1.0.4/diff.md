# Comparing `tmp/debug_cmd-1.0.3.tar.gz` & `tmp/debug_cmd-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debug_cmd-1.0.3.tar", last modified: Wed Jun 14 08:47:19 2023, max compression
+gzip compressed data, was "debug_cmd-1.0.4.tar", last modified: Wed Jun 14 08:51:06 2023, max compression
```

## Comparing `debug_cmd-1.0.3.tar` & `debug_cmd-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:47:19.255215 debug_cmd-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-14 08:46:56.000000 debug_cmd-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-14 08:47:19.255215 debug_cmd-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-14 08:46:56.000000 debug_cmd-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:47:19.251215 debug_cmd-1.0.3/debug_cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 08:46:56.000000 debug_cmd-1.0.3/debug_cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-06-14 08:46:56.000000 debug_cmd-1.0.3/debug_cmd/debug_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:47:19.255215 debug_cmd-1.0.3/debug_cmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-14 08:47:19.000000 debug_cmd-1.0.3/debug_cmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-14 08:47:19.000000 debug_cmd-1.0.3/debug_cmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:47:19.000000 debug_cmd-1.0.3/debug_cmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-14 08:47:19.000000 debug_cmd-1.0.3/debug_cmd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 08:47:19.000000 debug_cmd-1.0.3/debug_cmd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 08:47:19.000000 debug_cmd-1.0.3/debug_cmd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 08:47:19.255215 debug_cmd-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-14 08:46:56.000000 debug_cmd-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:51:06.087743 debug_cmd-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-14 08:50:50.000000 debug_cmd-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-14 08:51:06.087743 debug_cmd-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-14 08:50:50.000000 debug_cmd-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:51:06.083743 debug_cmd-1.0.4/debug_cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 08:50:50.000000 debug_cmd-1.0.4/debug_cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-06-14 08:50:50.000000 debug_cmd-1.0.4/debug_cmd/debug_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:51:06.087743 debug_cmd-1.0.4/debug_cmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-14 08:51:06.000000 debug_cmd-1.0.4/debug_cmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-14 08:51:06.000000 debug_cmd-1.0.4/debug_cmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:51:06.000000 debug_cmd-1.0.4/debug_cmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-14 08:51:06.000000 debug_cmd-1.0.4/debug_cmd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 08:51:06.000000 debug_cmd-1.0.4/debug_cmd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 08:51:06.000000 debug_cmd-1.0.4/debug_cmd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 08:51:06.087743 debug_cmd-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-14 08:50:50.000000 debug_cmd-1.0.4/setup.py
```

### Comparing `debug_cmd-1.0.3/LICENSE` & `debug_cmd-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `debug_cmd-1.0.3/PKG-INFO` & `debug_cmd-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debug_cmd
-Version: 1.0.3
+Version: 1.0.4
 Summary: Debug linux command error by using GPT/LLM.
 Home-page: https://github.com/megmogmog1965/debug_cmd
 Author: Yusuke Kawatsu
 Author-email: mail@sample.com
 License: MIT
 Keywords: gpt debug
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `debug_cmd-1.0.3/debug_cmd/debug_cmd.py` & `debug_cmd-1.0.4/debug_cmd/debug_cmd.py`

 * *Files identical despite different names*

### Comparing `debug_cmd-1.0.3/debug_cmd.egg-info/PKG-INFO` & `debug_cmd-1.0.4/debug_cmd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debug-cmd
-Version: 1.0.3
+Version: 1.0.4
 Summary: Debug linux command error by using GPT/LLM.
 Home-page: https://github.com/megmogmog1965/debug_cmd
 Author: Yusuke Kawatsu
 Author-email: mail@sample.com
 License: MIT
 Keywords: gpt debug
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `debug_cmd-1.0.3/setup.py` & `debug_cmd-1.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 with open(path.join(path.abspath(path.dirname(__file__)), 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='debug_cmd',
     packages=['debug_cmd'],
-    version='1.0.3',
+    version='1.0.4',
     license='MIT',
-    install_requires=['openai'],
+    install_requires=['openai', 'langchain'],
     author='Yusuke Kawatsu',
     author_email='mail@sample.com',
     url='https://github.com/megmogmog1965/debug_cmd',
     description='Debug linux command error by using GPT/LLM.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='gpt debug',
```

