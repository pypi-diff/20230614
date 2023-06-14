# Comparing `tmp/uk_gov_dash_components-1.9.2.tar.gz` & `tmp/uk_gov_dash_components-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uk_gov_dash_components-1.9.2.tar", last modified: Thu Dec 15 16:42:26 2022, max compression
+gzip compressed data, was "uk_gov_dash_components-1.9.3.tar", last modified: Fri Dec 16 09:33:51 2022, max compression
```

## Comparing `uk_gov_dash_components-1.9.2.tar` & `uk_gov_dash_components-1.9.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 16:42:26.494013 uk_gov_dash_components-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-15 16:40:13.000000 uk_gov_dash_components-1.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      464 2022-12-15 16:40:13.000000 uk_gov_dash_components-1.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2022-12-15 16:42:26.494013 uk_gov_dash_components-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2022-12-15 16:40:13.000000 uk_gov_dash_components-1.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2022-12-15 16:40:13.000000 uk_gov_dash_components-1.9.2/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-15 16:42:26.494013 uk_gov_dash_components-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      813 2022-12-15 16:40:13.000000 uk_gov_dash_components-1.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 16:42:26.490013 uk_gov_dash_components-1.9.2/uk_gov_dash_components/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2022-12-15 16:42:19.000000 uk_gov_dash_components-1.9.2/uk_gov_dash_components/Accordion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2022-12-15 16:42:19.000000 uk_gov_dash_components-1.9.2/uk_gov_dash_components/AutoComplete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2022-12-15 16:42:19.000000 uk_gov_dash_components-1.9.2/uk_gov_dash_components/CheckboxList.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2022-12-15 16:42:19.000000 uk_gov_dash_components-1.9.2/uk_gov_dash_components/ComboBox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2022-12-15 16:42:19.000000 uk_gov_dash_components-1.9.2/uk_gov_dash_components/ComponentTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2022-12-15 16:42:19.000000 uk_gov_dash_components-1.9.2/uk_gov_dash_components/Dropdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2022-12-15 16:42:19.000000 uk_gov_dash_components-1.9.2/uk_gov_dash_components/ExpandableMenuItem.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2022-12-15 16:42:19.000000 uk_gov_dash_components-1.9.2/uk_gov_dash_components/ListBox.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2022-12-15 16:42:19.000000 uk_gov_dash_components-1.9.2/uk_gov_dash_components/Popover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2022-12-15 16:40:13.000000 uk_gov_dash_components-1.9.2/uk_gov_dash_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2022-12-15 16:42:19.000000 uk_gov_dash_components-1.9.2/uk_gov_dash_components/_imports_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2022-12-15 16:42:19.000000 uk_gov_dash_components-1.9.2/uk_gov_dash_components/dropdownArrowDown.py
--rw-r--r--   0 runner    (1001) docker     (123)    27035 2022-12-15 16:42:19.000000 uk_gov_dash_components-1.9.2/uk_gov_dash_components/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2022-12-15 16:42:18.000000 uk_gov_dash_components-1.9.2/uk_gov_dash_components/package-info.json
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2022-12-15 16:42:19.000000 uk_gov_dash_components-1.9.2/uk_gov_dash_components/status.py
--rw-r--r--   0 runner    (1001) docker     (123)   239968 2022-12-15 16:42:18.000000 uk_gov_dash_components-1.9.2/uk_gov_dash_components/uk_gov_dash_components.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      106 2022-12-15 16:42:18.000000 uk_gov_dash_components-1.9.2/uk_gov_dash_components/uk_gov_dash_components.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 16:42:26.494013 uk_gov_dash_components-1.9.2/uk_gov_dash_components.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2022-12-15 16:42:26.000000 uk_gov_dash_components-1.9.2/uk_gov_dash_components.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      912 2022-12-15 16:42:26.000000 uk_gov_dash_components-1.9.2/uk_gov_dash_components.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 16:42:26.000000 uk_gov_dash_components-1.9.2/uk_gov_dash_components.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-15 16:42:26.000000 uk_gov_dash_components-1.9.2/uk_gov_dash_components.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 09:33:51.084873 uk_gov_dash_components-1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 09:31:36.000000 uk_gov_dash_components-1.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2022-12-16 09:31:36.000000 uk_gov_dash_components-1.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2022-12-16 09:33:51.084873 uk_gov_dash_components-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2022-12-16 09:31:36.000000 uk_gov_dash_components-1.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2022-12-16 09:31:36.000000 uk_gov_dash_components-1.9.3/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-16 09:33:51.084873 uk_gov_dash_components-1.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2022-12-16 09:31:36.000000 uk_gov_dash_components-1.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 09:33:51.084873 uk_gov_dash_components-1.9.3/uk_gov_dash_components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2022-12-16 09:33:44.000000 uk_gov_dash_components-1.9.3/uk_gov_dash_components/Accordion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2022-12-16 09:33:44.000000 uk_gov_dash_components-1.9.3/uk_gov_dash_components/AutoComplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2022-12-16 09:33:44.000000 uk_gov_dash_components-1.9.3/uk_gov_dash_components/CheckboxList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2022-12-16 09:33:44.000000 uk_gov_dash_components-1.9.3/uk_gov_dash_components/ComboBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2022-12-16 09:33:44.000000 uk_gov_dash_components-1.9.3/uk_gov_dash_components/ComponentTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2022-12-16 09:33:44.000000 uk_gov_dash_components-1.9.3/uk_gov_dash_components/Dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2022-12-16 09:33:44.000000 uk_gov_dash_components-1.9.3/uk_gov_dash_components/ExpandableMenuItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2022-12-16 09:33:44.000000 uk_gov_dash_components-1.9.3/uk_gov_dash_components/ListBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2022-12-16 09:33:44.000000 uk_gov_dash_components-1.9.3/uk_gov_dash_components/Popover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2022-12-16 09:31:36.000000 uk_gov_dash_components-1.9.3/uk_gov_dash_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2022-12-16 09:33:44.000000 uk_gov_dash_components-1.9.3/uk_gov_dash_components/_imports_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2022-12-16 09:33:44.000000 uk_gov_dash_components-1.9.3/uk_gov_dash_components/dropdownArrowDown.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27035 2022-12-16 09:33:44.000000 uk_gov_dash_components-1.9.3/uk_gov_dash_components/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2022-12-16 09:33:43.000000 uk_gov_dash_components-1.9.3/uk_gov_dash_components/package-info.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2022-12-16 09:33:44.000000 uk_gov_dash_components-1.9.3/uk_gov_dash_components/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)   239968 2022-12-16 09:33:42.000000 uk_gov_dash_components-1.9.3/uk_gov_dash_components/uk_gov_dash_components.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2022-12-16 09:33:42.000000 uk_gov_dash_components-1.9.3/uk_gov_dash_components/uk_gov_dash_components.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 09:33:51.084873 uk_gov_dash_components-1.9.3/uk_gov_dash_components.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2022-12-16 09:33:51.000000 uk_gov_dash_components-1.9.3/uk_gov_dash_components.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2022-12-16 09:33:51.000000 uk_gov_dash_components-1.9.3/uk_gov_dash_components.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-16 09:33:51.000000 uk_gov_dash_components-1.9.3/uk_gov_dash_components.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-16 09:33:51.000000 uk_gov_dash_components-1.9.3/uk_gov_dash_components.egg-info/top_level.txt
```

### Comparing `uk_gov_dash_components-1.9.2/PKG-INFO` & `uk_gov_dash_components-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uk_gov_dash_components
-Version: 1.9.2
+Version: 1.9.3
 Summary: Dash components for Gov UK
 Author: DLUHC GovUk <pythonvisualisations@levellingup.gov.uk>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `uk_gov_dash_components-1.9.2/README.md` & `uk_gov_dash_components-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `uk_gov_dash_components-1.9.2/package.json` & `uk_gov_dash_components-1.9.3/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'1.9.3'"}*

```diff
@@ -62,9 +62,9 @@
         "build:backends": "dash-generate-components ./src/lib/components uk_gov_dash_components -p package-info.json --r-prefix 'govuk' --jl-prefix 'govuk' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack-serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "1.9.2"
+    "version": "1.9.3"
 }
```

### Comparing `uk_gov_dash_components-1.9.2/setup.py` & `uk_gov_dash_components-1.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `uk_gov_dash_components-1.9.2/uk_gov_dash_components/Accordion.py` & `uk_gov_dash_components-1.9.3/uk_gov_dash_components/Accordion.py`

 * *Files identical despite different names*

### Comparing `uk_gov_dash_components-1.9.2/uk_gov_dash_components/AutoComplete.py` & `uk_gov_dash_components-1.9.3/uk_gov_dash_components/AutoComplete.py`

 * *Files identical despite different names*

### Comparing `uk_gov_dash_components-1.9.2/uk_gov_dash_components/CheckboxList.py` & `uk_gov_dash_components-1.9.3/uk_gov_dash_components/CheckboxList.py`

 * *Files identical despite different names*

### Comparing `uk_gov_dash_components-1.9.2/uk_gov_dash_components/ComboBox.py` & `uk_gov_dash_components-1.9.3/uk_gov_dash_components/ComboBox.py`

 * *Files identical despite different names*

### Comparing `uk_gov_dash_components-1.9.2/uk_gov_dash_components/ComponentTemplate.py` & `uk_gov_dash_components-1.9.3/uk_gov_dash_components/ComponentTemplate.py`

 * *Files identical despite different names*

### Comparing `uk_gov_dash_components-1.9.2/uk_gov_dash_components/Dropdown.py` & `uk_gov_dash_components-1.9.3/uk_gov_dash_components/Dropdown.py`

 * *Files identical despite different names*

### Comparing `uk_gov_dash_components-1.9.2/uk_gov_dash_components/ExpandableMenuItem.py` & `uk_gov_dash_components-1.9.3/uk_gov_dash_components/ExpandableMenuItem.py`

 * *Files identical despite different names*

### Comparing `uk_gov_dash_components-1.9.2/uk_gov_dash_components/ListBox.py` & `uk_gov_dash_components-1.9.3/uk_gov_dash_components/ListBox.py`

 * *Files identical despite different names*

### Comparing `uk_gov_dash_components-1.9.2/uk_gov_dash_components/Popover.py` & `uk_gov_dash_components-1.9.3/uk_gov_dash_components/Popover.py`

 * *Files identical despite different names*

### Comparing `uk_gov_dash_components-1.9.2/uk_gov_dash_components/__init__.py` & `uk_gov_dash_components-1.9.3/uk_gov_dash_components/__init__.py`

 * *Files identical despite different names*

### Comparing `uk_gov_dash_components-1.9.2/uk_gov_dash_components/_imports_.py` & `uk_gov_dash_components-1.9.3/uk_gov_dash_components/_imports_.py`

 * *Files identical despite different names*

### Comparing `uk_gov_dash_components-1.9.2/uk_gov_dash_components/dropdownArrowDown.py` & `uk_gov_dash_components-1.9.3/uk_gov_dash_components/dropdownArrowDown.py`

 * *Files identical despite different names*

### Comparing `uk_gov_dash_components-1.9.2/uk_gov_dash_components/metadata.json` & `uk_gov_dash_components-1.9.3/uk_gov_dash_components/metadata.json`

 * *Files identical despite different names*

### Comparing `uk_gov_dash_components-1.9.2/uk_gov_dash_components/package-info.json` & `uk_gov_dash_components-1.9.3/uk_gov_dash_components/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'1.9.3'"}*

```diff
@@ -62,9 +62,9 @@
         "build:backends": "dash-generate-components ./src/lib/components uk_gov_dash_components -p package-info.json --r-prefix 'govuk' --jl-prefix 'govuk' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack-serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "1.9.2"
+    "version": "1.9.3"
 }
```

### Comparing `uk_gov_dash_components-1.9.2/uk_gov_dash_components/status.py` & `uk_gov_dash_components-1.9.3/uk_gov_dash_components/status.py`

 * *Files identical despite different names*

### Comparing `uk_gov_dash_components-1.9.2/uk_gov_dash_components/uk_gov_dash_components.min.js` & `uk_gov_dash_components-1.9.3/uk_gov_dash_components/uk_gov_dash_components.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -64,15 +64,15 @@
             var t = function(e) {
                     return /\/_dash-component-suites\//.test(e.src)
                 }(o()),
                 n = i(e);
             if (!t) return n;
             var r = n.split("/"),
                 a = r.slice(-1)[0].split(".");
-            return a.splice(1, 0, "v1_9_2m1671122533"), r.splice(-1, 1, a.join(".")), r.join("/")
+            return a.splice(1, 0, "v1_9_3m1671183218"), r.splice(-1, 1, a.join(".")), r.join("/")
         }
     }
     return n(n.s = 34)
 }([function(e, t) {
     e.exports = window.React
 }, function(e, t) {
     e.exports = window.PropTypes
```

### Comparing `uk_gov_dash_components-1.9.2/uk_gov_dash_components.egg-info/PKG-INFO` & `uk_gov_dash_components-1.9.3/uk_gov_dash_components.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uk-gov-dash-components
-Version: 1.9.2
+Version: 1.9.3
 Summary: Dash components for Gov UK
 Author: DLUHC GovUk <pythonvisualisations@levellingup.gov.uk>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `uk_gov_dash_components-1.9.2/uk_gov_dash_components.egg-info/SOURCES.txt` & `uk_gov_dash_components-1.9.3/uk_gov_dash_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

