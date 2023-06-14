# Comparing `tmp/mailscrambler-0.1.1.tar.gz` & `tmp/mailscrambler-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailscrambler-0.1.1.tar", last modified: Wed Jun 14 06:31:50 2023, max compression
+gzip compressed data, was "mailscrambler-0.1.2.tar", last modified: Wed Jun 14 06:38:50 2023, max compression
```

## Comparing `mailscrambler-0.1.1.tar` & `mailscrambler-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 demetriobattaglia   (501) staff       (20)        0 2023-06-14 06:31:50.354987 mailscrambler-0.1.1/
--rw-r--r--   0 demetriobattaglia   (501) staff       (20)     1075 2023-06-08 08:48:52.000000 mailscrambler-0.1.1/LICENSE
--rw-r--r--   0 demetriobattaglia   (501) staff       (20)     4358 2023-06-14 06:31:50.354831 mailscrambler-0.1.1/PKG-INFO
--rw-r--r--   0 demetriobattaglia   (501) staff       (20)     3761 2023-06-14 06:31:10.000000 mailscrambler-0.1.1/README.md
--rw-r--r--   0 demetriobattaglia   (501) staff       (20)      588 2023-06-14 06:31:32.000000 mailscrambler-0.1.1/pyproject.toml
--rw-r--r--   0 demetriobattaglia   (501) staff       (20)       38 2023-06-14 06:31:50.355057 mailscrambler-0.1.1/setup.cfg
--rw-r--r--   0 demetriobattaglia   (501) staff       (20)      282 2023-06-08 09:08:26.000000 mailscrambler-0.1.1/setup.py
-drwxr-xr-x   0 demetriobattaglia   (501) staff       (20)        0 2023-06-14 06:31:50.351837 mailscrambler-0.1.1/src/
-drwxr-xr-x   0 demetriobattaglia   (501) staff       (20)        0 2023-06-14 06:31:50.353579 mailscrambler-0.1.1/src/mailscrambler/
--rw-r--r--   0 demetriobattaglia   (501) staff       (20)       92 2023-06-08 09:45:09.000000 mailscrambler-0.1.1/src/mailscrambler/__init__.py
--rw-r--r--   0 demetriobattaglia   (501) staff       (20)     4745 2023-06-14 06:24:09.000000 mailscrambler-0.1.1/src/mailscrambler/mailscrambler.py
-drwxr-xr-x   0 demetriobattaglia   (501) staff       (20)        0 2023-06-14 06:31:50.354620 mailscrambler-0.1.1/src/mailscrambler.egg-info/
--rw-r--r--   0 demetriobattaglia   (501) staff       (20)     4358 2023-06-14 06:31:50.000000 mailscrambler-0.1.1/src/mailscrambler.egg-info/PKG-INFO
--rw-r--r--   0 demetriobattaglia   (501) staff       (20)      270 2023-06-14 06:31:50.000000 mailscrambler-0.1.1/src/mailscrambler.egg-info/SOURCES.txt
--rw-r--r--   0 demetriobattaglia   (501) staff       (20)        1 2023-06-14 06:31:50.000000 mailscrambler-0.1.1/src/mailscrambler.egg-info/dependency_links.txt
--rw-r--r--   0 demetriobattaglia   (501) staff       (20)       14 2023-06-14 06:31:50.000000 mailscrambler-0.1.1/src/mailscrambler.egg-info/top_level.txt
+drwxr-xr-x   0 demetriobattaglia   (501) staff       (20)        0 2023-06-14 06:38:50.036020 mailscrambler-0.1.2/
+-rw-r--r--   0 demetriobattaglia   (501) staff       (20)     1075 2023-06-08 08:48:52.000000 mailscrambler-0.1.2/LICENSE
+-rw-r--r--   0 demetriobattaglia   (501) staff       (20)     4358 2023-06-14 06:38:50.035862 mailscrambler-0.1.2/PKG-INFO
+-rw-r--r--   0 demetriobattaglia   (501) staff       (20)     3761 2023-06-14 06:31:10.000000 mailscrambler-0.1.2/README.md
+-rw-r--r--   0 demetriobattaglia   (501) staff       (20)      588 2023-06-14 06:38:23.000000 mailscrambler-0.1.2/pyproject.toml
+-rw-r--r--   0 demetriobattaglia   (501) staff       (20)       38 2023-06-14 06:38:50.036094 mailscrambler-0.1.2/setup.cfg
+-rw-r--r--   0 demetriobattaglia   (501) staff       (20)      282 2023-06-08 09:08:26.000000 mailscrambler-0.1.2/setup.py
+drwxr-xr-x   0 demetriobattaglia   (501) staff       (20)        0 2023-06-14 06:38:50.032679 mailscrambler-0.1.2/src/
+drwxr-xr-x   0 demetriobattaglia   (501) staff       (20)        0 2023-06-14 06:38:50.034338 mailscrambler-0.1.2/src/mailscrambler/
+-rw-r--r--   0 demetriobattaglia   (501) staff       (20)       92 2023-06-08 09:45:09.000000 mailscrambler-0.1.2/src/mailscrambler/__init__.py
+-rw-r--r--   0 demetriobattaglia   (501) staff       (20)     4743 2023-06-14 06:38:04.000000 mailscrambler-0.1.2/src/mailscrambler/mailscrambler.py
+drwxr-xr-x   0 demetriobattaglia   (501) staff       (20)        0 2023-06-14 06:38:50.035605 mailscrambler-0.1.2/src/mailscrambler.egg-info/
+-rw-r--r--   0 demetriobattaglia   (501) staff       (20)     4358 2023-06-14 06:38:50.000000 mailscrambler-0.1.2/src/mailscrambler.egg-info/PKG-INFO
+-rw-r--r--   0 demetriobattaglia   (501) staff       (20)      270 2023-06-14 06:38:50.000000 mailscrambler-0.1.2/src/mailscrambler.egg-info/SOURCES.txt
+-rw-r--r--   0 demetriobattaglia   (501) staff       (20)        1 2023-06-14 06:38:50.000000 mailscrambler-0.1.2/src/mailscrambler.egg-info/dependency_links.txt
+-rw-r--r--   0 demetriobattaglia   (501) staff       (20)       14 2023-06-14 06:38:50.000000 mailscrambler-0.1.2/src/mailscrambler.egg-info/top_level.txt
```

### Comparing `mailscrambler-0.1.1/LICENSE` & `mailscrambler-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mailscrambler-0.1.1/PKG-INFO` & `mailscrambler-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailscrambler
-Version: 0.1.1
+Version: 0.1.2
 Summary: E-mail scrambling library
 Home-page: https://www.github.com/deme3/emailscrambler
 Author: Demetrio Battaglia
 Author-email: Demetrio Battaglia <deme3.iot@gmail.com>
 Project-URL: Homepage, https://github.com/deme3/emailscrambler
 Project-URL: Bug Tracker, https://github.com/deme3/emailscrambler/issues
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mailscrambler Version: 0.1.1 Summary: E-mail
+Metadata-Version: 2.1 Name: mailscrambler Version: 0.1.2 Summary: E-mail
 scrambling library Home-page: https://www.github.com/deme3/emailscrambler
 Author: Demetrio Battaglia Author-email: Demetrio Battaglia
 iot@gmail.com> Project-URL: Homepage, https://github.com/deme3/emailscrambler
 Project-URL: Bug Tracker, https://github.com/deme3/emailscrambler/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
```

### Comparing `mailscrambler-0.1.1/README.md` & `mailscrambler-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mailscrambler-0.1.1/pyproject.toml` & `mailscrambler-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mailscrambler"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Demetrio Battaglia", email="deme3.iot@gmail.com" },
 ]
 description = "E-mail scrambling library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mailscrambler-0.1.1/src/mailscrambler/mailscrambler.py` & `mailscrambler-0.1.2/src/mailscrambler/mailscrambler.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
   """Takes in an e-mail address and returns a JavaScript-enabled obfuscated mailto link"""
   if body:
     body = body.replace('\n', '%0D%0A')
 
   caption = (obfuscate(scramble(custom_caption)) if custom_caption else obfuscate(emailto)) if custom_caption else None
   mail_output = obfuscate(scramble(emailto)) if do_scramble else obfuscate(emailto)
   mail_body = (obfuscate(scramble(body)) if do_scramble else obfuscate(body)) if body else None
-  return '<script type="text/javascript">document.write(\'<a href="mailto:' + mail_output + '"' + (" data-scrambled" if do_scramble else "") + (f" data-body=\"{mail_body}\"" if body else None) + (f" data-custom-caption=\"{caption}\"" if custom_caption else '') + '>' + mail_output + '</a>\');</script>'
+  return '<script type="text/javascript">document.write(\'<a href="mailto:' + mail_output + '"' + (" data-scrambled" if do_scramble else "") + (f" data-body=\"{mail_body}\"" if body else "") + (f" data-custom-caption=\"{caption}\"" if custom_caption else '') + '>' + mail_output + '</a>\');</script>'
 
 def deobfuscator() -> str:
   """
     Code adapted from https://github.com/ThibWeb/email-scramble
     Licensed under ISC License, Copyright (c) 2016, Thibaud Colas
   """
   return """
```

### Comparing `mailscrambler-0.1.1/src/mailscrambler.egg-info/PKG-INFO` & `mailscrambler-0.1.2/src/mailscrambler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailscrambler
-Version: 0.1.1
+Version: 0.1.2
 Summary: E-mail scrambling library
 Home-page: https://www.github.com/deme3/emailscrambler
 Author: Demetrio Battaglia
 Author-email: Demetrio Battaglia <deme3.iot@gmail.com>
 Project-URL: Homepage, https://github.com/deme3/emailscrambler
 Project-URL: Bug Tracker, https://github.com/deme3/emailscrambler/issues
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mailscrambler Version: 0.1.1 Summary: E-mail
+Metadata-Version: 2.1 Name: mailscrambler Version: 0.1.2 Summary: E-mail
 scrambling library Home-page: https://www.github.com/deme3/emailscrambler
 Author: Demetrio Battaglia Author-email: Demetrio Battaglia
 iot@gmail.com> Project-URL: Homepage, https://github.com/deme3/emailscrambler
 Project-URL: Bug Tracker, https://github.com/deme3/emailscrambler/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
```

