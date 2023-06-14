# Comparing `tmp/JBPhD-2.3.1.tar.gz` & `tmp/JBPhD-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JBPhD-2.3.1.tar", last modified: Wed Jun 14 11:01:11 2023, max compression
+gzip compressed data, was "JBPhD-2.3.2.tar", last modified: Wed Jun 14 15:49:23 2023, max compression
```

## Comparing `JBPhD-2.3.1.tar` & `JBPhD-2.3.2.tar`

### file list

```diff
@@ -1,81 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 11:01:08.000000 JBPhD-2.3.1/
-drwxrwxrwx   0        0        0        0 2023-06-14 11:01:08.000000 JBPhD-2.3.1/JBPhD.egg-info/
--rw-rw-rw-   0        0        0      269 2023-06-14 11:01:08.000000 JBPhD-2.3.1/JBPhD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1564 2023-06-14 11:01:08.000000 JBPhD-2.3.1/JBPhD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 11:01:08.000000 JBPhD-2.3.1/JBPhD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-14 11:01:08.000000 JBPhD-2.3.1/JBPhD.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      127 2023-06-14 11:01:08.000000 JBPhD-2.3.1/JBPhD.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-14 11:01:08.000000 JBPhD-2.3.1/JBPhD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       49 2023-06-06 14:46:58.000000 JBPhD-2.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0       26 2023-05-07 16:04:18.000000 JBPhD-2.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0      269 2023-06-14 11:01:12.000000 JBPhD-2.3.1/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-05-07 16:42:22.000000 JBPhD-2.3.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-14 11:01:08.000000 JBPhD-2.3.1/Task/
--rw-rw-rw-   0        0        0   256120 2023-06-06 10:39:06.000000 JBPhD-2.3.1/Task/BL.PNG
--rw-rw-rw-   0        0        0   256871 2023-06-06 10:40:52.000000 JBPhD-2.3.1/Task/BR.PNG
--rw-rw-rw-   0        0        0   256274 2023-06-06 10:36:30.000000 JBPhD-2.3.1/Task/Back_Left.PNG
--rw-rw-rw-   0        0        0   256511 2023-06-06 10:36:30.000000 JBPhD-2.3.1/Task/Back_Right.PNG
--rw-rw-rw-   0        0        0    60437 2023-02-02 09:16:10.000000 JBPhD-2.3.1/Task/Consent Form.docx
--rw-rw-rw-   0        0        0     6403 2023-05-25 21:47:58.000000 JBPhD-2.3.1/Task/Consent.py
--rw-rw-rw-   0        0        0      911 2023-05-18 15:51:28.000000 JBPhD-2.3.1/Task/Dependencies.py
--rw-rw-rw-   0        0        0    11435 2023-06-13 10:51:44.000000 JBPhD-2.3.1/Task/Dependency Installation.py
--rw-rw-rw-   0        0        0      156 2023-05-25 21:19:50.000000 JBPhD-2.3.1/Task/Email Errors.txt
--rw-rw-rw-   0        0        0      552 2023-05-06 17:47:44.000000 JBPhD-2.3.1/Task/Email Output.py
--rw-rw-rw-   0        0        0     4085 2023-06-14 10:26:42.000000 JBPhD-2.3.1/Task/Export.py
--rw-rw-rw-   0        0        0   249966 2023-06-06 10:40:42.000000 JBPhD-2.3.1/Task/FL.PNG
--rw-rw-rw-   0        0        0   249859 2023-06-06 10:41:22.000000 JBPhD-2.3.1/Task/FR.PNG
--rw-rw-rw-   0        0        0   249107 2023-06-06 10:36:30.000000 JBPhD-2.3.1/Task/Front_Left.PNG
--rw-rw-rw-   0        0        0   249006 2023-06-06 10:36:30.000000 JBPhD-2.3.1/Task/Front_Right.PNG
--rw-rw-rw-   0        0        0   281708 2023-04-07 13:54:00.000000 JBPhD-2.3.1/Task/ImageSample.PNG
--rw-rw-rw-   0        0        0   256120 2023-06-06 10:38:02.000000 JBPhD-2.3.1/Task/Inverse_Back_Left.PNG
--rw-rw-rw-   0        0        0   256871 2023-06-06 10:40:46.000000 JBPhD-2.3.1/Task/Inverse_Back_Right.PNG
--rw-rw-rw-   0        0        0   249966 2023-06-06 10:40:32.000000 JBPhD-2.3.1/Task/Inverse_Front_Left.PNG
--rw-rw-rw-   0        0        0   249859 2023-06-06 10:41:18.000000 JBPhD-2.3.1/Task/Inverse_Front_Right.PNG
--rw-rw-rw-   0        0        0      382 2023-05-25 16:51:56.000000 JBPhD-2.3.1/Task/Location.py
--rw-rw-rw-   0        0        0       54 2023-05-07 14:35:12.000000 JBPhD-2.3.1/Task/MANIFEST.in.txt
--rw-rw-rw-   0        0        0    14031 2023-04-07 13:54:00.000000 JBPhD-2.3.1/Task/Manikin Back Down Left.png
--rw-rw-rw-   0        0        0    13918 2023-04-07 13:54:00.000000 JBPhD-2.3.1/Task/Manikin Back Up Right.png
--rw-rw-rw-   0        0        0    16784 2023-04-07 13:54:00.000000 JBPhD-2.3.1/Task/Manikin front Down Right.png
--rw-rw-rw-   0        0        0    20357 2023-04-07 13:54:00.000000 JBPhD-2.3.1/Task/Manikin front Up Right.png
--rw-rw-rw-   0        0        0        1 2023-06-13 10:53:28.000000 JBPhD-2.3.1/Task/N-Back count.txt
--rw-rw-rw-   0        0        0    22361 2023-06-10 22:31:34.000000 JBPhD-2.3.1/Task/N-Back.py
--rw-rw-rw-   0        0        0   765972 2023-05-24 14:10:50.000000 JBPhD-2.3.1/Task/PIS.docx
--rw-rw-rw-   0        0        0    20182 2023-05-24 14:11:06.000000 JBPhD-2.3.1/Task/PIS.txt
--rwxrwxrwx   0        0        0      680 2023-04-23 19:01:06.000000 JBPhD-2.3.1/Task/Python Install.bat
--rw-rw-rw-   0        0        0       20 2023-05-07 14:41:38.000000 JBPhD-2.3.1/Task/README.txt.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 10:53:12.000000 JBPhD-2.3.1/Task/RT count.txt
--rw-rw-rw-   0        0        0    20946 2023-06-09 15:09:44.000000 JBPhD-2.3.1/Task/Reaction Time Task - Copy.py
--rwxrwxrwx   0        0        0      448 2023-05-07 14:17:02.000000 JBPhD-2.3.1/Task/Suffix.bat
--rw-rw-rw-   0        0        0        1 2023-06-13 11:16:30.000000 JBPhD-2.3.1/Task/Switch count.txt
--rw-rw-rw-   0        0        0    30983 2023-06-13 11:04:42.000000 JBPhD-2.3.1/Task/Switching.py
--rw-rw-rw-   0        0        0    13647 2023-06-13 11:03:28.000000 JBPhD-2.3.1/Task/Task.py
--rw-rw-rw-   0        0        0     6627 2023-05-24 20:53:36.000000 JBPhD-2.3.1/Task/Trial.py
--rw-rw-rw-   0        0        0   256274 2023-06-06 10:39:36.000000 JBPhD-2.3.1/Task/UBL.PNG
--rw-rw-rw-   0        0        0   256511 2023-06-06 10:39:32.000000 JBPhD-2.3.1/Task/UBR.PNG
--rw-rw-rw-   0        0        0   249107 2023-06-06 10:39:26.000000 JBPhD-2.3.1/Task/UFL.PNG
--rw-rw-rw-   0        0        0   249006 2023-06-06 10:39:18.000000 JBPhD-2.3.1/Task/UFR.PNG
-drwxrwxrwx   0        0        0        0 2023-06-14 11:01:08.000000 JBPhD-2.3.1/Task/__pycache__/
--rw-rw-rw-   0        0        0     5027 2023-05-07 22:15:14.000000 JBPhD-2.3.1/Task/__pycache__/Dependencies.cpython-311.pyc
--rw-rw-rw-   0        0        0     6538 2023-05-24 13:46:36.000000 JBPhD-2.3.1/Task/__pycache__/Export.cpython-311.pyc
--rw-rw-rw-   0        0        0      698 2023-05-25 16:52:10.000000 JBPhD-2.3.1/Task/__pycache__/Location.cpython-311.pyc
--rw-rw-rw-   0        0        0    19777 2023-06-04 22:02:52.000000 JBPhD-2.3.1/Task/__pycache__/Task.cpython-311.pyc
--rw-rw-rw-   0        0        0      931 2023-05-05 14:18:56.000000 JBPhD-2.3.1/Task/__pycache__/spwf.cpython-311.pyc
--rw-rw-rw-   0        0        0     3162 2023-04-07 13:54:00.000000 JBPhD-2.3.1/Task/asterisk.png
--rw-rw-rw-   0        0        0    47189 2023-04-07 13:54:00.000000 JBPhD-2.3.1/Task/circle.jpg
--rw-rw-rw-   0        0        0     2371 2023-06-14 10:25:18.000000 JBPhD-2.3.1/Task/gdap.json
--rw-rw-rw-   0        0        0    38788 2023-04-07 13:54:00.000000 JBPhD-2.3.1/Task/greentick.png
--rw-rw-rw-   0        0        0       54 2023-05-07 14:31:32.000000 JBPhD-2.3.1/Task/help.txt
--rw-rw-rw-   0        0        0      491 2023-05-14 16:12:16.000000 JBPhD-2.3.1/Task/pins.csv
--rw-rw-rw-   0        0        0    24503 2023-04-07 13:54:00.000000 JBPhD-2.3.1/Task/redcross.png
--rw-rw-rw-   0        0        0    98588 2023-04-07 13:54:00.000000 JBPhD-2.3.1/Task/reddot.png
--rw-rw-rw-   0        0        0      566 2023-05-07 14:26:16.000000 JBPhD-2.3.1/Task/setup.py
--rw-rw-rw-   0        0        0      472 2023-05-05 14:17:12.000000 JBPhD-2.3.1/Task/spwf.py
--rw-rw-rw-   0        0        0       44 2023-04-24 16:27:34.000000 JBPhD-2.3.1/Task/spwfoutput.txt
--rw-rw-rw-   0        0        0      100 2023-04-24 16:27:34.000000 JBPhD-2.3.1/Task/spwfvalue.txt
--rw-rw-rw-   0        0        0       14 2023-06-13 10:57:50.000000 JBPhD-2.3.1/Task/suffix.txt
--rw-rw-rw-   0        0        0   161693 2023-04-07 13:54:00.000000 JBPhD-2.3.1/Task/trial.jpeg
--rw-rw-rw-   0        0        0   432254 2023-05-04 10:35:10.000000 JBPhD-2.3.1/Task/uop.ico
--rw-rw-rw-   0        0        0     3908 2023-05-04 10:32:40.000000 JBPhD-2.3.1/Task/uop.jpeg
--rw-rw-rw-   0        0        0     7038 2023-04-16 20:40:14.000000 JBPhD-2.3.1/Task/uop.png
--rw-rw-rw-   0        0        0       42 2023-06-14 11:01:12.000000 JBPhD-2.3.1/setup.cfg
--rw-rw-rw-   0        0        0      863 2023-06-14 11:00:32.000000 JBPhD-2.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 15:49:22.000000 JBPhD-2.3.2/
+drwxrwxrwx   0        0        0        0 2023-06-14 15:49:22.000000 JBPhD-2.3.2/JBPhD.egg-info/
+-rw-rw-rw-   0        0        0      269 2023-06-14 15:49:22.000000 JBPhD-2.3.2/JBPhD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1545 2023-06-14 15:49:22.000000 JBPhD-2.3.2/JBPhD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 15:49:22.000000 JBPhD-2.3.2/JBPhD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-14 15:49:22.000000 JBPhD-2.3.2/JBPhD.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      127 2023-06-14 15:49:22.000000 JBPhD-2.3.2/JBPhD.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-14 15:49:22.000000 JBPhD-2.3.2/JBPhD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       49 2023-06-06 14:46:58.000000 JBPhD-2.3.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2023-05-07 16:04:18.000000 JBPhD-2.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      269 2023-06-14 15:49:24.000000 JBPhD-2.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-05-07 16:42:22.000000 JBPhD-2.3.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 15:49:22.000000 JBPhD-2.3.2/Task/
+-rw-rw-rw-   0        0        0   256120 2023-06-06 10:39:06.000000 JBPhD-2.3.2/Task/BL.PNG
+-rw-rw-rw-   0        0        0   256871 2023-06-06 10:40:52.000000 JBPhD-2.3.2/Task/BR.PNG
+-rw-rw-rw-   0        0        0   256274 2023-06-06 10:36:30.000000 JBPhD-2.3.2/Task/Back_Left.PNG
+-rw-rw-rw-   0        0        0   256511 2023-06-06 10:36:30.000000 JBPhD-2.3.2/Task/Back_Right.PNG
+-rw-rw-rw-   0        0        0    60437 2023-02-02 09:16:10.000000 JBPhD-2.3.2/Task/Consent Form.docx
+-rw-rw-rw-   0        0        0     6403 2023-05-25 21:47:58.000000 JBPhD-2.3.2/Task/Consent.py
+-rw-rw-rw-   0        0        0      911 2023-05-18 15:51:28.000000 JBPhD-2.3.2/Task/Dependencies.py
+-rw-rw-rw-   0        0        0    11462 2023-06-14 15:29:28.000000 JBPhD-2.3.2/Task/Dependency Installation.py
+-rw-rw-rw-   0        0        0     3867 2023-06-14 14:51:46.000000 JBPhD-2.3.2/Task/Export.py
+-rw-rw-rw-   0        0        0   249966 2023-06-06 10:40:42.000000 JBPhD-2.3.2/Task/FL.PNG
+-rw-rw-rw-   0        0        0   249859 2023-06-06 10:41:22.000000 JBPhD-2.3.2/Task/FR.PNG
+-rw-rw-rw-   0        0        0   249107 2023-06-06 10:36:30.000000 JBPhD-2.3.2/Task/Front_Left.PNG
+-rw-rw-rw-   0        0        0   249006 2023-06-06 10:36:30.000000 JBPhD-2.3.2/Task/Front_Right.PNG
+-rw-rw-rw-   0        0        0   281708 2023-04-07 13:54:00.000000 JBPhD-2.3.2/Task/ImageSample.PNG
+-rw-rw-rw-   0        0        0   256120 2023-06-06 10:38:02.000000 JBPhD-2.3.2/Task/Inverse_Back_Left.PNG
+-rw-rw-rw-   0        0        0   256871 2023-06-06 10:40:46.000000 JBPhD-2.3.2/Task/Inverse_Back_Right.PNG
+-rw-rw-rw-   0        0        0   249966 2023-06-06 10:40:32.000000 JBPhD-2.3.2/Task/Inverse_Front_Left.PNG
+-rw-rw-rw-   0        0        0   249859 2023-06-06 10:41:18.000000 JBPhD-2.3.2/Task/Inverse_Front_Right.PNG
+-rw-rw-rw-   0        0        0      382 2023-05-25 16:51:56.000000 JBPhD-2.3.2/Task/Location.py
+-rw-rw-rw-   0        0        0       54 2023-05-07 14:35:12.000000 JBPhD-2.3.2/Task/MANIFEST.in.txt
+-rw-rw-rw-   0        0        0    14031 2023-04-07 13:54:00.000000 JBPhD-2.3.2/Task/Manikin Back Down Left.png
+-rw-rw-rw-   0        0        0    13918 2023-04-07 13:54:00.000000 JBPhD-2.3.2/Task/Manikin Back Up Right.png
+-rw-rw-rw-   0        0        0    16784 2023-04-07 13:54:00.000000 JBPhD-2.3.2/Task/Manikin front Down Right.png
+-rw-rw-rw-   0        0        0    20357 2023-04-07 13:54:00.000000 JBPhD-2.3.2/Task/Manikin front Up Right.png
+-rw-rw-rw-   0        0        0        1 2023-06-14 15:32:48.000000 JBPhD-2.3.2/Task/N-Back count.txt
+-rw-rw-rw-   0        0        0    21881 2023-06-14 15:32:40.000000 JBPhD-2.3.2/Task/N-Back.py
+-rw-rw-rw-   0        0        0   765972 2023-05-24 14:10:50.000000 JBPhD-2.3.2/Task/PIS.docx
+-rw-rw-rw-   0        0        0    20182 2023-05-24 14:11:06.000000 JBPhD-2.3.2/Task/PIS.txt
+-rwxrwxrwx   0        0        0      680 2023-04-23 19:01:06.000000 JBPhD-2.3.2/Task/Python Install.bat
+-rw-rw-rw-   0        0        0       20 2023-05-07 14:41:38.000000 JBPhD-2.3.2/Task/README.txt.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 15:46:08.000000 JBPhD-2.3.2/Task/RT count.txt
+-rw-rw-rw-   0        0        0    20951 2023-06-14 15:46:02.000000 JBPhD-2.3.2/Task/Reaction Time Task - Copy.py
+-rwxrwxrwx   0        0        0      448 2023-05-07 14:17:02.000000 JBPhD-2.3.2/Task/Suffix.bat
+-rw-rw-rw-   0        0        0        1 2023-06-14 15:47:34.000000 JBPhD-2.3.2/Task/Switch count.txt
+-rw-rw-rw-   0        0        0    30497 2023-06-14 14:48:34.000000 JBPhD-2.3.2/Task/Switching.py
+-rw-rw-rw-   0        0        0    13647 2023-06-13 11:03:28.000000 JBPhD-2.3.2/Task/Task.py
+-rw-rw-rw-   0        0        0     6627 2023-05-24 20:53:36.000000 JBPhD-2.3.2/Task/Trial.py
+-rw-rw-rw-   0        0        0   256274 2023-06-06 10:39:36.000000 JBPhD-2.3.2/Task/UBL.PNG
+-rw-rw-rw-   0        0        0   256511 2023-06-06 10:39:32.000000 JBPhD-2.3.2/Task/UBR.PNG
+-rw-rw-rw-   0        0        0   249107 2023-06-06 10:39:26.000000 JBPhD-2.3.2/Task/UFL.PNG
+-rw-rw-rw-   0        0        0   249006 2023-06-06 10:39:18.000000 JBPhD-2.3.2/Task/UFR.PNG
+drwxrwxrwx   0        0        0        0 2023-06-14 15:49:22.000000 JBPhD-2.3.2/Task/__pycache__/
+-rw-rw-rw-   0        0        0     5027 2023-05-07 22:15:14.000000 JBPhD-2.3.2/Task/__pycache__/Dependencies.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6538 2023-05-24 13:46:36.000000 JBPhD-2.3.2/Task/__pycache__/Export.cpython-311.pyc
+-rw-rw-rw-   0        0        0      698 2023-05-25 16:52:10.000000 JBPhD-2.3.2/Task/__pycache__/Location.cpython-311.pyc
+-rw-rw-rw-   0        0        0    19777 2023-06-04 22:02:52.000000 JBPhD-2.3.2/Task/__pycache__/Task.cpython-311.pyc
+-rw-rw-rw-   0        0        0      563 2023-06-14 14:40:54.000000 JBPhD-2.3.2/Task/__pycache__/spwf.cpython-310.pyc
+-rw-rw-rw-   0        0        0      931 2023-05-05 14:18:56.000000 JBPhD-2.3.2/Task/__pycache__/spwf.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3162 2023-04-07 13:54:00.000000 JBPhD-2.3.2/Task/asterisk.png
+-rw-rw-rw-   0        0        0    47189 2023-04-07 13:54:00.000000 JBPhD-2.3.2/Task/circle.jpg
+-rw-rw-rw-   0        0        0     2371 2023-06-14 10:25:18.000000 JBPhD-2.3.2/Task/gdap.json
+-rw-rw-rw-   0        0        0    38788 2023-04-07 13:54:00.000000 JBPhD-2.3.2/Task/greentick.png
+-rw-rw-rw-   0        0        0      491 2023-05-14 16:12:16.000000 JBPhD-2.3.2/Task/pins.csv
+-rw-rw-rw-   0        0        0    24503 2023-04-07 13:54:00.000000 JBPhD-2.3.2/Task/redcross.png
+-rw-rw-rw-   0        0        0    98588 2023-04-07 13:54:00.000000 JBPhD-2.3.2/Task/reddot.png
+-rw-rw-rw-   0        0        0      566 2023-05-07 14:26:16.000000 JBPhD-2.3.2/Task/setup.py
+-rw-rw-rw-   0        0        0      472 2023-05-05 14:17:12.000000 JBPhD-2.3.2/Task/spwf.py
+-rw-rw-rw-   0        0        0       44 2023-04-24 16:27:34.000000 JBPhD-2.3.2/Task/spwfoutput.txt
+-rw-rw-rw-   0        0        0      100 2023-04-24 16:27:34.000000 JBPhD-2.3.2/Task/spwfvalue.txt
+-rw-rw-rw-   0        0        0       19 2023-06-14 15:28:32.000000 JBPhD-2.3.2/Task/suffix.txt
+-rw-rw-rw-   0        0        0   161693 2023-04-07 13:54:00.000000 JBPhD-2.3.2/Task/trial.jpeg
+-rw-rw-rw-   0        0        0   432254 2023-05-04 10:35:10.000000 JBPhD-2.3.2/Task/uop.ico
+-rw-rw-rw-   0        0        0     3908 2023-05-04 10:32:40.000000 JBPhD-2.3.2/Task/uop.jpeg
+-rw-rw-rw-   0        0        0     7038 2023-04-16 20:40:14.000000 JBPhD-2.3.2/Task/uop.png
+-rw-rw-rw-   0        0        0       42 2023-06-14 15:49:24.000000 JBPhD-2.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      863 2023-06-14 15:49:00.000000 JBPhD-2.3.2/setup.py
```

### Comparing `JBPhD-2.3.1/JBPhD.egg-info/SOURCES.txt` & `JBPhD-2.3.2/JBPhD.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 Task/BR.PNG
 Task/Back_Left.PNG
 Task/Back_Right.PNG
 Task/Consent Form.docx
 Task/Consent.py
 Task/Dependencies.py
 Task/Dependency Installation.py
-Task/Email Errors.txt
-Task/Email Output.py
 Task/Export.py
 Task/FL.PNG
 Task/FR.PNG
 Task/Front_Left.PNG
 Task/Front_Right.PNG
 Task/ImageSample.PNG
 Task/Inverse_Back_Left.PNG
@@ -51,15 +49,14 @@
 Task/UBR.PNG
 Task/UFL.PNG
 Task/UFR.PNG
 Task/asterisk.png
 Task/circle.jpg
 Task/gdap.json
 Task/greentick.png
-Task/help.txt
 Task/pins.csv
 Task/redcross.png
 Task/reddot.png
 Task/setup.py
 Task/spwf.py
 Task/spwfoutput.txt
 Task/spwfvalue.txt
@@ -68,8 +65,9 @@
 Task/uop.ico
 Task/uop.jpeg
 Task/uop.png
 Task/__pycache__/Dependencies.cpython-311.pyc
 Task/__pycache__/Export.cpython-311.pyc
 Task/__pycache__/Location.cpython-311.pyc
 Task/__pycache__/Task.cpython-311.pyc
+Task/__pycache__/spwf.cpython-310.pyc
 Task/__pycache__/spwf.cpython-311.pyc
```

### Comparing `JBPhD-2.3.1/Task/BL.PNG` & `JBPhD-2.3.2/Task/BL.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/BR.PNG` & `JBPhD-2.3.2/Task/BR.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/Back_Left.PNG` & `JBPhD-2.3.2/Task/Back_Left.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/Back_Right.PNG` & `JBPhD-2.3.2/Task/Back_Right.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/Consent Form.docx` & `JBPhD-2.3.2/Task/Consent Form.docx`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/Consent.py` & `JBPhD-2.3.2/Task/Consent.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/Dependencies.py` & `JBPhD-2.3.2/Task/Dependencies.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/Dependency Installation.py` & `JBPhD-2.3.2/Task/Dependency Installation.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 import Location
 from sendgrid import SendGridAPIClient
 from sendgrid.helpers.mail import Mail, Attachment, FileContent, FileName, FileType, Disposition
 
 location = Location.first_word
 if location == 'ECHO':
     outputloc = 'Non-university Device'
-elif location == 'uni.ds.port.ac.uk':
+
+
+elif location == 'uni.ds.port.ac.uk' or 'static.port.ac.uk':
     outputloc = 'University Device'
 
 print("Welcome to the task \n\n")
 print(f'Connection: {outputloc}')
 
 #print(python_path)
 now = datetime.now()
```

### Comparing `JBPhD-2.3.1/Task/Export.py` & `JBPhD-2.3.2/Task/Export.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     SERVICE_ACCOUNT_FILE = 'gdap.json'
 
     LOCAL_FOLDER_PATH = folder_name
 
     #DESTINATION_FOLDER_ID = '1rUysUpmMihZTLPA8XL1INjRdA7bGbwZQ'
     DESTINATION_FOLDER_ID = '1bEpzafbGDmQWBaiFTnXb6Rxod3i9y7vG'
 
-    # Authenticate and authorize the service account
     creds = Credentials.from_service_account_file(SERVICE_ACCOUNT_FILE)
     credentials = service_account.Credentials.from_service_account_file(
     SERVICE_ACCOUNT_FILE,
     scopes=['https://www.googleapis.com/auth/drive']
 )
     drive_service = build('drive', 'v3', credentials=creds)
 
@@ -74,21 +73,19 @@
         folder_id = create_folder(folder_name, parent_id)
         # Upload each file in the folder to the created folder
         for file_name in os.listdir(local_folder_path):
             file_path = os.path.join(local_folder_path, file_name)
             if os.path.isfile(file_path):
                 upload_file(file_path, folder_id)
             elif os.path.isdir(file_path):
-                # Upload the subfolder recursively
                 upload_folder(file_path, folder_id)
     
-    # Call the function to upload the entire folder to Google Drive as one folder, containing the individual files
     upload_folder(LOCAL_FOLDER_PATH, DESTINATION_FOLDER_ID)
 
 try:
     upload()
-    print("Export complete")
+    #print("Export complete")
 except Exception as e:
     with open(depfile, mode='a+') as f:
         f.write(f'At {outputtime} an API error was experienced: \n\n ------------------------------------------------------ \n\n')
         f.write(str(e))
         print(e)
```

### Comparing `JBPhD-2.3.1/Task/FL.PNG` & `JBPhD-2.3.2/Task/FL.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/FR.PNG` & `JBPhD-2.3.2/Task/FR.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/Front_Left.PNG` & `JBPhD-2.3.2/Task/Front_Left.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/Front_Right.PNG` & `JBPhD-2.3.2/Task/Front_Right.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/ImageSample.PNG` & `JBPhD-2.3.2/Task/ImageSample.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/Inverse_Back_Left.PNG` & `JBPhD-2.3.2/Task/Inverse_Back_Left.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/Inverse_Back_Right.PNG` & `JBPhD-2.3.2/Task/Inverse_Back_Right.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/Inverse_Front_Left.PNG` & `JBPhD-2.3.2/Task/Inverse_Front_Left.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/Inverse_Front_Right.PNG` & `JBPhD-2.3.2/Task/Inverse_Front_Right.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/Manikin Back Down Left.png` & `JBPhD-2.3.2/Task/Manikin Back Down Left.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/Manikin Back Up Right.png` & `JBPhD-2.3.2/Task/Manikin Back Up Right.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/Manikin front Down Right.png` & `JBPhD-2.3.2/Task/Manikin front Down Right.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/Manikin front Up Right.png` & `JBPhD-2.3.2/Task/Manikin front Up Right.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/N-Back.py` & `JBPhD-2.3.2/Task/N-Back.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,29 +365,15 @@
                     score = 0
                 else:
                     correct()
                     score = 1
 
             endRT = time.time()
             RT = (endRT - starterRT)
-            overalltime = timenow - starterRT
-            
-        if overalltime > 3:
-            Game_Running = False
-            RT = overalltime
-            DISPLAYSURF.fill(WHITE)
-            pygame.time.wait(500)
-            pygame.display.update()
-            pygame.time.wait(500)
-            end = time.time()
-            score = 0
-               
-                # can bin off any triggers of 16, suggests missed trials
-                
-            break            
+          
 
             with open(filename, mode="a+") as file:
                 file.write(f"{date_time_string}, {count}, {score}, N-Back\n")
 
             with open(filename2, mode="a+") as file:
                 file.write(f"{date_time_string}, {count}, {RT}, N-Back\n")
```

### Comparing `JBPhD-2.3.1/Task/PIS.docx` & `JBPhD-2.3.2/Task/PIS.docx`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/PIS.txt` & `JBPhD-2.3.2/Task/PIS.txt`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/Python Install.bat` & `JBPhD-2.3.2/Task/Python Install.bat`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/Reaction Time Task - Copy.py` & `JBPhD-2.3.2/Task/Reaction Time Task - Copy.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,14 +399,15 @@
 global cir
 ast = 0
 cir = 0
 
 def task():
 
     timer = random.randint(1,5)
+    timeout = 3
     global ast
     global cir
     if timer == 1:
      wait = 1100
     if timer == 2:
      wait = 1200
     if timer == 3:
@@ -679,23 +680,23 @@
 
 with open(count_file, 'w') as f:
     f.write(str(count))
 
 trialcounter = 0
 
 
-'''show_welcome_screen()
+show_welcome_screen()
 intro()
 
 for i in range(1,7):
     practice()
     trialcounter += 1
 
-intertrial()'''
+intertrial()
 
 for i in range(1,41):
     task()
     trialcounter += 1
-'''
+
 exitscreen()
 import Export
-sysexit()'''
+sysexit()
```

### Comparing `JBPhD-2.3.1/Task/Switching.py` & `JBPhD-2.3.2/Task/Switching.py`

 * *Files 2% similar despite different names*

```diff
@@ -1020,42 +1020,27 @@
     screen.blit(text, text_rect)
 
     pygame.display.update()
     # pygame.time.delay(500)
     pygame.time.delay(10000)
 
 def trialorder():
-    for i in range(0, 46):
+    for i in range(0, 64):
         torder = random.randint(1, 2)
         if torder == 1:
             maths()
-            print("Lower Count: ",lowercount)
-            print("Higher Count: ",highercount)
-            
         else:
             ball()
-
-            print("Total Count ",ballcount)
-            print("Front Left ", FL)
-            print("Front Right ", FR)
-            print("Back Left", BL)
-            print("Back Right ",BR)
-            print("Upside Front Left ",UFL)
-            print("Upside Front Right ",UFR) 
-            print("Upside Back Left ",UBL)
-            print("Upside Back Right ", UBR)
-            print("\n\n")
-
-
  
 trialcounter = 0
 
 fileremoval()
 show_welcome_screen()
-intro()
-introR()
-mathsintro()
+for i in range(1,3):
+    intro()
+    introR()
+    mathsintro()
 intertrial()
 trialorder()
 exitscreen()
 import Export
 pygame.quit()
```

### Comparing `JBPhD-2.3.1/Task/Task.py` & `JBPhD-2.3.2/Task/Task.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/Trial.py` & `JBPhD-2.3.2/Task/Trial.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/UBL.PNG` & `JBPhD-2.3.2/Task/UBL.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/UBR.PNG` & `JBPhD-2.3.2/Task/UBR.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/UFL.PNG` & `JBPhD-2.3.2/Task/UFL.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/UFR.PNG` & `JBPhD-2.3.2/Task/UFR.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/__pycache__/Dependencies.cpython-311.pyc` & `JBPhD-2.3.2/Task/__pycache__/Dependencies.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/__pycache__/Export.cpython-311.pyc` & `JBPhD-2.3.2/Task/__pycache__/Export.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/__pycache__/Location.cpython-311.pyc` & `JBPhD-2.3.2/Task/__pycache__/Location.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/__pycache__/Task.cpython-311.pyc` & `JBPhD-2.3.2/Task/__pycache__/Task.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/__pycache__/spwf.cpython-311.pyc` & `JBPhD-2.3.2/Task/__pycache__/spwf.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/asterisk.png` & `JBPhD-2.3.2/Task/asterisk.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/circle.jpg` & `JBPhD-2.3.2/Task/circle.jpg`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/gdap.json` & `JBPhD-2.3.2/Task/gdap.json`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/greentick.png` & `JBPhD-2.3.2/Task/greentick.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/redcross.png` & `JBPhD-2.3.2/Task/redcross.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/reddot.png` & `JBPhD-2.3.2/Task/reddot.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/setup.py` & `JBPhD-2.3.2/Task/setup.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/trial.jpeg` & `JBPhD-2.3.2/Task/trial.jpeg`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/uop.ico` & `JBPhD-2.3.2/Task/uop.ico`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/uop.jpeg` & `JBPhD-2.3.2/Task/uop.jpeg`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/Task/uop.png` & `JBPhD-2.3.2/Task/uop.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.3.1/setup.py` & `JBPhD-2.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 packagereqs = ['sendgrid', 'plyer', 'pygame', 'pandas', 'google-auth', 'google-auth-oauthlib', 'google-auth-httplib2', 'google-api-python-client', 'Pillow', 'Scipy', 'Numpy']
 
 with open('README.txt', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='JBPhD',
-    version='2.3.1',
+    version='2.3.2',
     packages=find_namespace_packages(include=['Task']),
     install_requires=packagereqs,
     entry_points={
         'console_scripts': [
             'myproject = myproject.main:main'
         ]
     },
```

