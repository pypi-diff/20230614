# Comparing `tmp/mds_account_primanota-6.0.4.tar.gz` & `tmp/mds_account_primanota-6.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mds_account_primanota-6.0.4.tar", last modified: Wed Jun 14 14:26:25 2023, max compression
+gzip compressed data, was "mds_account_primanota-6.4.3.tar", last modified: Thu Nov 24 11:38:01 2022, max compression
```

## Comparing `mds_account_primanota-6.0.4.tar` & `mds_account_primanota-6.4.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-14 14:26:25.047360 mds_account_primanota-6.0.4/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1709 2023-06-14 14:26:25.047360 mds_account_primanota-6.0.4/PKG-INFO
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      429 2023-06-14 14:25:45.000000 mds_account_primanota-6.0.4/README.rst
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      405 2022-05-02 14:31:11.000000 mds_account_primanota-6.0.4/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     2669 2023-06-14 14:06:33.000000 mds_account_primanota-6.0.4/analytic.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1010 2022-05-02 14:30:48.000000 mds_account_primanota-6.0.4/analytic.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-14 14:26:25.039360 mds_account_primanota-6.0.4/locale/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     6793 2023-06-14 14:06:33.000000 mds_account_primanota-6.0.4/locale/de.po
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     6164 2023-06-14 14:06:33.000000 mds_account_primanota-6.0.4/locale/en.po
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-14 14:26:25.043360 mds_account_primanota-6.0.4/mds_account_primanota.egg-info/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1709 2023-06-14 14:26:24.000000 mds_account_primanota-6.0.4/mds_account_primanota.egg-info/PKG-INFO
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      728 2023-06-14 14:26:24.000000 mds_account_primanota-6.0.4/mds_account_primanota.egg-info/SOURCES.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-14 14:26:24.000000 mds_account_primanota-6.0.4/mds_account_primanota.egg-info/dependency_links.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       85 2023-06-14 14:26:24.000000 mds_account_primanota-6.0.4/mds_account_primanota.egg-info/entry_points.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-14 14:26:24.000000 mds_account_primanota-6.0.4/mds_account_primanota.egg-info/not-zip-safe
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       44 2023-06-14 14:26:24.000000 mds_account_primanota-6.0.4/mds_account_primanota.egg-info/requires.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-06-14 14:26:24.000000 mds_account_primanota-6.0.4/mds_account_primanota.egg-info/top_level.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      572 2022-05-02 08:05:24.000000 mds_account_primanota-6.0.4/menu.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    11740 2023-06-14 10:21:31.000000 mds_account_primanota-6.0.4/primanota.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     2577 2022-05-02 14:31:11.000000 mds_account_primanota-6.0.4/primanota.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-06-14 14:26:25.047360 mds_account_primanota-6.0.4/setup.cfg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3568 2023-06-14 10:21:31.000000 mds_account_primanota-6.0.4/setup.py
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-14 14:26:25.039360 mds_account_primanota-6.0.4/tests/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      409 2023-06-14 14:11:36.000000 mds_account_primanota-6.0.4/tests/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    11649 2023-06-14 14:21:49.000000 mds_account_primanota-6.0.4/tests/test_primanota.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      134 2023-06-14 14:25:53.000000 mds_account_primanota-6.0.4/tryton.cfg
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2022-05-02 08:05:24.000000 mds_account_primanota-6.0.4/versiondep.txt
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-14 14:26:25.043360 mds_account_primanota-6.0.4/view/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      505 2022-05-02 14:30:48.000000 mds_account_primanota-6.0.4/view/analytic_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      351 2023-06-14 14:06:33.000000 mds_account_primanota-6.0.4/view/analytic_list.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      358 2022-05-02 14:30:49.000000 mds_account_primanota-6.0.4/view/analyticline_list.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      700 2022-05-02 14:31:11.000000 mds_account_primanota-6.0.4/view/primanota_context_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     2449 2022-05-02 14:30:49.000000 mds_account_primanota-6.0.4/view/primanota_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      873 2023-06-14 10:21:31.000000 mds_account_primanota-6.0.4/view/primanota_list.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      316 2022-05-02 14:30:49.000000 mds_account_primanota-6.0.4/view/taxline_list.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2022-11-24 11:38:01.992449 mds_account_primanota-6.4.3/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1482 2022-11-24 11:38:01.992449 mds_account_primanota-6.4.3/PKG-INFO
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      274 2022-11-24 11:35:13.000000 mds_account_primanota-6.4.3/README.rst
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      405 2022-10-05 07:12:51.000000 mds_account_primanota-6.4.3/__init__.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      503 2022-10-05 07:12:51.000000 mds_account_primanota-6.4.3/analytic.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1010 2022-10-05 07:12:51.000000 mds_account_primanota-6.4.3/analytic.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2022-11-24 11:38:01.988449 mds_account_primanota-6.4.3/locale/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6524 2022-10-05 07:12:51.000000 mds_account_primanota-6.4.3/locale/de.po
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     5895 2022-10-05 07:12:51.000000 mds_account_primanota-6.4.3/locale/en.po
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2022-11-24 11:38:01.992449 mds_account_primanota-6.4.3/mds_account_primanota.egg-info/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1482 2022-11-24 11:38:01.000000 mds_account_primanota-6.4.3/mds_account_primanota.egg-info/PKG-INFO
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      728 2022-11-24 11:38:01.000000 mds_account_primanota-6.4.3/mds_account_primanota.egg-info/SOURCES.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2022-11-24 11:38:01.000000 mds_account_primanota-6.4.3/mds_account_primanota.egg-info/dependency_links.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       85 2022-11-24 11:38:01.000000 mds_account_primanota-6.4.3/mds_account_primanota.egg-info/entry_points.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2022-11-24 11:38:01.000000 mds_account_primanota-6.4.3/mds_account_primanota.egg-info/not-zip-safe
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       44 2022-11-24 11:38:01.000000 mds_account_primanota-6.4.3/mds_account_primanota.egg-info/requires.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2022-11-24 11:38:01.000000 mds_account_primanota-6.4.3/mds_account_primanota.egg-info/top_level.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      572 2022-10-05 07:12:51.000000 mds_account_primanota-6.4.3/menu.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    11740 2022-11-24 11:33:40.000000 mds_account_primanota-6.4.3/primanota.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2577 2022-10-05 07:12:51.000000 mds_account_primanota-6.4.3/primanota.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2022-11-24 11:38:01.992449 mds_account_primanota-6.4.3/setup.cfg
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     3568 2022-11-24 11:33:40.000000 mds_account_primanota-6.4.3/setup.py
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2022-11-24 11:38:01.992449 mds_account_primanota-6.4.3/tests/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      583 2022-10-05 07:12:51.000000 mds_account_primanota-6.4.3/tests/__init__.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     9077 2022-11-24 11:33:40.000000 mds_account_primanota-6.4.3/tests/test_primanota.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      133 2022-11-24 11:35:21.000000 mds_account_primanota-6.4.3/tryton.cfg
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2022-10-05 07:12:51.000000 mds_account_primanota-6.4.3/versiondep.txt
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2022-11-24 11:38:01.992449 mds_account_primanota-6.4.3/view/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      505 2022-10-05 07:12:51.000000 mds_account_primanota-6.4.3/view/analytic_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      308 2022-10-05 07:12:51.000000 mds_account_primanota-6.4.3/view/analytic_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      358 2022-10-05 07:12:51.000000 mds_account_primanota-6.4.3/view/analyticline_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      700 2022-10-05 07:12:51.000000 mds_account_primanota-6.4.3/view/primanota_context_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2449 2022-10-05 07:12:51.000000 mds_account_primanota-6.4.3/view/primanota_form.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     1081 2022-11-24 11:33:46.000000 mds_account_primanota-6.4.3/view/primanota_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      316 2022-10-05 07:12:51.000000 mds_account_primanota-6.4.3/view/taxline_list.xml
```

### Comparing `mds_account_primanota-6.0.4/PKG-INFO` & `mds_account_primanota-6.4.3/mds_account_primanota.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: mds_account_primanota
-Version: 6.0.4
+Name: mds-account-primanota
+Version: 6.4.3
 Summary: Tryton module to add a primanota-view.
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Description: mds-account-primanota
         =====================
@@ -13,36 +13,27 @@
         Install
         =======
         
         pip install mds-account-primanota
         
         Requires
         ========
-        - Tryton 6.0
+        - Tryton 6.4
         
         Changes
         =======
         
-        *6.0.4 - 14.06.2023*
+        *6.4.3 - 24.11.2022*
         
-        - add: column 'analytic lines' - to search for existing/missing analytic-lines
+        - add: some columns now are optional
         
-        *6.0.2 - 03.05.2022*
-        
-        - add: search in 'origin' and 'line_origin'
-        
-        *6.0.1 - 02.05.2022*
-        
-        - add: context search
-        
-        *6.0.0 - 01.05.2022*
+        *6.4.2 - 05.10.2022*
         
         - init
         
-        
 Keywords: tryton account primanota
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Customer Service
```

### Comparing `mds_account_primanota-6.0.4/analytic.xml` & `mds_account_primanota-6.4.3/analytic.xml`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.0.4/locale/de.po` & `mds_account_primanota-6.4.3/locale/de.po`

 * *Files 2% similar despite different names*

```diff
@@ -191,22 +191,14 @@
 msgid "The exchange rate of the second currency."
 msgstr "Der Wechselkurs der Zweitwährung."
 
 msgctxt "field:account_primanota.primanota,analytic_lines:"
 msgid "Analytic Lines"
 msgstr "Kostenstelle Positionen"
 
-msgctxt "field:account_primanota.primanota,has_analytic_lines:"
-msgid "Analytic Lines"
-msgstr "Kostenstellen"
-
-msgctxt "help:account_primanota.primanota,has_analytic_lines:"
-msgid "Account move line has analytic lines."
-msgstr "Buchungszeile hat Kostenstellenzeilen."
-
 
 #######################################
 # account_primanota.primanota.context #
 #######################################
 msgctxt "model:account_primanota.primanota.context,name:"
 msgid "Primanota Context"
 msgstr "Primanota Kontext"
```

### Comparing `mds_account_primanota-6.0.4/locale/en.po` & `mds_account_primanota-6.4.3/locale/en.po`

 * *Files 2% similar despite different names*

```diff
@@ -186,22 +186,14 @@
 msgid "The exchange rate of the second currency."
 msgstr "The exchange rate of the second currency."
 
 msgctxt "field:account_primanota.primanota,analytic_lines:"
 msgid "Analytic Lines"
 msgstr "Analytic Lines"
 
-msgctxt "field:account_primanota.primanota,has_analytic_lines:"
-msgid "Analytic Lines"
-msgstr "Analytic Lines"
-
-msgctxt "help:account_primanota.primanota,has_analytic_lines:"
-msgid "Account move line has analytic lines."
-msgstr "Account move line has analytic lines."
-
 msgctxt "model:account_primanota.primanota.context,name:"
 msgid "Primanota Context"
 msgstr "Primanota Context"
 
 msgctxt "field:account_primanota.primanota.context,company:"
 msgid "Company"
 msgstr "Company"
```

### Comparing `mds_account_primanota-6.0.4/mds_account_primanota.egg-info/PKG-INFO` & `mds_account_primanota-6.4.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: mds-account-primanota
-Version: 6.0.4
+Name: mds_account_primanota
+Version: 6.4.3
 Summary: Tryton module to add a primanota-view.
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Description: mds-account-primanota
         =====================
@@ -13,36 +13,27 @@
         Install
         =======
         
         pip install mds-account-primanota
         
         Requires
         ========
-        - Tryton 6.0
+        - Tryton 6.4
         
         Changes
         =======
         
-        *6.0.4 - 14.06.2023*
+        *6.4.3 - 24.11.2022*
         
-        - add: column 'analytic lines' - to search for existing/missing analytic-lines
+        - add: some columns now are optional
         
-        *6.0.2 - 03.05.2022*
-        
-        - add: search in 'origin' and 'line_origin'
-        
-        *6.0.1 - 02.05.2022*
-        
-        - add: context search
-        
-        *6.0.0 - 01.05.2022*
+        *6.4.2 - 05.10.2022*
         
         - init
         
-        
 Keywords: tryton account primanota
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Customer Service
```

### Comparing `mds_account_primanota-6.0.4/mds_account_primanota.egg-info/SOURCES.txt` & `mds_account_primanota-6.4.3/mds_account_primanota.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.0.4/menu.xml` & `mds_account_primanota-6.4.3/menu.xml`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.0.4/primanota.py` & `mds_account_primanota-6.4.3/primanota.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
     def on_change_with_currency(self, name=None):
         if self.account:
             return self.account.currency.id
 
     @fields.depends('account')
     def on_change_with_currency_digits(self, name=None):
         if self.account:
-            return self.account.currency_digits
+            return self.account.currency.digits
         else:
             return 2
 
     @fields.depends('second_currency')
     def on_change_with_second_currency_digits(self, name=None):
         if self.second_currency:
             return self.second_currency.digits
```

### Comparing `mds_account_primanota-6.0.4/primanota.xml` & `mds_account_primanota-6.4.3/primanota.xml`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.0.4/setup.py` & `mds_account_primanota-6.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         l2 = i.strip().split(';')
         if len(l2) < 4:
             continue
         modversion[l2[0]] = {'min':l2[1], 'max':l2[2], 'prefix':l2[3]}
 
 # tryton-version
 major_version = 6
-minor_version = 0
+minor_version = 4
 
 requires = []
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res|webdav)(\W|$)', dep):
         if dep in modversion.keys():
             prefix = 'mds'
             if len(modversion[dep]['prefix']) > 0:
```

### Comparing `mds_account_primanota-6.0.4/tests/test_primanota.py` & `mds_account_primanota-6.4.3/tests/test_primanota.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,92 +1,60 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
-from trytond.tests.test_tryton import (
-    ModuleTestCase, with_transaction, activate_module, drop_db)
+from trytond.tests.test_tryton import ModuleTestCase, with_transaction
 from trytond.pool import Pool
 from trytond.transaction import Transaction
+from trytond.exceptions import UserError
 from trytond.modules.company.tests import create_company, set_company
 from trytond.modules.account.tests import create_chart, get_fiscalyear
 from datetime import date
 from decimal import Decimal
 from unittest.mock import MagicMock
 
 
 class PMTestCase(ModuleTestCase):
     'Test pm module'
     module = 'account_primanota'
 
-    @classmethod
-    def setUpClass(cls):
-        drop_db()
-        activate_module([
-            'account', 'analytic_account', 'account_primanota'], 'en')
-
     def prep_fiscalyear(self, company1):
         """ prepare fiscal year, sequences...
         """
         pool = Pool()
         FiscalYear = pool.get('account.fiscalyear')
+        Sequence = pool.get('ir.sequence.strict')
 
         fisc_year = get_fiscalyear(company1, today=date(2020, 1, 15))
         fisc_year.save()
         FiscalYear.create_period([fisc_year])
 
-    def prep_analytic_accounts(self, company):
-        """ add analytic accounts
-        """
-        AnalyticAccount = Pool().get('analytic_account.account')
-
-        account_root, = AnalyticAccount.create([{
-            'type': 'root',
-            'name': 'mds',
-            'code': 'ROOT',
-            'company': company.id,
-            'parent': None,
-            'state': 'opened',
-            }])
-
-        account, = AnalyticAccount.create([{
-            'root': account_root.id,
-            'type': 'normal',
-            'name': 'Office',
-            'code': 'K001',
-            'company': company.id,
-            'parent': account_root.id,
-            'state': 'opened',
-            }])
-        return account
-
     @with_transaction()
     def test_account_move(self):
         """ create account move, check values
         """
         pool = Pool()
         AccountMove = pool.get('account.move')
         Journal = pool.get('account.journal')
         Period = pool.get('account.period')
+        TaxLine = pool.get('account.tax.line')
         Account = pool.get('account.account')
         Tax = pool.get('account.tax')
         PrimaNota = pool.get('account_primanota.primanota')
         IrDate = pool.get('ir.date')
 
         IrDate.today = MagicMock(return_value=date(2020, 5, 3))
 
         company1 = create_company('m-ds')
         with set_company(company1):
             with Transaction().set_context({'company': company1.id}):
-                create_chart(company=company1, tax=True)
+                chart1 = create_chart(company = company1, tax = True)
                 self.prep_fiscalyear(company1)
-                analytic = self.prep_analytic_accounts(company1)
 
                 account_lst = Account.search([
-                    ('name', 'in', [
-                        'Main Expense', 'Main Revenue',
-                        'Main Receivable'])
+                    ('name', 'in', ['Main Expense', 'Main Revenue', 'Main Receivable'])
                     ], order=[('name', 'ASC')])
                 self.assertEqual(len(account_lst), 3)
                 self.assertEqual(account_lst[0].rec_name, 'Main Expense')
                 self.assertEqual(account_lst[1].rec_name, 'Main Receivable')
                 self.assertEqual(account_lst[2].rec_name, 'Main Revenue')
                 account_lst[0].code = '001'
                 account_lst[0].save()
@@ -107,20 +75,14 @@
                     'period': Period.find(company1.id, date=date(2020, 5, 2)),
                     'description': 'Test 1',
                     'lines': [('create', [{
                         'debit': Decimal('10.0'),
                         'credit': Decimal('0.0'),
                         'account': account_lst[2].id,
                         'description': 'Line 1',
-                        'analytic_lines': [('create', [{
-                            'account': analytic.id,
-                            'date': date(2020, 5, 1),
-                            'debit': Decimal('10.0'),
-                            'credit': Decimal('0.0'),
-                            }])],
                         'tax_lines': [('create', [{
                             'amount': Decimal('10.0'),
                             'type': 'base',
                             'tax': tax_lst[0].id,
                             }])],
                         }, {
                         'debit': Decimal('0.0'),
@@ -149,85 +111,65 @@
                 self.assertEqual(pm_lst[0].description, 'Test 1')
                 self.assertEqual(pm_lst[0].line_description, 'Line 2')
                 self.assertEqual(pm_lst[0].origin.description, 'Test 1')
                 self.assertEqual(pm_lst[0].line_origin.description, 'Line 1')
                 self.assertEqual(pm_lst[0].state, 'posted')
                 self.assertEqual(pm_lst[0].debit, Decimal('0.0'))
                 self.assertEqual(pm_lst[0].credit, Decimal('10.0'))
-                self.assertEqual(
-                    pm_lst[0].account.rec_name,
-                    '002 - Main Receivable')
+                self.assertEqual(pm_lst[0].account.rec_name, '002 - Main Receivable')
                 self.assertEqual(pm_lst[0].account_code, '002')
                 self.assertEqual(pm_lst[0].party.rec_name, 'm-ds')
                 self.assertEqual(pm_lst[0].reconciliation, None)
                 self.assertEqual(len(pm_lst[0].reconciliations_delegated), 0)
                 self.assertEqual(len(pm_lst[0].tax_lines), 0)
                 self.assertEqual(pm_lst[0].amount_second_currency, None)
                 self.assertEqual(pm_lst[0].rate_second_currency, None)
                 self.assertEqual(pm_lst[0].second_currency, None)
                 self.assertEqual(pm_lst[0].currency.rec_name, 'usd')
                 self.assertEqual(pm_lst[0].currency_digits, 2)
                 self.assertEqual(pm_lst[0].second_currency_digits, 2)
-                self.assertEqual(
-                    pm_lst[0].rec_name,
-                    '1 [1] 05/01/2020 002 usd0.00/usd10.00')
-                self.assertEqual(pm_lst[0].has_analytic_lines, False)
-                self.assertEqual(len(pm_lst[0].analytic_lines), 0)
+                self.assertEqual(pm_lst[0].rec_name, '1 [1] 05/01/2020 002 usd0.00/usd10.00')
 
                 # 1
                 self.assertEqual(pm_lst[1].movenumber, '1')
                 self.assertEqual(pm_lst[1].post_number, '1')
                 self.assertEqual(pm_lst[1].period.rec_name, '2020-05')
                 self.assertEqual(pm_lst[1].journal.rec_name, 'Revenue')
                 self.assertEqual(pm_lst[1].date, date(2020, 5, 1))
                 self.assertEqual(pm_lst[1].description, 'Test 1')
                 self.assertEqual(pm_lst[1].line_description, 'Line 1')
                 self.assertEqual(pm_lst[1].origin.description, 'Test 1')
                 self.assertEqual(pm_lst[1].line_origin, None)
                 self.assertEqual(pm_lst[1].state, 'posted')
                 self.assertEqual(pm_lst[1].debit, Decimal('10.0'))
                 self.assertEqual(pm_lst[1].credit, Decimal('0.0'))
-                self.assertEqual(
-                    pm_lst[1].account.rec_name,
-                    '003 - Main Revenue')
+                self.assertEqual(pm_lst[1].account.rec_name, '003 - Main Revenue')
                 self.assertEqual(pm_lst[1].account_code, '003')
                 self.assertEqual(pm_lst[1].party, None)
                 self.assertEqual(pm_lst[1].reconciliation, None)
                 self.assertEqual(len(pm_lst[1].reconciliations_delegated), 0)
                 self.assertEqual(len(pm_lst[1].tax_lines), 1)
-                self.assertEqual(
-                    pm_lst[1].tax_lines[0].amount,
-                    Decimal('10.0'))
+                self.assertEqual(pm_lst[1].tax_lines[0].amount, Decimal('10.0'))
                 self.assertEqual(pm_lst[1].amount_second_currency, None)
                 self.assertEqual(pm_lst[1].rate_second_currency, None)
                 self.assertEqual(pm_lst[1].second_currency, None)
                 self.assertEqual(pm_lst[1].currency.rec_name, 'usd')
                 self.assertEqual(pm_lst[1].currency_digits, 2)
                 self.assertEqual(pm_lst[1].second_currency_digits, 2)
-                self.assertEqual(
-                    pm_lst[1].rec_name,
-                    '1 [1] 05/01/2020 003 usd10.00/usd0.00')
-                self.assertEqual(pm_lst[1].has_analytic_lines, True)
-                self.assertEqual(len(pm_lst[1].analytic_lines), 1)
-                self.assertEqual(
-                    pm_lst[1].analytic_lines[0].account.code,
-                    'K001')
+                self.assertEqual(pm_lst[1].rec_name, '1 [1] 05/01/2020 003 usd10.00/usd0.00')
 
                 # searcher
                 # search in party
-                self.assertEqual(PrimaNota.search_count([
-                    ('rec_name', '=', 'm-ds')]), 1)
+                self.assertEqual(PrimaNota.search_count([('rec_name', '=', 'm-ds')]), 1)
                 # post-number/move-number
-                self.assertEqual(PrimaNota.search_count([
-                    ('rec_name', '=', '1')]), 2)
+                self.assertEqual(PrimaNota.search_count([('rec_name', '=', '1')]), 2)
 
                 # line-origin
                 self.assertEqual(PrimaNota.search_count([
-                    ('line_origin.description', '=',
-                        'Line 1', 'account.move.line')
+                    ('line_origin.description', '=', 'Line 1', 'account.move.line')
                     ]), 1)
                 self.assertEqual(PrimaNota.search_count([
                     ('line_origin.description', '=', 'Line 1')
                     ]), 1)
                 self.assertEqual(PrimaNota.search_count([
                     ('line_origin', 'ilike', '%003%')
                     ]), 1)
@@ -239,27 +181,11 @@
                 self.assertEqual(PrimaNota.search_count([
                     ('origin.description', '=', 'Test 1')
                     ]), 2)
                 self.assertEqual(PrimaNota.search_count([
                     ('origin', 'ilike', '%1%')
                     ]), 2)
 
-                # analytic lines
-                self.assertEqual(PrimaNota.search_count([
-                    ('has_analytic_lines', '=', True)
-                    ]), 1)
-                self.assertEqual(PrimaNota.search_count([
-                    ('has_analytic_lines', '=', False)
-                    ]), 1)
-                a_line, = PrimaNota.search([
-                    ('has_analytic_lines', '=', True)])
-                self.assertEqual(len(a_line.analytic_lines), 1)
-                self.assertEqual(
-                    a_line.analytic_lines[0].account.code,
-                    'K001')
-                self.assertEqual(a_line.debit, Decimal('10.0'))
-                self.assertEqual(a_line.credit, Decimal('0.0'))
-
 # end PMTestCase
 
 
 del ModuleTestCase
```

### Comparing `mds_account_primanota-6.0.4/view/primanota_context_form.xml` & `mds_account_primanota-6.4.3/view/primanota_context_form.xml`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.0.4/view/primanota_form.xml` & `mds_account_primanota-6.4.3/view/primanota_form.xml`

 * *Files identical despite different names*

