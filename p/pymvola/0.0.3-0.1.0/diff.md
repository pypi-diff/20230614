# Comparing `tmp/pymvola-0.0.3.tar.gz` & `tmp/pymvola-0.1.0.tar.gz`

## Comparing `pymvola-0.0.3.tar` & `pymvola-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pymvola-0.0.3/requirements.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pymvola-0.0.3/.vscode/settings.json
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 pymvola-0.0.3/pymvola/__init__.py
--rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 pymvola-0.0.3/pymvola/core.py
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 pymvola-0.0.3/pymvola/exceptions.py
--rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 pymvola-0.0.3/pymvola/models.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 pymvola-0.0.3/pymvola/util/__init__.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 pymvola-0.0.3/pymvola/util/authorization.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 pymvola-0.0.3/pymvola/util/consts.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 pymvola-0.0.3/pymvola/util/date_.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 pymvola-0.0.3/pymvola/util/enumeration.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pymvola-0.0.3/pymvola/util/uuid_.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymvola-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 pymvola-0.0.3/tests/test_models_msisdn.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 pymvola-0.0.3/tests/test_models_transaction.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 pymvola-0.0.3/tests/test_pymvola.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 pymvola-0.0.3/tests/test_util_authorization.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pymvola-0.0.3/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pymvola-0.0.3/LICENSE
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pymvola-0.0.3/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 pymvola-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pymvola-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pymvola-0.1.0/requirements.txt
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pymvola-0.1.0/requirements_dev.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pymvola-0.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 pymvola-0.1.0/pymvola/__init__.py
+-rw-r--r--   0        0        0     6538 2020-02-02 00:00:00.000000 pymvola-0.1.0/pymvola/core.py
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 pymvola-0.1.0/pymvola/exceptions.py
+-rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 pymvola-0.1.0/pymvola/models.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 pymvola-0.1.0/pymvola/util/__init__.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 pymvola-0.1.0/pymvola/util/authorization.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 pymvola-0.1.0/pymvola/util/consts.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 pymvola-0.1.0/pymvola/util/date_.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 pymvola-0.1.0/pymvola/util/enumeration.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pymvola-0.1.0/pymvola/util/uuid_.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymvola-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 pymvola-0.1.0/tests/test_models_msisdn.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 pymvola-0.1.0/tests/test_models_transaction.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 pymvola-0.1.0/tests/test_pymvola.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 pymvola-0.1.0/tests/test_util_authorization.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pymvola-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pymvola-0.1.0/LICENSE
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pymvola-0.1.0/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 pymvola-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pymvola-0.1.0/PKG-INFO
```

### Comparing `pymvola-0.0.3/pymvola/core.py` & `pymvola-0.1.0/pymvola/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             )
         except Exception as err:
             raise GenericException(err) from err
 
         response_json = response.json()
 
         if response.ok:
-            return response_json["access_token"]
+            return response, response_json["access_token"]
 
         raise MVolaResponseException(response)
 
     def init_transaction(self, transaction: Transaction):
         """Init a transaction.
 
         Args:
@@ -149,15 +149,15 @@
         response_json = response.json()
 
         if response.ok:
             transaction.original_transaction_reference = response_json[
                 "serverCorrelationId"
             ]
             transaction.status = Transaction.Status.INITIED
-            return transaction
+            return response, transaction
 
         raise MVolaResponseException(response)
 
     def get_transaction_status(self, transaction_id: str):
         """Get the status of a transaction.
 
         Args:
@@ -187,10 +187,10 @@
         response = requests.request(
             "GET", url, headers=headers, data=payload, timeout=self.conf["timeout"]
         )
 
         response_json = response.json()
 
         if response.ok:
-            return response_json["status"]
+            return response, response_json["status"]
 
         raise MVolaResponseException(response)
```

### Comparing `pymvola-0.0.3/pymvola/exceptions.py` & `pymvola-0.1.0/pymvola/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymvola-0.0.3/pymvola/models.py` & `pymvola-0.1.0/pymvola/models.py`

 * *Files identical despite different names*

### Comparing `pymvola-0.0.3/pymvola/util/authorization.py` & `pymvola-0.1.0/pymvola/util/authorization.py`

 * *Files identical despite different names*

### Comparing `pymvola-0.0.3/pymvola/util/date_.py` & `pymvola-0.1.0/pymvola/util/date_.py`

 * *Files identical despite different names*

### Comparing `pymvola-0.0.3/pymvola/util/enumeration.py` & `pymvola-0.1.0/pymvola/util/enumeration.py`

 * *Files identical despite different names*

### Comparing `pymvola-0.0.3/tests/test_models_msisdn.py` & `pymvola-0.1.0/tests/test_models_msisdn.py`

 * *Files identical despite different names*

### Comparing `pymvola-0.0.3/tests/test_models_transaction.py` & `pymvola-0.1.0/tests/test_models_transaction.py`

 * *Files identical despite different names*

### Comparing `pymvola-0.0.3/tests/test_pymvola.py` & `pymvola-0.1.0/tests/test_pymvola.py`

 * *Files identical despite different names*

### Comparing `pymvola-0.0.3/.gitignore` & `pymvola-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pymvola-0.0.3/LICENSE` & `pymvola-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymvola-0.0.3/PKG-INFO` & `pymvola-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymvola
-Version: 0.0.3
+Version: 0.1.0
 Summary: Open source and easy use of the MVola API
 Author-email: ryuka <lovanirina.ran@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

