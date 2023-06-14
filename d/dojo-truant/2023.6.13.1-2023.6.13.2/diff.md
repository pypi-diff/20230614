# Comparing `tmp/dojo_truant-2023.6.13.1.tar.gz` & `tmp/dojo_truant-2023.6.13.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dojo_truant-2023.6.13.1.tar", last modified: Wed Jun 14 07:00:28 2023, max compression
+gzip compressed data, was "dojo_truant-2023.6.13.2.tar", last modified: Wed Jun 14 07:14:11 2023, max compression
```

## Comparing `dojo_truant-2023.6.13.1.tar` & `dojo_truant-2023.6.13.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:00:28.277153 dojo_truant-2023.6.13.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-14 07:00:11.000000 dojo_truant-2023.6.13.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-14 07:00:28.277153 dojo_truant-2023.6.13.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-14 07:00:11.000000 dojo_truant-2023.6.13.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:00:28.277153 dojo_truant-2023.6.13.1/dojo/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-14 07:00:11.000000 dojo_truant-2023.6.13.1/dojo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-06-14 07:00:11.000000 dojo_truant-2023.6.13.1/dojo/api.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 07:00:11.000000 dojo_truant-2023.6.13.1/dojo/api_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-14 07:00:11.000000 dojo_truant-2023.6.13.1/dojo/development_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-14 07:00:11.000000 dojo_truant-2023.6.13.1/dojo/dojo_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-14 07:00:11.000000 dojo_truant-2023.6.13.1/dojo/engagement.py
--rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-06-14 07:00:11.000000 dojo_truant-2023.6.13.1/dojo/finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-14 07:00:11.000000 dojo_truant-2023.6.13.1/dojo/jira_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-14 07:00:11.000000 dojo_truant-2023.6.13.1/dojo/jira_product_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-14 07:00:11.000000 dojo_truant-2023.6.13.1/dojo/product.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-14 07:00:11.000000 dojo_truant-2023.6.13.1/dojo/product_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-14 07:00:11.000000 dojo_truant-2023.6.13.1/dojo/stub_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-14 07:00:11.000000 dojo_truant-2023.6.13.1/dojo/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-14 07:00:11.000000 dojo_truant-2023.6.13.1/dojo/test_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-14 07:00:11.000000 dojo_truant-2023.6.13.1/dojo/write_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:00:28.277153 dojo_truant-2023.6.13.1/dojo_truant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-14 07:00:28.000000 dojo_truant-2023.6.13.1/dojo_truant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-14 07:00:28.000000 dojo_truant-2023.6.13.1/dojo_truant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 07:00:28.000000 dojo_truant-2023.6.13.1/dojo_truant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 07:00:28.000000 dojo_truant-2023.6.13.1/dojo_truant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-14 07:00:28.000000 dojo_truant-2023.6.13.1/dojo_truant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-14 07:00:11.000000 dojo_truant-2023.6.13.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 07:00:28.277153 dojo_truant-2023.6.13.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:14:11.483798 dojo_truant-2023.6.13.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-14 07:14:11.483798 dojo_truant-2023.6.13.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:14:11.483798 dojo_truant-2023.6.13.2/dojo/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/api_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/development_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/dojo_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/engagement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/jira_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/jira_product_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/stub_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/dojo/write_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:14:11.483798 dojo_truant-2023.6.13.2/dojo_truant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-14 07:14:11.000000 dojo_truant-2023.6.13.2/dojo_truant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-14 07:14:11.000000 dojo_truant-2023.6.13.2/dojo_truant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 07:14:11.000000 dojo_truant-2023.6.13.2/dojo_truant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 07:14:11.000000 dojo_truant-2023.6.13.2/dojo_truant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-14 07:14:11.000000 dojo_truant-2023.6.13.2/dojo_truant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-14 07:13:54.000000 dojo_truant-2023.6.13.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 07:14:11.483798 dojo_truant-2023.6.13.2/setup.cfg
```

### Comparing `dojo_truant-2023.6.13.1/LICENSE.txt` & `dojo_truant-2023.6.13.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.1/PKG-INFO` & `dojo_truant-2023.6.13.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo_truant
-Version: 2023.6.13.1
+Version: 2023.6.13.2
 Summary: A minimal client for deject dojo to be used by me in my projects. Most functionality should be absent.
 Author-email: Chris Halbersma <chalbersma@auditboard.com>
 License: BSD-3-Clause
 Keywords: defectDojo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `dojo_truant-2023.6.13.1/dojo/__init__.py` & `dojo_truant-2023.6.13.2/dojo/__init__.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.1/dojo/api.py` & `dojo_truant-2023.6.13.2/dojo/api.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.1/dojo/development_environment.py` & `dojo_truant-2023.6.13.2/dojo/development_environment.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.1/dojo/dojo_group.py` & `dojo_truant-2023.6.13.2/dojo/dojo_group.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.1/dojo/engagement.py` & `dojo_truant-2023.6.13.2/dojo/engagement.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.1/dojo/finding.py` & `dojo_truant-2023.6.13.2/dojo/finding.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,24 +157,26 @@
         Adds a Metadata Object to this Finding
         '''
 
         existing_metadata_endpoint = "/findings/{}/metadata/".format(self.id)
 
         current_metadata_json = self.api_call(endpoint=existing_metadata_endpoint,
                                               method="GET",
+                                              token=True,
                                               return_json=True)
 
         current_metadata = {x["name"]: x["value"] for x in current_metadata_json}
 
         if str(name) not in current_metadata.keys() or overwrite is True:
             # Place New metadata
 
             new_meta = {"name": str(name),
                         "value": str(value)}
 
             new_metadata_json = self.api_call(endpoint=existing_metadata_endpoint,
                                               method="POST",
+                                              token=True,
                                               json=new_meta,
                                               return_json=True)
 
         else:
             self.logger.debug("Not Overwriting Current Metadata")
```

### Comparing `dojo_truant-2023.6.13.1/dojo/jira_instance.py` & `dojo_truant-2023.6.13.2/dojo/jira_instance.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.1/dojo/jira_product_configuration.py` & `dojo_truant-2023.6.13.2/dojo/jira_product_configuration.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.1/dojo/product.py` & `dojo_truant-2023.6.13.2/dojo/product.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.1/dojo/product_type.py` & `dojo_truant-2023.6.13.2/dojo/product_type.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.1/dojo/stub_finding.py` & `dojo_truant-2023.6.13.2/dojo/stub_finding.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.1/dojo/test.py` & `dojo_truant-2023.6.13.2/dojo/test.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.1/dojo/test_type.py` & `dojo_truant-2023.6.13.2/dojo/test_type.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.1/dojo/write_chain.py` & `dojo_truant-2023.6.13.2/dojo/write_chain.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.1/dojo_truant.egg-info/PKG-INFO` & `dojo_truant-2023.6.13.2/dojo_truant.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo-truant
-Version: 2023.6.13.1
+Version: 2023.6.13.2
 Summary: A minimal client for deject dojo to be used by me in my projects. Most functionality should be absent.
 Author-email: Chris Halbersma <chalbersma@auditboard.com>
 License: BSD-3-Clause
 Keywords: defectDojo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `dojo_truant-2023.6.13.1/pyproject.toml` & `dojo_truant-2023.6.13.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "twine",
   "setuptools"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dojo_truant"
-version = "2023.6.13.1"
+version = "2023.6.13.2"
 authors = [
     {name = "Chris Halbersma", email = "chalbersma@auditboard.com"},
 ]
 description = "A minimal client for deject dojo to be used by me in my projects. Most functionality should be absent."
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = ["defectDojo"]
```

