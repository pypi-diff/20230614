# Comparing `tmp/ezbeq-1.0.1.tar.gz` & `tmp/ezbeq-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezbeq-1.0.1.tar", max compression
+gzip compressed data, was "ezbeq-1.0.2.tar", max compression
```

## Comparing `ezbeq-1.0.1.tar` & `ezbeq-1.0.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1066 2023-06-12 08:12:12.019156 ezbeq-1.0.1/LICENSE
--rw-r--r--   0        0        0    11494 2023-06-12 08:12:12.019156 ezbeq-1.0.1/README.md
--rw-r--r--   0        0        0        6 2023-06-12 08:13:49.010714 ezbeq-1.0.1/ezbeq/VERSION
--rw-r--r--   0        0        0        0 2023-06-12 08:12:12.055156 ezbeq-1.0.1/ezbeq/__init__.py
--rw-r--r--   0        0        0       57 2023-06-12 08:12:12.055156 ezbeq-1.0.1/ezbeq/apis/__init__.py
--rw-r--r--   0        0        0      569 2023-06-12 08:12:12.055156 ezbeq-1.0.1/ezbeq/apis/audiotypes.py
--rw-r--r--   0        0        0      510 2023-06-12 08:12:12.055156 ezbeq-1.0.1/ezbeq/apis/authors.py
--rw-r--r--   0        0        0     1572 2023-06-12 08:12:12.055156 ezbeq-1.0.1/ezbeq/apis/catalogue.py
--rw-r--r--   0        0        0      526 2023-06-12 08:12:12.055156 ezbeq-1.0.1/ezbeq/apis/contenttypes.py
--rw-r--r--   0        0        0    26001 2023-06-12 08:12:12.055156 ezbeq-1.0.1/ezbeq/apis/devices.py
--rw-r--r--   0        0        0      518 2023-06-12 08:12:12.055156 ezbeq-1.0.1/ezbeq/apis/languages.py
--rw-r--r--   0        0        0      686 2023-06-12 08:12:12.055156 ezbeq-1.0.1/ezbeq/apis/meta.py
--rw-r--r--   0        0        0     2306 2023-06-12 08:12:12.055156 ezbeq-1.0.1/ezbeq/apis/search.py
--rw-r--r--   0        0        0      346 2023-06-12 08:12:12.055156 ezbeq-1.0.1/ezbeq/apis/version.py
--rw-r--r--   0        0        0     6514 2023-06-12 08:12:12.055156 ezbeq-1.0.1/ezbeq/apis/ws.py
--rw-r--r--   0        0        0      516 2023-06-12 08:12:12.055156 ezbeq-1.0.1/ezbeq/apis/years.py
--rw-r--r--   0        0        0    27881 2023-06-12 08:12:12.055156 ezbeq-1.0.1/ezbeq/camilladsp.py
--rw-r--r--   0        0        0    12806 2023-06-12 08:12:12.055156 ezbeq-1.0.1/ezbeq/catalogue.py
--rw-r--r--   0        0        0     8752 2023-06-12 08:12:12.055156 ezbeq-1.0.1/ezbeq/config.py
--rw-r--r--   0        0        0     8573 2023-06-12 08:12:12.055156 ezbeq-1.0.1/ezbeq/device.py
--rw-r--r--   0        0        0    12197 2023-06-12 08:12:12.055156 ezbeq-1.0.1/ezbeq/htp1.py
--rw-r--r--   0        0        0     4483 2023-06-12 08:12:12.055156 ezbeq-1.0.1/ezbeq/iir.py
--rw-r--r--   0        0        0    22779 2023-06-12 08:12:12.055156 ezbeq-1.0.1/ezbeq/jriver.py
--rw-r--r--   0        0        0     7014 2023-06-12 08:12:12.055156 ezbeq-1.0.1/ezbeq/main.py
--rw-r--r--   0        0        0    40966 2023-06-12 08:12:12.055156 ezbeq-1.0.1/ezbeq/minidsp.py
--rw-r--r--   0        0        0     8309 2023-06-12 08:12:12.055156 ezbeq-1.0.1/ezbeq/qsys.py
--rw-r--r--   0        0        0     4303 2023-06-12 08:13:48.018718 ezbeq-1.0.1/ezbeq/ui/android-chrome-192x192.png
--rw-r--r--   0        0        0    14091 2023-06-12 08:13:48.018718 ezbeq-1.0.1/ezbeq/ui/android-chrome-512x512.png
--rw-r--r--   0        0        0     3262 2023-06-12 08:13:48.018718 ezbeq-1.0.1/ezbeq/ui/apple-touch-icon.png
--rw-r--r--   0        0        0   852107 2023-06-12 08:13:48.690715 ezbeq-1.0.1/ezbeq/ui/assets/index-3477b443.js
--rw-r--r--   0        0        0     5721 2023-06-12 08:13:48.686715 ezbeq-1.0.1/ezbeq/ui/assets/index-fce6f16f.css
--rw-r--r--   0        0        0    65456 2023-06-12 08:13:48.686715 ezbeq-1.0.1/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff
--rw-r--r--   0        0        0     9628 2023-06-12 08:13:48.686715 ezbeq-1.0.1/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2
--rw-r--r--   0        0        0    15344 2023-06-12 08:13:48.686715 ezbeq-1.0.1/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2
--rw-r--r--   0        0        0     7112 2023-06-12 08:13:48.686715 ezbeq-1.0.1/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2
--rw-r--r--   0        0        0    15744 2023-06-12 08:13:48.686715 ezbeq-1.0.1/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2
--rw-r--r--   0        0        0    11872 2023-06-12 08:13:48.686715 ezbeq-1.0.1/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2
--rw-r--r--   0        0        0     5560 2023-06-12 08:13:48.686715 ezbeq-1.0.1/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2
--rw-r--r--   0        0        0      246 2023-06-12 08:13:48.018718 ezbeq-1.0.1/ezbeq/ui/browserconfig.xml
--rw-r--r--   0        0        0      702 2023-06-12 08:13:48.018718 ezbeq-1.0.1/ezbeq/ui/favicon-16x16.png
--rw-r--r--   0        0        0     1310 2023-06-12 08:13:48.018718 ezbeq-1.0.1/ezbeq/ui/favicon-32x32.png
--rw-r--r--   0        0        0     7406 2023-06-12 08:13:48.018718 ezbeq-1.0.1/ezbeq/ui/favicon.ico
--rw-r--r--   0        0        0     1012 2023-06-12 08:13:48.690715 ezbeq-1.0.1/ezbeq/ui/index.html
--rw-r--r--   0        0        0     2533 2023-06-12 08:13:48.018718 ezbeq-1.0.1/ezbeq/ui/mstile-150x150.png
--rw-r--r--   0        0        0       67 2023-06-12 08:13:48.018718 ezbeq-1.0.1/ezbeq/ui/robots.txt
--rw-r--r--   0        0        0     3278 2023-06-12 08:13:48.018718 ezbeq-1.0.1/ezbeq/ui/safari-pinned-tab.svg
--rw-r--r--   0        0        0      436 2023-06-12 08:13:48.018718 ezbeq-1.0.1/ezbeq/ui/site.webmanifest
--rw-r--r--   0        0        0     1312 2023-06-12 08:12:12.059156 ezbeq-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    12528 1970-01-01 00:00:00.000000 ezbeq-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-14 06:53:27.534013 ezbeq-1.0.2/LICENSE
+-rw-r--r--   0        0        0    11494 2023-06-14 06:53:27.534013 ezbeq-1.0.2/README.md
+-rw-r--r--   0        0        0        6 2023-06-14 06:55:25.232825 ezbeq-1.0.2/ezbeq/VERSION
+-rw-r--r--   0        0        0        0 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/__init__.py
+-rw-r--r--   0        0        0       57 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/apis/__init__.py
+-rw-r--r--   0        0        0      569 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/apis/audiotypes.py
+-rw-r--r--   0        0        0      510 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/apis/authors.py
+-rw-r--r--   0        0        0     1572 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/apis/catalogue.py
+-rw-r--r--   0        0        0      526 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/apis/contenttypes.py
+-rw-r--r--   0        0        0    26001 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/apis/devices.py
+-rw-r--r--   0        0        0      518 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/apis/languages.py
+-rw-r--r--   0        0        0      686 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/apis/meta.py
+-rw-r--r--   0        0        0     2439 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/apis/search.py
+-rw-r--r--   0        0        0      346 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/apis/version.py
+-rw-r--r--   0        0        0     6514 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/apis/ws.py
+-rw-r--r--   0        0        0      516 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/apis/years.py
+-rw-r--r--   0        0        0    27881 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/camilladsp.py
+-rw-r--r--   0        0        0    12896 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/catalogue.py
+-rw-r--r--   0        0        0     8752 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/config.py
+-rw-r--r--   0        0        0     8573 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/device.py
+-rw-r--r--   0        0        0    12197 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/htp1.py
+-rw-r--r--   0        0        0     4483 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/iir.py
+-rw-r--r--   0        0        0    22779 2023-06-14 06:53:27.570014 ezbeq-1.0.2/ezbeq/jriver.py
+-rw-r--r--   0        0        0     7014 2023-06-14 06:53:27.574014 ezbeq-1.0.2/ezbeq/main.py
+-rw-r--r--   0        0        0    40966 2023-06-14 06:53:27.574014 ezbeq-1.0.2/ezbeq/minidsp.py
+-rw-r--r--   0        0        0     8309 2023-06-14 06:53:27.574014 ezbeq-1.0.2/ezbeq/qsys.py
+-rw-r--r--   0        0        0     4303 2023-06-14 06:55:23.844789 ezbeq-1.0.2/ezbeq/ui/android-chrome-192x192.png
+-rw-r--r--   0        0        0    14091 2023-06-14 06:55:23.844789 ezbeq-1.0.2/ezbeq/ui/android-chrome-512x512.png
+-rw-r--r--   0        0        0     3262 2023-06-14 06:55:23.844789 ezbeq-1.0.2/ezbeq/ui/apple-touch-icon.png
+-rw-r--r--   0        0        0   852107 2023-06-14 06:55:24.748813 ezbeq-1.0.2/ezbeq/ui/assets/index-3477b443.js
+-rw-r--r--   0        0        0     5721 2023-06-14 06:55:24.748813 ezbeq-1.0.2/ezbeq/ui/assets/index-fce6f16f.css
+-rw-r--r--   0        0        0    65456 2023-06-14 06:55:24.748813 ezbeq-1.0.2/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff
+-rw-r--r--   0        0        0     9628 2023-06-14 06:55:24.748813 ezbeq-1.0.2/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2
+-rw-r--r--   0        0        0    15344 2023-06-14 06:55:24.744812 ezbeq-1.0.2/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2
+-rw-r--r--   0        0        0     7112 2023-06-14 06:55:24.748813 ezbeq-1.0.2/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2
+-rw-r--r--   0        0        0    15744 2023-06-14 06:55:24.748813 ezbeq-1.0.2/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2
+-rw-r--r--   0        0        0    11872 2023-06-14 06:55:24.748813 ezbeq-1.0.2/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2
+-rw-r--r--   0        0        0     5560 2023-06-14 06:55:24.748813 ezbeq-1.0.2/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2
+-rw-r--r--   0        0        0      246 2023-06-14 06:55:23.844789 ezbeq-1.0.2/ezbeq/ui/browserconfig.xml
+-rw-r--r--   0        0        0      702 2023-06-14 06:55:23.844789 ezbeq-1.0.2/ezbeq/ui/favicon-16x16.png
+-rw-r--r--   0        0        0     1310 2023-06-14 06:55:23.844789 ezbeq-1.0.2/ezbeq/ui/favicon-32x32.png
+-rw-r--r--   0        0        0     7406 2023-06-14 06:55:23.844789 ezbeq-1.0.2/ezbeq/ui/favicon.ico
+-rw-r--r--   0        0        0     1012 2023-06-14 06:55:24.748813 ezbeq-1.0.2/ezbeq/ui/index.html
+-rw-r--r--   0        0        0     2533 2023-06-14 06:55:23.844789 ezbeq-1.0.2/ezbeq/ui/mstile-150x150.png
+-rw-r--r--   0        0        0       67 2023-06-14 06:55:23.844789 ezbeq-1.0.2/ezbeq/ui/robots.txt
+-rw-r--r--   0        0        0     3278 2023-06-14 06:55:23.844789 ezbeq-1.0.2/ezbeq/ui/safari-pinned-tab.svg
+-rw-r--r--   0        0        0      436 2023-06-14 06:55:23.844789 ezbeq-1.0.2/ezbeq/ui/site.webmanifest
+-rw-r--r--   0        0        0     1312 2023-06-14 06:53:27.574014 ezbeq-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    12528 1970-01-01 00:00:00.000000 ezbeq-1.0.2/PKG-INFO
```

### Comparing `ezbeq-1.0.1/LICENSE` & `ezbeq-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/README.md` & `ezbeq-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/apis/audiotypes.py` & `ezbeq-1.0.2/ezbeq/apis/audiotypes.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/apis/catalogue.py` & `ezbeq-1.0.2/ezbeq/apis/catalogue.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/apis/contenttypes.py` & `ezbeq-1.0.2/ezbeq/apis/contenttypes.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/apis/devices.py` & `ezbeq-1.0.2/ezbeq/apis/devices.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/apis/languages.py` & `ezbeq-1.0.2/ezbeq/apis/languages.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/apis/meta.py` & `ezbeq-1.0.2/ezbeq/apis/meta.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/apis/search.py` & `ezbeq-1.0.2/ezbeq/apis/search.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,32 +18,35 @@
         self.__parser = reqparse.RequestParser()
         self.__parser.add_argument('authors', action='append')
         self.__parser.add_argument('years', type=int, action='append')
         self.__parser.add_argument('audiotypes', action='append')
         self.__parser.add_argument('contenttypes', action='append')
         self.__parser.add_argument('fields', action='append')
         self.__parser.add_argument('text')
+        self.__parser.add_argument('tmdbid')
 
     @api.param('authors', 'The author of the BEQ filter, if multiple values provided any match will be returned')
     @api.param('years', 'The production year of the entry, if multiple values provided any match will be returned')
     @api.param('audiotypes', 'The audio type of the entry, if multiple values provided any match will be returned')
     @api.param('authors', 'The content type of the entry, if multiple values provided any match will be returned')
     @api.param('text', 'Provides a case insensitive search against the following fields: formattedTitle, altTitle, collection. Value is returned if the supplied text is contained in any of those fields.')
     @api.param('fields', 'The entry fields to return in the output')
+    @api.param('tmdbid', 'TheMovieDB id')
     def get(self):
         catalogue = self.__provider.catalogue
         args = self.__parser.parse_args()
         authors = args.get('authors')
         years = args.get('years')
         audio_types = args.get('audiotypes')
         content_types = args.get('contenttypes')
         text = args.get('text')
+        tmdb_id = args.get('tmdbid')
         fields = args.get('fields')
         return [self.__filter_fields(c.for_search, fields)
-                for c in catalogue if c.matches(authors, years, audio_types, content_types, text)]
+                for c in catalogue if c.matches(authors, years, audio_types, content_types, tmdb_id, text)]
 
     @staticmethod
     def __filter_fields(entry: dict, fields: list):
         if fields:
             return {k: v for k, v in entry.items() if k in fields}
         else:
             return entry
```

### Comparing `ezbeq-1.0.1/ezbeq/apis/ws.py` & `ezbeq-1.0.2/ezbeq/apis/ws.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/apis/years.py` & `ezbeq-1.0.2/ezbeq/apis/years.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/camilladsp.py` & `ezbeq-1.0.2/ezbeq/camilladsp.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/catalogue.py` & `ezbeq-1.0.2/ezbeq/catalogue.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,20 +124,21 @@
             self.for_search['note'] = self.note
         if self.warning:
             self.for_search['warning'] = self.warning
         if self.collection and 'name' in self.collection:
             self.for_search['collection'] = self.collection['name']
 
     def matches(self, authors: List[str], years: List[int], audio_types: List[str], content_types: List[str],
-                text: Optional[str]):
-        if not authors or self.author in authors:
-            if not years or self.year in years:
-                if not audio_types or any(a_t in audio_types for a_t in self.audio_types):
-                    if not content_types or self.content_type in content_types:
-                        return not text or self.__text_match(text)
+                tmdb_id: str, text: Optional[str]):
+        if not tmdb_id or self.the_movie_db == tmdb_id:
+            if not authors or self.author in authors:
+                if not years or self.year in years:
+                    if not audio_types or any(a_t in audio_types for a_t in self.audio_types):
+                        if not content_types or self.content_type in content_types:
+                            return not text or self.__text_match(text)
         return False
 
     def __text_match(self, text: str):
         t = text.lower()
         return t in self.formatted_title.lower() \
             or t in self.alt_title \
             or t in self.for_search.get('collection', '').lower()
```

### Comparing `ezbeq-1.0.1/ezbeq/config.py` & `ezbeq-1.0.2/ezbeq/config.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/device.py` & `ezbeq-1.0.2/ezbeq/device.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/htp1.py` & `ezbeq-1.0.2/ezbeq/htp1.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/iir.py` & `ezbeq-1.0.2/ezbeq/iir.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/jriver.py` & `ezbeq-1.0.2/ezbeq/jriver.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/main.py` & `ezbeq-1.0.2/ezbeq/main.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/minidsp.py` & `ezbeq-1.0.2/ezbeq/minidsp.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/qsys.py` & `ezbeq-1.0.2/ezbeq/qsys.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/ui/android-chrome-192x192.png` & `ezbeq-1.0.2/ezbeq/ui/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/ui/android-chrome-512x512.png` & `ezbeq-1.0.2/ezbeq/ui/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/ui/apple-touch-icon.png` & `ezbeq-1.0.2/ezbeq/ui/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/ui/assets/index-3477b443.js` & `ezbeq-1.0.2/ezbeq/ui/assets/index-3477b443.js`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/ui/assets/index-fce6f16f.css` & `ezbeq-1.0.2/ezbeq/ui/assets/index-fce6f16f.css`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff` & `ezbeq-1.0.2/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2` & `ezbeq-1.0.2/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2` & `ezbeq-1.0.2/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2` & `ezbeq-1.0.2/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2` & `ezbeq-1.0.2/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2` & `ezbeq-1.0.2/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2` & `ezbeq-1.0.2/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/ui/favicon-16x16.png` & `ezbeq-1.0.2/ezbeq/ui/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/ui/favicon-32x32.png` & `ezbeq-1.0.2/ezbeq/ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/ui/favicon.ico` & `ezbeq-1.0.2/ezbeq/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/ui/index.html` & `ezbeq-1.0.2/ezbeq/ui/index.html`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/ui/mstile-150x150.png` & `ezbeq-1.0.2/ezbeq/ui/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/ezbeq/ui/safari-pinned-tab.svg` & `ezbeq-1.0.2/ezbeq/ui/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.1/pyproject.toml` & `ezbeq-1.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ezbeq"
-version = "1.0.1"
+version = "1.0.2"
 description = "A webapp which can send beqcatalogue filters to a DSP device"
 authors = ["3ll3d00d <mattkhan+ezbeq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://ezbeq.readthedocs.io/"
 repository = "https://github.com/3ll3d00d/ezbeq"
 include = [
```

### Comparing `ezbeq-1.0.1/PKG-INFO` & `ezbeq-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezbeq
-Version: 1.0.1
+Version: 1.0.2
 Summary: A webapp which can send beqcatalogue filters to a DSP device
 Home-page: https://ezbeq.readthedocs.io/
 License: MIT
 Author: 3ll3d00d
 Author-email: mattkhan+ezbeq@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

