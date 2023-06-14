# Comparing `tmp/phone_gen-2.3.1.tar.gz` & `tmp/phone_gen-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phone_gen-2.3.1.tar", last modified: Sat Jun  3 11:58:29 2023, max compression
+gzip compressed data, was "phone_gen-2.3.2.tar", last modified: Wed Jun 14 08:07:48 2023, max compression
```

## Comparing `phone_gen-2.3.1.tar` & `phone_gen-2.3.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:58:29.720630 phone_gen-2.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:58:29.716630 phone_gen-2.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:58:29.720630 phone_gen-2.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-03 11:58:13.000000 phone_gen-2.3.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-03 11:58:13.000000 phone_gen-2.3.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-03 11:58:13.000000 phone_gen-2.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-03 11:58:13.000000 phone_gen-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-03 11:58:29.720630 phone_gen-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-03 11:58:13.000000 phone_gen-2.3.1/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-06-03 11:58:13.000000 phone_gen-2.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:58:29.720630 phone_gen-2.3.1/dev_tools/
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-06-03 11:58:13.000000 phone_gen-2.3.1/dev_tools/patterns_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-03 11:58:13.000000 phone_gen-2.3.1/dev_tools/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:58:29.720630 phone_gen-2.3.1/phone_gen/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-03 11:58:13.000000 phone_gen-2.3.1/phone_gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-03 11:58:29.000000 phone_gen-2.3.1/phone_gen/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-06-03 11:58:13.000000 phone_gen-2.3.1/phone_gen/_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-03 11:58:13.000000 phone_gen-2.3.1/phone_gen/alt_patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-03 11:58:13.000000 phone_gen-2.3.1/phone_gen/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-06-03 11:58:13.000000 phone_gen-2.3.1/phone_gen/country_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-06-03 11:58:13.000000 phone_gen-2.3.1/phone_gen/iso3.py
--rw-r--r--   0 runner    (1001) docker     (123)    87915 2023-06-03 11:58:13.000000 phone_gen-2.3.1/phone_gen/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:58:29.720630 phone_gen-2.3.1/phone_gen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-03 11:58:29.000000 phone_gen-2.3.1/phone_gen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-03 11:58:29.000000 phone_gen-2.3.1/phone_gen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 11:58:29.000000 phone_gen-2.3.1/phone_gen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-03 11:58:29.000000 phone_gen-2.3.1/phone_gen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-03 11:58:29.000000 phone_gen-2.3.1/phone_gen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-03 11:58:29.724630 phone_gen-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-03 11:58:13.000000 phone_gen-2.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:58:29.720630 phone_gen-2.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-03 11:58:13.000000 phone_gen-2.3.1/tests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-03 11:58:13.000000 phone_gen-2.3.1/tests/test_alt_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-03 11:58:13.000000 phone_gen-2.3.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-03 11:58:13.000000 phone_gen-2.3.1/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-03 11:58:13.000000 phone_gen-2.3.1/tests/test_load_alt_patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-03 11:58:13.000000 phone_gen-2.3.1/tests/test_phone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:07:48.430148 phone_gen-2.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:07:48.426148 phone_gen-2.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:07:48.430148 phone_gen-2.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-14 08:07:37.000000 phone_gen-2.3.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-14 08:07:37.000000 phone_gen-2.3.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-14 08:07:37.000000 phone_gen-2.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-14 08:07:37.000000 phone_gen-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-14 08:07:48.430148 phone_gen-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-14 08:07:37.000000 phone_gen-2.3.2/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-06-14 08:07:37.000000 phone_gen-2.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:07:48.430148 phone_gen-2.3.2/dev_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-06-14 08:07:37.000000 phone_gen-2.3.2/dev_tools/patterns_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-14 08:07:37.000000 phone_gen-2.3.2/dev_tools/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:07:48.430148 phone_gen-2.3.2/phone_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-14 08:07:37.000000 phone_gen-2.3.2/phone_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 08:07:48.000000 phone_gen-2.3.2/phone_gen/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-06-14 08:07:37.000000 phone_gen-2.3.2/phone_gen/_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-14 08:07:37.000000 phone_gen-2.3.2/phone_gen/alt_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-14 08:07:37.000000 phone_gen-2.3.2/phone_gen/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-06-14 08:07:37.000000 phone_gen-2.3.2/phone_gen/country_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-06-14 08:07:37.000000 phone_gen-2.3.2/phone_gen/iso3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87928 2023-06-14 08:07:37.000000 phone_gen-2.3.2/phone_gen/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:07:48.430148 phone_gen-2.3.2/phone_gen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-14 08:07:48.000000 phone_gen-2.3.2/phone_gen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-14 08:07:48.000000 phone_gen-2.3.2/phone_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:07:48.000000 phone_gen-2.3.2/phone_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-14 08:07:48.000000 phone_gen-2.3.2/phone_gen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 08:07:48.000000 phone_gen-2.3.2/phone_gen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-14 08:07:48.430148 phone_gen-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-14 08:07:37.000000 phone_gen-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:07:48.430148 phone_gen-2.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-14 08:07:37.000000 phone_gen-2.3.2/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-14 08:07:37.000000 phone_gen-2.3.2/tests/test_alt_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-14 08:07:37.000000 phone_gen-2.3.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-14 08:07:37.000000 phone_gen-2.3.2/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-14 08:07:37.000000 phone_gen-2.3.2/tests/test_load_alt_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-14 08:07:37.000000 phone_gen-2.3.2/tests/test_phone.py
```

### Comparing `phone_gen-2.3.1/.github/workflows/python-package.yml` & `phone_gen-2.3.2/.github/workflows/python-package.yml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install flake8 pep8-naming pytest black pytest-cov phonenumbers==8.13.13
+          python -m pip install flake8 pep8-naming pytest black pytest-cov phonenumbers==8.13.14
           python -m pip install -e .
       - name: Flake8
         run: |
           flake8 phone_gen
       - name: Black
         run: |
           black --check phone_gen
```

### Comparing `phone_gen-2.3.1/.github/workflows/python-publish.yml` & `phone_gen-2.3.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.1/.gitignore` & `phone_gen-2.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.1/LICENSE` & `phone_gen-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.1/PKG-INFO` & `phone_gen-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phone_gen
-Version: 2.3.1
+Version: 2.3.2
 Summary: International phone number generation
 Home-page: https://github.com/tolstislon/phone-gen
 Author: tolstislon
 Author-email: tolstislon@gmail.com
 License: MIT License
 Keywords: testing,test-data,phone-number,phone,test-data-generator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `phone_gen-2.3.1/README.md` & `phone_gen-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.1/dev_tools/patterns_generator.py` & `phone_gen-2.3.2/dev_tools/patterns_generator.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.1/dev_tools/update.py` & `phone_gen-2.3.2/dev_tools/update.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.1/phone_gen/__init__.py` & `phone_gen-2.3.2/phone_gen/__init__.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.1/phone_gen/_generator.py` & `phone_gen-2.3.2/phone_gen/_generator.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.1/phone_gen/alt_patterns.py` & `phone_gen-2.3.2/phone_gen/alt_patterns.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.1/phone_gen/cli.py` & `phone_gen-2.3.2/phone_gen/cli.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.1/phone_gen/country_name.py` & `phone_gen-2.3.2/phone_gen/country_name.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.1/phone_gen/iso3.py` & `phone_gen-2.3.2/phone_gen/iso3.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.1/phone_gen/patterns.py` & `phone_gen-2.3.2/phone_gen/patterns.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 """
-Auto-generated file 2023-06-03 11:49:59 UTC
-Resource: https://github.com/google/libphonenumber v8.13.13
+Auto-generated file 2023-06-14 08:01:41 UTC
+Resource: https://github.com/google/libphonenumber v8.13.14
 """
 
 
 PATTERNS = {
-    "info": "libphonenumber v8.13.13",
+    "info": "libphonenumber v8.13.14",
     "data": {
         "AC": {
             "code": "247",
             "pattern": "((6[2-467][\\d]{3}))",
             "mobile": "((4[\\d]{4}))",
         },
         "AD": {
@@ -317,15 +317,15 @@
             "code": "593",
             "pattern": "(([2-7][2-7][\\d]{6}))",
             "mobile": "((964[0-2][\\d]{5})|(9(39)|([57][89])|(6[0-36-9])|([89][\\d])[\\d]{6}))",
         },
         "EE": {
             "code": "372",
             "pattern": "(((3[23589])|(4[3-8])|(6[\\d])|(7[1-9])|(88)[\\d]{5}))",
-            "mobile": "(((5[\\d]{5})|(8(1(0(000)|([3-9][\\d][\\d]))|((1(0[236])|(1[\\d]))|((2[0-59])|([3-79][\\d])[\\d])[\\d]))|(2(0(000)|((19)|([2-7][\\d])[\\d]))|((([124-6][\\d])|(3[5-9])[\\d])|(7([3679][\\d])|(8[13-9]))|(8([2-6][\\d])|(7[01]))[\\d]))|([349][\\d]{4}))[\\d][\\d])|(5(([02][\\d])|(5[0-478])[\\d])|(1([0-8][\\d])|(95))|(6(4[0-4])|(5[1-589]))[\\d]{3}))",
+            "mobile": "(((5[\\d]{5})|(8(1(0(000)|([3-9][\\d][\\d]))|((1(0[236])|(1[\\d]))|((2[0-59])|([3-79][\\d])[\\d])[\\d]))|(2(0(000)|((19)|([2-7][\\d])[\\d]))|((([124-6][\\d])|(3[5-9])[\\d])|(7([0-3679][\\d])|(8[13-9]))|(8([2-6][\\d])|(7[01]))[\\d]))|([349][\\d]{4}))[\\d][\\d])|(5(([02][\\d])|(5[0-478])[\\d])|(1([0-8][\\d])|(95))|(6(4[0-4])|(5[1-589]))[\\d]{3}))",
         },
         "EG": {
             "code": "20",
             "pattern": "((13[23][\\d]{6})|((15)|(57)[\\d]{6:7})|((2[2-4])|(3)|(4[05-8])|(5[05])|(6[24-689])|(8[2468])|(9[235-7])[\\d]{7}))",
             "mobile": "((1[0-25][\\d]{8}))",
         },
         "EH": {
@@ -342,15 +342,15 @@
             "code": "34",
             "pattern": "((96906(0[0-8])|(1[1-9])|([2-9][\\d])[\\d][\\d])|(9(69(0[0-57-9])|([1-9][\\d]))|(73([0-8][\\d])|(9[1-9]))[\\d]{4})|((8([1356][\\d])|([28][0-8])|([47][1-9]))|(9([135][\\d])|([268][0-8])|(4[1-9])|(7[124-9]))[\\d]{6}))",
             "mobile": "(((590[16]00[\\d])|(9(6906(09)|(10))|(7390[\\d][\\d]))[\\d][\\d])|((6[\\d])|(7[1-48])[\\d]{7}))",
         },
         "ET": {
             "code": "251",
             "pattern": "((11667[01][\\d]{3})|((11(1(1[124])|(2[2-7])|(3[1-5])|(5[5-8])|(8[6-8]))|(2(13)|(3[6-8])|(5[89])|(7[05-9])|(8[2-6]))|(3(2[01])|(3[0-289])|(4[1289])|(7[1-4])|(87))|(4(1[69])|(3[2-49])|(4[0-3])|(6[5-8]))|(5(1[578])|(44)|(5[0-4]))|(6(1[578])|(2[69])|(39)|(4[5-7])|(5[0-5])|(6[0-59])|(8[015-8])))|(2(2(11[1-9])|(22[0-7])|(33[\\d])|(44[1467])|(66[1-68]))|(5(11[124-6])|(33[2-8])|(44[1467])|(55[14])|(66[1-3679])|(77[124-79])|(880)))|(3(3(11[0-46-8])|((22)|(55)[0-6])|(33[0134689])|(44[04])|(66[01467]))|(4(44[0-8])|(55[0-69])|(66[0-3])|(77[1-5])))|(4(6(119)|(22[0-24-7])|(33[1-5])|(44[13-69])|(55[14-689])|(660)|(88[1-4]))|(7((11)|(22)[1-9])|(33[13-7])|(44[13-6])|(55[1-689])))|(5(7(227)|(55[05])|((66)|(77)[14-8]))|(8(11[149])|(22[013-79])|(33[0-68])|(44[013-8])|(550)|(66[1-5])|(77[\\d])))[\\d]{4}))",
-            "mobile": "((7001[\\d]{5})|((7(0[1-9])|(1[0-8])|(22)|(77)|(86)|(99))|(9[\\d][\\d])[\\d]{6}))",
+            "mobile": "((700[1-9][\\d]{5})|((7(0[1-9])|(1[0-8])|(22)|(77)|(86)|(99))|(9[\\d][\\d])[\\d]{6}))",
         },
         "FI": {
             "code": "358",
             "pattern": "(((1[3-79][1-8])|([235689][1-8][\\d])[\\d]{2:6}))",
             "mobile": "((4946[\\d]{2:6})|((4[0-8])|(50)[\\d]{4:8}))",
         },
         "FJ": {
@@ -523,15 +523,15 @@
             "code": "964",
             "pattern": "((1[\\d]{7})|((2[13-5])|(3[02367])|(4[023])|(5[03])|(6[026])[\\d]{6:7}))",
             "mobile": "((7[3-9][\\d]{8}))",
         },
         "IR": {
             "code": "98",
             "pattern": "(((1[137])|(2[13-68])|(3[1458])|(4[145])|(5[1468])|(6[16])|(7[1467])|(8[13467])([03-57][\\d]{7})|([16][\\d]{3}([\\d]{4})?)|([289][\\d]{3}([\\d]([\\d]{3})?)?))|(94(000[09])|(2(121)|([2689]0[\\d]))|(30[0-2][\\d])|(4(111)|(40[\\d]))[\\d]{4}))",
-            "mobile": "((9((0([0-35][\\d])|(4[4-6]))|(([13][\\d])|(2[0-3])[\\d])[\\d])|(9([0-46][\\d][\\d])|(5[15]0)|(8(1[\\d])|(88))|(9(0[0-3])|([19][\\d])|(21)|(77)|(8[7-9])))[\\d]{5}))",
+            "mobile": "((9((0([0-35][\\d])|(4[4-6]))|(([13][\\d])|(2[0-3])[\\d])[\\d])|(9([0-46][\\d][\\d])|(5[15]0)|(8([12][\\d])|(88))|(9(0[0-3])|([19][\\d])|(21)|(69)|(77)|(8[7-9])))[\\d]{5}))",
         },
         "IS": {
             "code": "354",
             "pattern": "(((4(1[0-24-69])|(2[0-7])|([37][0-8])|(4[0-24589])|(5[0-68])|(6[\\d])|(8[0-36-8]))|(5(05)|([156][\\d])|(2[02578])|(3[0-579])|(4[03-7])|(7[0-2578])|(8[0-35-9])|(9[013-689]))|(872)[\\d]{4}))",
             "mobile": "(((38[589][\\d][\\d])|(6(1[1-8])|(2[0-6])|(3[026-9])|(4[014679])|(5[0159])|(6[0-69])|(70)|(8[06-8])|(9[\\d]))|(7(5[057])|([6-9][\\d]))|(8(2[0-59])|([3-69][\\d])|(8[238]))[\\d]{4}))",
         },
         "IT": {
@@ -708,21 +708,21 @@
         "ML": {
             "code": "223",
             "pattern": "((2(07[0-8])|(12[67])[\\d]{4})|((2(02)|(1[4-689]))|(4(0[0-4])|(4[1-39]))[\\d]{5}))",
             "mobile": "((2(0(01)|(79))|(17[\\d])[\\d]{4})|((5[01])|([679][\\d])|(8[2-49])[\\d]{6}))",
         },
         "MM": {
             "code": "95",
-            "pattern": "(((1((2[\\d])|(3[56])|([89][0-6])[\\d])|(4(2[29])|(39)|(62)|(7[0-2])|(83))|(6))|(2(2(00)|(8[34]))|(4(0[\\d])|([26]2)|(39)|(7[0-2])|(83))|(51[\\d][\\d]))|(4(2(2[\\d][\\d])|(48[013]))|(3(20[\\d])|(4(70)|(83))|(56))|(420[\\d])|(5470))|(6(0([23])|(88[\\d]))|((124)|([56]2[\\d])[\\d])|(2472)|(3(20[\\d])|(470))|(4(2[04][\\d])|(472))|(7((3[\\d])|(8[01459])[\\d])|(4(39)|([67]0))))[\\d]{4})|(5(2(2[\\d]{5:6})|(47[02][\\d]{4}))|((3472)|(4(2(1)|(86))|(470))|(522[\\d])|(6(20[\\d])|(483))|(7(20[\\d])|(48[01]))|(8(20[\\d])|(47[02]))|(9(20[\\d])|(470))[\\d]{4}))|(7((0470)|(4(25[\\d])|(470))|(5(202)|(470)|(96[\\d]))[\\d]{4})|(1(20[\\d]{4:5})|(4(70)|(83)[\\d]{4})))|(8(1(2[\\d]{5:6})|(4(10)|(7[01][\\d])[\\d]{3}))|(2(2[\\d]{5:6})|((320)|(490[\\d])[\\d]{3}))|((3(2[\\d][\\d])|(470))|(4[24-7])|(5((2[\\d])|(51)[\\d])|(4([1-35-9][\\d])|(4[0-57-9])))|(6[23])[\\d]{4}))|((1[2-6][\\d])|(4(2[24-8])|(3[2-7])|([46][2-6])|(5[3-5]))|(5([27][2-8])|(3[2-68])|(4[24-8])|(5[23])|(6[2-4])|(8[24-7])|(9[2-7]))|(6([19]20)|(42[03-6])|((52)|(7[45])[\\d]))|(7([04][24-8])|([15][2-7])|(22)|(3[2-4]))|(8(1[2-689])|(2[2-8])|([35]2[\\d]))[\\d]{4})|(25[\\d]{5:6})|((2[2-9])|(6(1[2356])|([24][2-6])|(3[24-6])|(5[2-4])|(6[2-8])|(7[235-7])|(8[245])|(9[24]))|(8(3[24])|(5[245]))[\\d]{4}))",
+            "pattern": "(((1((2[\\d])|(3[56])|([89][0-6])[\\d])|(4(2[29])|(62)|(7[0-2])|(83))|(6))|(2(2(00)|(8[34]))|(4(0[\\d])|([26]2)|(7[0-2])|(83))|(51[\\d][\\d]))|(4(2(2[\\d][\\d])|(48[013]))|(3(20[\\d])|(4(70)|(83))|(56))|(420[\\d])|(5470))|(6(0([23])|(88[\\d]))|((124)|([56]2[\\d])[\\d])|(2472)|(3(20[\\d])|(470))|(4(2[04][\\d])|(472))|(7((3[\\d])|(8[01459])[\\d])|(4[67]0)))[\\d]{4})|(5(2(2[\\d]{5:6})|(47[02][\\d]{4}))|((3472)|(4(2(1)|(86))|(470))|(522[\\d])|(6(20[\\d])|(483))|(7(20[\\d])|(48[01]))|(8(20[\\d])|(47[02]))|(9(20[\\d])|(470))[\\d]{4}))|(7((0470)|(4(25[\\d])|(470))|(5(202)|(470)|(96[\\d]))[\\d]{4})|(1(20[\\d]{4:5})|(4(70)|(83)[\\d]{4})))|(8(1(2[\\d]{5:6})|(4(10)|(7[01][\\d])[\\d]{3}))|(2(2[\\d]{5:6})|((320)|(490[\\d])[\\d]{3}))|((3(2[\\d][\\d])|(470))|(4[24-7])|(5((2[\\d])|(51)[\\d])|(4([1-35-9][\\d])|(4[0-57-9])))|(6[23])[\\d]{4}))|((1[2-6][\\d])|(4(2[24-8])|(3[2-7])|([46][2-6])|(5[3-5]))|(5([27][2-8])|(3[2-68])|(4[24-8])|(5[23])|(6[2-4])|(8[24-7])|(9[2-7]))|(6([19]20)|(42[03-6])|((52)|(7[45])[\\d]))|(7([04][24-8])|([15][2-7])|(22)|(3[2-4]))|(8(1[2-689])|(2[2-8])|([35]2[\\d]))[\\d]{4})|(25[\\d]{5:6})|((2[2-9])|(6(1[2356])|([24][2-6])|(3[24-6])|(5[2-4])|(6[2-8])|(7[235-7])|(8[245])|(9[24]))|(8(3[24])|(5[245]))[\\d]{4}))",
             "mobile": "(((17[01])|(9(2([0-4])|([56][\\d][\\d]))|((3([0-36])|(4[\\d]))|((6[\\d])|(8[89])|(9[4-8])[\\d])|(7(3)|(40)|([5-9][\\d]))[\\d])|(4(([0245][\\d])|([1379])[\\d])|(88))|(5[0-6])[\\d])[\\d]{4})|(9[69]1[\\d]{6})|(9([68][\\d])|(9[089])[\\d]{5}))",
         },
         "MN": {
             "code": "976",
             "pattern": "(([12]2[1-3][\\d]{5:6})|(7(0[0-5][\\d])|(128)[\\d]{4})|(([12](1)|(27))|(5[368])[\\d]{6})|([12](3[2-8])|(4[2-68])|(5[1-4689])[\\d]{6:7}))",
-            "mobile": "(((83[01])|(920)[\\d]{5})|((5[05])|(6[069])|(8[015689])|(9[013-9])[\\d]{6}))",
+            "mobile": "(((83[01])|(92[039])[\\d]{5})|((5[05])|(6[069])|(8[015689])|(9[013-9])[\\d]{6}))",
         },
         "MO": {
             "code": "853",
             "pattern": "(((28[2-9])|(8(11)|([2-57-9][\\d]))[\\d]{5}))",
             "mobile": "((6800[0-79][\\d]{3})|(6([235][\\d][\\d])|(6(0[0-5])|([1-9][\\d]))|(8(0[1-9])|([14-8][\\d])|(2[5-9])|([39][0-4]))[\\d]{4}))",
         },
         "MP": {
@@ -834,19 +834,19 @@
             "code": "683",
             "pattern": "(([47][\\d]{3}))",
             "mobile": "((888[4-9][\\d]{3}))",
         },
         "NZ": {
             "code": "64",
             "pattern": "((24099[\\d]{3})|((3[2-79])|([49][2-9])|(6[235-9])|(7[2-57-9])[\\d]{6}))",
-            "mobile": "((2[0-27-9][\\d]{7:8})|(21[\\d]{6}))",
+            "mobile": "((2[0-27-9][\\d]{7:8})|(2(1[\\d])|(75)[\\d]{5}))",
         },
         "OM": {
             "code": "968",
-            "pattern": "((2[2-6][\\d]{6}))",
+            "pattern": "((2[1-6][\\d]{6}))",
             "mobile": "((1505[\\d]{4})|((7([1289][\\d])|(7[0-5]))|(9(0[1-9])|([1-9][\\d]))[\\d]{5}))",
         },
         "PA": {
             "code": "507",
             "pattern": "(((1(0[\\d])|(1[479])|(2[37])|(3[0137])|(4[17])|(5[05])|(6[58])|(7[0167])|(8[2358])|(9[1389]))|(2([0235-79][\\d])|(1[0-7])|(4[013-9])|(8[02-9]))|(3([089][\\d])|(1[0-7])|(2[0-5])|(33)|(4[0-79])|(5[0-35])|(6[068])|(7[0-8]))|(4(00)|(3[0-579])|(4[\\d])|(7[0-57-9]))|(5([01][\\d])|(2[0-7])|([56]0)|(79))|(7(0[09])|(2[0-26-8])|(3[03])|(4[04])|(5[05-9])|(6[056])|(7[0-24-9])|(8[5-9])|(90))|(8(09)|(2[89])|(3[\\d])|(4[0-24-689])|(5[014])|(8[02]))|(9(0[5-9])|(1[0135-8])|(2[036-9])|(3[35-79])|(40)|(5[0457-9])|(6[05-9])|(7[04-9])|(8[35-8])|(9[\\d]))[\\d]{4}))",
             "mobile": "(((1[16]1)|(21[89])|(6[\\d]{3})|(8(1[01])|(7[23]))[\\d]{4}))",
         },
```

### Comparing `phone_gen-2.3.1/phone_gen.egg-info/PKG-INFO` & `phone_gen-2.3.2/phone_gen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phone-gen
-Version: 2.3.1
+Version: 2.3.2
 Summary: International phone number generation
 Home-page: https://github.com/tolstislon/phone-gen
 Author: tolstislon
 Author-email: tolstislon@gmail.com
 License: MIT License
 Keywords: testing,test-data,phone-number,phone,test-data-generator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `phone_gen-2.3.1/phone_gen.egg-info/SOURCES.txt` & `phone_gen-2.3.2/phone_gen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.1/setup.py` & `phone_gen-2.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.1/tests/test_alt_pattern.py` & `phone_gen-2.3.2/tests/test_alt_pattern.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.1/tests/test_cli.py` & `phone_gen-2.3.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.1/tests/test_generator.py` & `phone_gen-2.3.2/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.1/tests/test_load_alt_patterns.py` & `phone_gen-2.3.2/tests/test_load_alt_patterns.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.1/tests/test_phone.py` & `phone_gen-2.3.2/tests/test_phone.py`

 * *Files identical despite different names*

