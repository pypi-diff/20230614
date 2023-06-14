# Comparing `tmp/django-permissions-policy-4.8.0.tar.gz` & `tmp/django-permissions-policy-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-permissions-policy-4.8.0.tar", last modified: Wed Feb 16 22:20:48 2022, max compression
+gzip compressed data, was "django-permissions-policy-4.9.0.tar", last modified: Fri Mar 25 23:41:31 2022, max compression
```

## Comparing `django-permissions-policy-4.8.0.tar` & `django-permissions-policy-4.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-02-16 22:20:48.089520 django-permissions-policy-4.8.0/
--rw-r--r--   0 chainz     (501) staff       (20)     7682 2022-02-16 22:20:36.000000 django-permissions-policy-4.8.0/HISTORY.rst
--rw-r--r--   0 chainz     (501) staff       (20)     1069 2022-01-19 15:28:02.000000 django-permissions-policy-4.8.0/LICENSE
--rw-r--r--   0 chainz     (501) staff       (20)      245 2021-12-28 23:43:58.000000 django-permissions-policy-4.8.0/MANIFEST.in
--rw-r--r--   0 chainz     (501) staff       (20)     5830 2022-02-16 22:20:48.089669 django-permissions-policy-4.8.0/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)     4566 2022-01-10 16:13:37.000000 django-permissions-policy-4.8.0/README.rst
--rw-r--r--   0 chainz     (501) staff       (20)      687 2022-01-19 11:13:54.000000 django-permissions-policy-4.8.0/pyproject.toml
--rw-r--r--   0 chainz     (501) staff       (20)     1563 2022-02-16 22:20:48.090368 django-permissions-policy-4.8.0/setup.cfg
--rw-r--r--   0 chainz     (501) staff       (20)       74 2022-01-19 11:13:54.000000 django-permissions-policy-4.8.0/setup.py
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-02-16 22:20:48.085075 django-permissions-policy-4.8.0/src/
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-02-16 22:20:48.087693 django-permissions-policy-4.8.0/src/django_permissions_policy/
--rw-r--r--   0 chainz     (501) staff       (20)     3717 2022-02-16 22:20:28.000000 django-permissions-policy-4.8.0/src/django_permissions_policy/__init__.py
--rw-r--r--   0 chainz     (501) staff       (20)        0 2021-08-07 11:26:22.000000 django-permissions-policy-4.8.0/src/django_permissions_policy/py.typed
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-02-16 22:20:48.089307 django-permissions-policy-4.8.0/src/django_permissions_policy.egg-info/
--rw-r--r--   0 chainz     (501) staff       (20)     5830 2022-02-16 22:20:47.000000 django-permissions-policy-4.8.0/src/django_permissions_policy.egg-info/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)      473 2022-02-16 22:20:48.000000 django-permissions-policy-4.8.0/src/django_permissions_policy.egg-info/SOURCES.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2022-02-16 22:20:47.000000 django-permissions-policy-4.8.0/src/django_permissions_policy.egg-info/dependency_links.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2022-02-16 22:20:47.000000 django-permissions-policy-4.8.0/src/django_permissions_policy.egg-info/not-zip-safe
--rw-r--r--   0 chainz     (501) staff       (20)       12 2022-02-16 22:20:48.000000 django-permissions-policy-4.8.0/src/django_permissions_policy.egg-info/requires.txt
--rw-r--r--   0 chainz     (501) staff       (20)       26 2022-02-16 22:20:48.000000 django-permissions-policy-4.8.0/src/django_permissions_policy.egg-info/top_level.txt
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-03-25 23:41:31.785341 django-permissions-policy-4.9.0/
+-rw-r--r--   0 chainz     (501) staff       (20)     7832 2022-03-25 23:41:17.000000 django-permissions-policy-4.9.0/HISTORY.rst
+-rw-r--r--   0 chainz     (501) staff       (20)     1069 2022-01-19 15:28:02.000000 django-permissions-policy-4.9.0/LICENSE
+-rw-r--r--   0 chainz     (501) staff       (20)      245 2021-12-28 23:43:58.000000 django-permissions-policy-4.9.0/MANIFEST.in
+-rw-r--r--   0 chainz     (501) staff       (20)     5796 2022-03-25 23:41:31.785582 django-permissions-policy-4.9.0/PKG-INFO
+-rw-r--r--   0 chainz     (501) staff       (20)     4532 2022-02-23 09:27:14.000000 django-permissions-policy-4.9.0/README.rst
+-rw-r--r--   0 chainz     (501) staff       (20)      687 2022-01-19 11:13:54.000000 django-permissions-policy-4.9.0/pyproject.toml
+-rw-r--r--   0 chainz     (501) staff       (20)     1563 2022-03-25 23:41:31.786591 django-permissions-policy-4.9.0/setup.cfg
+-rw-r--r--   0 chainz     (501) staff       (20)       74 2022-01-19 11:13:54.000000 django-permissions-policy-4.9.0/setup.py
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-03-25 23:41:31.767217 django-permissions-policy-4.9.0/src/
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-03-25 23:41:31.781278 django-permissions-policy-4.9.0/src/django_permissions_policy/
+-rw-r--r--   0 chainz     (501) staff       (20)     3747 2022-03-25 23:41:06.000000 django-permissions-policy-4.9.0/src/django_permissions_policy/__init__.py
+-rw-r--r--   0 chainz     (501) staff       (20)        0 2021-08-07 11:26:22.000000 django-permissions-policy-4.9.0/src/django_permissions_policy/py.typed
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-03-25 23:41:31.784915 django-permissions-policy-4.9.0/src/django_permissions_policy.egg-info/
+-rw-r--r--   0 chainz     (501) staff       (20)     5796 2022-03-25 23:41:31.000000 django-permissions-policy-4.9.0/src/django_permissions_policy.egg-info/PKG-INFO
+-rw-r--r--   0 chainz     (501) staff       (20)      473 2022-03-25 23:41:31.000000 django-permissions-policy-4.9.0/src/django_permissions_policy.egg-info/SOURCES.txt
+-rw-r--r--   0 chainz     (501) staff       (20)        1 2022-03-25 23:41:31.000000 django-permissions-policy-4.9.0/src/django_permissions_policy.egg-info/dependency_links.txt
+-rw-r--r--   0 chainz     (501) staff       (20)        1 2022-03-25 23:41:29.000000 django-permissions-policy-4.9.0/src/django_permissions_policy.egg-info/not-zip-safe
+-rw-r--r--   0 chainz     (501) staff       (20)       12 2022-03-25 23:41:31.000000 django-permissions-policy-4.9.0/src/django_permissions_policy.egg-info/requires.txt
+-rw-r--r--   0 chainz     (501) staff       (20)       26 2022-03-25 23:41:31.000000 django-permissions-policy-4.9.0/src/django_permissions_policy.egg-info/top_level.txt
```

### Comparing `django-permissions-policy-4.8.0/HISTORY.rst` & `django-permissions-policy-4.9.0/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 =======
 History
 =======
 
+4.9.0 (2022-03-25)
+------------------
+
+* Updated to the latest set of features from Chrome 100 dev.
+
+  New features:
+
+  - ``ch-partitioned-cookies``
+
 4.8.0 (2022-02-16)
 ------------------
 
 * Updated to the latest set of features from Chrome 100 dev.
 
   New features:
```

### Comparing `django-permissions-policy-4.8.0/LICENSE` & `django-permissions-policy-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-permissions-policy-4.8.0/PKG-INFO` & `django-permissions-policy-4.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-permissions-policy
-Version: 4.8.0
+Version: 4.9.0
 Summary: Set the draft security HTTP header Permissions-Policy (previously Feature-Policy) on your Django app.
 Home-page: https://github.com/adamchainz/django-permissions-policy
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-permissions-policy/blob/main/HISTORY.rst
 Project-URL: Twitter, https://twitter.com/adamchainz
@@ -100,15 +100,14 @@
            "camera": [],
            "display-capture": [],
            "document-domain": [],
            "encrypted-media": [],
            "fullscreen": [],
            "geolocation": [],
            "gyroscope": [],
-           "interest-cohort": [],
            "magnetometer": [],
            "microphone": [],
            "midi": [],
            "payment": [],
            "usb": [],
        }
```

### Comparing `django-permissions-policy-4.8.0/README.rst` & `django-permissions-policy-4.9.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,14 @@
            "camera": [],
            "display-capture": [],
            "document-domain": [],
            "encrypted-media": [],
            "fullscreen": [],
            "geolocation": [],
            "gyroscope": [],
-           "interest-cohort": [],
            "magnetometer": [],
            "microphone": [],
            "midi": [],
            "payment": [],
            "usb": [],
        }
```

### Comparing `django-permissions-policy-4.8.0/pyproject.toml` & `django-permissions-policy-4.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-permissions-policy-4.8.0/setup.cfg` & `django-permissions-policy-4.9.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-permissions-policy
-version = 4.8.0
+version = 4.9.0
 description = Set the draft security HTTP header Permissions-Policy (previously Feature-Policy) on your Django app.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Adam Johnson
 author_email = me@adamj.eu
 url = https://github.com/adamchainz/django-permissions-policy
 project_urls =
```

### Comparing `django-permissions-policy-4.8.0/src/django_permissions_policy/__init__.py` & `django-permissions-policy-4.9.0/src/django_permissions_policy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     "attribution-reporting",
     "autoplay",
     "camera",
     "ch-device-memory",
     "ch-downlink",
     "ch-dpr",
     "ch-ect",
+    "ch-partitioned-cookies",
     "ch-prefers-color-scheme",
     "ch-rtt",
     "ch-ua",
     "ch-ua-arch",
     "ch-ua-bitness",
     "ch-ua-full-version",
     "ch-ua-full-version-list",
```

### Comparing `django-permissions-policy-4.8.0/src/django_permissions_policy.egg-info/PKG-INFO` & `django-permissions-policy-4.9.0/src/django_permissions_policy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-permissions-policy
-Version: 4.8.0
+Version: 4.9.0
 Summary: Set the draft security HTTP header Permissions-Policy (previously Feature-Policy) on your Django app.
 Home-page: https://github.com/adamchainz/django-permissions-policy
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-permissions-policy/blob/main/HISTORY.rst
 Project-URL: Twitter, https://twitter.com/adamchainz
@@ -100,15 +100,14 @@
            "camera": [],
            "display-capture": [],
            "document-domain": [],
            "encrypted-media": [],
            "fullscreen": [],
            "geolocation": [],
            "gyroscope": [],
-           "interest-cohort": [],
            "magnetometer": [],
            "microphone": [],
            "midi": [],
            "payment": [],
            "usb": [],
        }
```

