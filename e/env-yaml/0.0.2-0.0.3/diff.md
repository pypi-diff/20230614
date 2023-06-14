# Comparing `tmp/env-yaml-0.0.2.tar.gz` & `tmp/env-yaml-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "env-yaml-0.0.2.tar", last modified: Wed Jun 14 17:57:48 2023, max compression
+gzip compressed data, was "env-yaml-0.0.3.tar", last modified: Wed Jun 14 18:28:35 2023, max compression
```

## Comparing `env-yaml-0.0.2.tar` & `env-yaml-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:57:48.376420 env-yaml-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-14 17:57:48.376420 env-yaml-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-14 17:57:28.000000 env-yaml-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 17:57:48.376420 env-yaml-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-14 17:57:28.000000 env-yaml-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:57:48.372420 env-yaml-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:57:48.376420 env-yaml-0.0.2/src/env_yaml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-14 17:57:48.000000 env-yaml-0.0.2/src/env_yaml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-14 17:57:48.000000 env-yaml-0.0.2/src/env_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 17:57:48.000000 env-yaml-0.0.2/src/env_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 17:57:48.000000 env-yaml-0.0.2/src/env_yaml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 17:57:48.000000 env-yaml-0.0.2/src/env_yaml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:28:35.567736 env-yaml-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-14 18:28:35.567736 env-yaml-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-14 18:28:19.000000 env-yaml-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 18:28:35.567736 env-yaml-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-14 18:28:19.000000 env-yaml-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:28:35.563736 env-yaml-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:28:35.567736 env-yaml-0.0.3/src/env_yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 18:28:19.000000 env-yaml-0.0.3/src/env_yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-14 18:28:19.000000 env-yaml-0.0.3/src/env_yaml/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:28:35.567736 env-yaml-0.0.3/src/env_yaml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-14 18:28:35.000000 env-yaml-0.0.3/src/env_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-14 18:28:35.000000 env-yaml-0.0.3/src/env_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 18:28:35.000000 env-yaml-0.0.3/src/env_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 18:28:35.000000 env-yaml-0.0.3/src/env_yaml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 18:28:35.000000 env-yaml-0.0.3/src/env_yaml.egg-info/top_level.txt
```

### Comparing `env-yaml-0.0.2/PKG-INFO` & `env-yaml-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: env-yaml
-Version: 0.0.2
+Version: 0.0.3
 Summary: Provides a yaml loader which substitutes environment variables and supports defaults
 Home-page: https://github.com/iamKunal/env-yaml-python
 Author: Kunal Gupta
 Description-Content-Type: text/markdown
 Provides-Extra: test
 
 # evn-yaml
```

### Comparing `env-yaml-0.0.2/README.md` & `env-yaml-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `env-yaml-0.0.2/setup.py` & `env-yaml-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
                   'environment variables and supports defaults',
       long_description=long_description,
       long_description_content_type='text/markdown',
 
       url='https://github.com/iamKunal/env-yaml-python',
       author='Kunal Gupta',
 
-      packages=find_packages(),
+      packages=find_packages('./src'),
 
       tests_require=tests_require,
       extras_require={
           'test': tests_require,
       },
       # test_suite='pytest.collector',
       install_requires=REQUIREMENTS,
```

### Comparing `env-yaml-0.0.2/src/env_yaml.egg-info/PKG-INFO` & `env-yaml-0.0.3/src/env_yaml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: env-yaml
-Version: 0.0.2
+Version: 0.0.3
 Summary: Provides a yaml loader which substitutes environment variables and supports defaults
 Home-page: https://github.com/iamKunal/env-yaml-python
 Author: Kunal Gupta
 Description-Content-Type: text/markdown
 Provides-Extra: test
 
 # evn-yaml
```

