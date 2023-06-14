# Comparing `tmp/mds_account_primanota-6.4.4.tar.gz` & `tmp/mds_account_primanota-6.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mds_account_primanota-6.4.4.tar", last modified: Wed Jun 14 14:57:37 2023, max compression
+gzip compressed data, was "mds_account_primanota-6.6.4.tar", last modified: Wed Jun 14 14:53:47 2023, max compression
```

## Comparing `mds_account_primanota-6.4.4.tar` & `mds_account_primanota-6.6.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-14 14:57:37.476582 mds_account_primanota-6.4.4/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1616 2023-06-14 14:57:37.476582 mds_account_primanota-6.4.4/PKG-INFO
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      376 2023-06-14 14:38:10.000000 mds_account_primanota-6.4.4/README.rst
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      405 2022-10-05 07:12:51.000000 mds_account_primanota-6.4.4/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     2669 2023-06-14 14:29:21.000000 mds_account_primanota-6.4.4/analytic.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1010 2022-10-05 07:12:51.000000 mds_account_primanota-6.4.4/analytic.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-14 14:57:37.476582 mds_account_primanota-6.4.4/locale/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     6793 2023-06-14 14:29:21.000000 mds_account_primanota-6.4.4/locale/de.po
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     6164 2023-06-14 14:29:21.000000 mds_account_primanota-6.4.4/locale/en.po
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-14 14:57:37.476582 mds_account_primanota-6.4.4/mds_account_primanota.egg-info/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1616 2023-06-14 14:57:37.000000 mds_account_primanota-6.4.4/mds_account_primanota.egg-info/PKG-INFO
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      728 2023-06-14 14:57:37.000000 mds_account_primanota-6.4.4/mds_account_primanota.egg-info/SOURCES.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-14 14:57:37.000000 mds_account_primanota-6.4.4/mds_account_primanota.egg-info/dependency_links.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       85 2023-06-14 14:57:37.000000 mds_account_primanota-6.4.4/mds_account_primanota.egg-info/entry_points.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-14 14:39:08.000000 mds_account_primanota-6.4.4/mds_account_primanota.egg-info/not-zip-safe
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       44 2023-06-14 14:57:37.000000 mds_account_primanota-6.4.4/mds_account_primanota.egg-info/requires.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-06-14 14:57:37.000000 mds_account_primanota-6.4.4/mds_account_primanota.egg-info/top_level.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      572 2022-10-05 07:12:51.000000 mds_account_primanota-6.4.4/menu.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    11740 2023-06-14 10:21:48.000000 mds_account_primanota-6.4.4/primanota.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2577 2022-10-05 07:12:51.000000 mds_account_primanota-6.4.4/primanota.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-06-14 14:57:37.476582 mds_account_primanota-6.4.4/setup.cfg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3568 2023-06-14 10:21:48.000000 mds_account_primanota-6.4.4/setup.py
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-14 14:57:37.476582 mds_account_primanota-6.4.4/tests/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      144 2023-06-14 14:33:13.000000 mds_account_primanota-6.4.4/tests/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    11660 2023-06-14 14:36:15.000000 mds_account_primanota-6.4.4/tests/test_primanota.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      133 2023-06-14 14:38:17.000000 mds_account_primanota-6.4.4/tryton.cfg
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2022-10-05 07:12:51.000000 mds_account_primanota-6.4.4/versiondep.txt
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-14 14:57:37.476582 mds_account_primanota-6.4.4/view/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      505 2022-10-05 07:12:51.000000 mds_account_primanota-6.4.4/view/analytic_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      377 2023-06-14 14:56:34.000000 mds_account_primanota-6.4.4/view/analytic_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      358 2022-10-05 07:12:51.000000 mds_account_primanota-6.4.4/view/analyticline_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      700 2022-10-05 07:12:51.000000 mds_account_primanota-6.4.4/view/primanota_context_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2449 2022-10-05 07:12:51.000000 mds_account_primanota-6.4.4/view/primanota_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1081 2022-11-24 11:33:46.000000 mds_account_primanota-6.4.4/view/primanota_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      316 2022-10-05 07:12:51.000000 mds_account_primanota-6.4.4/view/taxline_list.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-14 14:53:47.517928 mds_account_primanota-6.6.4/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1648 2023-06-14 14:53:47.517928 mds_account_primanota-6.6.4/PKG-INFO
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      339 2023-06-14 14:51:55.000000 mds_account_primanota-6.6.4/README.rst
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      405 2023-04-06 08:58:35.000000 mds_account_primanota-6.6.4/__init__.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     2669 2023-06-14 14:40:56.000000 mds_account_primanota-6.6.4/analytic.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1010 2023-04-06 08:58:35.000000 mds_account_primanota-6.6.4/analytic.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-14 14:53:47.509928 mds_account_primanota-6.6.4/locale/
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     6793 2023-06-14 14:40:56.000000 mds_account_primanota-6.6.4/locale/de.po
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     6164 2023-06-14 14:40:56.000000 mds_account_primanota-6.6.4/locale/en.po
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-14 14:53:47.517928 mds_account_primanota-6.6.4/mds_account_primanota.egg-info/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1648 2023-06-14 14:53:47.000000 mds_account_primanota-6.6.4/mds_account_primanota.egg-info/PKG-INFO
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      728 2023-06-14 14:53:47.000000 mds_account_primanota-6.6.4/mds_account_primanota.egg-info/SOURCES.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-14 14:53:47.000000 mds_account_primanota-6.6.4/mds_account_primanota.egg-info/dependency_links.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       85 2023-06-14 14:53:47.000000 mds_account_primanota-6.6.4/mds_account_primanota.egg-info/entry_points.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-14 14:53:47.000000 mds_account_primanota-6.6.4/mds_account_primanota.egg-info/not-zip-safe
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       44 2023-06-14 14:53:47.000000 mds_account_primanota-6.6.4/mds_account_primanota.egg-info/requires.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-06-14 14:53:47.000000 mds_account_primanota-6.6.4/mds_account_primanota.egg-info/top_level.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      572 2023-04-06 08:58:35.000000 mds_account_primanota-6.6.4/menu.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    11740 2023-04-06 09:15:03.000000 mds_account_primanota-6.6.4/primanota.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2577 2023-04-06 08:58:35.000000 mds_account_primanota-6.6.4/primanota.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-06-14 14:53:47.517928 mds_account_primanota-6.6.4/setup.cfg
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     3659 2023-06-14 14:40:43.000000 mds_account_primanota-6.6.4/setup.py
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-14 14:53:47.509928 mds_account_primanota-6.6.4/tests/
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      144 2023-06-14 14:41:09.000000 mds_account_primanota-6.6.4/tests/__init__.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    11660 2023-06-14 14:41:54.000000 mds_account_primanota-6.6.4/tests/test_primanota.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      133 2023-06-14 14:52:04.000000 mds_account_primanota-6.6.4/tryton.cfg
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-04-06 08:58:35.000000 mds_account_primanota-6.6.4/versiondep.txt
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-14 14:53:47.513928 mds_account_primanota-6.6.4/view/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      505 2023-04-06 08:58:35.000000 mds_account_primanota-6.6.4/view/analytic_form.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      377 2023-06-14 14:49:11.000000 mds_account_primanota-6.6.4/view/analytic_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      358 2023-04-06 08:58:35.000000 mds_account_primanota-6.6.4/view/analyticline_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      700 2023-04-06 08:58:35.000000 mds_account_primanota-6.6.4/view/primanota_context_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2449 2023-04-06 08:58:35.000000 mds_account_primanota-6.6.4/view/primanota_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1081 2023-04-06 08:58:35.000000 mds_account_primanota-6.6.4/view/primanota_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      316 2023-04-06 08:58:35.000000 mds_account_primanota-6.6.4/view/taxline_list.xml
```

### Comparing `mds_account_primanota-6.4.4/PKG-INFO` & `mds_account_primanota-6.6.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mds_account_primanota
-Version: 6.4.4
+Version: 6.6.4
 Summary: Tryton module to add a primanota-view.
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Description: mds-account-primanota
         =====================
@@ -13,30 +13,26 @@
         Install
         =======
         
         pip install mds-account-primanota
         
         Requires
         ========
-        - Tryton 6.4
+        - Tryton 6.6
         
         Changes
         =======
         
-        *6.4.4 - 14.06.2023*
+        *6.6.4 - 14.06.2023*
         
         - add: column 'analytic lines' - to search for existing/missing analytic-lines
         
-        *6.4.3 - 24.11.2022*
+        *6.6.3 - 06.04.2023*
         
-        - add: some columns now are optional
-        
-        *6.4.2 - 05.10.2022*
-        
-        - init
+        - compatibility to Tryton 6.6
         
 Keywords: tryton account primanota
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,7 +43,9 @@
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Natural Language :: German
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
```

### Comparing `mds_account_primanota-6.4.4/analytic.py` & `mds_account_primanota-6.6.4/analytic.py`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.4.4/analytic.xml` & `mds_account_primanota-6.6.4/analytic.xml`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.4.4/locale/de.po` & `mds_account_primanota-6.6.4/locale/de.po`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.4.4/locale/en.po` & `mds_account_primanota-6.6.4/locale/en.po`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.4.4/mds_account_primanota.egg-info/PKG-INFO` & `mds_account_primanota-6.6.4/mds_account_primanota.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mds-account-primanota
-Version: 6.4.4
+Version: 6.6.4
 Summary: Tryton module to add a primanota-view.
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Description: mds-account-primanota
         =====================
@@ -13,30 +13,26 @@
         Install
         =======
         
         pip install mds-account-primanota
         
         Requires
         ========
-        - Tryton 6.4
+        - Tryton 6.6
         
         Changes
         =======
         
-        *6.4.4 - 14.06.2023*
+        *6.6.4 - 14.06.2023*
         
         - add: column 'analytic lines' - to search for existing/missing analytic-lines
         
-        *6.4.3 - 24.11.2022*
+        *6.6.3 - 06.04.2023*
         
-        - add: some columns now are optional
-        
-        *6.4.2 - 05.10.2022*
-        
-        - init
+        - compatibility to Tryton 6.6
         
 Keywords: tryton account primanota
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,7 +43,9 @@
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Natural Language :: German
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
```

### Comparing `mds_account_primanota-6.4.4/mds_account_primanota.egg-info/SOURCES.txt` & `mds_account_primanota-6.6.4/mds_account_primanota.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.4.4/menu.xml` & `mds_account_primanota-6.6.4/menu.xml`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.4.4/primanota.py` & `mds_account_primanota-6.6.4/primanota.py`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.4.4/primanota.xml` & `mds_account_primanota-6.6.4/primanota.xml`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.4.4/setup.py` & `mds_account_primanota-6.6.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         l2 = i.strip().split(';')
         if len(l2) < 4:
             continue
         modversion[l2[0]] = {'min':l2[1], 'max':l2[2], 'prefix':l2[3]}
 
 # tryton-version
 major_version = 6
-minor_version = 4
+minor_version = 6
 
 requires = []
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res|webdav)(\W|$)', dep):
         if dep in modversion.keys():
             prefix = 'mds'
             if len(modversion[dep]['prefix']) > 0:
@@ -83,14 +83,16 @@
     'Topic :: Office/Business :: Financial :: Accounting',
     'Natural Language :: German',
     'Natural Language :: English',
     'Operating System :: OS Independent',
     'License :: OSI Approved :: GNU General Public License (GPL)',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
     ],
 
     keywords='tryton account primanota',
     package_dir={'trytond.modules.%s' % MODULE: '.'},
     packages=[
         'trytond.modules.%s' % MODULE,
         ],
```

### Comparing `mds_account_primanota-6.4.4/tests/test_primanota.py` & `mds_account_primanota-6.6.4/tests/test_primanota.py`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.4.4/view/primanota_context_form.xml` & `mds_account_primanota-6.6.4/view/primanota_context_form.xml`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.4.4/view/primanota_form.xml` & `mds_account_primanota-6.6.4/view/primanota_form.xml`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.4.4/view/primanota_list.xml` & `mds_account_primanota-6.6.4/view/primanota_list.xml`

 * *Files identical despite different names*

