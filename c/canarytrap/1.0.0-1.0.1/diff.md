# Comparing `tmp/canarytrap-1.0.0.tar.gz` & `tmp/canarytrap-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canarytrap-1.0.0.tar", last modified: Wed Jun 14 07:05:14 2023, max compression
+gzip compressed data, was "canarytrap-1.0.1.tar", last modified: Wed Jun 14 11:08:28 2023, max compression
```

## Comparing `canarytrap-1.0.0.tar` & `canarytrap-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 07:05:14.133394 canarytrap-1.0.0/
--rw-rw-rw-   0        0        0     1089 2023-06-14 05:49:00.000000 canarytrap-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2317 2023-06-14 07:05:14.132398 canarytrap-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2003 2023-06-14 06:58:49.000000 canarytrap-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 07:05:14.107465 canarytrap-1.0.0/canarytrap/
--rw-rw-rw-   0        0        0       52 2023-06-14 06:53:15.000000 canarytrap-1.0.0/canarytrap/__init__.py
--rw-rw-rw-   0        0        0     2999 2023-06-14 06:53:15.000000 canarytrap-1.0.0/canarytrap/text.py
-drwxrwxrwx   0        0        0        0 2023-06-14 07:05:14.127426 canarytrap-1.0.0/canarytrap.egg-info/
--rw-rw-rw-   0        0        0     2317 2023-06-14 07:05:14.000000 canarytrap-1.0.0/canarytrap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-06-14 07:05:14.000000 canarytrap-1.0.0/canarytrap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 07:05:14.000000 canarytrap-1.0.0/canarytrap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-14 07:05:14.000000 canarytrap-1.0.0/canarytrap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 07:05:14.133394 canarytrap-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      567 2023-06-14 07:03:39.000000 canarytrap-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 07:05:14.130403 canarytrap-1.0.0/tests/
--rw-rw-rw-   0        0        0        0 2023-06-14 06:31:21.000000 canarytrap-1.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0     1387 2023-06-14 06:54:28.000000 canarytrap-1.0.0/tests/test_text.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:08:28.695536 canarytrap-1.0.1/
+-rw-rw-rw-   0        0        0     1089 2023-06-14 10:51:47.000000 canarytrap-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2317 2023-06-14 11:08:28.694546 canarytrap-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2003 2023-06-14 10:51:47.000000 canarytrap-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 11:08:28.675840 canarytrap-1.0.1/canarytrap/
+-rw-rw-rw-   0        0        0       52 2023-06-14 10:51:47.000000 canarytrap-1.0.1/canarytrap/__init__.py
+-rw-rw-rw-   0        0        0     3324 2023-06-14 11:06:43.000000 canarytrap-1.0.1/canarytrap/text.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:08:28.690532 canarytrap-1.0.1/canarytrap.egg-info/
+-rw-rw-rw-   0        0        0     2317 2023-06-14 11:08:28.000000 canarytrap-1.0.1/canarytrap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-06-14 11:08:28.000000 canarytrap-1.0.1/canarytrap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 11:08:28.000000 canarytrap-1.0.1/canarytrap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-14 11:08:28.000000 canarytrap-1.0.1/canarytrap.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 11:08:28.695536 canarytrap-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      567 2023-06-14 11:07:11.000000 canarytrap-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:08:28.693537 canarytrap-1.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-14 10:51:47.000000 canarytrap-1.0.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     1827 2023-06-14 11:02:56.000000 canarytrap-1.0.1/tests/test_text.py
```

### Comparing `canarytrap-1.0.0/LICENSE` & `canarytrap-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `canarytrap-1.0.0/PKG-INFO` & `canarytrap-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canarytrap
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package to watermark text.
 Home-page: https://github.com/MatthewLeeCode/CanaryTrap
 Author: Matthew Lee
 Author-email: matthewleemattner@gmail.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `canarytrap-1.0.0/README.md` & `canarytrap-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `canarytrap-1.0.0/canarytrap/text.py` & `canarytrap-1.0.1/canarytrap/text.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,74 @@
 """
 Canary Trap for text
 """
 from typing import Tuple
 from random import randint
 
 
-def unicode_space_encode(text:str, binary:int|None = None) -> Tuple[str, str]:
+def unicode_space_encode(text:str, binary_string:str|None = None) -> Tuple[str, str]:
     """ Encode spaces in text to unicode spaces based on a binary value
 
     If the text has 12 spaces and the binary value is 1100, then the first 2 spaces will be unicode spaces.
     If no binary value is provided, then the binary value is randomized
 
     Args:
         text: The text to encode
-        binary: The binary value to use. Defaults to None.
+        binary: The binary value to use. Each 1 means a replacement of a space char with a blank char. 
+        Defaults to None.
 
     Returns:
         The encoded text and the binary value used
 
     Raises:
         ValueError: If the binary value (in terms of string length) is too large for the number of spaces in the text
     """
     blank_space = "\u200E"
     space_count = text.count(" ")
     space_indicies = [i for i, char in enumerate(text) if char == " "]
 
-    if binary is None:
+    if binary_string is None:
         binary = randint(0, 2**space_count - 1)
+        binary_string = bin(binary)[2:]
 
-    # Check if binary length (not number) is less than space count
-    binary_string = bin(binary)[2:]
     if len(binary_string) > space_count:
         raise ValueError("The length of the binary string is too large for the number of spaces in the text")
 
     # For all instances of '1', replcae the next space
     text_list = list(text)
     for i, space_index in zip(range(len(binary_string)), space_indicies):
         if binary_string[i] == '1':
             text_list[space_index] = blank_space
     
     text = "".join(text_list)
+    text = text.replace(blank_space, f"{blank_space} ")
+    binary_string = unicode_space_to_binary_str(text)
     return text, binary_string
 
 
 def unicode_space_to_binary_str(text:str) -> str:
     """ Convert unicode spaces to binary
 
     Args:
         text: The text to convert
 
     Returns:
         The binary string
     """
     blank_space = "\u200E"
     binary_string = ""
-
+    
+    skip_next = False 
     for char in text:
+        if skip_next:
+            skip_next = False
+            continue
         if char == blank_space:
             binary_string += "1"
+            skip_next = True
         elif char == " ":
             binary_string += "0"
     
     return binary_string
 
 
 def unicode_space_match(text:str, binary_str:str) -> float:
@@ -77,14 +84,15 @@
     Example:
         >>> text = "Hello world[unicode]this[unicode]is text"
         >>> binary = 0b0101 # Only half the values match where the unicode is
         >>> unicode_space_match(text, binary) 
         0.5
     """
     blank_space = "\u200E"
+    text = text.replace(f"{blank_space} ", blank_space)
     space_count = text.count(" ") + text.count(blank_space)
     space_indicies = [i for i, char in enumerate(text) if char == " " or char == blank_space]
 
     match_count = 0
     for bin_val, space_index in zip(binary_str, space_indicies):
         if bin_val == '1' and text[space_index] == blank_space:
             match_count += 1
```

### Comparing `canarytrap-1.0.0/canarytrap.egg-info/PKG-INFO` & `canarytrap-1.0.1/canarytrap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canarytrap
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package to watermark text.
 Home-page: https://github.com/MatthewLeeCode/CanaryTrap
 Author: Matthew Lee
 Author-email: matthewleemattner@gmail.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `canarytrap-1.0.0/setup.py` & `canarytrap-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="canarytrap",
-    version="1.0.0",
+    version="1.0.1",
     description="A Python package to watermark text.",
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     author="Matthew Lee",
     author_email="matthewleemattner@gmail.com",
     url="https://github.com/MatthewLeeCode/CanaryTrap",
     packages=find_packages(),
```

