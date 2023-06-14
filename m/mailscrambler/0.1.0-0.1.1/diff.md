# Comparing `tmp/mailscrambler-0.1.0.tar.gz` & `tmp/mailscrambler-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailscrambler-0.1.0.tar", last modified: Wed Jun 14 06:25:18 2023, max compression
+gzip compressed data, was "mailscrambler-0.1.1.tar", last modified: Wed Jun 14 06:31:50 2023, max compression
```

## Comparing `mailscrambler-0.1.0.tar` & `mailscrambler-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 demetriobattaglia   (501) staff       (20)        0 2023-06-14 06:25:18.045060 mailscrambler-0.1.0/
--rw-r--r--   0 demetriobattaglia   (501) staff       (20)     1075 2023-06-08 08:48:52.000000 mailscrambler-0.1.0/LICENSE
--rw-r--r--   0 demetriobattaglia   (501) staff       (20)     3309 2023-06-14 06:25:18.044892 mailscrambler-0.1.0/PKG-INFO
--rw-r--r--   0 demetriobattaglia   (501) staff       (20)     2712 2023-06-08 10:03:37.000000 mailscrambler-0.1.0/README.md
--rw-r--r--   0 demetriobattaglia   (501) staff       (20)      588 2023-06-13 13:10:48.000000 mailscrambler-0.1.0/pyproject.toml
--rw-r--r--   0 demetriobattaglia   (501) staff       (20)       38 2023-06-14 06:25:18.045121 mailscrambler-0.1.0/setup.cfg
--rw-r--r--   0 demetriobattaglia   (501) staff       (20)      282 2023-06-08 09:08:26.000000 mailscrambler-0.1.0/setup.py
-drwxr-xr-x   0 demetriobattaglia   (501) staff       (20)        0 2023-06-14 06:25:18.041867 mailscrambler-0.1.0/src/
-drwxr-xr-x   0 demetriobattaglia   (501) staff       (20)        0 2023-06-14 06:25:18.043660 mailscrambler-0.1.0/src/mailscrambler/
--rw-r--r--   0 demetriobattaglia   (501) staff       (20)       92 2023-06-08 09:45:09.000000 mailscrambler-0.1.0/src/mailscrambler/__init__.py
--rw-r--r--   0 demetriobattaglia   (501) staff       (20)     4745 2023-06-14 06:24:09.000000 mailscrambler-0.1.0/src/mailscrambler/mailscrambler.py
-drwxr-xr-x   0 demetriobattaglia   (501) staff       (20)        0 2023-06-14 06:25:18.044661 mailscrambler-0.1.0/src/mailscrambler.egg-info/
--rw-r--r--   0 demetriobattaglia   (501) staff       (20)     3309 2023-06-14 06:25:18.000000 mailscrambler-0.1.0/src/mailscrambler.egg-info/PKG-INFO
--rw-r--r--   0 demetriobattaglia   (501) staff       (20)      270 2023-06-14 06:25:18.000000 mailscrambler-0.1.0/src/mailscrambler.egg-info/SOURCES.txt
--rw-r--r--   0 demetriobattaglia   (501) staff       (20)        1 2023-06-14 06:25:18.000000 mailscrambler-0.1.0/src/mailscrambler.egg-info/dependency_links.txt
--rw-r--r--   0 demetriobattaglia   (501) staff       (20)       14 2023-06-14 06:25:18.000000 mailscrambler-0.1.0/src/mailscrambler.egg-info/top_level.txt
+drwxr-xr-x   0 demetriobattaglia   (501) staff       (20)        0 2023-06-14 06:31:50.354987 mailscrambler-0.1.1/
+-rw-r--r--   0 demetriobattaglia   (501) staff       (20)     1075 2023-06-08 08:48:52.000000 mailscrambler-0.1.1/LICENSE
+-rw-r--r--   0 demetriobattaglia   (501) staff       (20)     4358 2023-06-14 06:31:50.354831 mailscrambler-0.1.1/PKG-INFO
+-rw-r--r--   0 demetriobattaglia   (501) staff       (20)     3761 2023-06-14 06:31:10.000000 mailscrambler-0.1.1/README.md
+-rw-r--r--   0 demetriobattaglia   (501) staff       (20)      588 2023-06-14 06:31:32.000000 mailscrambler-0.1.1/pyproject.toml
+-rw-r--r--   0 demetriobattaglia   (501) staff       (20)       38 2023-06-14 06:31:50.355057 mailscrambler-0.1.1/setup.cfg
+-rw-r--r--   0 demetriobattaglia   (501) staff       (20)      282 2023-06-08 09:08:26.000000 mailscrambler-0.1.1/setup.py
+drwxr-xr-x   0 demetriobattaglia   (501) staff       (20)        0 2023-06-14 06:31:50.351837 mailscrambler-0.1.1/src/
+drwxr-xr-x   0 demetriobattaglia   (501) staff       (20)        0 2023-06-14 06:31:50.353579 mailscrambler-0.1.1/src/mailscrambler/
+-rw-r--r--   0 demetriobattaglia   (501) staff       (20)       92 2023-06-08 09:45:09.000000 mailscrambler-0.1.1/src/mailscrambler/__init__.py
+-rw-r--r--   0 demetriobattaglia   (501) staff       (20)     4745 2023-06-14 06:24:09.000000 mailscrambler-0.1.1/src/mailscrambler/mailscrambler.py
+drwxr-xr-x   0 demetriobattaglia   (501) staff       (20)        0 2023-06-14 06:31:50.354620 mailscrambler-0.1.1/src/mailscrambler.egg-info/
+-rw-r--r--   0 demetriobattaglia   (501) staff       (20)     4358 2023-06-14 06:31:50.000000 mailscrambler-0.1.1/src/mailscrambler.egg-info/PKG-INFO
+-rw-r--r--   0 demetriobattaglia   (501) staff       (20)      270 2023-06-14 06:31:50.000000 mailscrambler-0.1.1/src/mailscrambler.egg-info/SOURCES.txt
+-rw-r--r--   0 demetriobattaglia   (501) staff       (20)        1 2023-06-14 06:31:50.000000 mailscrambler-0.1.1/src/mailscrambler.egg-info/dependency_links.txt
+-rw-r--r--   0 demetriobattaglia   (501) staff       (20)       14 2023-06-14 06:31:50.000000 mailscrambler-0.1.1/src/mailscrambler.egg-info/top_level.txt
```

### Comparing `mailscrambler-0.1.0/LICENSE` & `mailscrambler-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mailscrambler-0.1.0/PKG-INFO` & `mailscrambler-0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailscrambler
-Version: 0.1.0
+Version: 0.1.1
 Summary: E-mail scrambling library
 Home-page: https://www.github.com/deme3/emailscrambler
 Author: Demetrio Battaglia
 Author-email: Demetrio Battaglia <deme3.iot@gmail.com>
 Project-URL: Homepage, https://github.com/deme3/emailscrambler
 Project-URL: Bug Tracker, https://github.com/deme3/emailscrambler/issues
 Classifier: Programming Language :: Python :: 3
@@ -47,14 +47,20 @@
 """
 
 # Combine scramble and obfuscate
 link = javascriptify('test@email.com', do_scramble=True)
 """
 <script type="text/javascript">document.write('<a href="mailto:&#x67;&#x72;&#x66;&#x67;&#x40;&#x72;&#x7a;&#x6e;&#x76;&#x79;&#x2e;&#x70;&#x62;&#x7a;" data-scrambled>&#x67;&#x72;&#x66;&#x67;&#x40;&#x72;&#x7a;&#x6e;&#x76;&#x79;&#x2e;&#x70;&#x62;&#x7a;</a>');</script>
 """
+
+# "Click <here> to report your issue":
+support_email = javascriptify('support@test.com', body='Name: \nProduct you encountered the issue with: \nYour issue:\n', custom_caption='here', do_scramble=True)
+"""
+Click {support_email} to report your issue
+<script type="text/javascript">document.write('<a href="mailto:&#x66;&#x68;&#x63;&#x63;&#x62;&#x65;&#x67;&#x40;&#x67;&#x72;&#x66;&#x67;&#x2e;&#x70;&#x62;&#x7a;" data-scrambled data-body="&#x41;&#x6e;&#x7a;&#x72;&#x3a;&#x20;&#x25;&#x35;&#x51;&#x25;&#x35;&#x4e;&#x43;&#x65;&#x62;&#x71;&#x68;&#x70;&#x67;&#x20;&#x6c;&#x62;&#x68;&#x20;&#x72;&#x61;&#x70;&#x62;&#x68;&#x61;&#x67;&#x72;&#x65;&#x72;&#x71;&#x20;&#x67;&#x75;&#x72;&#x20;&#x76;&#x66;&#x66;&#x68;&#x72;&#x20;&#x6a;&#x76;&#x67;&#x75;&#x3a;&#x20;&#x25;&#x35;&#x51;&#x25;&#x35;&#x4e;&#x4c;&#x62;&#x68;&#x65;&#x20;&#x76;&#x66;&#x66;&#x68;&#x72;&#x3a;&#x25;&#x35;&#x51;&#x25;&#x35;&#x4e;" data-custom-caption="&#x75;&#x72;&#x65;&#x72;">&#x66;&#x68;&#x63;&#x63;&#x62;&#x65;&#x67;&#x40;&#x67;&#x72;&#x66;&#x67;&#x2e;&#x70;&#x62;&#x7a;</a>');</script>
 ```
 
 To embed a deobfuscator in your HTML page, you can call the `deobfuscator` function:
 
 ```python
 from mailscrambler import deobfuscator
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mailscrambler Version: 0.1.0 Summary: E-mail
+Metadata-Version: 2.1 Name: mailscrambler Version: 0.1.1 Summary: E-mail
 scrambling library Home-page: https://www.github.com/deme3/emailscrambler
 Author: Demetrio Battaglia Author-email: Demetrio Battaglia
 iot@gmail.com> Project-URL: Homepage, https://github.com/deme3/emailscrambler
 Project-URL: Bug Tracker, https://github.com/deme3/emailscrambler/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
@@ -13,26 +13,30 @@
 Scramble an email address scrambled = scramble('test@email.com') print
 (scrambled) # grfg@rznvy.pbz # Obfuscate an email address obfuscated =
 obfuscate('test@email.com') print(obfuscated) """
 &#x74;&#x65;&#x73;&#x74;&#x40;&#x65;&#x6d;&#x61;&#x69;&#x6c;&#x2e;&#x63;&#x6f;&#x6d;
 """ # HTML Embeddable link = javascriptify('test@email.com') """
  """ # Combine scramble and obfuscate link = javascriptify('test@email.com',
 do_scramble=True) """
- """ ``` To embed a deobfuscator in your HTML page, you can call the
-`deobfuscator` function: ```python from mailscrambler import deobfuscator #
-[...] # Embed the deobfuscator page_body += javascriptify('test@email.com',
-do_scramble=True) page_body += deobfuscator() # [...] ``` Note that unless
-scrambling is used, deobfuscator is not necessary. ## License MIT License ```
-MIT License Copyright (c) 2023 Demetrio Battaglia Permission is hereby granted,
-free of charge, to any person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the Software without
-restriction, including without limitation the rights to use, copy, modify,
-merge, publish, distribute, sublicense, and/or sell copies of the Software, and
-to permit persons to whom the Software is furnished to do so, subject to the
-following conditions: The above copyright notice and this permission notice
-shall be included in all copies or substantial portions of the Software. THE
-SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
-INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. ```
+ """ # "Click  to report your issue": support_email = javascriptify
+('support@test.com', body='Name: \nProduct you encountered the issue with:
+\nYour issue:\n', custom_caption='here', do_scramble=True) """ Click
+{support_email} to report your issue
+ ``` To embed a deobfuscator in your HTML page, you can call the `deobfuscator`
+function: ```python from mailscrambler import deobfuscator # [...] # Embed the
+deobfuscator page_body += javascriptify('test@email.com', do_scramble=True)
+page_body += deobfuscator() # [...] ``` Note that unless scrambling is used,
+deobfuscator is not necessary. ## License MIT License ``` MIT License Copyright
+(c) 2023 Demetrio Battaglia Permission is hereby granted, free of charge, to
+any person obtaining a copy of this software and associated documentation files
+(the "Software"), to deal in the Software without restriction, including
+without limitation the rights to use, copy, modify, merge, publish, distribute,
+sublicense, and/or sell copies of the Software, and to permit persons to whom
+the Software is furnished to do so, subject to the following conditions: The
+above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS
+IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
+LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE
+AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
+CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
+SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. ```
```

### Comparing `mailscrambler-0.1.0/README.md` & `mailscrambler-0.1.1/src/mailscrambler.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: mailscrambler
+Version: 0.1.1
+Summary: E-mail scrambling library
+Home-page: https://www.github.com/deme3/emailscrambler
+Author: Demetrio Battaglia
+Author-email: Demetrio Battaglia <deme3.iot@gmail.com>
+Project-URL: Homepage, https://github.com/deme3/emailscrambler
+Project-URL: Bug Tracker, https://github.com/deme3/emailscrambler/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # mailscrambler
 
 A simple Python library to scramble and obfuscate email addresses in HTML pages, also comes with JavaScript deobfuscator.
 
 ## Installation
 
 ```bash
@@ -31,14 +47,20 @@
 """
 
 # Combine scramble and obfuscate
 link = javascriptify('test@email.com', do_scramble=True)
 """
 <script type="text/javascript">document.write('<a href="mailto:&#x67;&#x72;&#x66;&#x67;&#x40;&#x72;&#x7a;&#x6e;&#x76;&#x79;&#x2e;&#x70;&#x62;&#x7a;" data-scrambled>&#x67;&#x72;&#x66;&#x67;&#x40;&#x72;&#x7a;&#x6e;&#x76;&#x79;&#x2e;&#x70;&#x62;&#x7a;</a>');</script>
 """
+
+# "Click <here> to report your issue":
+support_email = javascriptify('support@test.com', body='Name: \nProduct you encountered the issue with: \nYour issue:\n', custom_caption='here', do_scramble=True)
+"""
+Click {support_email} to report your issue
+<script type="text/javascript">document.write('<a href="mailto:&#x66;&#x68;&#x63;&#x63;&#x62;&#x65;&#x67;&#x40;&#x67;&#x72;&#x66;&#x67;&#x2e;&#x70;&#x62;&#x7a;" data-scrambled data-body="&#x41;&#x6e;&#x7a;&#x72;&#x3a;&#x20;&#x25;&#x35;&#x51;&#x25;&#x35;&#x4e;&#x43;&#x65;&#x62;&#x71;&#x68;&#x70;&#x67;&#x20;&#x6c;&#x62;&#x68;&#x20;&#x72;&#x61;&#x70;&#x62;&#x68;&#x61;&#x67;&#x72;&#x65;&#x72;&#x71;&#x20;&#x67;&#x75;&#x72;&#x20;&#x76;&#x66;&#x66;&#x68;&#x72;&#x20;&#x6a;&#x76;&#x67;&#x75;&#x3a;&#x20;&#x25;&#x35;&#x51;&#x25;&#x35;&#x4e;&#x4c;&#x62;&#x68;&#x65;&#x20;&#x76;&#x66;&#x66;&#x68;&#x72;&#x3a;&#x25;&#x35;&#x51;&#x25;&#x35;&#x4e;" data-custom-caption="&#x75;&#x72;&#x65;&#x72;">&#x66;&#x68;&#x63;&#x63;&#x62;&#x65;&#x67;&#x40;&#x67;&#x72;&#x66;&#x67;&#x2e;&#x70;&#x62;&#x7a;</a>');</script>
 ```
 
 To embed a deobfuscator in your HTML page, you can call the `deobfuscator` function:
 
 ```python
 from mailscrambler import deobfuscator
```

#### html2text {}

```diff
@@ -1,30 +1,42 @@
-# mailscrambler A simple Python library to scramble and obfuscate email
+Metadata-Version: 2.1 Name: mailscrambler Version: 0.1.1 Summary: E-mail
+scrambling library Home-page: https://www.github.com/deme3/emailscrambler
+Author: Demetrio Battaglia Author-email: Demetrio Battaglia
+iot@gmail.com> Project-URL: Homepage, https://github.com/deme3/emailscrambler
+Project-URL: Bug Tracker, https://github.com/deme3/emailscrambler/issues
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
+LICENSE # mailscrambler A simple Python library to scramble and obfuscate email
 addresses in HTML pages, also comes with JavaScript deobfuscator. ##
 Installation ```bash pip install mailscrambler ``` ## Usage ```python from
 mailscrambler import scramble, obfuscate, javascriptify, deobfuscator #
 Scramble an email address scrambled = scramble('test@email.com') print
 (scrambled) # grfg@rznvy.pbz # Obfuscate an email address obfuscated =
 obfuscate('test@email.com') print(obfuscated) """
 &#x74;&#x65;&#x73;&#x74;&#x40;&#x65;&#x6d;&#x61;&#x69;&#x6c;&#x2e;&#x63;&#x6f;&#x6d;
 """ # HTML Embeddable link = javascriptify('test@email.com') """
  """ # Combine scramble and obfuscate link = javascriptify('test@email.com',
 do_scramble=True) """
- """ ``` To embed a deobfuscator in your HTML page, you can call the
-`deobfuscator` function: ```python from mailscrambler import deobfuscator #
-[...] # Embed the deobfuscator page_body += javascriptify('test@email.com',
-do_scramble=True) page_body += deobfuscator() # [...] ``` Note that unless
-scrambling is used, deobfuscator is not necessary. ## License MIT License ```
-MIT License Copyright (c) 2023 Demetrio Battaglia Permission is hereby granted,
-free of charge, to any person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the Software without
-restriction, including without limitation the rights to use, copy, modify,
-merge, publish, distribute, sublicense, and/or sell copies of the Software, and
-to permit persons to whom the Software is furnished to do so, subject to the
-following conditions: The above copyright notice and this permission notice
-shall be included in all copies or substantial portions of the Software. THE
-SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
-INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. ```
+ """ # "Click  to report your issue": support_email = javascriptify
+('support@test.com', body='Name: \nProduct you encountered the issue with:
+\nYour issue:\n', custom_caption='here', do_scramble=True) """ Click
+{support_email} to report your issue
+ ``` To embed a deobfuscator in your HTML page, you can call the `deobfuscator`
+function: ```python from mailscrambler import deobfuscator # [...] # Embed the
+deobfuscator page_body += javascriptify('test@email.com', do_scramble=True)
+page_body += deobfuscator() # [...] ``` Note that unless scrambling is used,
+deobfuscator is not necessary. ## License MIT License ``` MIT License Copyright
+(c) 2023 Demetrio Battaglia Permission is hereby granted, free of charge, to
+any person obtaining a copy of this software and associated documentation files
+(the "Software"), to deal in the Software without restriction, including
+without limitation the rights to use, copy, modify, merge, publish, distribute,
+sublicense, and/or sell copies of the Software, and to permit persons to whom
+the Software is furnished to do so, subject to the following conditions: The
+above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS
+IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
+LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE
+AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
+CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
+SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. ```
```

### Comparing `mailscrambler-0.1.0/pyproject.toml` & `mailscrambler-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mailscrambler"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Demetrio Battaglia", email="deme3.iot@gmail.com" },
 ]
 description = "E-mail scrambling library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mailscrambler-0.1.0/src/mailscrambler/mailscrambler.py` & `mailscrambler-0.1.1/src/mailscrambler/mailscrambler.py`

 * *Files identical despite different names*

