# Comparing `tmp/collective.linguatags-2.0.tar.gz` & `tmp/collective.linguatags-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.linguatags-2.0.tar", last modified: Wed Nov 17 00:49:41 2021, max compression
+gzip compressed data, was "collective.linguatags-2.0.1.tar", last modified: Wed Jun 14 07:52:45 2023, max compression
```

## Comparing `collective.linguatags-2.0.tar` & `collective.linguatags-2.0.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2021-11-17 00:49:41.752679 collective.linguatags-2.0/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      487 2021-11-17 00:49:40.000000 collective.linguatags-2.0/CHANGES.rst
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       98 2021-11-17 00:49:40.000000 collective.linguatags-2.0/CONTRIBUTORS.rst
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      111 2021-11-17 00:49:40.000000 collective.linguatags-2.0/MANIFEST.in
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     4054 2021-11-17 00:49:41.752679 collective.linguatags-2.0/PKG-INFO
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1881 2021-11-17 00:49:40.000000 collective.linguatags-2.0/README.rst
--rwxrwxr-x   0 jensens   (1000) jensens   (1000)      212 2021-11-17 00:49:40.000000 collective.linguatags-2.0/bootstrap.sh
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2021-11-17 00:49:41.744679 collective.linguatags-2.0/docs/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)    18092 2021-11-17 00:49:40.000000 collective.linguatags-2.0/docs/LICENSE.GPL
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      665 2021-11-17 00:49:40.000000 collective.linguatags-2.0/docs/LICENSE.rst
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       84 2021-11-17 00:49:40.000000 collective.linguatags-2.0/docs/index.rst
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      342 2021-11-17 00:49:41.752679 collective.linguatags-2.0/setup.cfg
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1702 2021-11-17 00:49:40.000000 collective.linguatags-2.0/setup.py
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2021-11-17 00:49:41.744679 collective.linguatags-2.0/src/
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2021-11-17 00:49:41.744679 collective.linguatags-2.0/src/collective/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       56 2021-11-17 00:49:40.000000 collective.linguatags-2.0/src/collective/__init__.py
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2021-11-17 00:49:41.748679 collective.linguatags-2.0/src/collective/linguatags/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      115 2021-11-17 00:49:40.000000 collective.linguatags-2.0/src/collective/linguatags/__init__.py
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2021-11-17 00:49:41.752679 collective.linguatags-2.0/src/collective/linguatags/browser/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)        0 2021-11-17 00:49:40.000000 collective.linguatags-2.0/src/collective/linguatags/browser/__init__.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      829 2021-11-17 00:49:40.000000 collective.linguatags-2.0/src/collective/linguatags/browser/configure.zcml
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1778 2021-11-17 00:49:40.000000 collective.linguatags-2.0/src/collective/linguatags/browser/controlpanel.pt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     2237 2021-11-17 00:49:40.000000 collective.linguatags-2.0/src/collective/linguatags/browser/controlpanel.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      794 2021-11-17 00:49:40.000000 collective.linguatags-2.0/src/collective/linguatags/browser/keywords.pt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      290 2021-11-17 00:49:40.000000 collective.linguatags-2.0/src/collective/linguatags/browser/keywords.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1164 2021-11-17 00:49:40.000000 collective.linguatags-2.0/src/collective/linguatags/configure.zcml
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      246 2021-11-17 00:49:40.000000 collective.linguatags-2.0/src/collective/linguatags/interfaces.py
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2021-11-17 00:49:41.752679 collective.linguatags-2.0/src/collective/linguatags/locales/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)        0 2021-11-17 00:49:40.000000 collective.linguatags-2.0/src/collective/linguatags/locales/collective.linguatags.pot
--rwxrwxr-x   0 jensens   (1000) jensens   (1000)      500 2021-11-17 00:49:40.000000 collective.linguatags-2.0/src/collective/linguatags/locales/update.sh
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2021-11-17 00:49:41.744679 collective.linguatags-2.0/src/collective/linguatags/profiles/
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2021-11-17 00:49:41.752679 collective.linguatags-2.0/src/collective/linguatags/profiles/default/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      189 2021-11-17 00:49:40.000000 collective.linguatags-2.0/src/collective/linguatags/profiles/default/browserlayer.xml
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      521 2021-11-17 00:49:40.000000 collective.linguatags-2.0/src/collective/linguatags/profiles/default/controlpanel.xml
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      123 2021-11-17 00:49:40.000000 collective.linguatags-2.0/src/collective/linguatags/profiles/default/metadata.xml
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2021-11-17 00:49:41.752679 collective.linguatags-2.0/src/collective/linguatags/profiles/uninstall/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      131 2021-11-17 00:49:40.000000 collective.linguatags-2.0/src/collective/linguatags/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      565 2021-11-17 00:49:40.000000 collective.linguatags-2.0/src/collective/linguatags/setuphandlers.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      382 2021-11-17 00:49:40.000000 collective.linguatags-2.0/src/collective/linguatags/storage.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      948 2021-11-17 00:49:40.000000 collective.linguatags-2.0/src/collective/linguatags/testing.py
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2021-11-17 00:49:41.752679 collective.linguatags-2.0/src/collective/linguatags/tests/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)        0 2021-11-17 00:49:40.000000 collective.linguatags-2.0/src/collective/linguatags/tests/__init__.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1799 2021-11-17 00:49:40.000000 collective.linguatags-2.0/src/collective/linguatags/tests/test_setup.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     2322 2021-11-17 00:49:40.000000 collective.linguatags-2.0/src/collective/linguatags/tests/test_translationdomain.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1275 2021-11-17 00:49:40.000000 collective.linguatags-2.0/src/collective/linguatags/translationdomain.py
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2021-11-17 00:49:41.748679 collective.linguatags-2.0/src/collective.linguatags.egg-info/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     4054 2021-11-17 00:49:41.000000 collective.linguatags-2.0/src/collective.linguatags.egg-info/PKG-INFO
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1621 2021-11-17 00:49:41.000000 collective.linguatags-2.0/src/collective.linguatags.egg-info/SOURCES.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)        1 2021-11-17 00:49:41.000000 collective.linguatags-2.0/src/collective.linguatags.egg-info/dependency_links.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       53 2021-11-17 00:49:41.000000 collective.linguatags-2.0/src/collective.linguatags.egg-info/entry_points.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       11 2021-11-17 00:49:41.000000 collective.linguatags-2.0/src/collective.linguatags.egg-info/namespace_packages.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)        1 2021-11-17 00:49:41.000000 collective.linguatags-2.0/src/collective.linguatags.egg-info/not-zip-safe
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      101 2021-11-17 00:49:41.000000 collective.linguatags-2.0/src/collective.linguatags.egg-info/requires.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       11 2021-11-17 00:49:41.000000 collective.linguatags-2.0/src/collective.linguatags.egg-info/top_level.txt
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 07:52:45.093560 collective.linguatags-2.0.1/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      655 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/CHANGES.rst
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       98 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/CONTRIBUTORS.rst
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      111 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/MANIFEST.in
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     4280 2023-06-14 07:52:45.093560 collective.linguatags-2.0.1/PKG-INFO
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1881 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/README.rst
+-rwxrwxr-x   0 jensens   (1000) jensens   (1000)      212 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/bootstrap.sh
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 07:52:45.089560 collective.linguatags-2.0.1/docs/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)    18092 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/docs/LICENSE.GPL
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      665 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/docs/LICENSE.rst
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       84 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/docs/index.rst
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      342 2023-06-14 07:52:45.093560 collective.linguatags-2.0.1/setup.cfg
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1735 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/setup.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 07:52:45.089560 collective.linguatags-2.0.1/src/
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 07:52:45.089560 collective.linguatags-2.0.1/src/collective/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       56 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/src/collective/__init__.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 07:52:45.089560 collective.linguatags-2.0.1/src/collective/linguatags/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      115 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/src/collective/linguatags/__init__.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 07:52:45.093560 collective.linguatags-2.0.1/src/collective/linguatags/browser/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)        0 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/src/collective/linguatags/browser/__init__.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      829 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/src/collective/linguatags/browser/configure.zcml
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1778 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/src/collective/linguatags/browser/controlpanel.pt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     2237 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/src/collective/linguatags/browser/controlpanel.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      794 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/src/collective/linguatags/browser/keywords.pt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      290 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/src/collective/linguatags/browser/keywords.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1160 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/src/collective/linguatags/configure.zcml
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      246 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/src/collective/linguatags/interfaces.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 07:52:45.093560 collective.linguatags-2.0.1/src/collective/linguatags/locales/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)        0 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/src/collective/linguatags/locales/collective.linguatags.pot
+-rwxrwxr-x   0 jensens   (1000) jensens   (1000)      500 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/src/collective/linguatags/locales/update.sh
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 07:52:45.089560 collective.linguatags-2.0.1/src/collective/linguatags/profiles/
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 07:52:45.093560 collective.linguatags-2.0.1/src/collective/linguatags/profiles/default/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      189 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/src/collective/linguatags/profiles/default/browserlayer.xml
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      521 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/src/collective/linguatags/profiles/default/controlpanel.xml
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      123 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/src/collective/linguatags/profiles/default/metadata.xml
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 07:52:45.093560 collective.linguatags-2.0.1/src/collective/linguatags/profiles/uninstall/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      131 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/src/collective/linguatags/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      565 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/src/collective/linguatags/setuphandlers.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      382 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/src/collective/linguatags/storage.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      948 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/src/collective/linguatags/testing.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 07:52:45.093560 collective.linguatags-2.0.1/src/collective/linguatags/tests/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)        0 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/src/collective/linguatags/tests/__init__.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1799 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/src/collective/linguatags/tests/test_setup.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     2322 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/src/collective/linguatags/tests/test_translationdomain.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1275 2023-06-14 07:52:44.000000 collective.linguatags-2.0.1/src/collective/linguatags/translationdomain.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 07:52:45.089560 collective.linguatags-2.0.1/src/collective.linguatags.egg-info/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     4280 2023-06-14 07:52:45.000000 collective.linguatags-2.0.1/src/collective.linguatags.egg-info/PKG-INFO
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1621 2023-06-14 07:52:45.000000 collective.linguatags-2.0.1/src/collective.linguatags.egg-info/SOURCES.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)        1 2023-06-14 07:52:45.000000 collective.linguatags-2.0.1/src/collective.linguatags.egg-info/dependency_links.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       53 2023-06-14 07:52:45.000000 collective.linguatags-2.0.1/src/collective.linguatags.egg-info/entry_points.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       11 2023-06-14 07:52:45.000000 collective.linguatags-2.0.1/src/collective.linguatags.egg-info/namespace_packages.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)        1 2023-06-14 07:52:45.000000 collective.linguatags-2.0.1/src/collective.linguatags.egg-info/not-zip-safe
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      117 2023-06-14 07:52:45.000000 collective.linguatags-2.0.1/src/collective.linguatags.egg-info/requires.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       11 2023-06-14 07:52:45.000000 collective.linguatags-2.0.1/src/collective.linguatags.egg-info/top_level.txt
```

### Comparing `collective.linguatags-2.0/PKG-INFO` & `collective.linguatags-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.linguatags
-Version: 2.0
+Version: 2.0.1
 Summary: Multilingual Keywords for Plone
 Home-page: https://pypi.python.org/pypi/collective.linguatags
 Author: Jens W. Klein
 Author-email: jk@kleinundpartner.at
 License: GPL version 2
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
@@ -75,14 +75,21 @@
         - Kim Paulissen
         
         
         
         Changelog
         =========
         
+        2.0.1 (2023-06-14)
+        ------------------
+        
+        - Remove unneeded `autoinclude` from `configure.zcml` and prevent from random namesapce declaration error.
+          [jensens, gogobd]
+        
+        
         2.0 (2021-11-17)
         ----------------
         
         - Fixes for Plone 6 support with BS5 [jensens]
         - Drop Plone 5.2 support. [jensens]
         - Drop Python 2 support. [jensens]
         - Move CI to GitHub Actions. [jensens]
```

### Comparing `collective.linguatags-2.0/README.rst` & `collective.linguatags-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `collective.linguatags-2.0/docs/LICENSE.GPL` & `collective.linguatags-2.0.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.linguatags-2.0/docs/LICENSE.rst` & `collective.linguatags-2.0.1/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.linguatags-2.0/setup.py` & `collective.linguatags-2.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="collective.linguatags",
-    version="2.0",
+    version="2.0.1",
     description="Multilingual Keywords for Plone",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
@@ -46,14 +46,15 @@
         "setuptools",
     ],
     extras_require={
         "test": [
             "plone.app.testing",
             "plone.app.contenttypes[test]",
             "plone.app.robotframework",
+            "zope.testrunner",
         ]
     },
     entry_points="""
     [z3c.autoinclude.plugin]
     target = plone
     """,
 )
```

### Comparing `collective.linguatags-2.0/src/collective/linguatags/browser/configure.zcml` & `collective.linguatags-2.0.1/src/collective/linguatags/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.linguatags-2.0/src/collective/linguatags/browser/controlpanel.pt` & `collective.linguatags-2.0.1/src/collective/linguatags/browser/controlpanel.pt`

 * *Files identical despite different names*

### Comparing `collective.linguatags-2.0/src/collective/linguatags/browser/controlpanel.py` & `collective.linguatags-2.0.1/src/collective/linguatags/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `collective.linguatags-2.0/src/collective/linguatags/browser/keywords.pt` & `collective.linguatags-2.0.1/src/collective/linguatags/browser/keywords.pt`

 * *Files identical despite different names*

### Comparing `collective.linguatags-2.0/src/collective/linguatags/configure.zcml` & `collective.linguatags-2.0.1/src/collective/linguatags/configure.zcml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <configure
     i18n_domain="collective.linguatags"
     xmlns="http://namespaces.zope.org/zope"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
     xmlns:i18n="http://namespaces.zope.org/i18n">
   <i18n:registerTranslations directory="locales" />
-  <includeDependencies package="." />
+  <include package="plone.api" />
   <include package=".browser" />
   <genericsetup:registerProfile
       description="Installs the collective.linguatags add-on."
       directory="profiles/default"
       name="default"
       post_handler=".setuphandlers.post_install"
       provides="Products.GenericSetup.interfaces.EXTENSION"
```

### Comparing `collective.linguatags-2.0/src/collective/linguatags/profiles/default/controlpanel.xml` & `collective.linguatags-2.0.1/src/collective/linguatags/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `collective.linguatags-2.0/src/collective/linguatags/setuphandlers.py` & `collective.linguatags-2.0.1/src/collective/linguatags/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.linguatags-2.0/src/collective/linguatags/testing.py` & `collective.linguatags-2.0.1/src/collective/linguatags/testing.py`

 * *Files identical despite different names*

### Comparing `collective.linguatags-2.0/src/collective/linguatags/tests/test_setup.py` & `collective.linguatags-2.0.1/src/collective/linguatags/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.linguatags-2.0/src/collective/linguatags/tests/test_translationdomain.py` & `collective.linguatags-2.0.1/src/collective/linguatags/tests/test_translationdomain.py`

 * *Files identical despite different names*

### Comparing `collective.linguatags-2.0/src/collective/linguatags/translationdomain.py` & `collective.linguatags-2.0.1/src/collective/linguatags/translationdomain.py`

 * *Files identical despite different names*

### Comparing `collective.linguatags-2.0/src/collective.linguatags.egg-info/PKG-INFO` & `collective.linguatags-2.0.1/src/collective.linguatags.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.linguatags
-Version: 2.0
+Version: 2.0.1
 Summary: Multilingual Keywords for Plone
 Home-page: https://pypi.python.org/pypi/collective.linguatags
 Author: Jens W. Klein
 Author-email: jk@kleinundpartner.at
 License: GPL version 2
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
@@ -75,14 +75,21 @@
         - Kim Paulissen
         
         
         
         Changelog
         =========
         
+        2.0.1 (2023-06-14)
+        ------------------
+        
+        - Remove unneeded `autoinclude` from `configure.zcml` and prevent from random namesapce declaration error.
+          [jensens, gogobd]
+        
+        
         2.0 (2021-11-17)
         ----------------
         
         - Fixes for Plone 6 support with BS5 [jensens]
         - Drop Plone 5.2 support. [jensens]
         - Drop Python 2 support. [jensens]
         - Move CI to GitHub Actions. [jensens]
```

### Comparing `collective.linguatags-2.0/src/collective.linguatags.egg-info/SOURCES.txt` & `collective.linguatags-2.0.1/src/collective.linguatags.egg-info/SOURCES.txt`

 * *Files identical despite different names*

