# Comparing `tmp/yplib-1.1.0.tar.gz` & `tmp/yplib-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.1.0.tar", last modified: Wed Jun 14 01:53:04 2023, max compression
+gzip compressed data, was "dist\yplib-1.1.1.tar", last modified: Wed Jun 14 02:06:42 2023, max compression
```

## Comparing `yplib-1.1.0.tar` & `yplib-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 01:53:04.547837 yplib-1.1.0/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-14 01:53:04.547837 yplib-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 01:53:04.547837 yplib-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-14 01:53:00.000000 yplib-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 01:53:04.544758 yplib-1.1.0/yplib/
--rw-rw-rw-   0        0        0      119 2023-06-14 01:52:25.000000 yplib-1.1.0/yplib/__init__.py
--rw-rw-rw-   0        0        0     2591 2023-06-14 01:51:32.000000 yplib-1.1.0/yplib/chart_html.py
--rw-rw-rw-   0        0        0     3555 2023-06-14 00:31:24.000000 yplib-1.1.0/yplib/file.py
--rw-rw-rw-   0        0        0    12635 2023-06-14 01:52:29.000000 yplib-1.1.0/yplib/index.py
--rw-rw-rw-   0        0        0     3517 2023-06-14 00:54:35.000000 yplib-1.1.0/yplib/test_my_fun.py
-drwxrwxrwx   0        0        0        0 2023-06-14 01:53:04.546849 yplib-1.1.0/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-14 01:53:04.000000 yplib-1.1.0/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-06-14 01:53:04.000000 yplib-1.1.0/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 01:53:04.000000 yplib-1.1.0/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 01:53:04.000000 yplib-1.1.0/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 02:06:42.061242 yplib-1.1.1/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-14 02:06:42.061123 yplib-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 02:06:42.061694 yplib-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-14 02:06:28.000000 yplib-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:06:42.058074 yplib-1.1.1/yplib/
+-rw-rw-rw-   0        0        0      119 2023-06-14 01:52:25.000000 yplib-1.1.1/yplib/__init__.py
+-rw-rw-rw-   0        0        0     3779 2023-06-14 02:06:14.000000 yplib-1.1.1/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     3555 2023-06-14 00:31:24.000000 yplib-1.1.1/yplib/file.py
+-rw-rw-rw-   0        0        0    12635 2023-06-14 01:52:29.000000 yplib-1.1.1/yplib/index.py
+-rw-rw-rw-   0        0        0     3517 2023-06-14 01:54:39.000000 yplib-1.1.1/yplib/test_my_fun.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:06:42.060433 yplib-1.1.1/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-14 02:06:41.000000 yplib-1.1.1/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-06-14 02:06:42.000000 yplib-1.1.1/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 02:06:42.000000 yplib-1.1.1/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 02:06:42.000000 yplib-1.1.1/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.1.0/LICENSE` & `yplib-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.1.0/PKG-INFO` & `yplib-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 1.1.0
+Version: 1.1.1
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-1.1.0/setup.py` & `yplib-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.1.0",
+  version="1.1.1",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-1.1.0/yplib/chart_html.py` & `yplib-1.1.1/yplib/chart_html.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         '</script>' \
         '</body>' \
         '</html>' \
         ''
     return s.replace('-option-', option)
 
 
+# 折线图的 html 模板代码
 def line_stack_html():
     option = '{' \
              '    title: {' \
              '        text: "-chart_name-",' \
              '    },' \
              '    tooltip: {' \
              '        trigger: "axis",' \
@@ -64,9 +65,46 @@
              '        boundaryGap: false,' \
              '        data: -x_list-,' \
              '    },' \
              '    legend: {' \
              '        -legend-,' \
              '    },' \
              '    series: -series-,' \
-             '};'
+             '}'
+    return chart_html(option)
+
+
+# 饼图的 html 模板代码
+def pie_html():
+    option = '{' \
+             '  tooltip: {' \
+             '    trigger: "item"' \
+             '  },' \
+             '  legend: {' \
+             '    top: "5%",' \
+             '    left: "center"' \
+             '  },' \
+             '  series: [' \
+             '    {' \
+             '      name: "Access From",' \
+             '      type: "pie",' \
+             '      radius: ["30%", "70%"],' \
+             '      itemStyle: {' \
+             '        borderRadius: 10,' \
+             '        borderColor: "#fff",' \
+             '        borderWidth: 1' \
+             '      },' \
+             '      emphasis: {' \
+             '        label: {' \
+             '          show: true,' \
+             '          fontSize: 30,' \
+             '          fontWeight: "bold"' \
+             '        }' \
+             '      },' \
+             '      labelLine: {' \
+             '        show: true' \
+             '      },' \
+             '      data: -data-' \
+             '    }' \
+             '  ]' \
+             '}'
     return chart_html(option)
```

### Comparing `yplib-1.1.0/yplib/file.py` & `yplib-1.1.1/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.1.0/yplib/index.py` & `yplib-1.1.1/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-1.1.0/yplib/test_my_fun.py` & `yplib-1.1.1/yplib/test_my_fun.py`

 * *Files identical despite different names*

### Comparing `yplib-1.1.0/yplib.egg-info/PKG-INFO` & `yplib-1.1.1/yplib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 1.1.0
+Version: 1.1.1
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

