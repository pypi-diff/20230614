# Comparing `tmp/easyFermi-1.1.1.tar.gz` & `tmp/easyFermi-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyFermi-1.1.1.tar", last modified: Sat May 20 14:12:54 2023, max compression
+gzip compressed data, was "easyFermi-1.1.2.tar", last modified: Wed Jun 14 14:31:34 2023, max compression
```

## Comparing `easyFermi-1.1.1.tar` & `easyFermi-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2023-05-20 14:12:54.372224 easyFermi-1.1.1/
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)     1522 2022-01-31 12:02:33.000000 easyFermi-1.1.1/LICENSE.txt
--rw-rw-r--   0 raniere   (1000) raniere   (1000)     1702 2023-05-20 14:12:54.372224 easyFermi-1.1.1/PKG-INFO
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)     1172 2022-08-22 09:22:30.000000 easyFermi-1.1.1/README.md
-drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2023-05-20 14:12:54.372224 easyFermi-1.1.1/easyFermi/
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)       63 2022-02-01 13:52:31.000000 easyFermi-1.1.1/easyFermi/__init__.py
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)    92545 2023-05-20 14:10:42.000000 easyFermi-1.1.1/easyFermi/easyFermi.py
-drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2023-05-20 14:12:54.372224 easyFermi-1.1.1/easyFermi/images/
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)    40332 2022-01-15 16:04:30.000000 easyFermi-1.1.1/easyFermi/images/easyFermiIcon.png
--rw-rw-r--   0 raniere   (1000) raniere   (1000)   120905 2023-03-08 11:57:13.000000 easyFermi-1.1.1/easyFermi/images/easyFermiWindow.png
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)   121691 2021-11-23 14:18:26.000000 easyFermi-1.1.1/easyFermi/images/fermi.png
-drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2023-05-20 14:12:54.372224 easyFermi-1.1.1/easyFermi.egg-info/
--rw-rw-r--   0 raniere   (1000) raniere   (1000)     1702 2023-05-20 14:12:54.000000 easyFermi-1.1.1/easyFermi.egg-info/PKG-INFO
--rw-rw-r--   0 raniere   (1000) raniere   (1000)      338 2023-05-20 14:12:54.000000 easyFermi-1.1.1/easyFermi.egg-info/SOURCES.txt
--rw-rw-r--   0 raniere   (1000) raniere   (1000)        1 2023-05-20 14:12:54.000000 easyFermi-1.1.1/easyFermi.egg-info/dependency_links.txt
--rw-rw-r--   0 raniere   (1000) raniere   (1000)       14 2023-05-20 14:12:54.000000 easyFermi-1.1.1/easyFermi.egg-info/requires.txt
--rw-rw-r--   0 raniere   (1000) raniere   (1000)       10 2023-05-20 14:12:54.000000 easyFermi-1.1.1/easyFermi.egg-info/top_level.txt
--rw-rw-r--   0 raniere   (1000) raniere   (1000)       38 2023-05-20 14:12:54.372224 easyFermi-1.1.1/setup.cfg
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)     1181 2023-05-20 14:11:32.000000 easyFermi-1.1.1/setup.py
+drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2023-06-14 14:31:34.253104 easyFermi-1.1.2/
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)     1522 2022-01-31 12:02:33.000000 easyFermi-1.1.2/LICENSE.txt
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)     1702 2023-06-14 14:31:34.253104 easyFermi-1.1.2/PKG-INFO
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)     1172 2022-08-22 09:22:30.000000 easyFermi-1.1.2/README.md
+drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2023-06-14 14:31:34.253104 easyFermi-1.1.2/easyFermi/
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)       63 2022-02-01 13:52:31.000000 easyFermi-1.1.2/easyFermi/__init__.py
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)    92547 2023-06-14 14:28:57.000000 easyFermi-1.1.2/easyFermi/easyFermi.py
+drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2023-06-14 14:31:34.253104 easyFermi-1.1.2/easyFermi/images/
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)    40332 2022-01-15 16:04:30.000000 easyFermi-1.1.2/easyFermi/images/easyFermiIcon.png
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)   120905 2023-03-08 11:57:13.000000 easyFermi-1.1.2/easyFermi/images/easyFermiWindow.png
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)   121691 2021-11-23 14:18:26.000000 easyFermi-1.1.2/easyFermi/images/fermi.png
+drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2023-06-14 14:31:34.253104 easyFermi-1.1.2/easyFermi.egg-info/
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)     1702 2023-06-14 14:31:34.000000 easyFermi-1.1.2/easyFermi.egg-info/PKG-INFO
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)      338 2023-06-14 14:31:34.000000 easyFermi-1.1.2/easyFermi.egg-info/SOURCES.txt
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)        1 2023-06-14 14:31:34.000000 easyFermi-1.1.2/easyFermi.egg-info/dependency_links.txt
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)       14 2023-06-14 14:31:34.000000 easyFermi-1.1.2/easyFermi.egg-info/requires.txt
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)       10 2023-06-14 14:31:34.000000 easyFermi-1.1.2/easyFermi.egg-info/top_level.txt
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)       38 2023-06-14 14:31:34.253104 easyFermi-1.1.2/setup.cfg
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)     1181 2023-06-14 14:30:04.000000 easyFermi-1.1.2/setup.py
```

### Comparing `easyFermi-1.1.1/LICENSE.txt` & `easyFermi-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easyFermi-1.1.1/PKG-INFO` & `easyFermi-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyFermi
-Version: 1.1.1
+Version: 1.1.2
 Summary: The easiest way to analyze Fermi-LAT data
 Author: Raniere de Menezes
 Author-email: <easyfermi@gmail.com>
 Keywords: python,fermi,GUI,graphical interface,easyFermi,gamma-rays
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easyFermi-1.1.1/README.md` & `easyFermi-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `easyFermi-1.1.1/easyFermi/easyFermi.py` & `easyFermi-1.1.2/easyFermi/easyFermi.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         self.checkBox_2 = QtWidgets.QCheckBox(self.groupBox_2)
         self.checkBox_2.setGeometry(QtCore.QRect(10, 100, 131, 23))
         self.checkBox_2.setChecked(True)
         self.checkBox_2.setObjectName("checkBox_2")
         self.spinBox = QtWidgets.QSpinBox(self.groupBox_2)
         self.spinBox.setEnabled(False)
         self.spinBox.setGeometry(QtCore.QRect(40, 40, 48, 26))
-        self.spinBox.setMinimum(3)
+        self.spinBox.setRange(3,999)
         self.spinBox.setProperty("value", 20)
         self.spinBox.setObjectName("spinBox")
         self.radioButton_2 = QtWidgets.QRadioButton(self.groupBox_2)
         self.radioButton_2.setEnabled(False)
         self.radioButton_2.setGeometry(QtCore.QRect(40, 190, 91, 23))
         self.radioButton_2.setChecked(False)
         self.radioButton_2.setAutoExclusive(True)
```

### Comparing `easyFermi-1.1.1/easyFermi/images/easyFermiIcon.png` & `easyFermi-1.1.2/easyFermi/images/easyFermiIcon.png`

 * *Files identical despite different names*

### Comparing `easyFermi-1.1.1/easyFermi/images/easyFermiWindow.png` & `easyFermi-1.1.2/easyFermi/images/easyFermiWindow.png`

 * *Files identical despite different names*

### Comparing `easyFermi-1.1.1/easyFermi/images/fermi.png` & `easyFermi-1.1.2/easyFermi/images/fermi.png`

 * *Files identical despite different names*

### Comparing `easyFermi-1.1.1/easyFermi.egg-info/PKG-INFO` & `easyFermi-1.1.2/easyFermi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyFermi
-Version: 1.1.1
+Version: 1.1.2
 Summary: The easiest way to analyze Fermi-LAT data
 Author: Raniere de Menezes
 Author-email: <easyfermi@gmail.com>
 Keywords: python,fermi,GUI,graphical interface,easyFermi,gamma-rays
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easyFermi-1.1.1/setup.py` & `easyFermi-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.1'
+VERSION = '1.1.2'
 DESCRIPTION = 'The easiest way to analyze Fermi-LAT data'
 LONG_DESCRIPTION = 'A GUI that allows to do measure the flux, create light curves, SEDs, and TS maps for Fermi-LAT data.'
 
 # Setting up
 setup(
     name="easyFermi",
     version=VERSION,
```

