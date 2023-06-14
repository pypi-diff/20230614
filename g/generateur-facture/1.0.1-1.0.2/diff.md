# Comparing `tmp/generateur_facture-1.0.1.tar.gz` & `tmp/generateur_facture-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generateur_facture-1.0.1.tar", last modified: Wed Jun 14 12:46:41 2023, max compression
+gzip compressed data, was "generateur_facture-1.0.2.tar", last modified: Wed Jun 14 12:55:36 2023, max compression
```

## Comparing `generateur_facture-1.0.1.tar` & `generateur_facture-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 12:46:41.269573 generateur_facture-1.0.1/
--rw-rw-rw-   0        0        0     2175 2023-06-14 12:04:19.000000 generateur_facture-1.0.1/CHANGES.rst
--rw-rw-rw-   0        0        0      139 2023-06-14 12:04:19.000000 generateur_facture-1.0.1/CONTRIBUTORS.rst
-drwxrwxrwx   0        0        0        0 2023-06-14 12:46:41.262055 generateur_facture-1.0.1/GenerateurFacture/
--rw-rw-rw-   0        0        0       92 2023-06-14 12:46:16.000000 generateur_facture-1.0.1/GenerateurFacture/__init__.py
--rw-rw-rw-   0        0        0    11486 2023-06-14 12:30:33.000000 generateur_facture-1.0.1/GenerateurFacture/api.py
--rw-rw-rw-   0        0        0     1497 2023-06-14 12:46:16.000000 generateur_facture-1.0.1/GenerateurFacture/conf.py
--rw-rw-rw-   0        0        0    10256 2023-06-14 12:43:18.000000 generateur_facture-1.0.1/GenerateurFacture/generator.py
--rw-rw-rw-   0        0        0    22401 2023-06-14 12:30:33.000000 generateur_facture-1.0.1/GenerateurFacture/pdf.py
--rw-rw-rw-   0        0        0     6769 2023-06-14 12:30:33.000000 generateur_facture-1.0.1/GenerateurFacture/pohoda.py
--rw-rw-rw-   0        0        0      156 2023-06-14 12:04:19.000000 generateur_facture-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5777 2023-06-14 12:46:41.269573 generateur_facture-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2953 2023-06-14 12:04:19.000000 generateur_facture-1.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-14 12:46:41.268558 generateur_facture-1.0.1/generateur_facture.egg-info/
--rw-rw-rw-   0        0        0     5777 2023-06-14 12:46:41.000000 generateur_facture-1.0.1/generateur_facture.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      444 2023-06-14 12:46:41.000000 generateur_facture-1.0.1/generateur_facture.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 12:46:41.000000 generateur_facture-1.0.1/generateur_facture.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-06-14 12:46:41.000000 generateur_facture-1.0.1/generateur_facture.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-14 12:46:41.000000 generateur_facture-1.0.1/generateur_facture.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      467 2023-06-14 12:46:41.271558 generateur_facture-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1819 2023-06-14 12:30:33.000000 generateur_facture-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:55:36.952094 generateur_facture-1.0.2/
+-rw-rw-rw-   0        0        0     2175 2023-06-14 12:04:19.000000 generateur_facture-1.0.2/CHANGES.rst
+-rw-rw-rw-   0        0        0      139 2023-06-14 12:04:19.000000 generateur_facture-1.0.2/CONTRIBUTORS.rst
+drwxrwxrwx   0        0        0        0 2023-06-14 12:55:36.944038 generateur_facture-1.0.2/GenerateurFacture/
+-rw-rw-rw-   0        0        0       92 2023-06-14 12:55:29.000000 generateur_facture-1.0.2/GenerateurFacture/__init__.py
+-rw-rw-rw-   0        0        0    11486 2023-06-14 12:30:33.000000 generateur_facture-1.0.2/GenerateurFacture/api.py
+-rw-rw-rw-   0        0        0     1503 2023-06-14 12:50:54.000000 generateur_facture-1.0.2/GenerateurFacture/conf.py
+-rw-rw-rw-   0        0        0    10256 2023-06-14 12:43:18.000000 generateur_facture-1.0.2/GenerateurFacture/generator.py
+-rw-rw-rw-   0        0        0    22401 2023-06-14 12:30:33.000000 generateur_facture-1.0.2/GenerateurFacture/pdf.py
+-rw-rw-rw-   0        0        0     6769 2023-06-14 12:30:33.000000 generateur_facture-1.0.2/GenerateurFacture/pohoda.py
+-rw-rw-rw-   0        0        0      156 2023-06-14 12:04:19.000000 generateur_facture-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5777 2023-06-14 12:55:36.952094 generateur_facture-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2953 2023-06-14 12:04:19.000000 generateur_facture-1.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-14 12:55:36.951095 generateur_facture-1.0.2/generateur_facture.egg-info/
+-rw-rw-rw-   0        0        0     5777 2023-06-14 12:55:36.000000 generateur_facture-1.0.2/generateur_facture.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      444 2023-06-14 12:55:36.000000 generateur_facture-1.0.2/generateur_facture.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 12:55:36.000000 generateur_facture-1.0.2/generateur_facture.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-06-14 12:55:36.000000 generateur_facture-1.0.2/generateur_facture.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-14 12:55:36.000000 generateur_facture-1.0.2/generateur_facture.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      467 2023-06-14 12:55:36.953095 generateur_facture-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1819 2023-06-14 12:30:33.000000 generateur_facture-1.0.2/setup.py
```

### Comparing `generateur_facture-1.0.1/CHANGES.rst` & `generateur_facture-1.0.2/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `generateur_facture-1.0.1/GenerateurFacture/api.py` & `generateur_facture-1.0.2/GenerateurFacture/api.py`

 * *Files identical despite different names*

### Comparing `generateur_facture-1.0.1/GenerateurFacture/conf.py` & `generateur_facture-1.0.2/GenerateurFacture/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -41,12 +41,12 @@
     if platform.platform() == "Linux":
         FONT_PATH = "/usr/share/fonts/truetype/dejavu/DejaVuSans.ttf"
         FONT_BOLD_PATH = "/usr/share/fonts/TTF/DejaVuSans-Bold.ttf"
     elif platform.platform() == "Darwin":
         FONT_PATH = "/Library/Fonts/DejaVuSans.ttf"
         FONT_BOLD_PATH = "/Library/Fonts/DejaVuSans-Bold.ttf"
     elif platform.platform() == "Windows":
-        FONT_PATH = "C:\Windows\Fonts\DejaVuSans.ttf"
-        FONT_BOLD_PATH = "C:\Windows\Fonts\DejaVuSans-Bold.ttf"
+        FONT_PATH = "C:\\Windows\\Fonts\\DejaVuSans.ttf"
+        FONT_BOLD_PATH = "C:\\Windows\\Fonts\\DejaVuSans-Bold.ttf"
 
 if not os.path.isfile(FONT_PATH):
     raise Exception("Fonts not found")
```

### Comparing `generateur_facture-1.0.1/GenerateurFacture/generator.py` & `generateur_facture-1.0.2/GenerateurFacture/generator.py`

 * *Files identical despite different names*

### Comparing `generateur_facture-1.0.1/GenerateurFacture/pdf.py` & `generateur_facture-1.0.2/GenerateurFacture/pdf.py`

 * *Files identical despite different names*

### Comparing `generateur_facture-1.0.1/GenerateurFacture/pohoda.py` & `generateur_facture-1.0.2/GenerateurFacture/pohoda.py`

 * *Files identical despite different names*

### Comparing `generateur_facture-1.0.1/PKG-INFO` & `generateur_facture-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generateur_facture
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library to generate PDF invoice.
 Home-page: https://github.com/creckx/InvoiceGenerator
 Author: Quentin DAVIN
 Author-email: quentin@rezonia.fr
 License: BSD
 Keywords: invoice invoices generator
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `generateur_facture-1.0.1/README.rst` & `generateur_facture-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `generateur_facture-1.0.1/generateur_facture.egg-info/PKG-INFO` & `generateur_facture-1.0.2/generateur_facture.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generateur-facture
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library to generate PDF invoice.
 Home-page: https://github.com/creckx/InvoiceGenerator
 Author: Quentin DAVIN
 Author-email: quentin@rezonia.fr
 License: BSD
 Keywords: invoice invoices generator
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `generateur_facture-1.0.1/setup.py` & `generateur_facture-1.0.2/setup.py`

 * *Files identical despite different names*

