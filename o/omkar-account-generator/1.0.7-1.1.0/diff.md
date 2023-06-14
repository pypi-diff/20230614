# Comparing `tmp/omkar_account_generator-1.0.7.tar.gz` & `tmp/omkar_account_generator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omkar_account_generator-1.0.7.tar", last modified: Wed Jun 14 11:50:01 2023, max compression
+gzip compressed data, was "omkar_account_generator-1.1.0.tar", last modified: Wed Jun 14 12:10:19 2023, max compression
```

## Comparing `omkar_account_generator-1.0.7.tar` & `omkar_account_generator-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 11:50:01.354973 omkar_account_generator-1.0.7/
--rw-rw-rw-   0        0        0     7251 2023-06-14 11:50:01.354973 omkar_account_generator-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     4810 2023-06-14 11:49:57.055366 omkar_account_generator-1.0.7/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-14 11:50:01.346960 omkar_account_generator-1.0.7/omkar_account_generator/
--rw-rw-rw-   0        0        0       63 2023-06-14 11:47:39.919568 omkar_account_generator-1.0.7/omkar_account_generator/__init__.py
--rw-rw-rw-   0        0        0     3155 2023-06-14 11:38:44.723951 omkar_account_generator-1.0.7/omkar_account_generator/account_generator.py
--rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 omkar_account_generator-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2264 2023-06-14 11:47:48.671595 omkar_account_generator-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:10:19.642022 omkar_account_generator-1.1.0/
+-rw-rw-rw-   0        0        0     7282 2023-06-14 12:10:19.642022 omkar_account_generator-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4825 2023-06-14 12:08:16.367537 omkar_account_generator-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-14 12:10:19.642022 omkar_account_generator-1.1.0/omkar_account_generator/
+-rw-rw-rw-   0        0        0       63 2023-06-14 11:47:39.919568 omkar_account_generator-1.1.0/omkar_account_generator/__init__.py
+-rw-rw-rw-   0        0        0     3155 2023-06-14 11:38:44.723951 omkar_account_generator-1.1.0/omkar_account_generator/account_generator.py
+-rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 omkar_account_generator-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2264 2023-06-14 12:10:15.096740 omkar_account_generator-1.1.0/setup.py
```

### Comparing `omkar_account_generator-1.0.7/PKG-INFO` & `omkar_account_generator-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: omkar_account_generator
-Version: 1.0.7
+Version: 1.1.0
 Summary: Generate user accounts
 Home-page: UNKNOWN
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
 Description: Omkar Account Generator
         =======================
@@ -26,20 +26,22 @@
         Usage
         -----
         
         1. ``generate_account(gender, country)``
         
         Generates an account
         
-        **Parameters** - ``gender`` (optional): The gender of the user account
-        to generate. Value can be ``Gender.MEN``, ``Gender.WOMEN``,
-        ``Gender.BOTH``. Default’s to ``Gender.BOTH`` - ``country`` (optional):
-        The country of the user account to generate. It accepts a value from the
-        ``Country`` enum. The default value is ``None``, which means the country
-        can be any country.
+        **Arguments**
+        
+        -  ``gender`` (optional): The gender of the user account to generate.
+           Value can be ``Gender.MEN``, ``Gender.WOMEN``, ``Gender.BOTH``.
+           Default’s to ``Gender.BOTH``
+        -  ``country`` (optional): The country of the user account to generate.
+           It accepts a value from the ``Country`` enum. The default value is
+           ``None``, which means the country can be any country.
         
         **Example**
         
         .. code:: python
         
            from omkar_account_generator import AccountGenerator, Gender, Country
         
@@ -66,15 +68,15 @@
                }
            }
         
         2. ``generate_accounts(n, gender, country)``
         
         Generates multiple user accounts.
         
-        **Parameters**
+        **Arguments**
         
         -  ``n``: The number of user accounts to generate.
         -  ``gender`` (optional): The gender of the user account to generate.
            Value can be ``Gender.MEN``, ``Gender.WOMEN``, ``Gender.BOTH``.
            Default’s to ``Gender.BOTH``
         -  ``country`` (optional): The country of the user account to generate.
            It accepts a value from the ``Country`` enum. The default value is
```

### Comparing `omkar_account_generator-1.0.7/README.rst` & `omkar_account_generator-1.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,22 @@
 Usage
 -----
 
 1. ``generate_account(gender, country)``
 
 Generates an account
 
-**Parameters** - ``gender`` (optional): The gender of the user account
-to generate. Value can be ``Gender.MEN``, ``Gender.WOMEN``,
-``Gender.BOTH``. Default’s to ``Gender.BOTH`` - ``country`` (optional):
-The country of the user account to generate. It accepts a value from the
-``Country`` enum. The default value is ``None``, which means the country
-can be any country.
+**Arguments**
+
+-  ``gender`` (optional): The gender of the user account to generate.
+   Value can be ``Gender.MEN``, ``Gender.WOMEN``, ``Gender.BOTH``.
+   Default’s to ``Gender.BOTH``
+-  ``country`` (optional): The country of the user account to generate.
+   It accepts a value from the ``Country`` enum. The default value is
+   ``None``, which means the country can be any country.
 
 **Example**
 
 .. code:: python
 
    from omkar_account_generator import AccountGenerator, Gender, Country
 
@@ -58,15 +60,15 @@
        }
    }
 
 2. ``generate_accounts(n, gender, country)``
 
 Generates multiple user accounts.
 
-**Parameters**
+**Arguments**
 
 -  ``n``: The number of user accounts to generate.
 -  ``gender`` (optional): The gender of the user account to generate.
    Value can be ``Gender.MEN``, ``Gender.WOMEN``, ``Gender.BOTH``.
    Default’s to ``Gender.BOTH``
 -  ``country`` (optional): The country of the user account to generate.
    It accepts a value from the ``Country`` enum. The default value is
```

### Comparing `omkar_account_generator-1.0.7/omkar_account_generator/account_generator.py` & `omkar_account_generator-1.1.0/omkar_account_generator/account_generator.py`

 * *Files identical despite different names*

### Comparing `omkar_account_generator-1.0.7/setup.py` & `omkar_account_generator-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     except:
       return None
     
             
 setup(
     name='omkar_account_generator',
     packages=['omkar_account_generator'],
-    version='1.0.7',
+    version='1.1.0',
     license='MIT',
     project_urls={
         "Documentation": "https://github.com/omkarcloud/omkar-account-generator",
         "Source": "https://github.com/omkarcloud/omkar-account-generator",
         "Tracker": "https://github.com/omkarcloud/omkar-account-generator/issues",
     },
```

