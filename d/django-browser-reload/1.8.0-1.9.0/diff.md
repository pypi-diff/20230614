# Comparing `tmp/django_browser_reload-1.8.0.tar.gz` & `tmp/django_browser_reload-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_browser_reload-1.8.0.tar", last modified: Tue Apr 11 18:26:02 2023, max compression
+gzip compressed data, was "django_browser_reload-1.9.0.tar", last modified: Mon Jun  5 21:15:22 2023, max compression
```

## Comparing `django_browser_reload-1.8.0.tar` & `django_browser_reload-1.9.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-11 18:26:02.496020 django_browser_reload-1.8.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1812 2023-04-11 18:25:59.000000 django_browser_reload-1.8.0/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:58:23.000000 django_browser_reload-1.8.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      130 2023-01-20 12:09:56.000000 django_browser_reload-1.8.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)     9832 2023-04-11 18:26:02.496102 django_browser_reload-1.8.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     8425 2023-01-20 11:36:46.000000 django_browser_reload-1.8.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      500 2023-02-28 09:05:51.000000 django_browser_reload-1.8.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1681 2023-04-11 18:26:02.496419 django_browser_reload-1.8.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-11 18:26:02.492169 django_browser_reload-1.8.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-11 18:26:02.494168 django_browser_reload-1.8.0/src/django_browser_reload/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:28.000000 django_browser_reload-1.8.0/src/django_browser_reload/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      324 2022-06-03 11:58:28.000000 django_browser_reload-1.8.0/src/django_browser_reload/apps.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      646 2022-06-03 11:58:28.000000 django_browser_reload-1.8.0/src/django_browser_reload/jinja.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2770 2022-11-08 22:26:11.000000 django_browser_reload-1.8.0/src/django_browser_reload/middleware.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:28.000000 django_browser_reload-1.8.0/src/django_browser_reload/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-11 18:26:02.492292 django_browser_reload-1.8.0/src/django_browser_reload/static/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-11 18:26:02.495281 django_browser_reload-1.8.0/src/django_browser_reload/static/django-browser-reload/
--rw-r--r--   0 adamjohnson   (501) staff       (20)      623 2022-06-03 11:58:28.000000 django_browser_reload-1.8.0/src/django_browser_reload/static/django-browser-reload/reload-listener.js
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2711 2023-04-11 18:15:57.000000 django_browser_reload-1.8.0/src/django_browser_reload/static/django-browser-reload/reload-worker.js
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-11 18:26:02.495540 django_browser_reload-1.8.0/src/django_browser_reload/templatetags/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:28.000000 django_browser_reload-1.8.0/src/django_browser_reload/templatetags/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      215 2022-11-04 10:25:47.000000 django_browser_reload-1.8.0/src/django_browser_reload/templatetags/django_browser_reload.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      211 2022-11-04 10:25:47.000000 django_browser_reload-1.8.0/src/django_browser_reload/urls.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     5141 2023-04-11 18:20:55.000000 django_browser_reload-1.8.0/src/django_browser_reload/views.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-11 18:26:02.494995 django_browser_reload-1.8.0/src/django_browser_reload.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     9832 2023-04-11 18:26:02.000000 django_browser_reload-1.8.0/src/django_browser_reload.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      938 2023-04-11 18:26:02.000000 django_browser_reload-1.8.0/src/django_browser_reload.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-04-11 18:26:02.000000 django_browser_reload-1.8.0/src/django_browser_reload.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-04-11 18:26:02.000000 django_browser_reload-1.8.0/src/django_browser_reload.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       12 2023-04-11 18:26:02.000000 django_browser_reload-1.8.0/src/django_browser_reload.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       22 2023-04-11 18:26:02.000000 django_browser_reload-1.8.0/src/django_browser_reload.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-11 18:26:02.495916 django_browser_reload-1.8.0/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)      781 2022-11-04 10:30:45.000000 django_browser_reload-1.8.0/tests/test_jinja.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     5179 2022-11-04 10:30:45.000000 django_browser_reload-1.8.0/tests/test_middleware.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     5001 2023-04-11 18:20:55.000000 django_browser_reload-1.8.0/tests/test_views.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-05 21:15:22.496430 django_browser_reload-1.9.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1992 2023-06-05 21:15:19.000000 django_browser_reload-1.9.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:58:23.000000 django_browser_reload-1.9.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      130 2023-01-20 12:09:56.000000 django_browser_reload-1.9.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     9788 2023-06-05 21:15:22.496590 django_browser_reload-1.9.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     8381 2023-06-05 21:08:14.000000 django_browser_reload-1.9.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      500 2023-02-28 09:05:51.000000 django_browser_reload-1.9.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1681 2023-06-05 21:15:22.496957 django_browser_reload-1.9.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-05 21:15:22.480754 django_browser_reload-1.9.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-05 21:15:22.494634 django_browser_reload-1.9.0/src/django_browser_reload/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:28.000000 django_browser_reload-1.9.0/src/django_browser_reload/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      324 2022-06-03 11:58:28.000000 django_browser_reload-1.9.0/src/django_browser_reload/apps.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      646 2023-06-05 20:18:52.000000 django_browser_reload-1.9.0/src/django_browser_reload/jinja.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2770 2023-06-05 20:52:27.000000 django_browser_reload-1.9.0/src/django_browser_reload/middleware.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:28.000000 django_browser_reload-1.9.0/src/django_browser_reload/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-05 21:15:22.480877 django_browser_reload-1.9.0/src/django_browser_reload/static/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-05 21:15:22.495690 django_browser_reload-1.9.0/src/django_browser_reload/static/django-browser-reload/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      623 2022-06-03 11:58:28.000000 django_browser_reload-1.9.0/src/django_browser_reload/static/django-browser-reload/reload-listener.js
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2711 2023-04-11 18:15:57.000000 django_browser_reload-1.9.0/src/django_browser_reload/static/django-browser-reload/reload-worker.js
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-05 21:15:22.495911 django_browser_reload-1.9.0/src/django_browser_reload/templatetags/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:28.000000 django_browser_reload-1.9.0/src/django_browser_reload/templatetags/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      215 2023-06-05 20:18:52.000000 django_browser_reload-1.9.0/src/django_browser_reload/templatetags/django_browser_reload.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      211 2022-11-04 10:25:47.000000 django_browser_reload-1.9.0/src/django_browser_reload/urls.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     6045 2023-06-05 21:08:14.000000 django_browser_reload-1.9.0/src/django_browser_reload/views.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-05 21:15:22.495421 django_browser_reload-1.9.0/src/django_browser_reload.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     9788 2023-06-05 21:15:22.000000 django_browser_reload-1.9.0/src/django_browser_reload.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      938 2023-06-05 21:15:22.000000 django_browser_reload-1.9.0/src/django_browser_reload.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-05 21:15:22.000000 django_browser_reload-1.9.0/src/django_browser_reload.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-05 21:15:22.000000 django_browser_reload-1.9.0/src/django_browser_reload.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       12 2023-06-05 21:15:22.000000 django_browser_reload-1.9.0/src/django_browser_reload.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       22 2023-06-05 21:15:22.000000 django_browser_reload-1.9.0/src/django_browser_reload.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-05 21:15:22.496304 django_browser_reload-1.9.0/tests/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      781 2022-11-04 10:30:45.000000 django_browser_reload-1.9.0/tests/test_jinja.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     5161 2023-06-05 10:24:57.000000 django_browser_reload-1.9.0/tests/test_middleware.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     7717 2023-06-05 21:08:14.000000 django_browser_reload-1.9.0/tests/test_views.py
```

### Comparing `django_browser_reload-1.8.0/CHANGELOG.rst` & `django_browser_reload-1.9.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =========
 Changelog
 =========
 
+1.9.0 (2023-06-05)
+------------------
+
+* Support ASGI on Django 4.2+.
+
+  Thanks to Alexandre Spaeth in `PR #148 <https://github.com/adamchainz/django-browser-reload/pull/148>`__.
+
 1.8.0 (2023-04-11)
 ------------------
 
 * Support use with `GzipMiddleware`, or other middleware that encodes the response.
 
 1.7.0 (2023-02-25)
 ------------------
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_el470et3_/tmpsuhagt4n_TarContainer/0/1.rst", line 74, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_el470et3_/tmpsuhagt4n_TarContainer/0/1.rst", line 74, column 0: CDATA terminal not found*

```diff
@@ -1,16 +1,18 @@
-========= Changelog ========= 1.8.0 (2023-04-11) ------------------ * Support
-use with `GzipMiddleware`, or other middleware that encodes the response. 1.7.0
-(2023-02-25) ------------------ * Support Django 4.2. 1.6.0 (2022-06-05) ------
------------- * Support Python 3.11. * Support Django 4.1. 1.5.0 (2022-05-18) --
----------------- * Add async support to the middleware, to reduce overhead on
-async projects. * Disable middleware at Django startup when ``DEBUG`` is
-``False``. 1.4.0 (2022-05-10) ------------------ * Drop support for Django 2.2,
-3.0, and 3.1. 1.3.0 (2022-01-13) ------------------ * âDebounceâ reload
-events with a 50 millisecond window. This fixes an issue with repeat triggers
-of the same reload event. It should also help workflows where several files
-change in quick succession. 1.2.0 (2022-01-10) ------------------ * Drop Python
-3.6 support. 1.1.1 (2022-01-10) ------------------ * Prevent restarting the
-server when static assets change. Thanks to Tim Kamanin for the report in
-`Issue #46
+========= Changelog ========= 1.9.0 (2023-06-05) ------------------ * Support
+ASGI on Django 4.2+. Thanks to Alexandre Spaeth in `PR #148
+github.com/adamchainz/django-browser-reload/pull/148>`__. 1.8.0 (2023-04-11) --
+---------------- * Support use with `GzipMiddleware`, or other middleware that
+encodes the response. 1.7.0 (2023-02-25) ------------------ * Support Django
+4.2. 1.6.0 (2022-06-05) ------------------ * Support Python 3.11. * Support
+Django 4.1. 1.5.0 (2022-05-18) ------------------ * Add async support to the
+middleware, to reduce overhead on async projects. * Disable middleware at
+Django startup when ``DEBUG`` is ``False``. 1.4.0 (2022-05-10) ----------------
+-- * Drop support for Django 2.2, 3.0, and 3.1. 1.3.0 (2022-01-13) ------------
+------ * âDebounceâ reload events with a 50 millisecond window. This fixes
+an issue with repeat triggers of the same reload event. It should also help
+workflows where several files change in quick succession. 1.2.0 (2022-01-10) --
+---------------- * Drop Python 3.6 support. 1.1.1 (2022-01-10) ----------------
+-- * Prevent restarting the server when static assets change. Thanks to Tim
+Kamanin for the report in `Issue #46
 github.com/adamchainz/django-browser-reload/issues/46>`__. * Use 'defer' in the
 ``
```

### Comparing `django_browser_reload-1.8.0/LICENSE` & `django_browser_reload-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_browser_reload-1.8.0/PKG-INFO` & `django_browser_reload-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_browser_reload
-Version: 1.8.0
+Version: 1.9.0
 Summary: Automatically reload your browser in development.
 Home-page: https://github.com/adamchainz/django-browser-reload
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-browser-reload/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -57,20 +57,28 @@
 Requirements
 ------------
 
 Python 3.7 to 3.11 supported.
 
 Django 3.2 to 4.2 supported.
 
+WSGI supported on all Django versions. ASGI supported on Django 4.2+.
+
 Your browser needs to support:
 
-* ``EventSource`` - `universally available <https://developer.mozilla.org/en-US/docs/Web/API/EventSource#browser_compatibility>`__.
+* |EventSource|__ - universally available.
+
+  .. |EventSource| replace:: ``EventSource``
+  __ https://developer.mozilla.org/en-US/docs/Web/API/EventSource#browser_compatibility
+
+* |SharedWorker|__ - available on Chrome, Edge, Firefox, and Opera for a long time.
+  Available on Safari since version 16 (2022-09-12).
 
-* ``SharedWorker`` - `available <https://developer.mozilla.org/en-US/docs/Web/API/SharedWorker#browser_compatibility>`__ on Chrome, Edge, Firefox, and Opera.
-  Safari removed support but `are reinstating it <https://bugs.webkit.org/show_bug.cgi?id=149850>`__ - they recently `merged the feature <https://twitter.com/chris_dumez/status/1491650913441701896>`__ (2022-02-10).
+  .. |SharedWorker| replace:: ``SharedWorker``
+  __ https://developer.mozilla.org/en-US/docs/Web/API/SharedWorker#browser_compatibility
 
 ----
 
 **Want to work smarter and faster?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers django-browser-reload and many other tools.
 I wrote django-browser-reload whilst working on the book!
 
@@ -93,15 +101,15 @@
 
        INSTALLED_APPS = [
            ...,
            "django_browser_reload",
            ...,
        ]
 
-4. Include the app URL’s in your root URLconf(s):
+4. Include the app URLs in your root URLconf:
 
    .. code-block:: python
 
        from django.urls import include, path
 
        urlpatterns = [
            ...,
@@ -116,30 +124,29 @@
 
       MIDDLEWARE = [
           # ...
           "django_browser_reload.middleware.BrowserReloadMiddleware",
           # ...
       ]
 
-   The middleware should be listed after any that encode the response, such as Django’s ``GZipMiddleware``.
+   The middleware should be listed after any others that encode the response, such as Django’s ``GZipMiddleware``.
 
    The middleware automatically inserts the required script tag on HTML responses before ``</body>`` when ``DEBUG`` is ``True``.
    It does so to every HTML response, meaning it will be included on Django’s debug pages, admin pages, etc.
    If you want more control, you can instead insert the script tag in your templates—see below.
 
 All done! 📯
 
 For faster and more efficient reloading, also set up `Django’s built-in Watchman support <https://adamj.eu/tech/2021/01/20/efficient-reloading-in-djangos-runserver-with-watchman/>`__.
 
 What It Does
 ------------
 
 When ``DEBUG`` is ``True``, the template tag includes a small script.
 This script connects back to the development server and will automatically reload when static assets or templates are modified, or after ``runserver`` restarts.
-(Detecting modification of Django templates requires Django 3.2+.)
 The reload only happens in the most recently opened tab.
 
 Example Project
 ---------------
 
 See the `example project <https://github.com/adamchainz/django-browser-reload/tree/main/example>`__ in the ``example/`` directory of the GitHub repository.
 Start it up and modify its files to see the reloading in action.
@@ -172,15 +179,15 @@
     {% load django_browser_reload %}
 
     {% block extrahead %}
         {{ block.super }}
         {% django_browser_reload_script %}
     {% endblock %}
 
-This follows Django’s documentation on `extending an overriden template <https://docs.djangoproject.com/en/4.0/howto/overriding-templates/#extending-an-overridden-template>`__.
+This follows Django’s documentation on `extending an overridden template <https://docs.djangoproject.com/en/4.0/howto/overriding-templates/#extending-an-overridden-template>`__.
 
 For **Jinja Templates**, you need to perform two steps.
 First, load the tag function into the globals of your `custom environment <https://docs.djangoproject.com/en/stable/topics/templates/#django.template.backends.jinja2.Jinja2>`__:
 
 .. code-block:: python
 
     # myproject/jinja2.py
@@ -223,21 +230,21 @@
                                listener  listener  listener
                                     \       |       /
       Django                         \      |      /
                                       \     |     /
     Events View --------------------> Shared worker
 
 The template tag includes a listener script on each page.
-This listener script starts or connects to a |SharedWorker|__, running a worker script.
-The worker script then connects to the events view in Django, using an |EventSource|__ to receive server-sent events.
+This listener script starts or connects to a |SharedWorker2|__, running a worker script.
+The worker script then connects to the events view in Django, using an |EventSource2|__ to receive server-sent events.
 
-.. |SharedWorker| replace:: ``SharedWorker``
+.. |SharedWorker2| replace:: ``SharedWorker``
 __ https://developer.mozilla.org/en-US/docs/Web/API/SharedWorker
 
-.. |EventSource| replace:: ``EventSource``
+.. |EventSource2| replace:: ``EventSource``
 __ https://developer.mozilla.org/en-US/docs/Web/API/EventSource
 
 This event source uses |StreamingHttpResponse|__ to send events to the worker.
 The view continues streaming events indefinitely, until disconnected.
 (This requires a thread and will not work if you use ``runserver``\’s |--nothreading option|__.)
 
 .. |--nothreading option| replace:: ``--nothreading`` option
```

### Comparing `django_browser_reload-1.8.0/README.rst` & `django_browser_reload-1.9.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -23,20 +23,28 @@
 Requirements
 ------------
 
 Python 3.7 to 3.11 supported.
 
 Django 3.2 to 4.2 supported.
 
+WSGI supported on all Django versions. ASGI supported on Django 4.2+.
+
 Your browser needs to support:
 
-* ``EventSource`` - `universally available <https://developer.mozilla.org/en-US/docs/Web/API/EventSource#browser_compatibility>`__.
+* |EventSource|__ - universally available.
+
+  .. |EventSource| replace:: ``EventSource``
+  __ https://developer.mozilla.org/en-US/docs/Web/API/EventSource#browser_compatibility
+
+* |SharedWorker|__ - available on Chrome, Edge, Firefox, and Opera for a long time.
+  Available on Safari since version 16 (2022-09-12).
 
-* ``SharedWorker`` - `available <https://developer.mozilla.org/en-US/docs/Web/API/SharedWorker#browser_compatibility>`__ on Chrome, Edge, Firefox, and Opera.
-  Safari removed support but `are reinstating it <https://bugs.webkit.org/show_bug.cgi?id=149850>`__ - they recently `merged the feature <https://twitter.com/chris_dumez/status/1491650913441701896>`__ (2022-02-10).
+  .. |SharedWorker| replace:: ``SharedWorker``
+  __ https://developer.mozilla.org/en-US/docs/Web/API/SharedWorker#browser_compatibility
 
 ----
 
 **Want to work smarter and faster?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers django-browser-reload and many other tools.
 I wrote django-browser-reload whilst working on the book!
 
@@ -59,15 +67,15 @@
 
        INSTALLED_APPS = [
            ...,
            "django_browser_reload",
            ...,
        ]
 
-4. Include the app URL’s in your root URLconf(s):
+4. Include the app URLs in your root URLconf:
 
    .. code-block:: python
 
        from django.urls import include, path
 
        urlpatterns = [
            ...,
@@ -82,30 +90,29 @@
 
       MIDDLEWARE = [
           # ...
           "django_browser_reload.middleware.BrowserReloadMiddleware",
           # ...
       ]
 
-   The middleware should be listed after any that encode the response, such as Django’s ``GZipMiddleware``.
+   The middleware should be listed after any others that encode the response, such as Django’s ``GZipMiddleware``.
 
    The middleware automatically inserts the required script tag on HTML responses before ``</body>`` when ``DEBUG`` is ``True``.
    It does so to every HTML response, meaning it will be included on Django’s debug pages, admin pages, etc.
    If you want more control, you can instead insert the script tag in your templates—see below.
 
 All done! 📯
 
 For faster and more efficient reloading, also set up `Django’s built-in Watchman support <https://adamj.eu/tech/2021/01/20/efficient-reloading-in-djangos-runserver-with-watchman/>`__.
 
 What It Does
 ------------
 
 When ``DEBUG`` is ``True``, the template tag includes a small script.
 This script connects back to the development server and will automatically reload when static assets or templates are modified, or after ``runserver`` restarts.
-(Detecting modification of Django templates requires Django 3.2+.)
 The reload only happens in the most recently opened tab.
 
 Example Project
 ---------------
 
 See the `example project <https://github.com/adamchainz/django-browser-reload/tree/main/example>`__ in the ``example/`` directory of the GitHub repository.
 Start it up and modify its files to see the reloading in action.
@@ -138,15 +145,15 @@
     {% load django_browser_reload %}
 
     {% block extrahead %}
         {{ block.super }}
         {% django_browser_reload_script %}
     {% endblock %}
 
-This follows Django’s documentation on `extending an overriden template <https://docs.djangoproject.com/en/4.0/howto/overriding-templates/#extending-an-overridden-template>`__.
+This follows Django’s documentation on `extending an overridden template <https://docs.djangoproject.com/en/4.0/howto/overriding-templates/#extending-an-overridden-template>`__.
 
 For **Jinja Templates**, you need to perform two steps.
 First, load the tag function into the globals of your `custom environment <https://docs.djangoproject.com/en/stable/topics/templates/#django.template.backends.jinja2.Jinja2>`__:
 
 .. code-block:: python
 
     # myproject/jinja2.py
@@ -189,21 +196,21 @@
                                listener  listener  listener
                                     \       |       /
       Django                         \      |      /
                                       \     |     /
     Events View --------------------> Shared worker
 
 The template tag includes a listener script on each page.
-This listener script starts or connects to a |SharedWorker|__, running a worker script.
-The worker script then connects to the events view in Django, using an |EventSource|__ to receive server-sent events.
+This listener script starts or connects to a |SharedWorker2|__, running a worker script.
+The worker script then connects to the events view in Django, using an |EventSource2|__ to receive server-sent events.
 
-.. |SharedWorker| replace:: ``SharedWorker``
+.. |SharedWorker2| replace:: ``SharedWorker``
 __ https://developer.mozilla.org/en-US/docs/Web/API/SharedWorker
 
-.. |EventSource| replace:: ``EventSource``
+.. |EventSource2| replace:: ``EventSource``
 __ https://developer.mozilla.org/en-US/docs/Web/API/EventSource
 
 This event source uses |StreamingHttpResponse|__ to send events to the worker.
 The view continues streaming events indefinitely, until disconnected.
 (This requires a thread and will not work if you use ``runserver``\’s |--nothreading option|__.)
 
 .. |--nothreading option| replace:: ``--nothreading`` option
```

### Comparing `django_browser_reload-1.8.0/setup.cfg` & `django_browser_reload-1.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_browser_reload
-version = 1.8.0
+version = 1.9.0
 description = Automatically reload your browser in development.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/adamchainz/django-browser-reload
 author = Adam Johnson
 author_email = me@adamj.eu
 license = MIT
```

### Comparing `django_browser_reload-1.8.0/src/django_browser_reload/jinja.py` & `django_browser_reload-1.9.0/src/django_browser_reload/jinja.py`

 * *Files identical despite different names*

### Comparing `django_browser_reload-1.8.0/src/django_browser_reload/middleware.py` & `django_browser_reload-1.9.0/src/django_browser_reload/middleware.py`

 * *Files identical despite different names*

### Comparing `django_browser_reload-1.8.0/src/django_browser_reload/static/django-browser-reload/reload-listener.js` & `django_browser_reload-1.9.0/src/django_browser_reload/static/django-browser-reload/reload-listener.js`

 * *Files identical despite different names*

### Comparing `django_browser_reload-1.8.0/src/django_browser_reload/static/django-browser-reload/reload-worker.js` & `django_browser_reload-1.9.0/src/django_browser_reload/static/django-browser-reload/reload-worker.js`

 * *Files identical despite different names*

### Comparing `django_browser_reload-1.8.0/src/django_browser_reload/views.py` & `django_browser_reload-1.9.0/src/django_browser_reload/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from __future__ import annotations
 
+import asyncio
 import json
 import threading
 from http import HTTPStatus
 from pathlib import Path
 from typing import Any
+from typing import AsyncGenerator
+from typing import Callable
 from typing import Generator
 
+import django
 from django.conf import settings
 from django.contrib.staticfiles.finders import AppDirectoriesFinder
 from django.contrib.staticfiles.finders import FileSystemFinder
 from django.contrib.staticfiles.finders import get_finders
 from django.core.files.storage import FileSystemStorage
+from django.core.handlers.asgi import ASGIRequest
 from django.dispatch import receiver
 from django.http import Http404
 from django.http import HttpRequest
 from django.http import HttpResponse
 from django.http import StreamingHttpResponse
 from django.http.response import HttpResponseBase
 from django.template import engines
@@ -141,22 +146,45 @@
 def events(request: HttpRequest) -> HttpResponseBase:
     if not settings.DEBUG:
         raise Http404()
 
     if not request.accepts("text/event-stream"):
         return HttpResponse(status=HTTPStatus.NOT_ACCEPTABLE)
 
-    def event_stream() -> Generator[bytes, None, None]:
-        while True:
-            yield message("ping", versionId=version_id)
-
-            should_reload = should_reload_event.wait(timeout=PING_DELAY)
-            if should_reload:
-                should_reload_event.clear()
-                yield message("reload")
+    event_stream: Callable[[], AsyncGenerator[bytes, None]] | Callable[
+        [], Generator[bytes, None, None]
+    ]
+
+    if isinstance(request, ASGIRequest):
+        if django.VERSION < (4, 2):
+            return HttpResponse(
+                "ASGI requires Django 4.2+",
+                status=HTTPStatus.NOT_IMPLEMENTED,
+                content_type="text/plain",
+            )
+
+        async def event_stream() -> AsyncGenerator[bytes, None]:
+            while True:
+                await asyncio.sleep(PING_DELAY)
+                yield message("ping", versionId=version_id)
+
+                if should_reload_event.is_set():
+                    should_reload_event.clear()
+                    yield message("reload")
+
+    else:
+
+        def event_stream() -> Generator[bytes, None, None]:
+            while True:
+                yield message("ping", versionId=version_id)
+
+                should_reload = should_reload_event.wait(timeout=PING_DELAY)
+                if should_reload:
+                    should_reload_event.clear()
+                    yield message("reload")
 
     response = StreamingHttpResponse(
         event_stream(),
         content_type="text/event-stream",
     )
     # Set a content-encoding to bypass GzipMiddleware etc.
     response["content-encoding"] = ""
```

### Comparing `django_browser_reload-1.8.0/src/django_browser_reload.egg-info/PKG-INFO` & `django_browser_reload-1.9.0/src/django_browser_reload.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-browser-reload
-Version: 1.8.0
+Version: 1.9.0
 Summary: Automatically reload your browser in development.
 Home-page: https://github.com/adamchainz/django-browser-reload
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-browser-reload/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -57,20 +57,28 @@
 Requirements
 ------------
 
 Python 3.7 to 3.11 supported.
 
 Django 3.2 to 4.2 supported.
 
+WSGI supported on all Django versions. ASGI supported on Django 4.2+.
+
 Your browser needs to support:
 
-* ``EventSource`` - `universally available <https://developer.mozilla.org/en-US/docs/Web/API/EventSource#browser_compatibility>`__.
+* |EventSource|__ - universally available.
+
+  .. |EventSource| replace:: ``EventSource``
+  __ https://developer.mozilla.org/en-US/docs/Web/API/EventSource#browser_compatibility
+
+* |SharedWorker|__ - available on Chrome, Edge, Firefox, and Opera for a long time.
+  Available on Safari since version 16 (2022-09-12).
 
-* ``SharedWorker`` - `available <https://developer.mozilla.org/en-US/docs/Web/API/SharedWorker#browser_compatibility>`__ on Chrome, Edge, Firefox, and Opera.
-  Safari removed support but `are reinstating it <https://bugs.webkit.org/show_bug.cgi?id=149850>`__ - they recently `merged the feature <https://twitter.com/chris_dumez/status/1491650913441701896>`__ (2022-02-10).
+  .. |SharedWorker| replace:: ``SharedWorker``
+  __ https://developer.mozilla.org/en-US/docs/Web/API/SharedWorker#browser_compatibility
 
 ----
 
 **Want to work smarter and faster?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers django-browser-reload and many other tools.
 I wrote django-browser-reload whilst working on the book!
 
@@ -93,15 +101,15 @@
 
        INSTALLED_APPS = [
            ...,
            "django_browser_reload",
            ...,
        ]
 
-4. Include the app URL’s in your root URLconf(s):
+4. Include the app URLs in your root URLconf:
 
    .. code-block:: python
 
        from django.urls import include, path
 
        urlpatterns = [
            ...,
@@ -116,30 +124,29 @@
 
       MIDDLEWARE = [
           # ...
           "django_browser_reload.middleware.BrowserReloadMiddleware",
           # ...
       ]
 
-   The middleware should be listed after any that encode the response, such as Django’s ``GZipMiddleware``.
+   The middleware should be listed after any others that encode the response, such as Django’s ``GZipMiddleware``.
 
    The middleware automatically inserts the required script tag on HTML responses before ``</body>`` when ``DEBUG`` is ``True``.
    It does so to every HTML response, meaning it will be included on Django’s debug pages, admin pages, etc.
    If you want more control, you can instead insert the script tag in your templates—see below.
 
 All done! 📯
 
 For faster and more efficient reloading, also set up `Django’s built-in Watchman support <https://adamj.eu/tech/2021/01/20/efficient-reloading-in-djangos-runserver-with-watchman/>`__.
 
 What It Does
 ------------
 
 When ``DEBUG`` is ``True``, the template tag includes a small script.
 This script connects back to the development server and will automatically reload when static assets or templates are modified, or after ``runserver`` restarts.
-(Detecting modification of Django templates requires Django 3.2+.)
 The reload only happens in the most recently opened tab.
 
 Example Project
 ---------------
 
 See the `example project <https://github.com/adamchainz/django-browser-reload/tree/main/example>`__ in the ``example/`` directory of the GitHub repository.
 Start it up and modify its files to see the reloading in action.
@@ -172,15 +179,15 @@
     {% load django_browser_reload %}
 
     {% block extrahead %}
         {{ block.super }}
         {% django_browser_reload_script %}
     {% endblock %}
 
-This follows Django’s documentation on `extending an overriden template <https://docs.djangoproject.com/en/4.0/howto/overriding-templates/#extending-an-overridden-template>`__.
+This follows Django’s documentation on `extending an overridden template <https://docs.djangoproject.com/en/4.0/howto/overriding-templates/#extending-an-overridden-template>`__.
 
 For **Jinja Templates**, you need to perform two steps.
 First, load the tag function into the globals of your `custom environment <https://docs.djangoproject.com/en/stable/topics/templates/#django.template.backends.jinja2.Jinja2>`__:
 
 .. code-block:: python
 
     # myproject/jinja2.py
@@ -223,21 +230,21 @@
                                listener  listener  listener
                                     \       |       /
       Django                         \      |      /
                                       \     |     /
     Events View --------------------> Shared worker
 
 The template tag includes a listener script on each page.
-This listener script starts or connects to a |SharedWorker|__, running a worker script.
-The worker script then connects to the events view in Django, using an |EventSource|__ to receive server-sent events.
+This listener script starts or connects to a |SharedWorker2|__, running a worker script.
+The worker script then connects to the events view in Django, using an |EventSource2|__ to receive server-sent events.
 
-.. |SharedWorker| replace:: ``SharedWorker``
+.. |SharedWorker2| replace:: ``SharedWorker``
 __ https://developer.mozilla.org/en-US/docs/Web/API/SharedWorker
 
-.. |EventSource| replace:: ``EventSource``
+.. |EventSource2| replace:: ``EventSource``
 __ https://developer.mozilla.org/en-US/docs/Web/API/EventSource
 
 This event source uses |StreamingHttpResponse|__ to send events to the worker.
 The view continues streaming events indefinitely, until disconnected.
 (This requires a thread and will not work if you use ``runserver``\’s |--nothreading option|__.)
 
 .. |--nothreading option| replace:: ``--nothreading`` option
```

### Comparing `django_browser_reload-1.8.0/src/django_browser_reload.egg-info/SOURCES.txt` & `django_browser_reload-1.9.0/src/django_browser_reload.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_browser_reload-1.8.0/tests/test_jinja.py` & `django_browser_reload-1.9.0/tests/test_jinja.py`

 * *Files identical despite different names*

### Comparing `django_browser_reload-1.8.0/tests/test_middleware.py` & `django_browser_reload-1.9.0/tests/test_middleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         # responses
         content_iter = iter(["<html><body>", "</body></html>"])
         self.response = StreamingHttpResponse(content_iter)
 
         response = self.middleware(self.request)
 
         assert isinstance(response, StreamingHttpResponse)
-        content = b"".join(response.streaming_content)
+        content = b"".join(response)
         assert content == b"<html><body></body></html>"
 
     def test_encoded_response(self):
         self.response["Content-Encoding"] = "zabble"
 
         response = self.middleware(self.request)
```

