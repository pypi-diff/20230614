# Comparing `tmp/ezbeq-1.0.2.tar.gz` & `tmp/ezbeq-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezbeq-1.0.2.tar", max compression
+gzip compressed data, was "ezbeq-1.0.3.tar", max compression
```

## Comparing `ezbeq-1.0.2.tar` & `ezbeq-1.0.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1066 2023-06-14 06:53:27.534013 ezbeq-1.0.2/LICENSE
--rw-r--r--   0        0        0    11494 2023-06-14 06:53:27.534013 ezbeq-1.0.2/README.md
--rw-r--r--   0        0        0        6 2023-06-14 06:55:25.232825 ezbeq-1.0.2/ezbeq/VERSION
--rw-r--r--   0        0        0        0 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/__init__.py
--rw-r--r--   0        0        0       57 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/apis/__init__.py
--rw-r--r--   0        0        0      569 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/apis/audiotypes.py
--rw-r--r--   0        0        0      510 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/apis/authors.py
--rw-r--r--   0        0        0     1572 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/apis/catalogue.py
--rw-r--r--   0        0        0      526 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/apis/contenttypes.py
--rw-r--r--   0        0        0    26001 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/apis/devices.py
--rw-r--r--   0        0        0      518 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/apis/languages.py
--rw-r--r--   0        0        0      686 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/apis/meta.py
--rw-r--r--   0        0        0     2439 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/apis/search.py
--rw-r--r--   0        0        0      346 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/apis/version.py
--rw-r--r--   0        0        0     6514 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/apis/ws.py
--rw-r--r--   0        0        0      516 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/apis/years.py
--rw-r--r--   0        0        0    27881 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/camilladsp.py
--rw-r--r--   0        0        0    12896 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/catalogue.py
--rw-r--r--   0        0        0     8752 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/config.py
--rw-r--r--   0        0        0     8573 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/device.py
--rw-r--r--   0        0        0    12197 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/htp1.py
--rw-r--r--   0        0        0     4483 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/iir.py
--rw-r--r--   0        0        0    22779 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/jriver.py
--rw-r--r--   0        0        0     7014 2023-06-14 06:53:27.574014 ezbeq-1.0.2/ezbeq/main.py
--rw-r--r--   0        0        0    40966 2023-06-14 06:53:27.574014 ezbeq-1.0.2/ezbeq/minidsp.py
--rw-r--r--   0        0        0     8309 2023-06-14 06:53:27.574014 ezbeq-1.0.2/ezbeq/qsys.py
--rw-r--r--   0        0        0     4303 2023-06-14 06:55:23.844789 ezbeq-1.0.2/ezbeq/ui/android-chrome-192x192.png
--rw-r--r--   0        0        0    14091 2023-06-14 06:55:23.844789 ezbeq-1.0.2/ezbeq/ui/android-chrome-512x512.png
--rw-r--r--   0        0        0     3262 2023-06-14 06:55:23.844789 ezbeq-1.0.2/ezbeq/ui/apple-touch-icon.png
--rw-r--r--   0        0        0   852107 2023-06-14 06:55:24.748813 ezbeq-1.0.2/ezbeq/ui/assets/index-3477b443.js
--rw-r--r--   0        0        0     5721 2023-06-14 06:55:24.748813 ezbeq-1.0.2/ezbeq/ui/assets/index-fce6f16f.css
--rw-r--r--   0        0        0    65456 2023-06-14 06:55:24.748813 ezbeq-1.0.2/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff
--rw-r--r--   0        0        0     9628 2023-06-14 06:55:24.748813 ezbeq-1.0.2/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2
--rw-r--r--   0        0        0    15344 2023-06-14 06:55:24.744812 ezbeq-1.0.2/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2
--rw-r--r--   0        0        0     7112 2023-06-14 06:55:24.748813 ezbeq-1.0.2/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2
--rw-r--r--   0        0        0    15744 2023-06-14 06:55:24.748813 ezbeq-1.0.2/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2
--rw-r--r--   0        0        0    11872 2023-06-14 06:55:24.748813 ezbeq-1.0.2/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2
--rw-r--r--   0        0        0     5560 2023-06-14 06:55:24.748813 ezbeq-1.0.2/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2
--rw-r--r--   0        0        0      246 2023-06-14 06:55:23.844789 ezbeq-1.0.2/ezbeq/ui/browserconfig.xml
--rw-r--r--   0        0        0      702 2023-06-14 06:55:23.844789 ezbeq-1.0.2/ezbeq/ui/favicon-16x16.png
--rw-r--r--   0        0        0     1310 2023-06-14 06:55:23.844789 ezbeq-1.0.2/ezbeq/ui/favicon-32x32.png
--rw-r--r--   0        0        0     7406 2023-06-14 06:55:23.844789 ezbeq-1.0.2/ezbeq/ui/favicon.ico
--rw-r--r--   0        0        0     1012 2023-06-14 06:55:24.748813 ezbeq-1.0.2/ezbeq/ui/index.html
--rw-r--r--   0        0        0     2533 2023-06-14 06:55:23.844789 ezbeq-1.0.2/ezbeq/ui/mstile-150x150.png
--rw-r--r--   0        0        0       67 2023-06-14 06:55:23.844789 ezbeq-1.0.2/ezbeq/ui/robots.txt
--rw-r--r--   0        0        0     3278 2023-06-14 06:55:23.844789 ezbeq-1.0.2/ezbeq/ui/safari-pinned-tab.svg
--rw-r--r--   0        0        0      436 2023-06-14 06:55:23.844789 ezbeq-1.0.2/ezbeq/ui/site.webmanifest
--rw-r--r--   0        0        0     1312 2023-06-14 06:53:27.574014 ezbeq-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    12528 1970-01-01 00:00:00.000000 ezbeq-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-14 07:08:40.362351 ezbeq-1.0.3/LICENSE
+-rw-r--r--   0        0        0    11494 2023-06-14 07:08:40.362351 ezbeq-1.0.3/README.md
+-rw-r--r--   0        0        0        6 2023-06-14 07:10:34.445586 ezbeq-1.0.3/ezbeq/VERSION
+-rw-r--r--   0        0        0        0 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/__init__.py
+-rw-r--r--   0        0        0       57 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/apis/__init__.py
+-rw-r--r--   0        0        0      569 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/apis/audiotypes.py
+-rw-r--r--   0        0        0      510 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/apis/authors.py
+-rw-r--r--   0        0        0     1572 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/apis/catalogue.py
+-rw-r--r--   0        0        0      526 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/apis/contenttypes.py
+-rw-r--r--   0        0        0    26001 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/apis/devices.py
+-rw-r--r--   0        0        0      518 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/apis/languages.py
+-rw-r--r--   0        0        0      686 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/apis/meta.py
+-rw-r--r--   0        0        0     2439 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/apis/search.py
+-rw-r--r--   0        0        0      346 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/apis/version.py
+-rw-r--r--   0        0        0     6514 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/apis/ws.py
+-rw-r--r--   0        0        0      516 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/apis/years.py
+-rw-r--r--   0        0        0    27881 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/camilladsp.py
+-rw-r--r--   0        0        0    12896 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/catalogue.py
+-rw-r--r--   0        0        0     8752 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/config.py
+-rw-r--r--   0        0        0     8573 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/device.py
+-rw-r--r--   0        0        0    12197 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/htp1.py
+-rw-r--r--   0        0        0     4483 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/iir.py
+-rw-r--r--   0        0        0    22779 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/jriver.py
+-rw-r--r--   0        0        0     7014 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/main.py
+-rw-r--r--   0        0        0    40966 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/minidsp.py
+-rw-r--r--   0        0        0     8309 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/qsys.py
+-rw-r--r--   0        0        0     4303 2023-06-14 07:10:33.033487 ezbeq-1.0.3/ezbeq/ui/android-chrome-192x192.png
+-rw-r--r--   0        0        0    14091 2023-06-14 07:10:33.033487 ezbeq-1.0.3/ezbeq/ui/android-chrome-512x512.png
+-rw-r--r--   0        0        0     3262 2023-06-14 07:10:33.033487 ezbeq-1.0.3/ezbeq/ui/apple-touch-icon.png
+-rw-r--r--   0        0        0   852111 2023-06-14 07:10:33.973553 ezbeq-1.0.3/ezbeq/ui/assets/index-83ab9065.js
+-rw-r--r--   0        0        0     5721 2023-06-14 07:10:33.973553 ezbeq-1.0.3/ezbeq/ui/assets/index-fce6f16f.css
+-rw-r--r--   0        0        0    65456 2023-06-14 07:10:33.973553 ezbeq-1.0.3/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff
+-rw-r--r--   0        0        0     9628 2023-06-14 07:10:33.973553 ezbeq-1.0.3/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2
+-rw-r--r--   0        0        0    15344 2023-06-14 07:10:33.973553 ezbeq-1.0.3/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2
+-rw-r--r--   0        0        0     7112 2023-06-14 07:10:33.973553 ezbeq-1.0.3/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2
+-rw-r--r--   0        0        0    15744 2023-06-14 07:10:33.973553 ezbeq-1.0.3/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2
+-rw-r--r--   0        0        0    11872 2023-06-14 07:10:33.973553 ezbeq-1.0.3/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2
+-rw-r--r--   0        0        0     5560 2023-06-14 07:10:33.973553 ezbeq-1.0.3/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2
+-rw-r--r--   0        0        0      246 2023-06-14 07:10:33.033487 ezbeq-1.0.3/ezbeq/ui/browserconfig.xml
+-rw-r--r--   0        0        0      702 2023-06-14 07:10:33.033487 ezbeq-1.0.3/ezbeq/ui/favicon-16x16.png
+-rw-r--r--   0        0        0     1310 2023-06-14 07:10:33.033487 ezbeq-1.0.3/ezbeq/ui/favicon-32x32.png
+-rw-r--r--   0        0        0     7406 2023-06-14 07:10:33.037488 ezbeq-1.0.3/ezbeq/ui/favicon.ico
+-rw-r--r--   0        0        0     1012 2023-06-14 07:10:33.973553 ezbeq-1.0.3/ezbeq/ui/index.html
+-rw-r--r--   0        0        0     2533 2023-06-14 07:10:33.037488 ezbeq-1.0.3/ezbeq/ui/mstile-150x150.png
+-rw-r--r--   0        0        0       67 2023-06-14 07:10:33.037488 ezbeq-1.0.3/ezbeq/ui/robots.txt
+-rw-r--r--   0        0        0     3278 2023-06-14 07:10:33.037488 ezbeq-1.0.3/ezbeq/ui/safari-pinned-tab.svg
+-rw-r--r--   0        0        0      436 2023-06-14 07:10:33.037488 ezbeq-1.0.3/ezbeq/ui/site.webmanifest
+-rw-r--r--   0        0        0     1312 2023-06-14 07:08:40.410354 ezbeq-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    12528 1970-01-01 00:00:00.000000 ezbeq-1.0.3/PKG-INFO
```

### Comparing `ezbeq-1.0.2/LICENSE` & `ezbeq-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/README.md` & `ezbeq-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/apis/audiotypes.py` & `ezbeq-1.0.3/ezbeq/apis/audiotypes.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/apis/catalogue.py` & `ezbeq-1.0.3/ezbeq/apis/catalogue.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/apis/contenttypes.py` & `ezbeq-1.0.3/ezbeq/apis/contenttypes.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/apis/devices.py` & `ezbeq-1.0.3/ezbeq/apis/devices.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/apis/languages.py` & `ezbeq-1.0.3/ezbeq/apis/languages.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/apis/meta.py` & `ezbeq-1.0.3/ezbeq/apis/meta.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/apis/search.py` & `ezbeq-1.0.3/ezbeq/apis/search.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/apis/ws.py` & `ezbeq-1.0.3/ezbeq/apis/ws.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/apis/years.py` & `ezbeq-1.0.3/ezbeq/apis/years.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/camilladsp.py` & `ezbeq-1.0.3/ezbeq/camilladsp.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/catalogue.py` & `ezbeq-1.0.3/ezbeq/catalogue.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/config.py` & `ezbeq-1.0.3/ezbeq/config.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/device.py` & `ezbeq-1.0.3/ezbeq/device.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/htp1.py` & `ezbeq-1.0.3/ezbeq/htp1.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/iir.py` & `ezbeq-1.0.3/ezbeq/iir.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/jriver.py` & `ezbeq-1.0.3/ezbeq/jriver.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/main.py` & `ezbeq-1.0.3/ezbeq/main.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/minidsp.py` & `ezbeq-1.0.3/ezbeq/minidsp.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/qsys.py` & `ezbeq-1.0.3/ezbeq/qsys.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/ui/android-chrome-192x192.png` & `ezbeq-1.0.3/ezbeq/ui/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/ui/android-chrome-512x512.png` & `ezbeq-1.0.3/ezbeq/ui/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/ui/apple-touch-icon.png` & `ezbeq-1.0.3/ezbeq/ui/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/ui/assets/index-3477b443.js` & `ezbeq-1.0.3/ezbeq/ui/assets/index-83ab9065.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -37406,15 +37406,15 @@
     }) => {
         const [p, f] = Qu("selectedAuthors", []), [h, m] = d.useState([]), [g, x] = d.useState([]), [b, y] = d.useState([]), [C, S] = d.useState([]), [I, $] = d.useState([]), [P, k] = d.useState(""), [O, _] = d.useState(!1), [R, F] = d.useState(-1), [z, E] = d.useState(!1), [T, N] = d.useState([]), D = () => {
             _(H => !H)
         };
         d.useEffect(() => {
             if (t) {
                 const H = Object.keys(t);
-                H.length > 0 && l(t[H[0]])
+                H.length > 0 && !o && l(t[H[0]])
             }
         }, [t, o, l]), d.useEffect(() => {
             const H = W => {
                     const X = P.toLowerCase();
                     return !!(W.formattedTitle.toLowerCase().includes(X) || W.hasOwnProperty("altTitle") && W.altTitle.toLowerCase().includes(X) || W.hasOwnProperty("collection") && W.collection.toLowerCase().includes(X))
                 },
                 Y = W => !!((!p.length || p.indexOf(W.author) > -1) && (!g.length || g.indexOf(W.year) > -1) && (!b.length || W.audioTypes.some(X => b.indexOf(X) > -1)) && (!C.length || C.indexOf(W.contentType) > -1) && (!I.length || I.indexOf(W.freshness) > -1) && (!h.length || h.indexOf(W.language) > -1) && (!P || H(W)));
```

### Comparing `ezbeq-1.0.2/ezbeq/ui/assets/index-fce6f16f.css` & `ezbeq-1.0.3/ezbeq/ui/assets/index-fce6f16f.css`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff` & `ezbeq-1.0.3/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2` & `ezbeq-1.0.3/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2` & `ezbeq-1.0.3/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2` & `ezbeq-1.0.3/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2` & `ezbeq-1.0.3/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2` & `ezbeq-1.0.3/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2` & `ezbeq-1.0.3/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/ui/favicon-16x16.png` & `ezbeq-1.0.3/ezbeq/ui/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/ui/favicon-32x32.png` & `ezbeq-1.0.3/ezbeq/ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/ui/favicon.ico` & `ezbeq-1.0.3/ezbeq/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/ui/index.html` & `ezbeq-1.0.3/ezbeq/ui/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     <link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
     <link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
     <link rel="mask-icon" href="/safari-pinned-tab.svg" color="#5bbad5">
     <meta name="theme-color" content="#ffffff">
     <meta name="msapplication-TileColor" content="#da532c">
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Roboto:300,400,500"/>
     <title>ezbeq</title>
-  <script type="module" crossorigin src="/assets/index-3477b443.js"></script>
+  <script type="module" crossorigin src="/assets/index-83ab9065.js"></script>
   <link rel="stylesheet" href="/assets/index-fce6f16f.css">
 </head>
 <body>
 <noscript>
     You need to enable JavaScript to run this app.
 </noscript>
 <div id="root"></div>
```

### Comparing `ezbeq-1.0.2/ezbeq/ui/mstile-150x150.png` & `ezbeq-1.0.3/ezbeq/ui/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/ezbeq/ui/safari-pinned-tab.svg` & `ezbeq-1.0.3/ezbeq/ui/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.2/pyproject.toml` & `ezbeq-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ezbeq"
-version = "1.0.2"
+version = "1.0.3"
 description = "A webapp which can send beqcatalogue filters to a DSP device"
 authors = ["3ll3d00d <mattkhan+ezbeq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://ezbeq.readthedocs.io/"
 repository = "https://github.com/3ll3d00d/ezbeq"
 include = [
```

### Comparing `ezbeq-1.0.2/PKG-INFO` & `ezbeq-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezbeq
-Version: 1.0.2
+Version: 1.0.3
 Summary: A webapp which can send beqcatalogue filters to a DSP device
 Home-page: https://ezbeq.readthedocs.io/
 License: MIT
 Author: 3ll3d00d
 Author-email: mattkhan+ezbeq@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

