# Comparing `tmp/paytring-1.0.0.tar.gz` & `tmp/paytring-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paytring-1.0.0.tar", last modified: Wed Jun 14 11:36:13 2023, max compression
+gzip compressed data, was "paytring-1.0.1.tar", last modified: Wed Jun 14 12:23:37 2023, max compression
```

## Comparing `paytring-1.0.0.tar` & `paytring-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 11:36:13.550381 paytring-1.0.0/
--rw-rw-rw-   0        0        0     1094 2023-06-14 07:35:06.000000 paytring-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     4733 2023-06-14 11:36:13.548373 paytring-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 11:36:13.505164 paytring-1.0.0/Paytring/
-drwxrwxrwx   0        0        0        0 2023-06-14 11:36:13.521766 paytring-1.0.0/Paytring/Paytring.egg-info/
--rw-rw-rw-   0        0        0     4733 2023-06-14 11:36:13.000000 paytring-1.0.0/Paytring/Paytring.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      714 2023-06-14 11:36:13.000000 paytring-1.0.0/Paytring/Paytring.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 11:36:13.000000 paytring-1.0.0/Paytring/Paytring.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-14 11:36:13.000000 paytring-1.0.0/Paytring/Paytring.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 11:36:13.000000 paytring-1.0.0/Paytring/Paytring.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-14 11:36:13.525197 paytring-1.0.0/Paytring/paytring/
--rw-rw-rw-   0        0        0      113 2023-06-02 11:09:08.000000 paytring-1.0.0/Paytring/paytring/__init__.py
--rw-rw-rw-   0        0        0     5066 2023-06-14 10:38:20.000000 paytring-1.0.0/Paytring/paytring/client.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:36:13.530133 paytring-1.0.0/Paytring/paytring/constant/
--rw-rw-rw-   0        0        0       52 2023-06-02 12:35:28.000000 paytring-1.0.0/Paytring/paytring/constant/__init__.py
--rw-rw-rw-   0        0        0      338 2023-06-14 10:54:48.000000 paytring-1.0.0/Paytring/paytring/constant/url.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:36:13.534355 paytring-1.0.0/Paytring/paytring/resources/
--rw-rw-rw-   0        0        0       69 2023-06-02 12:35:26.000000 paytring-1.0.0/Paytring/paytring/resources/__init__.py
--rw-rw-rw-   0        0        0      337 2023-06-14 10:54:33.000000 paytring-1.0.0/Paytring/paytring/resources/paytring.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:36:13.545375 paytring-1.0.0/Paytring/paytring/utility/
--rw-rw-rw-   0        0        0       66 2023-06-02 12:35:13.000000 paytring-1.0.0/Paytring/paytring/utility/__init__.py
--rw-rw-rw-   0        0        0     2638 2023-06-14 10:54:41.000000 paytring-1.0.0/Paytring/paytring/utility/utility.py
--rw-rw-rw-   0        0        0       42 2023-06-14 11:36:13.551373 paytring-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      846 2023-06-14 11:35:51.000000 paytring-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:23:37.441696 paytring-1.0.1/
+-rw-rw-rw-   0        0        0     1094 2023-06-14 07:35:06.000000 paytring-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     5098 2023-06-14 12:23:37.441696 paytring-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 12:23:37.397946 paytring-1.0.1/Paytring/
+drwxrwxrwx   0        0        0        0 2023-06-14 12:23:37.411419 paytring-1.0.1/Paytring/paytring/
+-rw-rw-rw-   0        0        0      113 2023-06-02 11:09:08.000000 paytring-1.0.1/Paytring/paytring/__init__.py
+-rw-rw-rw-   0        0        0     5066 2023-06-14 10:38:20.000000 paytring-1.0.1/Paytring/paytring/client.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:23:37.430262 paytring-1.0.1/Paytring/paytring/constant/
+-rw-rw-rw-   0        0        0       52 2023-06-02 12:35:28.000000 paytring-1.0.1/Paytring/paytring/constant/__init__.py
+-rw-rw-rw-   0        0        0      338 2023-06-14 10:54:48.000000 paytring-1.0.1/Paytring/paytring/constant/url.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:23:37.433202 paytring-1.0.1/Paytring/paytring/resources/
+-rw-rw-rw-   0        0        0       69 2023-06-02 12:35:26.000000 paytring-1.0.1/Paytring/paytring/resources/__init__.py
+-rw-rw-rw-   0        0        0      337 2023-06-14 10:54:33.000000 paytring-1.0.1/Paytring/paytring/resources/paytring.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:23:37.437939 paytring-1.0.1/Paytring/paytring/utility/
+-rw-rw-rw-   0        0        0       66 2023-06-02 12:35:13.000000 paytring-1.0.1/Paytring/paytring/utility/__init__.py
+-rw-rw-rw-   0        0        0     2638 2023-06-14 10:54:41.000000 paytring-1.0.1/Paytring/paytring/utility/utility.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:23:37.425086 paytring-1.0.1/Paytring/paytring.egg-info/
+-rw-rw-rw-   0        0        0     5098 2023-06-14 12:23:37.000000 paytring-1.0.1/Paytring/paytring.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-06-14 12:23:37.000000 paytring-1.0.1/Paytring/paytring.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 12:23:37.000000 paytring-1.0.1/Paytring/paytring.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-14 12:23:37.000000 paytring-1.0.1/Paytring/paytring.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-14 12:23:37.000000 paytring-1.0.1/Paytring/paytring.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 12:23:37.441696 paytring-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      846 2023-06-14 12:23:08.000000 paytring-1.0.1/setup.py
```

### Comparing `paytring-1.0.0/LICENSE.txt` & `paytring-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `paytring-1.0.0/PKG-INFO` & `paytring-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,85 +1,98 @@
 Metadata-Version: 2.1
 Name: paytring
-Version: 1.0.0
+Version: 1.0.1
 Summary: A SDK which helps to create, fetch or refund an order on Paytring
 Home-page: https://github.com/paytring/python-sdk
 Author: Paytirng
 Author-email: developer@paytring.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Paytring\Python
-## Set-Up key and secret in env
-    key = "{{Your key}}"
-    secret = "{{Your secret}}"
-
-### Usage
+---
+### Installation
+---
+The source code is currently hosted on GitHub at : https://github.com/paytring/python-sdk
 
-```python
-from paytring.client import Order
+Binary installers for the latest released version are available at the Python Package Index (PyPI)
 
 ```
+pip install paytring
+```
 
-#### Create Order
+## Set-Up Environment Variables
+---
+```
+import  os
+    os.environ['key'] = "your_key"
+    os.environ['secret'] = "your_secret"
+```
+## Usage
+---
+```
+from paytring.client import Order
+```
 
-```python
-Create instance of class Order
+#### Create Instance
+```
 order = Order()
 ```
 
-
+## Create Order
 ---
-Input Parameter
+##### Input Parameter
 
 - Receipt ID(string)
 - Amount(string)
 - Callback Url(string)
 - Customer Info ( Dictionary )
-- Currency
+- Currency (String : INR or USD)
+
+#### Methods
 
-Function
 ```python
 customer_info = {
     "cname": "test",
-    "email": "abc@gmail.com",
+    "email": "abc@gmail.com" -> it will be baseEncode256,
     "phone": "phone"
 }
 
 
 order.create(
     receipt_id,
     amount,
     callback_url,
     customer_info,
     currrency
 )
 ```
 
-##### Response
+#### Response
+
 ```
 {
 "status": true,
 "url": "www.makepayment.com",
 "order_id": "365769619161481216"
 }
 ```
 
-### Fetch Order
+## Fetch Order
 ---
-Input Parameter
+##### Input Paramete
 
 - Order ID(string)
 
-Function
+#### Methods
 ```
 
 order.fetch(
     order_id
 )
 ```
 
@@ -137,21 +150,21 @@
         },
         "additional_charges": 0,
         "mdr": ""
     }
 }
 ```
 
-### Fetch Order By Receipt-ID
+## Fetch Order By Receipt-ID
 ---
-Input Parameter
+#### Input Paramete
 
 - Receipt ID(string)
 
-Function
+#### Methods
 ```
 
 order.fetch_by_receipt_id(
     receipt_id
 )
 ```
 
@@ -209,39 +222,38 @@
         },
         "additional_charges": 0,
         "mdr": ""
     }
 }
 ```
 
-### Refund Order
+## Refund Order
 ---
-Input Parameter
+##### Input Paramete
 
 - Order ID(string)
 
-Function
+#### Methods
 ```
 
 order.refund(
     order_id
 )
 ```
 
 ### Response
 
----
-Success Response
+#### Success Response
 ```
 {
     "status": true,
     "message": "Refund has been initiated"
 }
 ```
-Error Response 
+#### Error Response 
 ```
 {
     "status": false,
     "error": {
         "message": "error message here",
         "code": 204
     }
```

### Comparing `paytring-1.0.0/Paytring/Paytring.egg-info/PKG-INFO` & `paytring-1.0.1/Paytring/paytring.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,85 +1,98 @@
 Metadata-Version: 2.1
 Name: paytring
-Version: 1.0.0
+Version: 1.0.1
 Summary: A SDK which helps to create, fetch or refund an order on Paytring
 Home-page: https://github.com/paytring/python-sdk
 Author: Paytirng
 Author-email: developer@paytring.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Paytring\Python
-## Set-Up key and secret in env
-    key = "{{Your key}}"
-    secret = "{{Your secret}}"
-
-### Usage
+---
+### Installation
+---
+The source code is currently hosted on GitHub at : https://github.com/paytring/python-sdk
 
-```python
-from paytring.client import Order
+Binary installers for the latest released version are available at the Python Package Index (PyPI)
 
 ```
+pip install paytring
+```
 
-#### Create Order
+## Set-Up Environment Variables
+---
+```
+import  os
+    os.environ['key'] = "your_key"
+    os.environ['secret'] = "your_secret"
+```
+## Usage
+---
+```
+from paytring.client import Order
+```
 
-```python
-Create instance of class Order
+#### Create Instance
+```
 order = Order()
 ```
 
-
+## Create Order
 ---
-Input Parameter
+##### Input Parameter
 
 - Receipt ID(string)
 - Amount(string)
 - Callback Url(string)
 - Customer Info ( Dictionary )
-- Currency
+- Currency (String : INR or USD)
+
+#### Methods
 
-Function
 ```python
 customer_info = {
     "cname": "test",
-    "email": "abc@gmail.com",
+    "email": "abc@gmail.com" -> it will be baseEncode256,
     "phone": "phone"
 }
 
 
 order.create(
     receipt_id,
     amount,
     callback_url,
     customer_info,
     currrency
 )
 ```
 
-##### Response
+#### Response
+
 ```
 {
 "status": true,
 "url": "www.makepayment.com",
 "order_id": "365769619161481216"
 }
 ```
 
-### Fetch Order
+## Fetch Order
 ---
-Input Parameter
+##### Input Paramete
 
 - Order ID(string)
 
-Function
+#### Methods
 ```
 
 order.fetch(
     order_id
 )
 ```
 
@@ -137,21 +150,21 @@
         },
         "additional_charges": 0,
         "mdr": ""
     }
 }
 ```
 
-### Fetch Order By Receipt-ID
+## Fetch Order By Receipt-ID
 ---
-Input Parameter
+#### Input Paramete
 
 - Receipt ID(string)
 
-Function
+#### Methods
 ```
 
 order.fetch_by_receipt_id(
     receipt_id
 )
 ```
 
@@ -209,39 +222,38 @@
         },
         "additional_charges": 0,
         "mdr": ""
     }
 }
 ```
 
-### Refund Order
+## Refund Order
 ---
-Input Parameter
+##### Input Paramete
 
 - Order ID(string)
 
-Function
+#### Methods
 ```
 
 order.refund(
     order_id
 )
 ```
 
 ### Response
 
----
-Success Response
+#### Success Response
 ```
 {
     "status": true,
     "message": "Refund has been initiated"
 }
 ```
-Error Response 
+#### Error Response 
 ```
 {
     "status": false,
     "error": {
         "message": "error message here",
         "code": 204
     }
```

### Comparing `paytring-1.0.0/Paytring/paytring/client.py` & `paytring-1.0.1/Paytring/paytring/client.py`

 * *Files identical despite different names*

### Comparing `paytring-1.0.0/Paytring/paytring/utility/utility.py` & `paytring-1.0.1/Paytring/paytring/utility/utility.py`

 * *Files identical despite different names*

### Comparing `paytring-1.0.0/setup.py` & `paytring-1.0.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("Paytring/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="paytring",
-    version="1.0.0",
+    version="1.0.1",
     description="A SDK which helps to create, fetch or refund an order on Paytring",
     package_dir={"": "Paytring"},
     packages=find_packages(where="Paytring"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/paytring/python-sdk",
     author="Paytirng",
```

