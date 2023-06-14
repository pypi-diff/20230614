# Comparing `tmp/dojo_truant-2023.6.12.0.tar.gz` & `tmp/dojo_truant-2023.6.13.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dojo_truant-2023.6.12.0.tar", last modified: Tue Jun 13 04:54:22 2023, max compression
+gzip compressed data, was "dojo_truant-2023.6.13.0.tar", last modified: Wed Jun 14 06:00:30 2023, max compression
```

## Comparing `dojo_truant-2023.6.12.0.tar` & `dojo_truant-2023.6.13.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 04:54:22.153690 dojo_truant-2023.6.12.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-13 04:54:22.153690 dojo_truant-2023.6.12.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 04:54:22.149690 dojo_truant-2023.6.12.0/dojo/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/api.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/api_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/development_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/dojo_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/engagement.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/jira_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/jira_product_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/product.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/product_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/stub_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/test_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/write_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 04:54:22.153690 dojo_truant-2023.6.12.0/dojo_truant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-13 04:54:22.000000 dojo_truant-2023.6.12.0/dojo_truant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-13 04:54:22.000000 dojo_truant-2023.6.12.0/dojo_truant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 04:54:22.000000 dojo_truant-2023.6.12.0/dojo_truant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 04:54:22.000000 dojo_truant-2023.6.12.0/dojo_truant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 04:54:22.000000 dojo_truant-2023.6.12.0/dojo_truant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 04:54:22.153690 dojo_truant-2023.6.12.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:00:30.710692 dojo_truant-2023.6.13.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-14 06:00:15.000000 dojo_truant-2023.6.13.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-14 06:00:30.710692 dojo_truant-2023.6.13.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-14 06:00:15.000000 dojo_truant-2023.6.13.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:00:30.706691 dojo_truant-2023.6.13.0/dojo/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-14 06:00:15.000000 dojo_truant-2023.6.13.0/dojo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-06-14 06:00:15.000000 dojo_truant-2023.6.13.0/dojo/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:00:15.000000 dojo_truant-2023.6.13.0/dojo/api_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-14 06:00:15.000000 dojo_truant-2023.6.13.0/dojo/development_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-14 06:00:15.000000 dojo_truant-2023.6.13.0/dojo/dojo_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-14 06:00:15.000000 dojo_truant-2023.6.13.0/dojo/engagement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-06-14 06:00:15.000000 dojo_truant-2023.6.13.0/dojo/finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-14 06:00:15.000000 dojo_truant-2023.6.13.0/dojo/jira_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-14 06:00:15.000000 dojo_truant-2023.6.13.0/dojo/jira_product_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-14 06:00:15.000000 dojo_truant-2023.6.13.0/dojo/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-14 06:00:15.000000 dojo_truant-2023.6.13.0/dojo/product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-14 06:00:15.000000 dojo_truant-2023.6.13.0/dojo/stub_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-14 06:00:15.000000 dojo_truant-2023.6.13.0/dojo/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-14 06:00:15.000000 dojo_truant-2023.6.13.0/dojo/test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-14 06:00:15.000000 dojo_truant-2023.6.13.0/dojo/write_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:00:30.710692 dojo_truant-2023.6.13.0/dojo_truant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-14 06:00:30.000000 dojo_truant-2023.6.13.0/dojo_truant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-14 06:00:30.000000 dojo_truant-2023.6.13.0/dojo_truant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 06:00:30.000000 dojo_truant-2023.6.13.0/dojo_truant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 06:00:30.000000 dojo_truant-2023.6.13.0/dojo_truant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-14 06:00:30.000000 dojo_truant-2023.6.13.0/dojo_truant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-14 06:00:15.000000 dojo_truant-2023.6.13.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 06:00:30.710692 dojo_truant-2023.6.13.0/setup.cfg
```

### Comparing `dojo_truant-2023.6.12.0/LICENSE.txt` & `dojo_truant-2023.6.13.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.12.0/PKG-INFO` & `dojo_truant-2023.6.13.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dojo_truant
-Version: 2023.6.12.0
-Summary: A minimal client for deject dojo to be used by me in my projects. Some functionality may be absent.
+Version: 2023.6.13.0
+Summary: A minimal client for deject dojo to be used by me in my projects. Most functionality should be absent.
 Author-email: Chris Halbersma <chalbersma@auditboard.com>
 License: BSD-3-Clause
 Keywords: defectDojo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `dojo_truant-2023.6.12.0/dojo/__init__.py` & `dojo_truant-2023.6.13.0/dojo/__init__.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.12.0/dojo/api.py` & `dojo_truant-2023.6.13.0/dojo/api.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.12.0/dojo/development_environment.py` & `dojo_truant-2023.6.13.0/dojo/development_environment.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.12.0/dojo/dojo_group.py` & `dojo_truant-2023.6.13.0/dojo/dojo_group.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.12.0/dojo/engagement.py` & `dojo_truant-2023.6.13.0/dojo/engagement.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.12.0/dojo/finding.py` & `dojo_truant-2023.6.13.0/dojo/product.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,136 +5,63 @@
 import string
 
 import requests
 
 import dojo
 
 
-class Finding(dojo.DAPI):
-    _endpoint = string.Template("/api/v2/findings/${id}/")
-    _post_endpoint = "/api/v2/findings/"
-    _search_endpoint = "/api/v2/findings/"
-
-    _model_validation = {
-        "test": {"type": (int, dojo.Test),
-                 "required": True},
-        "thread_id": {"type": int,
-                      "required": False},
-        "found_by": {"type": list,
-                     "required": True},
-        "url": {"type": str,
-                "required": False},
-        "tags": {"type": list,
-                 "required": False},
-        "push_to_jira": {"type": bool,
-                         "required": False},
-        "vulnerability_ids": {"type": list,
-                              "required": False},
-        "reporter": {"type": int,
-                     "required": False},
-        "title": {"type": str,
-                  "required": True},
-        "date": {"type": str,
-                 "required": False,
-                 "regex": "\d{4}-\d{2}-\d{2}"},
-        "sla_start_date": {"type": str,
-                           "required": False,
-                           "regex": "\d{4}-\d{2}-\d{2}"},
-        "cwe": {"type": int,
-                "required": False},
-        "cvssv3": {"type": str,
-                  "required": False,
-                  "cvss": 3},
-        "cvssv3_score": {"type": float,
-                        "required": False},
-        "severity": {"type": str,
-                     "required": True,
-                     "enum": ("Critical", "High", "Medium", "Low", "Informtional")},
-        "description": {"type": str,
-                        "required": True},
-        "mitigation": {"type": str,
-                       "required": False},
-        "impact": {"type": str,
-                   "required": False},
-        "steps_to_reproduce": {"type": str,
-                               "required": False},
-        "severity_justification": {"type": str,
-                                   "required": False},
-        "references": {"type": str,
-                       "required": False},
-        "active": {"type": bool,
-                   "required": True},
-        "verified": {"type": bool,
-                     "required": True},
-        "false_p": {"type": bool,
-                    "required": False},
-        "duplicate": {"type": bool,
-                      "required": False},
-        "out_of_scope": {"type": bool,
-                         "required": False},
-        "risk_accepted": {"type": bool,
-                          "required": False},
-        "under_review": {"type": bool,
-                         "required": False},
-        "under_defect_review": {"type": bool,
-                                "required": False},
-        "is_mitigated": {"type": bool,
-                         "required": False},
-        "numerical_severity": {"type": str,
-                               "required": True},
-        "line": {"type": int,
-                 "required": False},
-        "file_path": {"type": str,
-                      "required": False},
-        "component_name": {"type": str,
-                           "required": False},
-        "component_version": {"type": str,
-                              "required": False},
-        "static_finding": {"type": bool,
-                           "required": False},
-        "dynamic_finding": {"type": bool,
-                            "required": False},
-        "unique_id_from_tool": {"type": str,
-                                "required": False},
-        "vuln_id_from_tool": {"type": str,
-                              "required": False},
-        "sast_source_object": {"type": str,
-                               "required": False},
-        "sast_sink_object": {"type": str,
-                             "required": False},
-        "sast_source_line": {"type": str,
-                             "required": False},
-        "sast_source_file_path": {"type": str,
-                                  "required": False},
-        "nb_occurences": {"type": int,
-                          "required": False},
-        "publish_date": {"type": str,
-                         "required": False,
-                         "regex": "\d{4}-\d{2}-\d{2}"},
-        "service": {"type": str,
-                    "required": False},
-        "planned_remediation_date": {"type": str,
-                                     "required": False,
-                                     "regex": "\d{4}-\d{2}-\d{2}"},
-
-        "review_requested_by": {"type": int,
-                                "required": False},
-
-        "defect_review_requested_by": {"type": int,
-                                       "required": False},
-
-        "sonarcube_issue": {"type": int,
-                            "required": False},
+class Product(dojo.DAPI):
+    _endpoint = string.Template("/api/v2/products/${id}/")
+    _post_endpoint = "/api/v2/products/"
+    _search_endpoint = "/api/v2/products/"
 
-        "reviewers": {"type": list,
-                      "required": False},
-
-    }
+    _model_validation = {"tags": {"type": list,
+                                  "required": False},
+                         "name": {"type": str},
+                         "description": {"type": str},
+                         "prod_numeric_grade": {"type": int,
+                                                "required": False},
+                         "business_criticality": {"type": str,
+                                                  "required": False,
+                                                  "enum": ("none", "very low", "low", "medium", "high", "very high")},
+                         "platform": {"type": str,
+                                      "required": False,
+                                      "enum": ("web", "mobile", "iot", "desktop", "web service")},
+                         "lifecycle": {"type": str,
+                                       "required": False,
+                                       "enum": ("retirement", "production", "construction")},
+                         "origin": {"type": str,
+                                    "required": False,
+                                    "enum": ("outsourced", "open source", "internal", "contractor", "purchased", "third party library")},
+                         "user_records": {"type": int,
+                                          "required": False},
+                         "revenue": {"type": str,
+                                     "required": False},
+                         "external_audience": {"type": bool,
+                                               "required": False},
+                         "internet_accessible": {"type": bool,
+                                                 "required": False},
+                         "enable_simple_risk_acceptance": {"type": bool,
+                                                           "required": False},
+                         "enable_full_risk_acceptance": {"type": bool,
+                                                         "required": False},
+                         "product_manager": {"type": int,
+                                             "required": False},
+                         "technical_contact": {"type": int,
+                                               "required": False},
+                         "team_manager": {"type": int,
+                                          "required": False},
+                         "prod_type": {"type": (int, dojo.Product_Type)},
+                         "sla_configuration": {"type": int,
+                                               "required": False},
+                         "regulations": {"type": list,
+                                         "required": False}
+                         }
 
     _obj_iterate = ".results[]"
 
-    _type = "finding"
+    _type = "product"
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
-        self.logger = logging.getLogger("DAPI.Finding")
+        self.logger = logging.getLogger("DAPI.Product")
```

### Comparing `dojo_truant-2023.6.12.0/dojo/jira_instance.py` & `dojo_truant-2023.6.13.0/dojo/jira_instance.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.12.0/dojo/jira_product_configuration.py` & `dojo_truant-2023.6.13.0/dojo/jira_product_configuration.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.12.0/dojo/product_type.py` & `dojo_truant-2023.6.13.0/dojo/product_type.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.12.0/dojo/stub_finding.py` & `dojo_truant-2023.6.13.0/dojo/stub_finding.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.12.0/dojo/test.py` & `dojo_truant-2023.6.13.0/dojo/test.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.12.0/dojo/test_type.py` & `dojo_truant-2023.6.13.0/dojo/test_type.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.12.0/dojo/write_chain.py` & `dojo_truant-2023.6.13.0/dojo/write_chain.py`

 * *Files 9% similar despite different names*

```diff
@@ -103,14 +103,25 @@
                 dojo_obj.data = tdata
                 dojo_obj.new_obj()
             else:
                 # One Found Update Existing Object
                 logger.info("update obj: {}".format(json.dumps(tdata)))
                 dojo_obj.update_obj(tdata)
 
+            for func, arguments in chain[x].get("extra_func", dict()).items():
+                try:
+                    getattr(dojo_obj, func)(*arguments.get("args", list()),
+                                            **arguments.get("kwargs", dict())
+                                            )
+                except Exception as extra_arg_fail:
+                    logger.warning("Unable to Run extra Arg : {} against {} ignoring".format(func, dojo_obj))
+                else:
+                    logger.debug("Ran Extra Arg : {} against {}".format(func, dojo_obj))
+
+
             template_obj[x] = dojo_obj
             if chain[x].get("named", None) is not None:
                 template_obj["N{}".format(chain[x]["named"])] = dojo_obj
     else:
         logger.warning("No Chain of Items Given")
 
     return template_obj
```

### Comparing `dojo_truant-2023.6.12.0/dojo_truant.egg-info/PKG-INFO` & `dojo_truant-2023.6.13.0/dojo_truant.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dojo-truant
-Version: 2023.6.12.0
-Summary: A minimal client for deject dojo to be used by me in my projects. Some functionality may be absent.
+Version: 2023.6.13.0
+Summary: A minimal client for deject dojo to be used by me in my projects. Most functionality should be absent.
 Author-email: Chris Halbersma <chalbersma@auditboard.com>
 License: BSD-3-Clause
 Keywords: defectDojo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `dojo_truant-2023.6.12.0/pyproject.toml` & `dojo_truant-2023.6.13.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,19 @@
   "twine",
   "setuptools"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dojo_truant"
-version = "2023.6.12.0"
+version = "2023.6.13.0"
 authors = [
     {name = "Chris Halbersma", email = "chalbersma@auditboard.com"},
 ]
-description = "A minimal client for deject dojo to be used by me in my projects. Some functionality may be absent."
+description = "A minimal client for deject dojo to be used by me in my projects. Most functionality should be absent."
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = ["defectDojo"]
 license = {text = "BSD-3-Clause"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
```

