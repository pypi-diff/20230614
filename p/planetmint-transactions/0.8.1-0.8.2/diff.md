# Comparing `tmp/planetmint_transactions-0.8.1.tar.gz` & `tmp/planetmint_transactions-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetmint_transactions-0.8.1.tar", max compression
+gzip compressed data, was "planetmint_transactions-0.8.2.tar", max compression
```

## Comparing `planetmint_transactions-0.8.1.tar` & `planetmint_transactions-0.8.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    34523 2023-05-02 09:05:46.099022 planetmint_transactions-0.8.1/LICENSE
--rw-r--r--   0        0        0       73 2023-05-02 09:05:46.099022 planetmint_transactions-0.8.1/README.md
--rw-r--r--   0        0        0      693 2023-05-02 09:05:46.099022 planetmint_transactions-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      953 2023-05-02 09:05:46.099022 planetmint_transactions-0.8.1/transactions/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 09:05:46.099022 planetmint_transactions-0.8.1/transactions/common/__init__.py
--rw-r--r--   0        0        0     1932 2023-05-02 09:05:46.099022 planetmint_transactions-0.8.1/transactions/common/crypto.py
--rw-r--r--   0        0        0     3427 2023-05-02 09:05:46.099022 planetmint_transactions-0.8.1/transactions/common/exceptions.py
--rw-r--r--   0        0        0     5029 2023-05-02 09:05:46.099022 planetmint_transactions-0.8.1/transactions/common/input.py
--rw-r--r--   0        0        0     1323 2023-05-02 09:05:46.099022 planetmint_transactions-0.8.1/transactions/common/memoize.py
--rw-r--r--   0        0        0     8319 2023-05-02 09:05:46.099022 planetmint_transactions-0.8.1/transactions/common/output.py
--rw-r--r--   0        0        0     2606 2023-05-02 09:05:46.099022 planetmint_transactions-0.8.1/transactions/common/schema/README.md
--rw-r--r--   0        0        0     5231 2023-05-02 09:05:46.099022 planetmint_transactions-0.8.1/transactions/common/schema/__init__.py
--rw-r--r--   0        0        0     3841 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v1.0/transaction.yaml
--rw-r--r--   0        0        0      787 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v1.0/transaction_create.yaml
--rw-r--r--   0        0        0      778 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v1.0/transaction_transfer.yaml
--rw-r--r--   0        0        0     5070 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v2.0/transaction.yaml
--rw-r--r--   0        0        0     1127 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v2.0/transaction_chain_migration_election.yaml
--rw-r--r--   0        0        0      742 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v2.0/transaction_create.yaml
--rw-r--r--   0        0        0      778 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v2.0/transaction_transfer.yaml
--rw-r--r--   0        0        0     1674 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v2.0/transaction_validator_election.yaml
--rw-r--r--   0        0        0      843 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v2.0/transaction_vote.yaml
--rw-r--r--   0        0        0     4363 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction.yaml
--rw-r--r--   0        0        0     1233 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_chain_migration_election.yaml
--rw-r--r--   0        0        0     1086 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_compose.yaml
--rw-r--r--   0        0        0      950 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_create.yaml
--rw-r--r--   0        0        0     1088 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_decompose.yaml
--rw-r--r--   0        0        0      933 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_transfer.yaml
--rw-r--r--   0        0        0     1780 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_validator_election.yaml
--rw-r--r--   0        0        0      843 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_vote.yaml
--rw-r--r--   0        0        0     1475 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/script.py
--rw-r--r--   0        0        0    33738 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/transaction.py
--rw-r--r--   0        0        0     2645 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/transaction_link.py
--rw-r--r--   0        0        0      332 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/transaction_mode_types.py
--rw-r--r--   0        0        0     7709 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/utils.py
--rw-r--r--   0        0        0        0 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/types/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/types/assets/__init__.py
--rw-r--r--   0        0        0     2865 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/types/assets/compose.py
--rw-r--r--   0        0        0     3280 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/types/assets/create.py
--rw-r--r--   0        0        0     3189 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/types/assets/decompose.py
--rw-r--r--   0        0        0     3867 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/types/assets/transfer.py
--rw-r--r--   0        0        0        0 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/types/elections/__init__.py
--rw-r--r--   0        0        0      529 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/types/elections/chain_migration_election.py
--rw-r--r--   0        0        0     2817 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/types/elections/election.py
--rw-r--r--   0        0        0      792 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/types/elections/validator_election.py
--rw-r--r--   0        0        0     1485 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/types/elections/validator_utils.py
--rw-r--r--   0        0        0     1410 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/types/elections/vote.py
--rw-r--r--   0        0        0      906 1970-01-01 00:00:00.000000 planetmint_transactions-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-14 07:11:13.907196 planetmint_transactions-0.8.2/LICENSE
+-rw-r--r--   0        0        0       73 2023-06-14 07:11:13.907196 planetmint_transactions-0.8.2/README.md
+-rw-r--r--   0        0        0      693 2023-06-14 07:11:13.907196 planetmint_transactions-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0      953 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/__init__.py
+-rw-r--r--   0        0        0     1932 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/crypto.py
+-rw-r--r--   0        0        0     3427 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/exceptions.py
+-rw-r--r--   0        0        0     5029 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/input.py
+-rw-r--r--   0        0        0     1323 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/memoize.py
+-rw-r--r--   0        0        0     8319 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/output.py
+-rw-r--r--   0        0        0     2606 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/schema/README.md
+-rw-r--r--   0        0        0     5231 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/schema/__init__.py
+-rw-r--r--   0        0        0     3841 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/schema/v1.0/transaction.yaml
+-rw-r--r--   0        0        0      787 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/schema/v1.0/transaction_create.yaml
+-rw-r--r--   0        0        0      778 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/schema/v1.0/transaction_transfer.yaml
+-rw-r--r--   0        0        0     5070 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/schema/v2.0/transaction.yaml
+-rw-r--r--   0        0        0     1127 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/schema/v2.0/transaction_chain_migration_election.yaml
+-rw-r--r--   0        0        0      742 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/schema/v2.0/transaction_create.yaml
+-rw-r--r--   0        0        0      778 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/schema/v2.0/transaction_transfer.yaml
+-rw-r--r--   0        0        0     1674 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/schema/v2.0/transaction_validator_election.yaml
+-rw-r--r--   0        0        0      843 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/schema/v2.0/transaction_vote.yaml
+-rw-r--r--   0        0        0     4363 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/schema/v3.0/transaction.yaml
+-rw-r--r--   0        0        0     1233 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/schema/v3.0/transaction_chain_migration_election.yaml
+-rw-r--r--   0        0        0     1086 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/schema/v3.0/transaction_compose.yaml
+-rw-r--r--   0        0        0      950 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/schema/v3.0/transaction_create.yaml
+-rw-r--r--   0        0        0     1088 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/schema/v3.0/transaction_decompose.yaml
+-rw-r--r--   0        0        0      933 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/schema/v3.0/transaction_transfer.yaml
+-rw-r--r--   0        0        0     1780 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/schema/v3.0/transaction_validator_election.yaml
+-rw-r--r--   0        0        0      843 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/schema/v3.0/transaction_vote.yaml
+-rw-r--r--   0        0        0     1475 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/script.py
+-rw-r--r--   0        0        0    33738 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/transaction.py
+-rw-r--r--   0        0        0     2645 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/transaction_link.py
+-rw-r--r--   0        0        0      332 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/transaction_mode_types.py
+-rw-r--r--   0        0        0     7709 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/common/utils.py
+-rw-r--r--   0        0        0        0 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/types/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/types/assets/__init__.py
+-rw-r--r--   0        0        0     2865 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/types/assets/compose.py
+-rw-r--r--   0        0        0     3280 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/types/assets/create.py
+-rw-r--r--   0        0        0     3189 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/types/assets/decompose.py
+-rw-r--r--   0        0        0     3867 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/types/assets/transfer.py
+-rw-r--r--   0        0        0        0 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/types/elections/__init__.py
+-rw-r--r--   0        0        0      529 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/types/elections/chain_migration_election.py
+-rw-r--r--   0        0        0     2817 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/types/elections/election.py
+-rw-r--r--   0        0        0      792 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/types/elections/validator_election.py
+-rw-r--r--   0        0        0     1485 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/types/elections/validator_utils.py
+-rw-r--r--   0        0        0     1410 2023-06-14 07:11:13.911196 planetmint_transactions-0.8.2/transactions/types/elections/vote.py
+-rw-r--r--   0        0        0      906 1970-01-01 00:00:00.000000 planetmint_transactions-0.8.2/PKG-INFO
```

### Comparing `planetmint_transactions-0.8.1/LICENSE` & `planetmint_transactions-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/pyproject.toml` & `planetmint_transactions-0.8.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "planetmint-transactions"
-version = "0.8.1"
+version = "0.8.2"
 description = "Python implementation of the planetmint transactions spec"
 authors = ["Lorenz Herzberger <lorenzherzberger@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "transactions" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-planetmint-cryptoconditions = "^1.2.0"
+planetmint-cryptoconditions = "^1.2.2"
 base58 = "^2.1.1"
 planetmint-py-cid = "^0.4.2"
 planetmint-ipld = "^0.0.3"
 python-rapidjson = "^1.8"
 jsonschema = "^4.16.0"
 PyYAML = "^6.0"
 zenroom = "^2.20.4"
```

### Comparing `planetmint_transactions-0.8.1/transactions/__init__.py` & `planetmint_transactions-0.8.2/transactions/__init__.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/crypto.py` & `planetmint_transactions-0.8.2/transactions/common/crypto.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/exceptions.py` & `planetmint_transactions-0.8.2/transactions/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/input.py` & `planetmint_transactions-0.8.2/transactions/common/input.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/memoize.py` & `planetmint_transactions-0.8.2/transactions/common/memoize.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/output.py` & `planetmint_transactions-0.8.2/transactions/common/output.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/schema/README.md` & `planetmint_transactions-0.8.2/transactions/common/schema/README.md`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/schema/__init__.py` & `planetmint_transactions-0.8.2/transactions/common/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/schema/v1.0/transaction.yaml` & `planetmint_transactions-0.8.2/transactions/common/schema/v1.0/transaction.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/schema/v1.0/transaction_create.yaml` & `planetmint_transactions-0.8.2/transactions/common/schema/v1.0/transaction_create.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/schema/v1.0/transaction_transfer.yaml` & `planetmint_transactions-0.8.2/transactions/common/schema/v1.0/transaction_transfer.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/schema/v2.0/transaction.yaml` & `planetmint_transactions-0.8.2/transactions/common/schema/v2.0/transaction.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/schema/v2.0/transaction_chain_migration_election.yaml` & `planetmint_transactions-0.8.2/transactions/common/schema/v2.0/transaction_chain_migration_election.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/schema/v2.0/transaction_create.yaml` & `planetmint_transactions-0.8.2/transactions/common/schema/v2.0/transaction_create.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/schema/v2.0/transaction_transfer.yaml` & `planetmint_transactions-0.8.2/transactions/common/schema/v2.0/transaction_transfer.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/schema/v2.0/transaction_validator_election.yaml` & `planetmint_transactions-0.8.2/transactions/common/schema/v2.0/transaction_validator_election.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/schema/v2.0/transaction_vote.yaml` & `planetmint_transactions-0.8.2/transactions/common/schema/v2.0/transaction_vote.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction.yaml` & `planetmint_transactions-0.8.2/transactions/common/schema/v3.0/transaction.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_chain_migration_election.yaml` & `planetmint_transactions-0.8.2/transactions/common/schema/v3.0/transaction_chain_migration_election.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_compose.yaml` & `planetmint_transactions-0.8.2/transactions/common/schema/v3.0/transaction_compose.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_create.yaml` & `planetmint_transactions-0.8.2/transactions/common/schema/v3.0/transaction_create.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_decompose.yaml` & `planetmint_transactions-0.8.2/transactions/common/schema/v3.0/transaction_decompose.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_transfer.yaml` & `planetmint_transactions-0.8.2/transactions/common/schema/v3.0/transaction_transfer.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_validator_election.yaml` & `planetmint_transactions-0.8.2/transactions/common/schema/v3.0/transaction_validator_election.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_vote.yaml` & `planetmint_transactions-0.8.2/transactions/common/schema/v3.0/transaction_vote.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/script.py` & `planetmint_transactions-0.8.2/transactions/common/script.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/transaction.py` & `planetmint_transactions-0.8.2/transactions/common/transaction.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/transaction_link.py` & `planetmint_transactions-0.8.2/transactions/common/transaction_link.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/common/utils.py` & `planetmint_transactions-0.8.2/transactions/common/utils.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/types/assets/compose.py` & `planetmint_transactions-0.8.2/transactions/types/assets/compose.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/types/assets/create.py` & `planetmint_transactions-0.8.2/transactions/types/assets/create.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/types/assets/decompose.py` & `planetmint_transactions-0.8.2/transactions/types/assets/decompose.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/types/assets/transfer.py` & `planetmint_transactions-0.8.2/transactions/types/assets/transfer.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/types/elections/chain_migration_election.py` & `planetmint_transactions-0.8.2/transactions/types/elections/chain_migration_election.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/types/elections/election.py` & `planetmint_transactions-0.8.2/transactions/types/elections/election.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/types/elections/validator_election.py` & `planetmint_transactions-0.8.2/transactions/types/elections/validator_election.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/types/elections/validator_utils.py` & `planetmint_transactions-0.8.2/transactions/types/elections/validator_utils.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/transactions/types/elections/vote.py` & `planetmint_transactions-0.8.2/transactions/types/elections/vote.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.1/PKG-INFO` & `planetmint_transactions-0.8.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: planetmint-transactions
-Version: 0.8.1
+Version: 0.8.2
 Summary: Python implementation of the planetmint transactions spec
 Author: Lorenz Herzberger
 Author-email: lorenzherzberger@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: base58 (>=2.1.1,<3.0.0)
 Requires-Dist: jsonschema (>=4.16.0,<5.0.0)
-Requires-Dist: planetmint-cryptoconditions (>=1.2.0,<2.0.0)
+Requires-Dist: planetmint-cryptoconditions (>=1.2.2,<2.0.0)
 Requires-Dist: planetmint-ipld (>=0.0.3,<0.0.4)
 Requires-Dist: planetmint-py-cid (>=0.4.2,<0.5.0)
 Requires-Dist: python-rapidjson (>=1.8,<2.0)
 Requires-Dist: zenroom (>=2.20.4,<3.0.0)
 Description-Content-Type: text/markdown
 
 # transactions
```

