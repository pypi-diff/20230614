# Comparing `tmp/pymvola-0.0.2.tar.gz` & `tmp/pymvola-0.0.3.tar.gz`

## Comparing `pymvola-0.0.2.tar` & `pymvola-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pymvola-0.0.2/requirements.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pymvola-0.0.2/.vscode/settings.json
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 pymvola-0.0.2/pymvola/__init__.py
--rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 pymvola-0.0.2/pymvola/core.py
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 pymvola-0.0.2/pymvola/exceptions.py
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 pymvola-0.0.2/pymvola/models.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 pymvola-0.0.2/pymvola/util/__init__.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 pymvola-0.0.2/pymvola/util/authorization.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 pymvola-0.0.2/pymvola/util/consts.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 pymvola-0.0.2/pymvola/util/date_.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 pymvola-0.0.2/pymvola/util/enumeration.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pymvola-0.0.2/pymvola/util/uuid_.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymvola-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 pymvola-0.0.2/tests/test_models_msisdn.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 pymvola-0.0.2/tests/test_models_transaction.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 pymvola-0.0.2/tests/test_pymvola.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 pymvola-0.0.2/tests/test_util_authorization.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pymvola-0.0.2/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pymvola-0.0.2/LICENSE
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pymvola-0.0.2/README.md
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pymvola-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 pymvola-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pymvola-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pymvola-0.0.3/.vscode/settings.json
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 pymvola-0.0.3/pymvola/__init__.py
+-rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 pymvola-0.0.3/pymvola/core.py
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 pymvola-0.0.3/pymvola/exceptions.py
+-rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 pymvola-0.0.3/pymvola/models.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 pymvola-0.0.3/pymvola/util/__init__.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 pymvola-0.0.3/pymvola/util/authorization.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 pymvola-0.0.3/pymvola/util/consts.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 pymvola-0.0.3/pymvola/util/date_.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 pymvola-0.0.3/pymvola/util/enumeration.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pymvola-0.0.3/pymvola/util/uuid_.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymvola-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 pymvola-0.0.3/tests/test_models_msisdn.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 pymvola-0.0.3/tests/test_models_transaction.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 pymvola-0.0.3/tests/test_pymvola.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 pymvola-0.0.3/tests/test_util_authorization.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pymvola-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pymvola-0.0.3/LICENSE
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pymvola-0.0.3/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 pymvola-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pymvola-0.0.3/PKG-INFO
```

### Comparing `pymvola-0.0.2/pymvola/core.py` & `pymvola-0.0.3/pymvola/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Author: Ryuka (lovanirina.ran@gmail.com)
 Date: 14/05/2023
 """
 
 import json
 
 import requests
-from pymvola.util import Env, get_uuid, now
+from pymvola.util import Env, get_uuid
 from pymvola.util.consts import (
     MVOLA_URL_PREPROD,
     MVOLA_URL_PROD,
     DEFAULT_TIMEOUT,
     MVOLA_URL_TRANSACTION_BASE,
 )
 from pymvola.util.enumeration import UserLanguage
@@ -113,14 +113,25 @@
 
         if response.ok:
             return response_json["access_token"]
 
         raise MVolaResponseException(response)
 
     def init_transaction(self, transaction: Transaction):
+        """Init a transaction.
+
+        Args:
+            transaction (Transaction): Instance of Transaction
+
+        Raises:
+            MVolaResponseException: When response is K.O
+
+        Returns:
+            Transaction: instance of Transaction but with original transaction id and new status.
+        """
         url = f"{self.url}{MVOLA_URL_TRANSACTION_BASE}/"
 
         payload = json.dumps(transaction.to_schema(self.conf["partner_name"]))
 
         headers = {
             "Content-Type": "application/json",
             "Cache-Control": "no-cache",
@@ -137,19 +148,31 @@
 
         response_json = response.json()
 
         if response.ok:
             transaction.original_transaction_reference = response_json[
                 "serverCorrelationId"
             ]
+            transaction.status = Transaction.Status.INITIED
             return transaction
 
         raise MVolaResponseException(response)
 
     def get_transaction_status(self, transaction_id: str):
+        """Get the status of a transaction.
+
+        Args:
+            transaction_id (str): transaction id provided by MVola
+
+        Raises:
+            MVolaResponseException: When response is K.O
+
+        Returns:
+            str: status of the given transaction id
+        """
         url = f"{self.url}{MVOLA_URL_TRANSACTION_BASE}/status/{transaction_id}"
 
         payload = {}
 
         headers = {
             "Content-Type": "application/json",
             "Cache-Control": "no-cache",
```

### Comparing `pymvola-0.0.2/pymvola/exceptions.py` & `pymvola-0.0.3/pymvola/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymvola-0.0.2/pymvola/models.py` & `pymvola-0.0.3/pymvola/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     MINIMAL_MSISDN_LEN,
 )
 from pymvola.util.enumeration import Currency
 from pymvola.util import get_uuid, now
 
 
 class Msisdn:
+    """Msisdn Class"""
+
     def __init__(self, msisdn) -> None:
         self.value = self.regularize_msisdn(msisdn)
         self.check_validity_of_msisdn(self.value)
 
     @classmethod
     def check_validity_of_msisdn(cls, msisdn: str) -> None:
         """Check the validity of a given msisdn
@@ -81,25 +83,32 @@
         super().check_validity_of_msisdn(msisdn)
         if bool(re.match(TELMA_PHONE_NUMBER_PATTERN, msisdn)):
             return
         raise InvalidMsisdn(msisdn)
 
 
 class Transaction:
+    """Represent a transaction."""
+
     class Status:
+        """Represent the different status of a Transaction."""
+
+        NOT_INITIED = "not_initied"
+        INITIED = "initied"
         PENDING = "pending"
         FAILED = "failed"
         COMPLETED = "completed"
 
     def __init__(
         self,
-        amount: int,
+        amount: float,
         description_text: str,
         creditor: object,
         debitor: object,
+        requesting_organisation_transaction_reference: str = None,
         **kwargs,
     ) -> None:
         # amount
         self.amount = str(amount)
 
         # currency
         if kwargs.get("currency") is None:
@@ -107,15 +116,20 @@
         else:
             self.currency = kwargs.get("currency")
 
         # descriptionText
         self.description_text = description_text
 
         # requestingOrganisationTransactionReference
-        self.requesting_organisation_transaction_reference = get_uuid()
+        if requesting_organisation_transaction_reference:
+            self.requesting_organisation_transaction_reference = (
+                requesting_organisation_transaction_reference
+            )
+        else:
+            self.requesting_organisation_transaction_reference = get_uuid()
 
         # requestDate
         self.request_date = now()
 
         # originalTransactionReference
         if kwargs.get("original_transaction_reference") is None:
             self.original_transaction_reference = ""
@@ -128,15 +142,19 @@
         self.debitor = Debitor(debitor)
         self.debit_party = [{"key": "msisdn", "value": f"{self.debitor}"}]
 
         # creditParty
         self.creditor = Creditor(creditor)
         self.credit_party = [{"key": "msisdn", "value": f"{self.creditor}"}]
 
+        # status
+        self.status = self.Status.NOT_INITIED
+
     def to_schema(self, partner_name) -> dict:
+        """Create a dict from the transaction that will be used to sent as data to MVola API."""
         return {
             "amount": self.amount,
             "currency": self.currency,
             "descriptionText": self.description_text,
             "requestingOrganisationTransactionReference": (
                 self.requesting_organisation_transaction_reference
             ),
```

### Comparing `pymvola-0.0.2/pymvola/util/authorization.py` & `pymvola-0.0.3/pymvola/util/authorization.py`

 * *Files identical despite different names*

### Comparing `pymvola-0.0.2/pymvola/util/date_.py` & `pymvola-0.0.3/pymvola/util/date_.py`

 * *Files identical despite different names*

### Comparing `pymvola-0.0.2/pymvola/util/enumeration.py` & `pymvola-0.0.3/pymvola/util/enumeration.py`

 * *Files identical despite different names*

### Comparing `pymvola-0.0.2/tests/test_models_msisdn.py` & `pymvola-0.0.3/tests/test_models_msisdn.py`

 * *Files identical despite different names*

### Comparing `pymvola-0.0.2/tests/test_models_transaction.py` & `pymvola-0.0.3/tests/test_models_transaction.py`

 * *Files identical despite different names*

### Comparing `pymvola-0.0.2/tests/test_pymvola.py` & `pymvola-0.0.3/tests/test_pymvola.py`

 * *Files identical despite different names*

### Comparing `pymvola-0.0.2/.gitignore` & `pymvola-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pymvola-0.0.2/LICENSE` & `pymvola-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymvola-0.0.2/PKG-INFO` & `pymvola-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pymvola
-Version: 0.0.2
+Version: 0.0.3
 Summary: Open source and easy use of the MVola API
 Author-email: ryuka <lovanirina.ran@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # PyMVola (Python MVola)
 
 Open source and easy use of the [MVola API](https://www.mvola.mg/devportal/).
 
 Inspired by [MVola from @rivo2302](https://github.com/rivo2302/Mvola) this is a complete rewrite of the MVola Client in python.
```

