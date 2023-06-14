# Comparing `tmp/encord_active_components-0.0.8.tar.gz` & `tmp/encord_active_components-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encord_active_components-0.0.8.tar", max compression
+gzip compressed data, was "encord_active_components-0.0.9.tar", max compression
```

## Comparing `encord_active_components-0.0.8.tar` & `encord_active_components-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      636 2023-03-28 12:29:54.979824 encord_active_components-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-27 15:06:17.356593 encord_active_components-0.0.8/src/encord_active_components/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 16:51:15.640814 encord_active_components-0.0.8/src/encord_active_components/components/__init__.py
--rw-r--r--   0        0        0     2181 2023-03-27 15:47:24.541663 encord_active_components-0.0.8/src/encord_active_components/components/pages_menu.py
--rw-r--r--   0        0        0      841 2023-03-27 15:47:24.542022 encord_active_components-0.0.8/src/encord_active_components/components/projects_page.py
--rw-r--r--   0        0        0      253 2023-03-03 15:18:49.358631 encord_active_components-0.0.8/src/encord_active_components/frontend/.gitignore
--rw-r--r--   0        0        0     1901 2023-03-27 15:06:17.357565 encord_active_components-0.0.8/src/encord_active_components/frontend/assets/annotations.svg
--rw-r--r--   0        0        0     1150 2023-03-27 15:06:17.357780 encord_active_components-0.0.8/src/encord_active_components/frontend/assets/classes.svg
--rw-r--r--   0        0        0    22292 2023-03-27 15:06:17.383465 encord_active_components-0.0.8/src/encord_active_components/frontend/assets/default_project_image.webp
--rw-r--r--   0        0        0      881 2023-03-27 15:06:17.357979 encord_active_components-0.0.8/src/encord_active_components/frontend/assets/empty.svg
--rw-r--r--   0        0        0     2496 2023-03-27 15:06:17.358189 encord_active_components-0.0.8/src/encord_active_components/frontend/assets/encord-import.svg
--rw-r--r--   0        0        0     1714 2023-03-27 15:06:17.358428 encord_active_components-0.0.8/src/encord_active_components/frontend/assets/file-image.svg
--rw-r--r--   0        0        0     1175 2023-03-27 15:06:17.358633 encord_active_components-0.0.8/src/encord_active_components/frontend/assets/import.svg
--rw-r--r--   0        0        0     1901 2023-03-28 12:26:16.864373 encord_active_components-0.0.8/src/encord_active_components/frontend/dist/assets/annotations-278aa65e.svg
--rw-r--r--   0        0        0     1150 2023-03-28 12:26:16.864453 encord_active_components-0.0.8/src/encord_active_components/frontend/dist/assets/classes-d8759926.svg
--rw-r--r--   0        0        0    22292 2023-03-28 12:26:16.864173 encord_active_components-0.0.8/src/encord_active_components/frontend/dist/assets/default_project_image-d39f461e.webp
--rw-r--r--   0        0        0      881 2023-03-28 12:26:16.863721 encord_active_components-0.0.8/src/encord_active_components/frontend/dist/assets/empty-aab39c98.svg
--rw-r--r--   0        0        0     2496 2023-03-28 12:26:16.864089 encord_active_components-0.0.8/src/encord_active_components/frontend/dist/assets/encord-import-1cb3a664.svg
--rw-r--r--   0        0        0     1714 2023-03-28 12:26:16.863761 encord_active_components-0.0.8/src/encord_active_components/frontend/dist/assets/file-image-f807a638.svg
--rw-r--r--   0        0        0     1175 2023-03-28 12:26:16.864111 encord_active_components-0.0.8/src/encord_active_components/frontend/dist/assets/import-b86d8e5d.svg
--rw-r--r--   0        0        0   568832 2023-03-28 12:26:16.864287 encord_active_components-0.0.8/src/encord_active_components/frontend/dist/assets/index-36dd0d8c.css
--rw-r--r--   0        0        0   593300 2023-03-28 12:26:16.864215 encord_active_components-0.0.8/src/encord_active_components/frontend/dist/assets/index-61a8f6a0.js
--rw-r--r--   0        0        0      404 2023-03-28 12:26:16.863928 encord_active_components-0.0.8/src/encord_active_components/frontend/dist/index.html
--rw-r--r--   0        0        0      311 2023-03-16 16:56:09.646946 encord_active_components-0.0.8/src/encord_active_components/frontend/index.html
--rw-r--r--   0        0        0   268212 2023-03-27 16:04:49.386490 encord_active_components-0.0.8/src/encord_active_components/frontend/package-lock.json
--rw-r--r--   0        0        0      814 2023-03-27 15:47:24.543859 encord_active_components-0.0.8/src/encord_active_components/frontend/package.json
--rw-r--r--   0        0        0      114 2023-03-03 15:18:49.407790 encord_active_components-0.0.8/src/encord_active_components/frontend/postcss.config.cjs
--rw-r--r--   0        0        0      466 2023-03-27 15:06:17.361962 encord_active_components-0.0.8/src/encord_active_components/frontend/tailwind.config.cjs
--rw-r--r--   0        0        0      559 2023-03-03 15:18:49.429946 encord_active_components-0.0.8/src/encord_active_components/frontend/tsconfig.json
--rw-r--r--   0        0        0      184 2023-03-03 15:18:49.441961 encord_active_components-0.0.8/src/encord_active_components/frontend/tsconfig.node.json
--rw-r--r--   0        0        0      178 2023-03-03 15:18:49.453528 encord_active_components-0.0.8/src/encord_active_components/frontend/vite.config.ts
--rw-r--r--   0        0        0      553 2023-03-27 16:15:21.260618 encord_active_components-0.0.8/src/encord_active_components/renderer.py
--rw-r--r--   0        0        0     1066 1970-01-01 00:00:00.000000 encord_active_components-0.0.8/setup.py
--rw-r--r--   0        0        0      623 1970-01-01 00:00:00.000000 encord_active_components-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      636 2023-04-05 11:14:58.868476 encord_active_components-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-30 14:28:44.001294 encord_active_components-0.0.9/src/encord_active_components/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-30 14:28:44.001453 encord_active_components-0.0.9/src/encord_active_components/components/__init__.py
+-rw-r--r--   0        0        0     2181 2023-03-30 14:28:44.002188 encord_active_components-0.0.9/src/encord_active_components/components/pages_menu.py
+-rw-r--r--   0        0        0      841 2023-03-30 14:28:44.002881 encord_active_components-0.0.9/src/encord_active_components/components/projects_page.py
+-rw-r--r--   0        0        0      253 2023-03-03 15:18:49.358631 encord_active_components-0.0.9/src/encord_active_components/frontend/.gitignore
+-rw-r--r--   0        0        0     1901 2023-03-30 14:28:44.004393 encord_active_components-0.0.9/src/encord_active_components/frontend/assets/annotations.svg
+-rw-r--r--   0        0        0     1150 2023-03-30 14:28:44.005070 encord_active_components-0.0.9/src/encord_active_components/frontend/assets/classes.svg
+-rw-r--r--   0        0        0    22292 2023-03-30 14:28:44.007000 encord_active_components-0.0.9/src/encord_active_components/frontend/assets/default_project_image.webp
+-rw-r--r--   0        0        0      881 2023-03-30 14:28:44.008126 encord_active_components-0.0.9/src/encord_active_components/frontend/assets/empty.svg
+-rw-r--r--   0        0        0     2496 2023-03-30 14:28:44.008767 encord_active_components-0.0.9/src/encord_active_components/frontend/assets/encord-import.svg
+-rw-r--r--   0        0        0     1714 2023-03-30 14:28:44.009304 encord_active_components-0.0.9/src/encord_active_components/frontend/assets/file-image.svg
+-rw-r--r--   0        0        0     1175 2023-03-30 14:28:44.010128 encord_active_components-0.0.9/src/encord_active_components/frontend/assets/import.svg
+-rw-r--r--   0        0        0     1901 2023-04-05 11:14:24.817401 encord_active_components-0.0.9/src/encord_active_components/frontend/dist/assets/annotations-278aa65e.svg
+-rw-r--r--   0        0        0     1150 2023-04-05 11:14:24.817448 encord_active_components-0.0.9/src/encord_active_components/frontend/dist/assets/classes-d8759926.svg
+-rw-r--r--   0        0        0    22292 2023-04-05 11:14:24.817195 encord_active_components-0.0.9/src/encord_active_components/frontend/dist/assets/default_project_image-d39f461e.webp
+-rw-r--r--   0        0        0      881 2023-04-05 11:14:24.817130 encord_active_components-0.0.9/src/encord_active_components/frontend/dist/assets/empty-aab39c98.svg
+-rw-r--r--   0        0        0     2496 2023-04-05 11:14:24.817359 encord_active_components-0.0.9/src/encord_active_components/frontend/dist/assets/encord-import-1cb3a664.svg
+-rw-r--r--   0        0        0     1714 2023-04-05 11:14:24.817322 encord_active_components-0.0.9/src/encord_active_components/frontend/dist/assets/file-image-f807a638.svg
+-rw-r--r--   0        0        0     1175 2023-04-05 11:14:24.817224 encord_active_components-0.0.9/src/encord_active_components/frontend/dist/assets/import-b86d8e5d.svg
+-rw-r--r--   0        0        0   568832 2023-04-05 11:14:24.817835 encord_active_components-0.0.9/src/encord_active_components/frontend/dist/assets/index-36dd0d8c.css
+-rw-r--r--   0        0        0   593283 2023-04-05 11:14:24.817915 encord_active_components-0.0.9/src/encord_active_components/frontend/dist/assets/index-b1789b4f.js
+-rw-r--r--   0        0        0      404 2023-04-05 11:14:24.817266 encord_active_components-0.0.9/src/encord_active_components/frontend/dist/index.html
+-rw-r--r--   0        0        0      311 2023-04-03 11:54:15.620129 encord_active_components-0.0.9/src/encord_active_components/frontend/index.html
+-rw-r--r--   0        0        0   268212 2023-04-05 10:52:11.126399 encord_active_components-0.0.9/src/encord_active_components/frontend/package-lock.json
+-rw-r--r--   0        0        0      814 2023-04-05 10:52:11.126941 encord_active_components-0.0.9/src/encord_active_components/frontend/package.json
+-rw-r--r--   0        0        0      114 2023-03-03 15:18:49.407790 encord_active_components-0.0.9/src/encord_active_components/frontend/postcss.config.cjs
+-rw-r--r--   0        0        0      466 2023-03-30 14:28:44.021175 encord_active_components-0.0.9/src/encord_active_components/frontend/tailwind.config.cjs
+-rw-r--r--   0        0        0      559 2023-03-03 15:18:49.429946 encord_active_components-0.0.9/src/encord_active_components/frontend/tsconfig.json
+-rw-r--r--   0        0        0      184 2023-03-03 15:18:49.441961 encord_active_components-0.0.9/src/encord_active_components/frontend/tsconfig.node.json
+-rw-r--r--   0        0        0      178 2023-03-03 15:18:49.453528 encord_active_components-0.0.9/src/encord_active_components/frontend/vite.config.ts
+-rw-r--r--   0        0        0      553 2023-04-05 10:52:11.130509 encord_active_components-0.0.9/src/encord_active_components/renderer.py
+-rw-r--r--   0        0        0     1066 1970-01-01 00:00:00.000000 encord_active_components-0.0.9/setup.py
+-rw-r--r--   0        0        0      623 1970-01-01 00:00:00.000000 encord_active_components-0.0.9/PKG-INFO
```

### Comparing `encord_active_components-0.0.8/pyproject.toml` & `encord_active_components-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encord-active-components"
-version = "0.0.8"
+version = "0.0.9"
 description = "Frontend components used by Encord Active"
 authors = ["Cord Technologies Limited <hello@encord.com>"]
 license = "Apache-2.0"
 
 packages = [{include = "encord_active_components", from = "src"}]
 include = ["src/encord_active_components/frontend/dist/**/*"]
 exclude = [
```

### Comparing `encord_active_components-0.0.8/src/encord_active_components/components/pages_menu.py` & `encord_active_components-0.0.9/src/encord_active_components/components/pages_menu.py`

 * *Files identical despite different names*

### Comparing `encord_active_components-0.0.8/src/encord_active_components/components/projects_page.py` & `encord_active_components-0.0.9/src/encord_active_components/components/projects_page.py`

 * *Files identical despite different names*

### Comparing `encord_active_components-0.0.8/src/encord_active_components/frontend/assets/annotations.svg` & `encord_active_components-0.0.9/src/encord_active_components/frontend/assets/annotations.svg`

 * *Files identical despite different names*

### Comparing `encord_active_components-0.0.8/src/encord_active_components/frontend/assets/classes.svg` & `encord_active_components-0.0.9/src/encord_active_components/frontend/assets/classes.svg`

 * *Files identical despite different names*

### Comparing `encord_active_components-0.0.8/src/encord_active_components/frontend/assets/default_project_image.webp` & `encord_active_components-0.0.9/src/encord_active_components/frontend/assets/default_project_image.webp`

 * *Files identical despite different names*

### Comparing `encord_active_components-0.0.8/src/encord_active_components/frontend/assets/empty.svg` & `encord_active_components-0.0.9/src/encord_active_components/frontend/assets/empty.svg`

 * *Files identical despite different names*

### Comparing `encord_active_components-0.0.8/src/encord_active_components/frontend/assets/encord-import.svg` & `encord_active_components-0.0.9/src/encord_active_components/frontend/assets/encord-import.svg`

 * *Files identical despite different names*

### Comparing `encord_active_components-0.0.8/src/encord_active_components/frontend/assets/file-image.svg` & `encord_active_components-0.0.9/src/encord_active_components/frontend/assets/file-image.svg`

 * *Files identical despite different names*

### Comparing `encord_active_components-0.0.8/src/encord_active_components/frontend/assets/import.svg` & `encord_active_components-0.0.9/src/encord_active_components/frontend/assets/import.svg`

 * *Files identical despite different names*

### Comparing `encord_active_components-0.0.8/src/encord_active_components/frontend/dist/assets/annotations-278aa65e.svg` & `encord_active_components-0.0.9/src/encord_active_components/frontend/dist/assets/annotations-278aa65e.svg`

 * *Files identical despite different names*

### Comparing `encord_active_components-0.0.8/src/encord_active_components/frontend/dist/assets/classes-d8759926.svg` & `encord_active_components-0.0.9/src/encord_active_components/frontend/dist/assets/classes-d8759926.svg`

 * *Files identical despite different names*

### Comparing `encord_active_components-0.0.8/src/encord_active_components/frontend/dist/assets/default_project_image-d39f461e.webp` & `encord_active_components-0.0.9/src/encord_active_components/frontend/dist/assets/default_project_image-d39f461e.webp`

 * *Files identical despite different names*

### Comparing `encord_active_components-0.0.8/src/encord_active_components/frontend/dist/assets/empty-aab39c98.svg` & `encord_active_components-0.0.9/src/encord_active_components/frontend/dist/assets/empty-aab39c98.svg`

 * *Files identical despite different names*

### Comparing `encord_active_components-0.0.8/src/encord_active_components/frontend/dist/assets/encord-import-1cb3a664.svg` & `encord_active_components-0.0.9/src/encord_active_components/frontend/dist/assets/encord-import-1cb3a664.svg`

 * *Files identical despite different names*

### Comparing `encord_active_components-0.0.8/src/encord_active_components/frontend/dist/assets/file-image-f807a638.svg` & `encord_active_components-0.0.9/src/encord_active_components/frontend/dist/assets/file-image-f807a638.svg`

 * *Files identical despite different names*

### Comparing `encord_active_components-0.0.8/src/encord_active_components/frontend/dist/assets/import-b86d8e5d.svg` & `encord_active_components-0.0.9/src/encord_active_components/frontend/dist/assets/import-b86d8e5d.svg`

 * *Files identical despite different names*

### Comparing `encord_active_components-0.0.8/src/encord_active_components/frontend/dist/assets/index-36dd0d8c.css` & `encord_active_components-0.0.9/src/encord_active_components/frontend/dist/assets/index-36dd0d8c.css`

 * *Files identical despite different names*

### Comparing `encord_active_components-0.0.8/src/encord_active_components/frontend/dist/assets/index-61a8f6a0.js` & `encord_active_components-0.0.9/src/encord_active_components/frontend/dist/assets/index-b1789b4f.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -29148,15 +29148,15 @@
         showDownloadedBadge: t = !1,
         onClick: n
     }) => Qt(VI, {
         onClick: n,
         children: [Q("figure", {
             className: "max-h-36 rounded",
             children: Q("img", {
-                src: e.imageUrl ? window.location.ancestorOrigins[0] + e.imageUrl : Oj,
+                src: e.imageUrl ? document.referrer + e.imageUrl : Oj,
                 alt: e.name
             })
         }), Qt("div", {
             className: "card-body w-full p-0 justify-between gap-1",
             children: [Q("h2", {
                 className: "card-title text-sm line-clamp-2",
                 children: e.name
```

### Comparing `encord_active_components-0.0.8/src/encord_active_components/frontend/package-lock.json` & `encord_active_components-0.0.9/src/encord_active_components/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `encord_active_components-0.0.8/src/encord_active_components/frontend/package.json` & `encord_active_components-0.0.9/src/encord_active_components/frontend/package.json`

 * *Files identical despite different names*

### Comparing `encord_active_components-0.0.8/src/encord_active_components/frontend/tsconfig.json` & `encord_active_components-0.0.9/src/encord_active_components/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `encord_active_components-0.0.8/src/encord_active_components/renderer.py` & `encord_active_components-0.0.9/src/encord_active_components/renderer.py`

 * *Files identical despite different names*

### Comparing `encord_active_components-0.0.8/setup.py` & `encord_active_components-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
                               'frontend/dist/assets/*']}
 
 install_requires = \
 ['streamlit>=1.19.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'encord-active-components',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Frontend components used by Encord Active',
     'long_description': 'None',
     'author': 'Cord Technologies Limited',
     'author_email': 'hello@encord.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `encord_active_components-0.0.8/PKG-INFO` & `encord_active_components-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encord-active-components
-Version: 0.0.8
+Version: 0.0.9
 Summary: Frontend components used by Encord Active
 License: Apache-2.0
 Author: Cord Technologies Limited
 Author-email: hello@encord.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

