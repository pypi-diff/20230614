# Comparing `tmp/a-bigelow.cdk-eventbridge-partner-processors-0.0.98.tar.gz` & `tmp/a-bigelow.cdk-eventbridge-partner-processors-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a-bigelow.cdk-eventbridge-partner-processors-0.0.98.tar", last modified: Sat Nov 12 00:22:04 2022, max compression
+gzip compressed data, was "a-bigelow.cdk-eventbridge-partner-processors-0.0.99.tar", last modified: Sun Nov 13 00:20:48 2022, max compression
```

## Comparing `a-bigelow.cdk-eventbridge-partner-processors-0.0.98.tar` & `a-bigelow.cdk-eventbridge-partner-processors-0.0.99.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 00:22:04.677537 a-bigelow.cdk-eventbridge-partner-processors-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-11-12 00:21:50.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-11-12 00:21:50.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5231 2022-11-12 00:22:04.677537 a-bigelow.cdk-eventbridge-partner-processors-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4249 2022-11-12 00:21:50.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-11-12 00:21:50.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-12 00:22:04.677537 a-bigelow.cdk-eventbridge-partner-processors-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1947 2022-11-12 00:21:50.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 00:22:04.677537 a-bigelow.cdk-eventbridge-partner-processors-0.0.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 00:22:04.677537 a-bigelow.cdk-eventbridge-partner-processors-0.0.98/src/a-bigelow/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 00:22:04.677537 a-bigelow.cdk-eventbridge-partner-processors-0.0.98/src/a-bigelow/cdk-eventbridge-partner-processors/
--rw-r--r--   0 runner    (1001) docker     (121)    31949 2022-11-12 00:21:50.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.98/src/a-bigelow/cdk-eventbridge-partner-processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 00:22:04.677537 a-bigelow.cdk-eventbridge-partner-processors-0.0.98/src/a-bigelow/cdk-eventbridge-partner-processors/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-11-12 00:21:50.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.98/src/a-bigelow/cdk-eventbridge-partner-processors/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26497 2022-11-12 00:21:50.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.98/src/a-bigelow/cdk-eventbridge-partner-processors/_jsii/cdk-eventbridge-partner-processors@0.0.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-12 00:21:50.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.98/src/a-bigelow/cdk-eventbridge-partner-processors/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 00:22:04.677537 a-bigelow.cdk-eventbridge-partner-processors-0.0.98/src/a_bigelow.cdk_eventbridge_partner_processors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5231 2022-11-12 00:22:04.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.98/src/a_bigelow.cdk_eventbridge_partner_processors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      704 2022-11-12 00:22:04.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.98/src/a_bigelow.cdk_eventbridge_partner_processors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-12 00:22:04.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.98/src/a_bigelow.cdk_eventbridge_partner_processors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-11-12 00:22:04.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.98/src/a_bigelow.cdk_eventbridge_partner_processors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-12 00:22:04.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.98/src/a_bigelow.cdk_eventbridge_partner_processors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 00:20:48.426975 a-bigelow.cdk-eventbridge-partner-processors-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-11-13 00:20:32.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-11-13 00:20:32.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5231 2022-11-13 00:20:48.426975 a-bigelow.cdk-eventbridge-partner-processors-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4249 2022-11-13 00:20:32.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      236 2022-11-13 00:20:32.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-13 00:20:48.426975 a-bigelow.cdk-eventbridge-partner-processors-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1947 2022-11-13 00:20:32.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 00:20:48.422975 a-bigelow.cdk-eventbridge-partner-processors-0.0.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 00:20:48.422975 a-bigelow.cdk-eventbridge-partner-processors-0.0.99/src/a-bigelow/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 00:20:48.422975 a-bigelow.cdk-eventbridge-partner-processors-0.0.99/src/a-bigelow/cdk-eventbridge-partner-processors/
+-rw-r--r--   0 runner    (1001) docker     (121)    31949 2022-11-13 00:20:32.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.99/src/a-bigelow/cdk-eventbridge-partner-processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 00:20:48.422975 a-bigelow.cdk-eventbridge-partner-processors-0.0.99/src/a-bigelow/cdk-eventbridge-partner-processors/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      450 2022-11-13 00:20:32.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.99/src/a-bigelow/cdk-eventbridge-partner-processors/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26495 2022-11-13 00:20:32.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.99/src/a-bigelow/cdk-eventbridge-partner-processors/_jsii/cdk-eventbridge-partner-processors@0.0.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-13 00:20:32.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.99/src/a-bigelow/cdk-eventbridge-partner-processors/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 00:20:48.426975 a-bigelow.cdk-eventbridge-partner-processors-0.0.99/src/a_bigelow.cdk_eventbridge_partner_processors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5231 2022-11-13 00:20:47.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.99/src/a_bigelow.cdk_eventbridge_partner_processors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      704 2022-11-13 00:20:48.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.99/src/a_bigelow.cdk_eventbridge_partner_processors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-13 00:20:47.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.99/src/a_bigelow.cdk_eventbridge_partner_processors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2022-11-13 00:20:48.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.99/src/a_bigelow.cdk_eventbridge_partner_processors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-13 00:20:48.000000 a-bigelow.cdk-eventbridge-partner-processors-0.0.99/src/a_bigelow.cdk_eventbridge_partner_processors.egg-info/top_level.txt
```

### Comparing `a-bigelow.cdk-eventbridge-partner-processors-0.0.98/LICENSE` & `a-bigelow.cdk-eventbridge-partner-processors-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `a-bigelow.cdk-eventbridge-partner-processors-0.0.98/PKG-INFO` & `a-bigelow.cdk-eventbridge-partner-processors-0.0.99/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a-bigelow.cdk-eventbridge-partner-processors
-Version: 0.0.98
+Version: 0.0.99
 Summary: cdk-eventbridge-partner-processors
 Home-page: https://github.com/a-bigelow/cdk-eventbridge-partner-processors.git
 Author: a-bigelow<adam@adambigelow.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/a-bigelow/cdk-eventbridge-partner-processors.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `a-bigelow.cdk-eventbridge-partner-processors-0.0.98/README.md` & `a-bigelow.cdk-eventbridge-partner-processors-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `a-bigelow.cdk-eventbridge-partner-processors-0.0.98/setup.py` & `a-bigelow.cdk-eventbridge-partner-processors-0.0.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "a-bigelow.cdk-eventbridge-partner-processors",
-    "version": "0.0.98",
+    "version": "0.0.99",
     "description": "cdk-eventbridge-partner-processors",
     "license": "Apache-2.0",
     "url": "https://github.com/a-bigelow/cdk-eventbridge-partner-processors.git",
     "long_description_content_type": "text/markdown",
     "author": "a-bigelow<adam@adambigelow.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "a-bigelow.cdk-eventbridge-partner-processors",
         "a-bigelow.cdk-eventbridge-partner-processors._jsii"
     ],
     "package_data": {
         "a-bigelow.cdk-eventbridge-partner-processors._jsii": [
-            "cdk-eventbridge-partner-processors@0.0.98.jsii.tgz"
+            "cdk-eventbridge-partner-processors@0.0.99.jsii.tgz"
         ],
         "a-bigelow.cdk-eventbridge-partner-processors": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `a-bigelow.cdk-eventbridge-partner-processors-0.0.98/src/a-bigelow/cdk-eventbridge-partner-processors/__init__.py` & `a-bigelow.cdk-eventbridge-partner-processors-0.0.99/src/a-bigelow/cdk-eventbridge-partner-processors/__init__.py`

 * *Files identical despite different names*

### Comparing `a-bigelow.cdk-eventbridge-partner-processors-0.0.98/src/a-bigelow/cdk-eventbridge-partner-processors/_jsii/cdk-eventbridge-partner-processors@0.0.98.jsii.tgz` & `a-bigelow.cdk-eventbridge-partner-processors-0.0.99/src/a-bigelow/cdk-eventbridge-partner-processors/_jsii/cdk-eventbridge-partner-processors@0.0.99.jsii.tgz`

 * *Files 22% similar despite different names*

#### Comparing `cdk-eventbridge-partner-processors@0.0.98.jsii.tgz-content` & `cdk-eventbridge-partner-processors@0.0.99.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'fingerprint'": "'j2pmIo3YWigCVde6BkzQo6RGZ3VgkUdvjp3VbRaCYbg='", "'version'": "'0.0.99'"}*

```diff
@@ -3018,15 +3018,15 @@
             }
         }
     },
     "description": "cdk-eventbridge-partner-processors",
     "docs": {
         "stability": "stable"
     },
-    "fingerprint": "y3Agwg35FbTS1azGqDHof9nafJ4dO/St9lwY7H6x4Us=",
+    "fingerprint": "j2pmIo3YWigCVde6BkzQo6RGZ3VgkUdvjp3VbRaCYbg=",
     "homepage": "https://github.com/a-bigelow/cdk-eventbridge-partner-processors.git",
     "jsiiVersion": "1.71.0 (build f1f58ae)",
     "keywords": [
         "cdk",
         "eventbridge",
         "github",
         "stripe",
@@ -3679,9 +3679,9 @@
                         "fqn": "aws-cdk-lib.aws_secretsmanager.ISecret"
                     }
                 }
             ],
             "symbolId": "src/Twilio:TwilioProps"
         }
     },
-    "version": "0.0.98"
+    "version": "0.0.99"
 }
```

##### package/lib/Github.js

###### js-beautify {}

```diff
@@ -19,10 +19,10 @@
         });
     }
 }
 exports.GitHubEventProcessor = GitHubEventProcessor;
 _a = JSII_RTTI_SYMBOL_1;
 GitHubEventProcessor[_a] = {
     fqn: "cdk-eventbridge-partner-processors.GitHubEventProcessor",
-    version: "0.0.98"
+    version: "0.0.99"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiR2l0aHViLmpzIiwic291cmNlUm9vdCI6IiIsInNvdXJjZXMiOlsiLi4vc3JjL0dpdGh1Yi50cyJdLCJuYW1lcyI6W10sIm1hcHBpbmdzIjoiOzs7OztBQUdBLHVDQUFvQztBQUNwQyx1REFBcUQ7QUFxQnJEOzs7R0FHRztBQUNILE1BQWEsb0JBQXFCLFNBQVEsa0NBQWdCO0lBQ3hELFlBQVksS0FBZ0IsRUFBRSxFQUFVLEVBQUUsS0FBa0I7UUFDMUQsS0FBSyxDQUFDLEtBQUssRUFBRSxFQUFFLEVBQUUsRUFBRSxHQUFHLEtBQUssRUFBRSxrQkFBa0IsRUFBRSxpQkFBTyxDQUFDLE1BQU0sRUFBRSxDQUFDLENBQUM7SUFDckUsQ0FBQzs7QUFISCxvREFJQyIsInNvdXJjZXNDb250ZW50IjpbImltcG9ydCB7IElFdmVudEJ1cyB9IGZyb20gJ2F3cy1jZGstbGliL2F3cy1ldmVudHMnO1xuaW1wb3J0IHsgSVNlY3JldCB9IGZyb20gJ2F3cy1jZGstbGliL2F3cy1zZWNyZXRzbWFuYWdlcic7XG5pbXBvcnQgeyBDb25zdHJ1Y3QgfSBmcm9tICdjb25zdHJ1Y3RzJztcbmltcG9ydCB7IFBhcnRuZXIgfSBmcm9tICcuL1BhcnRuZXInO1xuaW1wb3J0IHsgUGFydG5lclByb2Nlc3NvciB9IGZyb20gJy4vUGFydG5lckZ1bmN0aW9uJztcblxuZXhwb3J0IGludGVyZmFjZSBHaXRIdWJQcm9wcyB7XG5cbiAgLyoqXG4gICAqIFNNIFNlY3JldCBjb250YWluaW5nIHRoZSBzZWNyZXQgc3RyaW5nIHVzZWQgdG8gdmFsaWRhdGUgd2ViaG9vayBldmVudHMuXG4gICAqL1xuICByZWFkb25seSB3ZWJob29rU2VjcmV0OiBJU2VjcmV0O1xuXG4gIC8qKlxuICAgKiBFdmVudGJ1cyB0byBzZW5kIEdpdEh1YiBldmVudHMgdG8uXG4gICAqL1xuICByZWFkb25seSBldmVudEJ1czogSUV2ZW50QnVzO1xuXG4gIC8qKlxuICAgKiBNYXhpbXVtIG51bWJlciBvZiBjb25jdXJyZW50IGludm9jYXRpb25zIG9uIHRoZSBmVVJMIGZ1bmN0aW9uIGJlZm9yZSB0cmlnZ2VyaW5nIHRoZSBhbGFybS5cbiAgICovXG4gIHJlYWRvbmx5IGxhbWJkYUludm9jYXRpb25BbGFybVRocmVzaG9sZDogbnVtYmVyO1xuXG59XG5cbi8qKlxuICogQ0RLIHdyYXBwZXIgZm9yIHRoZSBHaXRIdWIgRXZlbnRicmlkZ2UgcHJvY2Vzc29yLlxuICogQHNlZSBodHRwczovL2RvY3MuYXdzLmFtYXpvbi5jb20vZXZlbnRicmlkZ2UvbGF0ZXN0L3VzZXJndWlkZS9lYi1zYWFzLWZ1cmxzLmh0bWwjZnVybHMtY29ubmVjdGlvbi1naXRodWJcbiAqL1xuZXhwb3J0IGNsYXNzIEdpdEh1YkV2ZW50UHJvY2Vzc29yIGV4dGVuZHMgUGFydG5lclByb2Nlc3NvciB7XG4gIGNvbnN0cnVjdG9yKHNjb3BlOiBDb25zdHJ1Y3QsIGlkOiBzdHJpbmcsIHByb3BzOiBHaXRIdWJQcm9wcykge1xuICAgIHN1cGVyKHNjb3BlLCBpZCwgeyAuLi5wcm9wcywgZXZlbnRicmlkZ2VQYXJ0bmVyOiBQYXJ0bmVyLkdJVEhVQiB9KTtcbiAgfVxufSJdfQ==
```

##### package/lib/PartnerFunction.js

###### js-beautify {}

```diff
@@ -44,10 +44,10 @@
         });
     }
 }
 exports.PartnerProcessor = PartnerProcessor;
 _a = JSII_RTTI_SYMBOL_1;
 PartnerProcessor[_a] = {
     fqn: "cdk-eventbridge-partner-processors.PartnerProcessor",
-    version: "0.0.98"
+    version: "0.0.99"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiUGFydG5lckZ1bmN0aW9uLmpzIiwic291cmNlUm9vdCI6IiIsInNvdXJjZXMiOlsiLi4vc3JjL1BhcnRuZXJGdW5jdGlvbi50cyJdLCJuYW1lcyI6W10sIm1hcHBpbmdzIjoiOzs7OztBQUFBLDZDQUF5RDtBQUV6RCx1REFBc0Y7QUFDdEYsK0NBQTRDO0FBRTVDLDJDQUF1QztBQUV2QyxpQ0FBeUM7QUEwQnpDOzs7O0dBSUc7QUFDSCxNQUFzQixnQkFBaUIsU0FBUSxzQkFBUztJQUd0RCxZQUFZLEtBQWdCLEVBQUUsRUFBVSxFQUFFLEtBQTJCO1FBQ25FLEtBQUssQ0FBQyxLQUFLLEVBQUUsRUFBRSxDQUFDLENBQUM7UUFFakIsSUFBSSxDQUFDLHFCQUFxQixHQUFHLElBQUkscUJBQVEsQ0FBQyxJQUFJLEVBQUUsR0FBRyxLQUFLLENBQUMsa0JBQWtCLGdCQUFnQixFQUFFO1lBQzNGLElBQUksRUFBRSxpQkFBSSxDQUFDLFVBQVUsQ0FBQyxlQUFNLENBQUMsY0FBYyxDQUFDLElBQUksRUFBRSxtQkFBbUIsRUFBRSw4Q0FBOEMsbUJBQUssQ0FBQyxFQUFFLENBQUMsSUFBSSxDQUFDLENBQUMsTUFBTSxFQUFFLENBQUMsRUFBRSxvQkFBb0IsS0FBSyxDQUFDLGtCQUFrQixnQkFBZ0IsQ0FBQztZQUM1TSxPQUFPLEVBQUUsb0JBQW9CO1lBQzdCLE9BQU8sRUFBRSxvQkFBTyxDQUFDLFVBQVU7WUFDM0IsVUFBVSxFQUFFLEdBQUc7WUFDZixPQUFPLEVBQUUsc0JBQVEsQ0FBQyxPQUFPLENBQUMsR0FBRyxDQUFDO1lBQzlCLDRCQUE0QixFQUFFLEVBQUU7WUFDaEMsV0FBVyxFQUFFO2dCQUNYLHlCQUF5QixFQUFFLEtBQUssQ0FBQyxhQUFhLENBQUMsU0FBUztnQkFDeEQsY0FBYyxFQUFFLEtBQUssQ0FBQyxRQUFRLENBQUMsWUFBWTthQUM1QztTQUNGLENBQUMsQ0FBQztRQUVILElBQUksQ0FBQyxlQUFlLEdBQUcsSUFBSSxzQkFBZSxDQUFDLElBQUksRUFBRSxHQUFHLEtBQUssQ0FBQyxrQkFBa0IsaUJBQWlCLEVBQUU7WUFDN0YsU0FBUyxFQUFFLEtBQUssQ0FBQyw4QkFBOEI7WUFDL0MsYUFBYSxFQUFFLElBQUksQ0FBQyxxQkFBcUI7U0FDMUMsQ0FBQyxDQUFDO1FBRUgsTUFBTSxJQUFJLEdBQUcsSUFBSSxDQUFDLHFCQUFxQixDQUFDLGNBQWMsQ0FBQyxFQUFFLFFBQVEsRUFBRSxnQ0FBbUIsQ0FBQyxJQUFJLEVBQUUsQ0FBQyxDQUFDO1FBRS9GLEtBQUssQ0FBQyxhQUFhLENBQUMsU0FBUyxDQUFDLElBQUksQ0FBQyxxQkFBcUIsQ0FBQyxDQUFDO1FBQzFELEtBQUssQ0FBQyxRQUFRLENBQUMsZ0JBQWdCLENBQUMsSUFBSSxDQUFDLHFCQUFxQixDQUFDLENBQUM7UUFFNUQsSUFBSSx1QkFBUyxDQUFDLElBQUksRUFBRSxHQUFHLEtBQUssQ0FBQyxrQkFBa0IsYUFBYSxFQUFFLEVBQUUsS0FBSyxFQUFFLElBQUksQ0FBQyxHQUFHLEVBQUUsQ0FBQyxDQUFDO0lBQ3JGLENBQUM7O0FBOUJILDRDQStCQyIsInNvdXJjZXNDb250ZW50IjpbImltcG9ydCB7IENmbk91dHB1dCwgRHVyYXRpb24sIFN0YWNrIH0gZnJvbSAnYXdzLWNkay1saWInO1xuaW1wb3J0IHsgSUV2ZW50QnVzIH0gZnJvbSAnYXdzLWNkay1saWIvYXdzLWV2ZW50cyc7XG5pbXBvcnQgeyBDb2RlLCBGdW5jdGlvbiwgRnVuY3Rpb25VcmxBdXRoVHlwZSwgUnVudGltZSB9IGZyb20gJ2F3cy1jZGstbGliL2F3cy1sYW1iZGEnO1xuaW1wb3J0IHsgQnVja2V0IH0gZnJvbSAnYXdzLWNkay1saWIvYXdzLXMzJztcbmltcG9ydCB7IElTZWNyZXQgfSBmcm9tICdhd3MtY2RrLWxpYi9hd3Mtc2VjcmV0c21hbmFnZXInO1xuaW1wb3J0IHsgQ29uc3RydWN0IH0gZnJvbSAnY29uc3RydWN0cyc7XG5pbXBvcnQgeyBQYXJ0bmVyIH0gZnJvbSAnLi9QYXJ0bmVyJztcbmltcG9ydCB7IEludm9jYXRpb25BbGFybSB9IGZyb20gJy4vVXRpbCc7XG5cbmV4cG9ydCBpbnRlcmZhY2UgUGFydG5lckZ1bmN0aW9uUHJvcHMge1xuXG4gIC8qKlxuICAgICAqIFNNIFNlY3JldCBjb250YWluaW5nIHRoZSBzZWNyZXQgc3RyaW5nIHVzZWQgdG8gdmFsaWRhdGUgd2ViaG9vayBldmVudHMuXG4gICAgICovXG4gIHJlYWRvbmx5IHdlYmhvb2tTZWNyZXQ6IElTZWNyZXQ7XG5cbiAgLyoqXG4gICAgICogRXZlbnRidXMgdG8gc2VuZCBQYXJ0bmVyIGV2ZW50cyB0by5cbiAgICAgKi9cbiAgcmVhZG9ubHkgZXZlbnRCdXM6IElFdmVudEJ1cztcblxuICAvKipcbiAgICAgKiBNYXhpbXVtIG51bWJlciBvZiBjb25jdXJyZW50IGludm9jYXRpb25zIG9uIHRoZSBmVVJMIGZ1bmN0aW9uIGJlZm9yZSB0cmlnZ2VyaW5nIHRoZSBhbGFybS5cbiAgICAgKi9cbiAgcmVhZG9ubHkgbGFtYmRhSW52b2NhdGlvbkFsYXJtVGhyZXNob2xkOiBudW1iZXI7XG5cbiAgLyoqXG4gICAgICogVGhlIHBhcnRuZXIgdG8gY3JlYXRlIGFuIGV2ZW50cyBwcm9jZXNzb3IgZm9yLlxuICAgICAqL1xuICByZWFkb25seSBldmVudGJyaWRnZVBhcnRuZXI6IFBhcnRuZXI7XG5cbn1cblxuLyoqXG4gKiBBYnN0cmFjdCBjbGFzcyBmb3IgTGFtYmRhLWRyaXZlbiBFdmVudGJyaWRnZSBpbnRlZ3JhdGlvbnMuXG4gKiBUaGlzIG9ubHkgd29ya3MgYmVjYXVzZSB0aGUgcGF0dGVybiBmb3IgdGhlIFMzIEtleXMgbGluZXMgdXAgdG86IGxhbWJkYS10ZW1wbGF0ZXMvPHBhcnRuZXI+LWxhbWJkYXNyYy56aXBcbiAqIEBzZWUgaHR0cHM6Ly9kb2NzLmF3cy5hbWF6b24uY29tL2V2ZW50YnJpZGdlL2xhdGVzdC91c2VyZ3VpZGUvZWItc2Fhcy1mdXJscy5odG1sXG4gKi9cbmV4cG9ydCBhYnN0cmFjdCBjbGFzcyBQYXJ0bmVyUHJvY2Vzc29yIGV4dGVuZHMgQ29uc3RydWN0IHtcbiAgcHVibGljIHBhcnRuZXJFdmVudHNGdW5jdGlvbjogRnVuY3Rpb247XG4gIHB1YmxpYyBpbnZvY2F0aW9uQWxhcm06IEludm9jYXRpb25BbGFybTtcbiAgY29uc3RydWN0b3Ioc2NvcGU6IENvbnN0cnVjdCwgaWQ6IHN0cmluZywgcHJvcHM6IFBhcnRuZXJGdW5jdGlvblByb3BzKSB7XG4gICAgc3VwZXIoc2NvcGUsIGlkKTtcblxuICAgIHRoaXMucGFydG5lckV2ZW50c0Z1bmN0aW9uID0gbmV3IEZ1bmN0aW9uKHRoaXMsIGAke3Byb3BzLmV2ZW50YnJpZGdlUGFydG5lcn1FdmVudHNGdW5jdGlvbmAsIHtcbiAgICAgIGNvZGU6IENvZGUuZnJvbUJ1Y2tldChCdWNrZXQuZnJvbUJ1Y2tldE5hbWUodGhpcywgJ0FXU0Z1bmN0aW9uQnVja2V0JywgYGV2ZW50YnJpZGdlLWluYm91bmQtd2ViaG9vay10ZW1wbGF0ZXMtcHJvZC0ke1N0YWNrLm9mKHRoaXMpLnJlZ2lvbn1gKSwgYGxhbWJkYS10ZW1wbGF0ZXMvJHtwcm9wcy5ldmVudGJyaWRnZVBhcnRuZXJ9LWxhbWJkYXNyYy56aXBgKSxcbiAgICAgIGhhbmRsZXI6ICdhcHAubGFtYmRhX2hhbmRsZXInLFxuICAgICAgcnVudGltZTogUnVudGltZS5QWVRIT05fM183LFxuICAgICAgbWVtb3J5U2l6ZTogMTI4LFxuICAgICAgdGltZW91dDogRHVyYXRpb24uc2Vjb25kcygxMDApLFxuICAgICAgcmVzZXJ2ZWRDb25jdXJyZW50RXhlY3V0aW9uczogMTAsXG4gICAgICBlbnZpcm9ubWVudDoge1xuICAgICAgICBHSVRIVUJfV0VCSE9PS19TRUNSRVRfQVJOOiBwcm9wcy53ZWJob29rU2VjcmV0LnNlY3JldEFybixcbiAgICAgICAgRVZFTlRfQlVTX05BTUU6IHByb3BzLmV2ZW50QnVzLmV2ZW50QnVzTmFtZSxcbiAgICAgIH0sXG4gICAgfSk7XG5cbiAgICB0aGlzLmludm9jYXRpb25BbGFybSA9IG5ldyBJbnZvY2F0aW9uQWxhcm0odGhpcywgYCR7cHJvcHMuZXZlbnRicmlkZ2VQYXJ0bmVyfUludm9jYXRpb25BbGFybWAsIHtcbiAgICAgIHRocmVzaG9sZDogcHJvcHMubGFtYmRhSW52b2NhdGlvbkFsYXJtVGhyZXNob2xkLFxuICAgICAgZXZlbnRGdW5jdGlvbjogdGhpcy5wYXJ0bmVyRXZlbnRzRnVuY3Rpb24sXG4gICAgfSk7XG5cbiAgICBjb25zdCBmVVJMID0gdGhpcy5wYXJ0bmVyRXZlbnRzRnVuY3Rpb24uYWRkRnVuY3Rpb25VcmwoeyBhdXRoVHlwZTogRnVuY3Rpb25VcmxBdXRoVHlwZS5OT05FIH0pO1xuXG4gICAgcHJvcHMud2ViaG9va1NlY3JldC5ncmFudFJlYWQodGhpcy5wYXJ0bmVyRXZlbnRzRnVuY3Rpb24pO1xuICAgIHByb3BzLmV2ZW50QnVzLmdyYW50UHV0RXZlbnRzVG8odGhpcy5wYXJ0bmVyRXZlbnRzRnVuY3Rpb24pO1xuXG4gICAgbmV3IENmbk91dHB1dCh0aGlzLCBgJHtwcm9wcy5ldmVudGJyaWRnZVBhcnRuZXJ9RnVuY3Rpb25VcmxgLCB7IHZhbHVlOiBmVVJMLnVybCB9KTtcbiAgfVxufSJdfQ==
```

##### package/lib/Stripe.js

###### js-beautify {}

```diff
@@ -19,10 +19,10 @@
         });
     }
 }
 exports.StripeEventProcessor = StripeEventProcessor;
 _a = JSII_RTTI_SYMBOL_1;
 StripeEventProcessor[_a] = {
     fqn: "cdk-eventbridge-partner-processors.StripeEventProcessor",
-    version: "0.0.98"
+    version: "0.0.99"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiU3RyaXBlLmpzIiwic291cmNlUm9vdCI6IiIsInNvdXJjZXMiOlsiLi4vc3JjL1N0cmlwZS50cyJdLCJuYW1lcyI6W10sIm1hcHBpbmdzIjoiOzs7OztBQUdBLHVDQUFvQztBQUNwQyx1REFBcUQ7QUFxQnJEOzs7R0FHRztBQUNILE1BQWEsb0JBQXFCLFNBQVEsa0NBQWdCO0lBQ3hELFlBQVksS0FBZ0IsRUFBRSxFQUFVLEVBQUUsS0FBa0I7UUFDMUQsS0FBSyxDQUFDLEtBQUssRUFBRSxFQUFFLEVBQUUsRUFBRSxHQUFHLEtBQUssRUFBRSxrQkFBa0IsRUFBRSxpQkFBTyxDQUFDLE1BQU0sRUFBRSxDQUFDLENBQUM7SUFDckUsQ0FBQzs7QUFISCxvREFJQyIsInNvdXJjZXNDb250ZW50IjpbImltcG9ydCB7IElFdmVudEJ1cyB9IGZyb20gJ2F3cy1jZGstbGliL2F3cy1ldmVudHMnO1xuaW1wb3J0IHsgSVNlY3JldCB9IGZyb20gJ2F3cy1jZGstbGliL2F3cy1zZWNyZXRzbWFuYWdlcic7XG5pbXBvcnQgeyBDb25zdHJ1Y3QgfSBmcm9tICdjb25zdHJ1Y3RzJztcbmltcG9ydCB7IFBhcnRuZXIgfSBmcm9tICcuL1BhcnRuZXInO1xuaW1wb3J0IHsgUGFydG5lclByb2Nlc3NvciB9IGZyb20gJy4vUGFydG5lckZ1bmN0aW9uJztcblxuZXhwb3J0IGludGVyZmFjZSBTdHJpcGVQcm9wcyB7XG5cbiAgLyoqXG4gICAqIFNNIFNlY3JldCBjb250YWluaW5nIHRoZSBzZWNyZXQgc3RyaW5nIHVzZWQgdG8gdmFsaWRhdGUgd2ViaG9vayBldmVudHMuXG4gICAqL1xuICByZWFkb25seSB3ZWJob29rU2VjcmV0OiBJU2VjcmV0O1xuXG4gIC8qKlxuICAgKiBFdmVudGJ1cyB0byBzZW5kIEdpdEh1YiBldmVudHMgdG8uXG4gICAqL1xuICByZWFkb25seSBldmVudEJ1czogSUV2ZW50QnVzO1xuXG4gIC8qKlxuICAgKiBNYXhpbXVtIG51bWJlciBvZiBjb25jdXJyZW50IGludm9jYXRpb25zIG9uIHRoZSBmVVJMIGZ1bmN0aW9uIGJlZm9yZSB0cmlnZ2VyaW5nIHRoZSBhbGFybS5cbiAgICovXG4gIHJlYWRvbmx5IGxhbWJkYUludm9jYXRpb25BbGFybVRocmVzaG9sZDogbnVtYmVyO1xuXG59XG5cbi8qKlxuICogQ0RLIHdyYXBwZXIgZm9yIHRoZSBTdHJpcGUgRXZlbnRicmlkZ2UgcHJvY2Vzc29yLlxuICogQHNlZSBodHRwczovL2RvY3MuYXdzLmFtYXpvbi5jb20vZXZlbnRicmlkZ2UvbGF0ZXN0L3VzZXJndWlkZS9lYi1zYWFzLWZ1cmxzLmh0bWwjZnVybHMtY29ubmVjdGlvbi1naXRodWJcbiAqL1xuZXhwb3J0IGNsYXNzIFN0cmlwZUV2ZW50UHJvY2Vzc29yIGV4dGVuZHMgUGFydG5lclByb2Nlc3NvciB7XG4gIGNvbnN0cnVjdG9yKHNjb3BlOiBDb25zdHJ1Y3QsIGlkOiBzdHJpbmcsIHByb3BzOiBTdHJpcGVQcm9wcykge1xuICAgIHN1cGVyKHNjb3BlLCBpZCwgeyAuLi5wcm9wcywgZXZlbnRicmlkZ2VQYXJ0bmVyOiBQYXJ0bmVyLlNUUklQRSB9KTtcbiAgfVxufSJdfQ==
```

##### package/lib/Twilio.js

###### js-beautify {}

```diff
@@ -19,10 +19,10 @@
         });
     }
 }
 exports.TwilioEventProcessor = TwilioEventProcessor;
 _a = JSII_RTTI_SYMBOL_1;
 TwilioEventProcessor[_a] = {
     fqn: "cdk-eventbridge-partner-processors.TwilioEventProcessor",
-    version: "0.0.98"
+    version: "0.0.99"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiVHdpbGlvLmpzIiwic291cmNlUm9vdCI6IiIsInNvdXJjZXMiOlsiLi4vc3JjL1R3aWxpby50cyJdLCJuYW1lcyI6W10sIm1hcHBpbmdzIjoiOzs7OztBQUdBLHVDQUFvQztBQUNwQyx1REFBcUQ7QUFxQnJEOzs7R0FHRztBQUNILE1BQWEsb0JBQXFCLFNBQVEsa0NBQWdCO0lBQ3hELFlBQVksS0FBZ0IsRUFBRSxFQUFVLEVBQUUsS0FBa0I7UUFDMUQsS0FBSyxDQUFDLEtBQUssRUFBRSxFQUFFLEVBQUUsRUFBRSxHQUFHLEtBQUssRUFBRSxrQkFBa0IsRUFBRSxpQkFBTyxDQUFDLE1BQU0sRUFBRSxDQUFDLENBQUM7SUFDckUsQ0FBQzs7QUFISCxvREFJQyIsInNvdXJjZXNDb250ZW50IjpbImltcG9ydCB7IElFdmVudEJ1cyB9IGZyb20gJ2F3cy1jZGstbGliL2F3cy1ldmVudHMnO1xuaW1wb3J0IHsgSVNlY3JldCB9IGZyb20gJ2F3cy1jZGstbGliL2F3cy1zZWNyZXRzbWFuYWdlcic7XG5pbXBvcnQgeyBDb25zdHJ1Y3QgfSBmcm9tICdjb25zdHJ1Y3RzJztcbmltcG9ydCB7IFBhcnRuZXIgfSBmcm9tICcuL1BhcnRuZXInO1xuaW1wb3J0IHsgUGFydG5lclByb2Nlc3NvciB9IGZyb20gJy4vUGFydG5lckZ1bmN0aW9uJztcblxuZXhwb3J0IGludGVyZmFjZSBUd2lsaW9Qcm9wcyB7XG5cbiAgLyoqXG4gICAgICogU00gU2VjcmV0IGNvbnRhaW5pbmcgdGhlIHNlY3JldCBzdHJpbmcgdXNlZCB0byB2YWxpZGF0ZSB3ZWJob29rIGV2ZW50cy5cbiAgICAgKi9cbiAgcmVhZG9ubHkgd2ViaG9va1NlY3JldDogSVNlY3JldDtcblxuICAvKipcbiAgICAgKiBFdmVudGJ1cyB0byBzZW5kIEdpdEh1YiBldmVudHMgdG8uXG4gICAgICovXG4gIHJlYWRvbmx5IGV2ZW50QnVzOiBJRXZlbnRCdXM7XG5cbiAgLyoqXG4gICAgICogTWF4aW11bSBudW1iZXIgb2YgY29uY3VycmVudCBpbnZvY2F0aW9ucyBvbiB0aGUgZlVSTCBmdW5jdGlvbiBiZWZvcmUgdHJpZ2dlcmluZyB0aGUgYWxhcm0uXG4gICAgICovXG4gIHJlYWRvbmx5IGxhbWJkYUludm9jYXRpb25BbGFybVRocmVzaG9sZDogbnVtYmVyO1xuXG59XG5cbi8qKlxuICogQ0RLIHdyYXBwZXIgZm9yIHRoZSBUd2lsaW8gRXZlbnRicmlkZ2UgcHJvY2Vzc29yLlxuICogQHNlZSBodHRwczovL2RvY3MuYXdzLmFtYXpvbi5jb20vZXZlbnRicmlkZ2UvbGF0ZXN0L3VzZXJndWlkZS9lYi1zYWFzLWZ1cmxzLmh0bWwjZnVybHMtY29ubmVjdGlvbi1naXRodWJcbiAqL1xuZXhwb3J0IGNsYXNzIFR3aWxpb0V2ZW50UHJvY2Vzc29yIGV4dGVuZHMgUGFydG5lclByb2Nlc3NvciB7XG4gIGNvbnN0cnVjdG9yKHNjb3BlOiBDb25zdHJ1Y3QsIGlkOiBzdHJpbmcsIHByb3BzOiBUd2lsaW9Qcm9wcykge1xuICAgIHN1cGVyKHNjb3BlLCBpZCwgeyAuLi5wcm9wcywgZXZlbnRicmlkZ2VQYXJ0bmVyOiBQYXJ0bmVyLlRXSUxJTyB9KTtcbiAgfVxufSJdfQ==
```

##### package/lib/Util.js

###### js-beautify {}

```diff
@@ -33,10 +33,10 @@
         });
     }
 }
 exports.InvocationAlarm = InvocationAlarm;
 _a = JSII_RTTI_SYMBOL_1;
 InvocationAlarm[_a] = {
     fqn: "cdk-eventbridge-partner-processors.InvocationAlarm",
-    version: "0.0.98"
+    version: "0.0.99"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiVXRpbC5qcyIsInNvdXJjZVJvb3QiOiIiLCJzb3VyY2VzIjpbIi4uL3NyYy9VdGlsLnRzIl0sIm5hbWVzIjpbXSwibWFwcGluZ3MiOiI7Ozs7O0FBQUEsNkNBQThDO0FBQzlDLCtEQUErRTtBQUUvRSwyQ0FBdUM7QUFjdkM7O0dBRUc7QUFDSCxNQUFhLGVBQWdCLFNBQVEsc0JBQVM7SUFDNUMsWUFBWSxLQUFnQixFQUFFLEVBQVUsRUFBRSxLQUEyQjtRQUNuRSxLQUFLLENBQUMsS0FBSyxFQUFFLEVBQUUsQ0FBQyxDQUFDO1FBRWpCLElBQUksc0JBQUssQ0FBQyxJQUFJLEVBQUUsaUJBQWlCLEVBQUU7WUFDakMsZ0JBQWdCLEVBQUUsYUFBYSxtQkFBSyxDQUFDLEVBQUUsQ0FBQyxJQUFJLENBQUMsQ0FBQyxTQUFTLDZDQUE2QztZQUNwRyxTQUFTLEVBQUUsMENBQTBDLG1CQUFLLENBQUMsRUFBRSxDQUFDLElBQUksQ0FBQyxDQUFDLFNBQVMsRUFBRTtZQUMvRSxpQkFBaUIsRUFBRSxDQUFDO1lBQ3BCLE1BQU0sRUFBRSxJQUFJLHVCQUFNLENBQUM7Z0JBQ2pCLFVBQVUsRUFBRSxhQUFhO2dCQUN6QixTQUFTLEVBQUUsWUFBWTtnQkFDdkIsTUFBTSxFQUFFLHNCQUFRLENBQUMsT0FBTyxDQUFDLEdBQUcsQ0FBQztnQkFDN0IsU0FBUyxFQUFFLEtBQUs7Z0JBQ2hCLGFBQWEsRUFBRTtvQkFDYixJQUFJLEVBQUUsY0FBYztvQkFDcEIsS0FBSyxFQUFFLEtBQUssQ0FBQyxhQUFhLENBQUMsWUFBWTtpQkFDeEM7YUFDRixDQUFDO1lBQ0YsU0FBUyxFQUFFLEtBQUssQ0FBQyxTQUFTO1lBQzFCLGtCQUFrQixFQUFFLG1DQUFrQixDQUFDLHNCQUFzQjtTQUM5RCxDQUFDLENBQUM7SUFDTCxDQUFDOztBQXJCSCwwQ0FzQkMiLCJzb3VyY2VzQ29udGVudCI6WyJpbXBvcnQgeyBEdXJhdGlvbiwgU3RhY2sgfSBmcm9tICdhd3MtY2RrLWxpYic7XG5pbXBvcnQgeyBBbGFybSwgQ29tcGFyaXNvbk9wZXJhdG9yLCBNZXRyaWMgfSBmcm9tICdhd3MtY2RrLWxpYi9hd3MtY2xvdWR3YXRjaCc7XG5pbXBvcnQgeyBJRnVuY3Rpb24gfSBmcm9tICdhd3MtY2RrLWxpYi9hd3MtbGFtYmRhJztcbmltcG9ydCB7IENvbnN0cnVjdCB9IGZyb20gJ2NvbnN0cnVjdHMnO1xuXG5leHBvcnQgaW50ZXJmYWNlIEludm9jYXRpb25BbGFybVByb3BzIHtcbiAgLyoqXG4gICAgICogTGFtYmRhIEludm9jYXRpb24gdGhyZXNob2xkLlxuICAgICAqL1xuICByZWFkb25seSB0aHJlc2hvbGQ6IG51bWJlcjtcblxuICAvKipcbiAgICAgKiBUaGUgZnVuY3Rpb24gdG8gbW9uaXRvci5cbiAgICAgKi9cbiAgcmVhZG9ubHkgZXZlbnRGdW5jdGlvbjogSUZ1bmN0aW9uO1xufVxuXG4vKipcbiAqIENsb3Vkd2F0Y2ggQWxhcm0gdXNlZCBhY3Jvc3MgdGhpcyBjb25zdHJ1Y3QgbGlicmFyeS5cbiAqL1xuZXhwb3J0IGNsYXNzIEludm9jYXRpb25BbGFybSBleHRlbmRzIENvbnN0cnVjdCB7XG4gIGNvbnN0cnVjdG9yKHNjb3BlOiBDb25zdHJ1Y3QsIGlkOiBzdHJpbmcsIHByb3BzOiBJbnZvY2F0aW9uQWxhcm1Qcm9wcykge1xuICAgIHN1cGVyKHNjb3BlLCBpZCk7XG5cbiAgICBuZXcgQWxhcm0odGhpcywgJ0ludm9jYXRpb25BbGFybScsIHtcbiAgICAgIGFsYXJtRGVzY3JpcHRpb246IGBBbGFybSBmb3IgJHtTdGFjay5vZih0aGlzKS5zdGFja05hbWV9IC0gSW5ib3VuZFdlYmhvb2sgTGFtYmRhIGZvciB0cmFmZmljIHNwaWtlc2AsXG4gICAgICBhbGFybU5hbWU6IGBJbmJvdW5kV2ViaG9vay1MYW1iZGEtSW52b2NhdGlvbi1BbGFybS0ke1N0YWNrLm9mKHRoaXMpLnN0YWNrTmFtZX1gLFxuICAgICAgZXZhbHVhdGlvblBlcmlvZHM6IDIsXG4gICAgICBtZXRyaWM6IG5ldyBNZXRyaWMoe1xuICAgICAgICBtZXRyaWNOYW1lOiAnSW52b2NhdGlvbnMnLFxuICAgICAgICBuYW1lc3BhY2U6ICdBV1MvTGFtYmRhJyxcbiAgICAgICAgcGVyaW9kOiBEdXJhdGlvbi5zZWNvbmRzKDMwMCksXG4gICAgICAgIHN0YXRpc3RpYzogJ1N1bScsXG4gICAgICAgIGRpbWVuc2lvbnNNYXA6IHtcbiAgICAgICAgICBOYW1lOiAnRnVuY3Rpb25OYW1lJyxcbiAgICAgICAgICBWYWx1ZTogcHJvcHMuZXZlbnRGdW5jdGlvbi5mdW5jdGlvbk5hbWUsXG4gICAgICAgIH0sXG4gICAgICB9KSxcbiAgICAgIHRocmVzaG9sZDogcHJvcHMudGhyZXNob2xkLFxuICAgICAgY29tcGFyaXNvbk9wZXJhdG9yOiBDb21wYXJpc29uT3BlcmF0b3IuR1JFQVRFUl9USEFOX1RIUkVTSE9MRCxcbiAgICB9KTtcbiAgfVxufSJdfQ==
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9673913043478262%*

 * *Differences: {"'devDependencies'": "{'jsii-docgen': '^7.0.146', 'projen': '^0.65.20'}", "'version'": "'0.0.99'"}*

```diff
@@ -16,19 +16,19 @@
         "eslint-import-resolver-node": "^0.3.6",
         "eslint-import-resolver-typescript": "^3.5.2",
         "eslint-plugin-import": "^2.26.0",
         "jest": "^27",
         "jest-junit": "^13",
         "jsii": "^1.71.0",
         "jsii-diff": "^1.71.0",
-        "jsii-docgen": "^7.0.145",
+        "jsii-docgen": "^7.0.146",
         "jsii-pacmak": "^1.71.0",
         "json-schema": "^0.4.0",
         "npm-check-updates": "^16",
-        "projen": "^0.65.19",
+        "projen": "^0.65.20",
         "standard-version": "^9",
         "ts-jest": "^27",
         "ts-node": "^10.9.1",
         "typescript": "^4.8.4"
     },
     "jest": {
         "clearMocks": true,
@@ -131,9 +131,9 @@
         "test:watch": "npx projen test:watch",
         "unbump": "npx projen unbump",
         "upgrade": "npx projen upgrade",
         "watch": "npx projen watch"
     },
     "stability": "stable",
     "types": "lib/index.d.ts",
-    "version": "0.0.98"
+    "version": "0.0.99"
 }
```

### Comparing `a-bigelow.cdk-eventbridge-partner-processors-0.0.98/src/a_bigelow.cdk_eventbridge_partner_processors.egg-info/PKG-INFO` & `a-bigelow.cdk-eventbridge-partner-processors-0.0.99/src/a_bigelow.cdk_eventbridge_partner_processors.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a-bigelow.cdk-eventbridge-partner-processors
-Version: 0.0.98
+Version: 0.0.99
 Summary: cdk-eventbridge-partner-processors
 Home-page: https://github.com/a-bigelow/cdk-eventbridge-partner-processors.git
 Author: a-bigelow<adam@adambigelow.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/a-bigelow/cdk-eventbridge-partner-processors.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `a-bigelow.cdk-eventbridge-partner-processors-0.0.98/src/a_bigelow.cdk_eventbridge_partner_processors.egg-info/SOURCES.txt` & `a-bigelow.cdk-eventbridge-partner-processors-0.0.99/src/a_bigelow.cdk_eventbridge_partner_processors.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/a-bigelow/cdk-eventbridge-partner-processors/__init__.py
 src/a-bigelow/cdk-eventbridge-partner-processors/py.typed
 src/a-bigelow/cdk-eventbridge-partner-processors/_jsii/__init__.py
-src/a-bigelow/cdk-eventbridge-partner-processors/_jsii/cdk-eventbridge-partner-processors@0.0.98.jsii.tgz
+src/a-bigelow/cdk-eventbridge-partner-processors/_jsii/cdk-eventbridge-partner-processors@0.0.99.jsii.tgz
 src/a_bigelow.cdk_eventbridge_partner_processors.egg-info/PKG-INFO
 src/a_bigelow.cdk_eventbridge_partner_processors.egg-info/SOURCES.txt
 src/a_bigelow.cdk_eventbridge_partner_processors.egg-info/dependency_links.txt
 src/a_bigelow.cdk_eventbridge_partner_processors.egg-info/requires.txt
 src/a_bigelow.cdk_eventbridge_partner_processors.egg-info/top_level.txt
```

