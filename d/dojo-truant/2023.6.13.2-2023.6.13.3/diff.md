# Comparing `tmp/dojo_truant-2023.6.13.2.tar.gz` & `tmp/dojo_truant-2023.6.13.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dojo_truant-2023.6.13.2.tar", last modified: Wed Jun 14 07:14:11 2023, max compression
+gzip compressed data, was "dojo_truant-2023.6.13.3.tar", last modified: Wed Jun 14 07:20:30 2023, max compression
```

## Comparing `dojo_truant-2023.6.13.2.tar` & `dojo_truant-2023.6.13.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:14:11.483798 dojo_truant-2023.6.13.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-14 07:14:11.483798 dojo_truant-2023.6.13.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:14:11.483798 dojo_truant-2023.6.13.2/dojo/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/api.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/api_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/development_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/dojo_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/engagement.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/jira_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/jira_product_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/product.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/product_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/stub_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/test_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/write_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:14:11.483798 dojo_truant-2023.6.13.2/dojo_truant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-14 07:14:11.000000 dojo_truant-2023.6.13.2/dojo_truant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-14 07:14:11.000000 dojo_truant-2023.6.13.2/dojo_truant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 07:14:11.000000 dojo_truant-2023.6.13.2/dojo_truant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 07:14:11.000000 dojo_truant-2023.6.13.2/dojo_truant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-14 07:14:11.000000 dojo_truant-2023.6.13.2/dojo_truant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 07:14:11.483798 dojo_truant-2023.6.13.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:20:30.938764 dojo_truant-2023.6.13.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-14 07:20:30.938764 dojo_truant-2023.6.13.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:20:30.938764 dojo_truant-2023.6.13.3/dojo/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/api_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/development_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/dojo_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/engagement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/jira_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/jira_product_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/stub_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/write_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:20:30.938764 dojo_truant-2023.6.13.3/dojo_truant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-14 07:20:30.000000 dojo_truant-2023.6.13.3/dojo_truant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-14 07:20:30.000000 dojo_truant-2023.6.13.3/dojo_truant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 07:20:30.000000 dojo_truant-2023.6.13.3/dojo_truant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 07:20:30.000000 dojo_truant-2023.6.13.3/dojo_truant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-14 07:20:30.000000 dojo_truant-2023.6.13.3/dojo_truant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 07:20:30.938764 dojo_truant-2023.6.13.3/setup.cfg
```

### Comparing `dojo_truant-2023.6.13.2/LICENSE.txt` & `dojo_truant-2023.6.13.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.2/PKG-INFO` & `dojo_truant-2023.6.13.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo_truant
-Version: 2023.6.13.2
+Version: 2023.6.13.3
 Summary: A minimal client for deject dojo to be used by me in my projects. Most functionality should be absent.
 Author-email: Chris Halbersma <chalbersma@auditboard.com>
 License: BSD-3-Clause
 Keywords: defectDojo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `dojo_truant-2023.6.13.2/dojo/__init__.py` & `dojo_truant-2023.6.13.3/dojo/__init__.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.2/dojo/api.py` & `dojo_truant-2023.6.13.3/dojo/api.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.2/dojo/development_environment.py` & `dojo_truant-2023.6.13.3/dojo/development_environment.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.2/dojo/dojo_group.py` & `dojo_truant-2023.6.13.3/dojo/dojo_group.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.2/dojo/engagement.py` & `dojo_truant-2023.6.13.3/dojo/engagement.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.2/dojo/finding.py` & `dojo_truant-2023.6.13.3/dojo/finding.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
     def add_meta(self, name=None, value=None, overwrite=False):
 
         '''
         Adds a Metadata Object to this Finding
         '''
 
-        existing_metadata_endpoint = "/findings/{}/metadata/".format(self.id)
+        existing_metadata_endpoint = "api/v2/findings/{}/metadata/".format(self.id)
 
         current_metadata_json = self.api_call(endpoint=existing_metadata_endpoint,
                                               method="GET",
                                               token=True,
                                               return_json=True)
 
         current_metadata = {x["name"]: x["value"] for x in current_metadata_json}
```

### Comparing `dojo_truant-2023.6.13.2/dojo/jira_instance.py` & `dojo_truant-2023.6.13.3/dojo/jira_instance.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.2/dojo/jira_product_configuration.py` & `dojo_truant-2023.6.13.3/dojo/jira_product_configuration.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.2/dojo/product.py` & `dojo_truant-2023.6.13.3/dojo/product.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.2/dojo/product_type.py` & `dojo_truant-2023.6.13.3/dojo/product_type.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.2/dojo/stub_finding.py` & `dojo_truant-2023.6.13.3/dojo/stub_finding.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.2/dojo/test.py` & `dojo_truant-2023.6.13.3/dojo/test.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.2/dojo/test_type.py` & `dojo_truant-2023.6.13.3/dojo/test_type.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.2/dojo/write_chain.py` & `dojo_truant-2023.6.13.3/dojo/write_chain.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.2/dojo_truant.egg-info/PKG-INFO` & `dojo_truant-2023.6.13.3/dojo_truant.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo-truant
-Version: 2023.6.13.2
+Version: 2023.6.13.3
 Summary: A minimal client for deject dojo to be used by me in my projects. Most functionality should be absent.
 Author-email: Chris Halbersma <chalbersma@auditboard.com>
 License: BSD-3-Clause
 Keywords: defectDojo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `dojo_truant-2023.6.13.2/pyproject.toml` & `dojo_truant-2023.6.13.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "twine",
   "setuptools"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dojo_truant"
-version = "2023.6.13.2"
+version = "2023.6.13.3"
 authors = [
     {name = "Chris Halbersma", email = "chalbersma@auditboard.com"},
 ]
 description = "A minimal client for deject dojo to be used by me in my projects. Most functionality should be absent."
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = ["defectDojo"]
```

