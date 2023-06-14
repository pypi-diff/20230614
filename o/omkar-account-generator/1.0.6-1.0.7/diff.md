# Comparing `tmp/omkar_account_generator-1.0.6.tar.gz` & `tmp/omkar_account_generator-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omkar_account_generator-1.0.6.tar", last modified: Wed Jun 14 11:38:51 2023, max compression
+gzip compressed data, was "omkar_account_generator-1.0.7.tar", last modified: Wed Jun 14 11:50:01 2023, max compression
```

## Comparing `omkar_account_generator-1.0.6.tar` & `omkar_account_generator-1.0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 11:38:51.904478 omkar_account_generator-1.0.6/
--rw-rw-rw-   0        0        0     7239 2023-06-14 11:38:51.912495 omkar_account_generator-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4798 2023-06-14 11:37:35.943897 omkar_account_generator-1.0.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-14 11:38:51.904478 omkar_account_generator-1.0.6/omkar_account_generator/
--rw-rw-rw-   0        0        0       47 2023-06-14 09:44:32.855130 omkar_account_generator-1.0.6/omkar_account_generator/__init__.py
--rw-rw-rw-   0        0        0     3155 2023-06-14 11:38:44.723951 omkar_account_generator-1.0.6/omkar_account_generator/account_generator.py
--rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 omkar_account_generator-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     2264 2023-06-14 11:19:15.595574 omkar_account_generator-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:50:01.354973 omkar_account_generator-1.0.7/
+-rw-rw-rw-   0        0        0     7251 2023-06-14 11:50:01.354973 omkar_account_generator-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4810 2023-06-14 11:49:57.055366 omkar_account_generator-1.0.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-14 11:50:01.346960 omkar_account_generator-1.0.7/omkar_account_generator/
+-rw-rw-rw-   0        0        0       63 2023-06-14 11:47:39.919568 omkar_account_generator-1.0.7/omkar_account_generator/__init__.py
+-rw-rw-rw-   0        0        0     3155 2023-06-14 11:38:44.723951 omkar_account_generator-1.0.7/omkar_account_generator/account_generator.py
+-rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 omkar_account_generator-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     2264 2023-06-14 11:47:48.671595 omkar_account_generator-1.0.7/setup.py
```

### Comparing `omkar_account_generator-1.0.6/PKG-INFO` & `omkar_account_generator-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: omkar_account_generator
-Version: 1.0.6
+Version: 1.0.7
 Summary: Generate user accounts
 Home-page: UNKNOWN
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
 Description: Omkar Account Generator
         =======================
@@ -137,16 +137,16 @@
                    "dob": {
                        "date": "1961-05-29T07:35:50.196Z",
                        "age": 62
                    }
                }
            ]
         
-        If my code helped you in creating accounts, please take a moment to `star the repository <https://github.com/omkarcloud/omkar-account-generator>`__. Your act of starring will help developers in discovering our Repository and contribute towards helping fellow developers in their automation tasks. Dhanyawad 🙏! Vande Mataram!
-        -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+        If my code helped you in creating accounts, please take a moment to `star the repository <https://github.com/omkarcloud/omkar-account-generator>`__. Your act of starring will help developers in discovering our Repository and contribute towards helping fellow developers in their account creation tasks. Dhanyawad 🙏! Vande Mataram!
+        -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
         
 Keywords: account-generator,account-creator,accountgenerator,generator,user-generator,dummy-users,user-data,fake-user,python,random-user-generator,account
 Platform: UNKNOWN
 Classifier: Framework :: Scrapy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `omkar_account_generator-1.0.6/README.rst` & `omkar_account_generator-1.0.7/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -129,9 +129,9 @@
            "dob": {
                "date": "1961-05-29T07:35:50.196Z",
                "age": 62
            }
        }
    ]
 
-If my code helped you in creating accounts, please take a moment to `star the repository <https://github.com/omkarcloud/omkar-account-generator>`__. Your act of starring will help developers in discovering our Repository and contribute towards helping fellow developers in their automation tasks. Dhanyawad 🙏! Vande Mataram!
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+If my code helped you in creating accounts, please take a moment to `star the repository <https://github.com/omkarcloud/omkar-account-generator>`__. Your act of starring will help developers in discovering our Repository and contribute towards helping fellow developers in their account creation tasks. Dhanyawad 🙏! Vande Mataram!
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
```

### Comparing `omkar_account_generator-1.0.6/omkar_account_generator/account_generator.py` & `omkar_account_generator-1.0.7/omkar_account_generator/account_generator.py`

 * *Files identical despite different names*

### Comparing `omkar_account_generator-1.0.6/setup.py` & `omkar_account_generator-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     except:
       return None
     
             
 setup(
     name='omkar_account_generator',
     packages=['omkar_account_generator'],
-    version='1.0.6',
+    version='1.0.7',
     license='MIT',
     project_urls={
         "Documentation": "https://github.com/omkarcloud/omkar-account-generator",
         "Source": "https://github.com/omkarcloud/omkar-account-generator",
         "Tracker": "https://github.com/omkarcloud/omkar-account-generator/issues",
     },
```

