# Comparing `tmp/aznt-0.0.41.tar.gz` & `tmp/aznt-0.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aznt-0.0.41.tar", last modified: Wed Mar 22 20:32:56 2023, max compression
+gzip compressed data, was "aznt-0.0.42.tar", last modified: Wed Jun 14 07:49:58 2023, max compression
```

## Comparing `aznt-0.0.41.tar` & `aznt-0.0.42.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 20:32:56.925668 aznt-0.0.41/
--rw-rw-rw-   0        0        0     1090 2023-01-31 09:03:04.000000 aznt-0.0.41/LICENCE.txt
--rw-rw-rw-   0        0        0       76 2023-03-22 20:32:15.000000 aznt-0.0.41/MANIFEST.in
--rw-rw-rw-   0        0        0    17061 2023-03-22 20:32:56.925668 aznt-0.0.41/PKG-INFO
--rw-rw-rw-   0        0        0    15982 2023-03-22 20:32:19.000000 aznt-0.0.41/README.md
-drwxrwxrwx   0        0        0        0 2023-03-22 20:32:56.878806 aznt-0.0.41/aznt/
--rw-rw-rw-   0        0        0        1 2023-01-31 09:03:08.000000 aznt-0.0.41/aznt/__init__.py
--rw-rw-rw-   0        0        0     8771 2023-01-31 09:03:08.000000 aznt-0.0.41/aznt/azntnumbers.py
--rw-rw-rw-   0        0        0     3360 2023-03-21 18:07:27.000000 aznt-0.0.41/aznt/azntplots.py
--rw-rw-rw-   0        0        0     1180 2023-01-31 09:03:08.000000 aznt-0.0.41/aznt/azntprimality.py
-drwxrwxrwx   0        0        0        0 2023-03-22 20:32:56.910050 aznt-0.0.41/aznt.egg-info/
--rw-rw-rw-   0        0        0    17061 2023-03-22 20:32:56.000000 aznt-0.0.41/aznt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-03-22 20:32:56.000000 aznt-0.0.41/aznt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 20:32:56.000000 aznt-0.0.41/aznt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-03-22 20:32:56.000000 aznt-0.0.41/aznt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-22 20:32:56.000000 aznt-0.0.41/aznt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1119 2023-03-22 20:32:23.000000 aznt-0.0.41/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-22 20:32:56.925668 aznt-0.0.41/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-14 07:49:58.451474 aznt-0.0.42/
+-rw-rw-rw-   0        0        0     1090 2023-01-31 07:03:04.000000 aznt-0.0.42/LICENCE.txt
+-rw-rw-rw-   0        0        0       76 2023-03-22 18:32:20.000000 aznt-0.0.42/MANIFEST.in
+-rw-rw-rw-   0        0        0    17530 2023-06-14 07:49:58.451474 aznt-0.0.42/PKG-INFO
+-rw-rw-rw-   0        0        0    16451 2023-06-14 07:46:49.000000 aznt-0.0.42/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 07:49:58.420199 aznt-0.0.42/aznt/
+-rw-rw-rw-   0        0        0        1 2023-01-31 07:04:46.000000 aznt-0.0.42/aznt/__init__.py
+-rw-rw-rw-   0        0        0     9463 2023-06-14 07:27:03.000000 aznt-0.0.42/aznt/azntnumbers.py
+-rw-rw-rw-   0        0        0     3360 2023-03-21 16:09:46.000000 aznt-0.0.42/aznt/azntplots.py
+-rw-rw-rw-   0        0        0     1180 2023-03-21 16:09:56.000000 aznt-0.0.42/aznt/azntprimality.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:49:58.451474 aznt-0.0.42/aznt.egg-info/
+-rw-rw-rw-   0        0        0    17530 2023-06-14 07:49:58.000000 aznt-0.0.42/aznt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-06-14 07:49:58.000000 aznt-0.0.42/aznt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 07:49:58.000000 aznt-0.0.42/aznt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-14 07:49:58.000000 aznt-0.0.42/aznt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-14 07:49:58.000000 aznt-0.0.42/aznt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1119 2023-06-14 07:49:27.000000 aznt-0.0.42/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 07:49:58.451474 aznt-0.0.42/setup.cfg
```

### Comparing `aznt-0.0.41/LICENCE.txt` & `aznt-0.0.42/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `aznt-0.0.41/PKG-INFO` & `aznt-0.0.42/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aznt
-Version: 0.0.41
+Version: 0.0.42
 Summary: From A to Z Number Theory
 Author-email: "Adrian Zapała, MSc" <adrian.zapala@outlook.com>
 Keywords: aznt,numbers,number theory,primes,prime numbers,math
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
@@ -19,15 +19,15 @@
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 ![Python Version](https://img.shields.io/badge/python-3.11-blue/)
-![aznt version](https://img.shields.io/badge/aznt-0.0.41-green)
+![aznt version](https://img.shields.io/badge/aznt-0.0.42-green)
 ![Beta version](https://img.shields.io/badge/beta-ver.-green)
 
 # `aznt` - From A to Z Number Theory
 
 * Number Theory library for Python with prime numbers.
 * **Important:** requires Python >= 3.11.
 * You can pass to author's GitHub at
@@ -449,14 +449,24 @@
 >>> pstats3(3)
     x                  π(x)                       PNT: Li(x)                Li(x) - π(x)         (Li(x) - π(x)) / π(x) [%]   
 1e+01     4                             6.165599504787298             2.165600                 54.139988                     
 1e+02     25                            30.12614158407963             5.126142                 20.504566                     
 1e+03     168                           177.60965799015221            9.609658                 5.720035
 ```
 
+## `fib()`
+Return dictionary of Fibonacci numbers from `0` to `n`. Key is an index, and a value is a specific Fibonacci number. First must create `Fibonacci` class object and then call `fib()` method on it.
+Time complexity: `O(n)`.<br>
+**<span style="color: coral">Examples</span>**
+```python
+>>> fob = Fibonacci(15)
+>>> print(fob.fib())
+{0: 0, 1: 1, 2: 1, 3: 2, 4: 3, 5: 5, 6: 8, 7: 13, 8: 21, 9: 34, 10: 55, 11: 89, 12: 144, 13: 233, 14: 377, 15: 610}
+```
+
 # Usage: `azntprimality` module functions
 
 ## `is_prime_naive1(n)`
 Return if number is a prime.
 Time complexity: `O(n)`.<br>
 **<span style="color: coral">Examples</span>**
 ```python
```

### Comparing `aznt-0.0.41/README.md` & `aznt-0.0.42/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ![Python Version](https://img.shields.io/badge/python-3.11-blue/)
-![aznt version](https://img.shields.io/badge/aznt-0.0.41-green)
+![aznt version](https://img.shields.io/badge/aznt-0.0.42-green)
 ![Beta version](https://img.shields.io/badge/beta-ver.-green)
 
 # `aznt` - From A to Z Number Theory
 
 * Number Theory library for Python with prime numbers.
 * **Important:** requires Python >= 3.11.
 * You can pass to author's GitHub at
@@ -425,14 +425,24 @@
 >>> pstats3(3)
     x                  π(x)                       PNT: Li(x)                Li(x) - π(x)         (Li(x) - π(x)) / π(x) [%]   
 1e+01     4                             6.165599504787298             2.165600                 54.139988                     
 1e+02     25                            30.12614158407963             5.126142                 20.504566                     
 1e+03     168                           177.60965799015221            9.609658                 5.720035
 ```
 
+## `fib()`
+Return dictionary of Fibonacci numbers from `0` to `n`. Key is an index, and a value is a specific Fibonacci number. First must create `Fibonacci` class object and then call `fib()` method on it.
+Time complexity: `O(n)`.<br>
+**<span style="color: coral">Examples</span>**
+```python
+>>> fob = Fibonacci(15)
+>>> print(fob.fib())
+{0: 0, 1: 1, 2: 1, 3: 2, 4: 3, 5: 5, 6: 8, 7: 13, 8: 21, 9: 34, 10: 55, 11: 89, 12: 144, 13: 233, 14: 377, 15: 610}
+```
+
 # Usage: `azntprimality` module functions
 
 ## `is_prime_naive1(n)`
 Return if number is a prime.
 Time complexity: `O(n)`.<br>
 **<span style="color: coral">Examples</span>**
 ```python
```

### Comparing `aznt-0.0.41/aznt/azntnumbers.py` & `aznt-0.0.42/aznt/azntnumbers.py`

 * *Files 2% similar despite different names*

```diff
@@ -316,8 +316,41 @@
 
     approx_error_absolute = [float(_pnt2[i]) - pi_x[i] for i in range(data_rows)]
     approx_error_relative = [approx_error_absolute[i] / pi_x[i] * 100 for i in range(data_rows)]
     headers = ["x", "\u03C0(x)", "PNT: Li(x)", "Li(x) - \u03C0(x)", "(Li(x) - \u03C0(x)) / \u03C0(x) [%]"]
 
     print(f"{headers[0]:^10}{headers[1]:^30}{headers[2]:^30}{headers[3]:^25}{headers[4]:^30}")
     for i in range(data_rows):
-        print(f"{_xs[i]:<10.0e}{pi_x[i]:<30}{float(_pnt2[i]):<30}{approx_error_absolute[i]:<25f}{approx_error_relative[i]:<30f}")
+        print(
+            f"{_xs[i]:<10.0e}{pi_x[i]:<30}{float(_pnt2[i]):<30}{approx_error_absolute[i]:<25f}{approx_error_relative[i]:<30f}")
+
+
+class Fibonacci:
+
+    def __init__(self, n):
+        self.n = n
+
+    def fib_generator(self):
+        """Helper function: generate Fibonacci sequence from 0 to n"""
+        a, b = 0, 1
+        i = 0
+        yield a
+        yield b
+        while i <= self.n - 2:
+            c = a + b
+            a = b
+            b = c
+            i += 1
+            yield c
+
+    def fib(self):
+        """Return Fibonacci sequence from 0 to n to a dictionary"""
+        dct = {}
+        for count, fb in enumerate(self.fib_generator()):
+            dct[count] = fb
+
+        return dct
+
+
+if __name__ == "__main__":
+    fob = Fibonacci(15)
+    print(fob.fib())
```

### Comparing `aznt-0.0.41/aznt/azntplots.py` & `aznt-0.0.42/aznt/azntplots.py`

 * *Files identical despite different names*

### Comparing `aznt-0.0.41/aznt/azntprimality.py` & `aznt-0.0.42/aznt/azntprimality.py`

 * *Files identical despite different names*

### Comparing `aznt-0.0.41/aznt.egg-info/PKG-INFO` & `aznt-0.0.42/aznt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aznt
-Version: 0.0.41
+Version: 0.0.42
 Summary: From A to Z Number Theory
 Author-email: "Adrian Zapała, MSc" <adrian.zapala@outlook.com>
 Keywords: aznt,numbers,number theory,primes,prime numbers,math
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
@@ -19,15 +19,15 @@
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 ![Python Version](https://img.shields.io/badge/python-3.11-blue/)
-![aznt version](https://img.shields.io/badge/aznt-0.0.41-green)
+![aznt version](https://img.shields.io/badge/aznt-0.0.42-green)
 ![Beta version](https://img.shields.io/badge/beta-ver.-green)
 
 # `aznt` - From A to Z Number Theory
 
 * Number Theory library for Python with prime numbers.
 * **Important:** requires Python >= 3.11.
 * You can pass to author's GitHub at
@@ -449,14 +449,24 @@
 >>> pstats3(3)
     x                  π(x)                       PNT: Li(x)                Li(x) - π(x)         (Li(x) - π(x)) / π(x) [%]   
 1e+01     4                             6.165599504787298             2.165600                 54.139988                     
 1e+02     25                            30.12614158407963             5.126142                 20.504566                     
 1e+03     168                           177.60965799015221            9.609658                 5.720035
 ```
 
+## `fib()`
+Return dictionary of Fibonacci numbers from `0` to `n`. Key is an index, and a value is a specific Fibonacci number. First must create `Fibonacci` class object and then call `fib()` method on it.
+Time complexity: `O(n)`.<br>
+**<span style="color: coral">Examples</span>**
+```python
+>>> fob = Fibonacci(15)
+>>> print(fob.fib())
+{0: 0, 1: 1, 2: 1, 3: 2, 4: 3, 5: 5, 6: 8, 7: 13, 8: 21, 9: 34, 10: 55, 11: 89, 12: 144, 13: 233, 14: 377, 15: 610}
+```
+
 # Usage: `azntprimality` module functions
 
 ## `is_prime_naive1(n)`
 Return if number is a prime.
 Time complexity: `O(n)`.<br>
 **<span style="color: coral">Examples</span>**
 ```python
```

### Comparing `aznt-0.0.41/pyproject.toml` & `aznt-0.0.42/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aznt"
-version = "0.0.41"
+version = "0.0.42"
 description = "From A to Z Number Theory"
 keywords = ["aznt", "numbers", "number theory", "primes", "prime numbers", "math"]
 authors = [
     {name = "Adrian Zapała, MSc", email = "adrian.zapala@outlook.com"},
 ]
 license = {file = "LICENSE.txt"}
 readme = "README.md"
```

