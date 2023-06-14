# Comparing `tmp/Flask-PyTelegramBotAPI-0.0.1.tar.gz` & `tmp/Flask-PyTelegramBotAPI-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Flask-PyTelegramBotAPI-0.0.1.tar", last modified: Wed Jun 14 20:29:58 2023, max compression
+gzip compressed data, was "dist/Flask-PyTelegramBotAPI-0.0.2.tar", last modified: Wed Jun 14 20:47:23 2023, max compression
```

## Comparing `Flask-PyTelegramBotAPI-0.0.1.tar` & `Flask-PyTelegramBotAPI-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 20:29:58.033043 Flask-PyTelegramBotAPI-0.0.1/
-drwxrwxr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 20:29:58.033043 Flask-PyTelegramBotAPI-0.0.1/Flask_PyTelegramBotAPI.egg-info/
--rw-rw-r--   0 sergey    (1000) sergey    (1000)      106 2023-06-14 20:29:57.000000 Flask-PyTelegramBotAPI-0.0.1/Flask_PyTelegramBotAPI.egg-info/PKG-INFO
--rw-rw-r--   0 sergey    (1000) sergey    (1000)      417 2023-06-14 20:29:58.000000 Flask-PyTelegramBotAPI-0.0.1/Flask_PyTelegramBotAPI.egg-info/SOURCES.txt
--rw-rw-r--   0 sergey    (1000) sergey    (1000)        1 2023-06-14 20:29:57.000000 Flask-PyTelegramBotAPI-0.0.1/Flask_PyTelegramBotAPI.egg-info/dependency_links.txt
--rw-rw-r--   0 sergey    (1000) sergey    (1000)        8 2023-06-14 20:29:57.000000 Flask-PyTelegramBotAPI-0.0.1/Flask_PyTelegramBotAPI.egg-info/requires.txt
--rw-rw-r--   0 sergey    (1000) sergey    (1000)       27 2023-06-14 20:29:57.000000 Flask-PyTelegramBotAPI-0.0.1/Flask_PyTelegramBotAPI.egg-info/top_level.txt
--rw-rw-r--   0 sergey    (1000) sergey    (1000)    18092 2023-05-15 06:48:50.000000 Flask-PyTelegramBotAPI-0.0.1/LICENSE
--rw-rw-r--   0 sergey    (1000) sergey    (1000)      106 2023-06-14 20:29:58.033043 Flask-PyTelegramBotAPI-0.0.1/PKG-INFO
--rw-rw-r--   0 sergey    (1000) sergey    (1000)       24 2023-05-15 06:48:50.000000 Flask-PyTelegramBotAPI-0.0.1/README.md
--rw-rw-r--   0 sergey    (1000) sergey    (1000)       38 2023-06-14 20:29:58.037043 Flask-PyTelegramBotAPI-0.0.1/setup.cfg
--rw-rw-r--   0 sergey    (1000) sergey    (1000)      275 2023-06-14 20:10:00.000000 Flask-PyTelegramBotAPI-0.0.1/setup.py
-drwxrwxr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 20:29:58.033043 Flask-PyTelegramBotAPI-0.0.1/src/
-drwxrwxr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 20:29:58.033043 Flask-PyTelegramBotAPI-0.0.1/src/flask_pytelegrambotapi/
--rw-rw-r--   0 sergey    (1000) sergey    (1000)      227 2023-06-03 20:00:47.000000 Flask-PyTelegramBotAPI-0.0.1/src/flask_pytelegrambotapi/__init__.py
--rw-rw-r--   0 sergey    (1000) sergey    (1000)     3972 2023-06-07 20:26:12.000000 Flask-PyTelegramBotAPI-0.0.1/src/flask_pytelegrambotapi/extension.py
--rw-rw-r--   0 sergey    (1000) sergey    (1000)       67 2023-05-17 09:35:36.000000 Flask-PyTelegramBotAPI-0.0.1/src/flask_pytelegrambotapi/mixins.py
--rw-rw-r--   0 sergey    (1000) sergey    (1000)      461 2023-05-16 11:59:07.000000 Flask-PyTelegramBotAPI-0.0.1/src/flask_pytelegrambotapi/utils.py
+drwxrwxr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 20:47:23.873468 Flask-PyTelegramBotAPI-0.0.2/
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)    18092 2023-05-15 06:48:50.000000 Flask-PyTelegramBotAPI-0.0.2/LICENSE
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)      161 2023-06-14 20:47:23.873468 Flask-PyTelegramBotAPI-0.0.2/PKG-INFO
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)       24 2023-05-15 06:48:50.000000 Flask-PyTelegramBotAPI-0.0.2/README.md
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)       38 2023-06-14 20:47:23.873468 Flask-PyTelegramBotAPI-0.0.2/setup.cfg
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)      373 2023-06-14 20:46:39.000000 Flask-PyTelegramBotAPI-0.0.2/setup.py
+drwxrwxr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 20:47:23.873468 Flask-PyTelegramBotAPI-0.0.2/src/
+drwxrwxr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 20:47:23.873468 Flask-PyTelegramBotAPI-0.0.2/src/Flask_PyTelegramBotAPI.egg-info/
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)      161 2023-06-14 20:47:23.000000 Flask-PyTelegramBotAPI-0.0.2/src/Flask_PyTelegramBotAPI.egg-info/PKG-INFO
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)      437 2023-06-14 20:47:23.000000 Flask-PyTelegramBotAPI-0.0.2/src/Flask_PyTelegramBotAPI.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)        1 2023-06-14 20:47:23.000000 Flask-PyTelegramBotAPI-0.0.2/src/Flask_PyTelegramBotAPI.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)        8 2023-06-14 20:47:23.000000 Flask-PyTelegramBotAPI-0.0.2/src/Flask_PyTelegramBotAPI.egg-info/requires.txt
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)       23 2023-06-14 20:47:23.000000 Flask-PyTelegramBotAPI-0.0.2/src/Flask_PyTelegramBotAPI.egg-info/top_level.txt
+drwxrwxr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 20:47:23.873468 Flask-PyTelegramBotAPI-0.0.2/src/flask_pytelegrambotapi/
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)      227 2023-06-03 20:00:47.000000 Flask-PyTelegramBotAPI-0.0.2/src/flask_pytelegrambotapi/__init__.py
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)     3972 2023-06-07 20:26:12.000000 Flask-PyTelegramBotAPI-0.0.2/src/flask_pytelegrambotapi/extension.py
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)       67 2023-05-17 09:35:36.000000 Flask-PyTelegramBotAPI-0.0.2/src/flask_pytelegrambotapi/mixins.py
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)      461 2023-05-16 11:59:07.000000 Flask-PyTelegramBotAPI-0.0.2/src/flask_pytelegrambotapi/utils.py
```

### Comparing `Flask-PyTelegramBotAPI-0.0.1/LICENSE` & `Flask-PyTelegramBotAPI-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-PyTelegramBotAPI-0.0.1/src/flask_pytelegrambotapi/extension.py` & `Flask-PyTelegramBotAPI-0.0.2/src/flask_pytelegrambotapi/extension.py`

 * *Files identical despite different names*

