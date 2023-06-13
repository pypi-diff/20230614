# Comparing `tmp/squad-gunicorn-121.0.4.tar.gz` & `tmp/squad-gunicorn-20.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squad-gunicorn-121.0.4.tar", last modified: Tue Jun 13 23:48:56 2023, max compression
+gzip compressed data, was "squad-gunicorn-20.0.4.tar", last modified: Mon Jun 12 07:21:07 2023, max compression
```

## Comparing `squad-gunicorn-121.0.4.tar` & `squad-gunicorn-20.0.4.tar`

### file list

```diff
@@ -1,347 +1,347 @@
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.434396 squad-gunicorn-121.0.4/
--rwxr-xr-x   0 vineetgupta   (501) staff       (20)      267 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/.gitignore
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1136 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/LICENSE
--rw-r--r--   0 vineetgupta   (501) staff       (20)      324 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/MANIFEST.in
--rw-r--r--   0 vineetgupta   (501) staff       (20)     3777 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/NOTICE
--rw-r--r--   0 vineetgupta   (501) staff       (20)     3481 2023-06-13 23:48:56.434475 squad-gunicorn-121.0.4/PKG-INFO
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1762 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/README.rst
--rw-r--r--   0 vineetgupta   (501) staff       (20)     6638 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/THANKS
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.374043 squad-gunicorn-121.0.4/docs/
--rw-r--r--   0 vineetgupta   (501) staff       (20)     5791 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/Makefile
--rw-r--r--   0 vineetgupta   (501) staff       (20)      288 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/README.rst
--rwxr-xr-x   0 vineetgupta   (501) staff       (20)     2853 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/docs/gunicorn_ext.py
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.374514 squad-gunicorn-121.0.4/docs/logo/
--rw-r--r--   0 vineetgupta   (501) staff       (20)    21550 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/logo/gunicorn.png
--rw-r--r--   0 vineetgupta   (501) staff       (20)    12798 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/logo/gunicorn.svg
--rw-r--r--   0 vineetgupta   (501) staff       (20)     5109 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/make.bat
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.377346 squad-gunicorn-121.0.4/docs/site/
--rw-r--r--   0 vineetgupta   (501) staff       (20)        0 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/.nojekyll
--rw-r--r--   0 vineetgupta   (501) staff       (20)       13 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/CNAME
--rw-r--r--   0 vineetgupta   (501) staff       (20)      340 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/community.html
--rw-r--r--   0 vineetgupta   (501) staff       (20)      304 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/configuration.html
--rw-r--r--   0 vineetgupta   (501) staff       (20)      300 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/configure.html
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.377492 squad-gunicorn-121.0.4/docs/site/css/
--rw-r--r--   0 vineetgupta   (501) staff       (20)     6671 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/css/style.css
--rw-r--r--   0 vineetgupta   (501) staff       (20)      343 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/deploy.html
--rw-r--r--   0 vineetgupta   (501) staff       (20)      342 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/deployment.html
--rw-r--r--   0 vineetgupta   (501) staff       (20)      297 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/design.html
--rw-r--r--   0 vineetgupta   (501) staff       (20)      294 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/faq.html
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.380534 squad-gunicorn-121.0.4/docs/site/images/
--rw-r--r--   0 vineetgupta   (501) staff       (20)    17551 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/images/about.jpg
--rw-r--r--   0 vineetgupta   (501) staff       (20)      408 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/images/arrow.png
--rw-r--r--   0 vineetgupta   (501) staff       (20)      611 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/images/banner-bg.jpg
--rw-r--r--   0 vineetgupta   (501) staff       (20)    15593 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/images/community.jpg
--rw-r--r--   0 vineetgupta   (501) staff       (20)    17566 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/images/documents.jpg
--rw-r--r--   0 vineetgupta   (501) staff       (20)    15962 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/images/downloads.jpg
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1771 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/images/favicon.png
--rw-r--r--   0 vineetgupta   (501) staff       (20)      255 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/images/footer-arrow.png
--rw-r--r--   0 vineetgupta   (501) staff       (20)     2499 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/images/footer-logo.jpg
--rw-r--r--   0 vineetgupta   (501) staff       (20)      335 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/images/greenbutton.jpg
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1553 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/images/gunicorn.png
--rw-r--r--   0 vineetgupta   (501) staff       (20)    21956 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/images/large_gunicorn.png
--rw-r--r--   0 vineetgupta   (501) staff       (20)     3145 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/images/logo-bottom.png
--rw-r--r--   0 vineetgupta   (501) staff       (20)    10238 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/images/logo.jpg
--rw-r--r--   0 vineetgupta   (501) staff       (20)     7343 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/images/logo.png
--rw-r--r--   0 vineetgupta   (501) staff       (20)      577 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/images/redbutton.jpg
--rw-r--r--   0 vineetgupta   (501) staff       (20)      440 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/images/separator.jpg
--rw-r--r--   0 vineetgupta   (501) staff       (20)     3450 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/images/title.png
--rw-r--r--   0 vineetgupta   (501) staff       (20)     2184 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/images/user1.jpg
--rw-r--r--   0 vineetgupta   (501) staff       (20)     7854 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/docs/site/index.html
--rw-r--r--   0 vineetgupta   (501) staff       (20)      298 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/install.html
--rw-r--r--   0 vineetgupta   (501) staff       (20)      298 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/installation.html
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.380680 squad-gunicorn-121.0.4/docs/site/js/
--rwxr-xr-x   0 vineetgupta   (501) staff       (20)     1479 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/js/main.js
--rw-r--r--   0 vineetgupta   (501) staff       (20)      295 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/news.html
--rw-r--r--   0 vineetgupta   (501) staff       (20)      294 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/run.html
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1990 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/sitemap.xml
--rw-r--r--   0 vineetgupta   (501) staff       (20)      294 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/tuning.html
--rw-r--r--   0 vineetgupta   (501) staff       (20)      294 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/site/usage.html
--rw-r--r--   0 vineetgupta   (501) staff       (20)     2088 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/sitemap_gen.py
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.384539 squad-gunicorn-121.0.4/docs/source/
--rw-r--r--   0 vineetgupta   (501) staff       (20)     6643 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/source/2010-news.rst
--rw-r--r--   0 vineetgupta   (501) staff       (20)     2092 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/source/2011-news.rst
--rw-r--r--   0 vineetgupta   (501) staff       (20)     4183 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/docs/source/2012-news.rst
--rw-r--r--   0 vineetgupta   (501) staff       (20)     3270 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/docs/source/2013-news.rst
--rw-r--r--   0 vineetgupta   (501) staff       (20)     6834 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/docs/source/2014-news.rst
--rw-r--r--   0 vineetgupta   (501) staff       (20)     5702 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/source/2015-news.rst
--rw-r--r--   0 vineetgupta   (501) staff       (20)     2911 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/source/2016-news.rst
--rw-r--r--   0 vineetgupta   (501) staff       (20)     2100 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/source/2017-news.rst
--rw-r--r--   0 vineetgupta   (501) staff       (20)     2956 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/source/2018-news.rst
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.384690 squad-gunicorn-121.0.4/docs/source/_static/
--rw-r--r--   0 vineetgupta   (501) staff       (20)    14398 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/source/_static/gunicorn.png
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1375 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/docs/source/community.rst
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1755 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/source/conf.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     3849 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/docs/source/configure.rst
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1933 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/docs/source/custom.rst
--rw-r--r--   0 vineetgupta   (501) staff       (20)    11588 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/docs/source/deploy.rst
--rw-r--r--   0 vineetgupta   (501) staff       (20)     6453 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/docs/source/design.rst
--rw-r--r--   0 vineetgupta   (501) staff       (20)     8402 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/docs/source/faq.rst
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1040 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/docs/source/index.rst
--rw-r--r--   0 vineetgupta   (501) staff       (20)     5204 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/docs/source/install.rst
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1325 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/source/instrumentation.rst
--rw-r--r--   0 vineetgupta   (501) staff       (20)     4870 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/docs/source/news.rst
--rw-r--r--   0 vineetgupta   (501) staff       (20)     6485 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/source/run.rst
--rw-r--r--   0 vineetgupta   (501) staff       (20)    29162 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/docs/source/settings.rst
--rw-r--r--   0 vineetgupta   (501) staff       (20)     5420 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/docs/source/signals.rst
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.389343 squad-gunicorn-121.0.4/examples/
--rw-r--r--   0 vineetgupta   (501) staff       (20)      738 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/alt_spec.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      204 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/bad.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      108 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/boot_fail.py
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.389615 squad-gunicorn-121.0.4/examples/deep/
--rw-r--r--   0 vineetgupta   (501) staff       (20)        0 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/deep/__init__.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      659 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/deep/test.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      676 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/echo.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     6691 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/examples/example_config.py
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.391600 squad-gunicorn-121.0.4/examples/frameworks/
--rw-r--r--   0 vineetgupta   (501) staff       (20)      198 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/cherryapp.py
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.391757 squad-gunicorn-121.0.4/examples/frameworks/django/
--rw-r--r--   0 vineetgupta   (501) staff       (20)       60 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/django/README
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.391919 squad-gunicorn-121.0.4/examples/frameworks/django/testing/
--rwxr-xr-x   0 vineetgupta   (501) staff       (20)      244 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/django/testing/manage.py
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.392521 squad-gunicorn-121.0.4/examples/frameworks/django/testing/testing/
--rw-r--r--   0 vineetgupta   (501) staff       (20)        0 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/django/testing/testing/__init__.py
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.392691 squad-gunicorn-121.0.4/examples/frameworks/django/testing/testing/apps/
--rw-r--r--   0 vineetgupta   (501) staff       (20)        0 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/django/testing/testing/apps/__init__.py
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.393881 squad-gunicorn-121.0.4/examples/frameworks/django/testing/testing/apps/someapp/
--rwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/django/testing/testing/apps/someapp/__init__.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      627 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/django/testing/testing/apps/someapp/middleware.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)        0 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/django/testing/testing/apps/someapp/models.py
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.394471 squad-gunicorn-121.0.4/examples/frameworks/django/testing/testing/apps/someapp/templates/
--rw-r--r--   0 vineetgupta   (501) staff       (20)      759 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/django/testing/testing/apps/someapp/templates/base.html
--rw-r--r--   0 vineetgupta   (501) staff       (20)      471 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/django/testing/testing/apps/someapp/templates/home.html
--rwxr-xr-x   0 vineetgupta   (501) staff       (20)      513 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/examples/frameworks/django/testing/testing/apps/someapp/tests.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      133 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/django/testing/testing/apps/someapp/urls.py
--rwxr-xr-x   0 vineetgupta   (501) staff       (20)     1548 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/django/testing/testing/apps/someapp/views.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     5730 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/django/testing/testing/settings.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      577 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/django/testing/testing/urls.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1359 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/django/testing/testing/wsgi.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      291 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/flask_sendfile.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      147 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/flaskapp.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      501 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/flaskapp_aiohttp_wsgi.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      338 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/pyramidapp.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      150 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/requirements.txt
--rw-r--r--   0 vineetgupta   (501) staff       (20)        9 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/requirements_cherryapp.txt
--rw-r--r--   0 vineetgupta   (501) staff       (20)        6 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/requirements_flaskapp.txt
--rw-r--r--   0 vineetgupta   (501) staff       (20)        8 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/requirements_pyramidapp.txt
--rw-r--r--   0 vineetgupta   (501) staff       (20)       10 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/requirements_tornadoapp.txt
--rw-r--r--   0 vineetgupta   (501) staff       (20)        7 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/requirements_webpyapp.txt
--rw-r--r--   0 vineetgupta   (501) staff       (20)      873 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/tornadoapp.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      197 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/frameworks/webpyapp.py
--rwxr-xr-x   0 vineetgupta   (501) staff       (20)      215 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/gunicorn_rc
--rw-r--r--   0 vineetgupta   (501) staff       (20)       13 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/hello.txt
--rw-r--r--   0 vineetgupta   (501) staff       (20)      448 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/log_app.ini
--rw-r--r--   0 vineetgupta   (501) staff       (20)      372 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/log_app.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      841 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/logging.conf
--rw-r--r--   0 vineetgupta   (501) staff       (20)      737 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/longpoll.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1470 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/multiapp.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      993 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/multidomainapp.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1980 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/nginx.conf
--rw-r--r--   0 vineetgupta   (501) staff       (20)      403 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/read_django_settings.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1015 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/readline_app.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      584 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/sendfile.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1257 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/server.crt
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1679 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/server.key
--rw-r--r--   0 vineetgupta   (501) staff       (20)      604 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/slowclient.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1339 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/standalone_app.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      182 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/supervisor.conf
--rw-r--r--   0 vineetgupta   (501) staff       (20)      659 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/test.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      620 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/timeout.py
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.394959 squad-gunicorn-121.0.4/examples/websocket/
--rw-r--r--   0 vineetgupta   (501) staff       (20)    15684 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/websocket/gevent_websocket.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1320 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/websocket/websocket.html
--rw-r--r--   0 vineetgupta   (501) staff       (20)    15729 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/websocket/websocket.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1020 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/examples/when_ready.conf.py
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.398389 squad-gunicorn-121.0.4/gunicorn/
--rw-r--r--   0 vineetgupta   (501) staff       (20)      279 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/gunicorn/__init__.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      171 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/gunicorn/__main__.py
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.399269 squad-gunicorn-121.0.4/gunicorn/app/
--rw-r--r--   0 vineetgupta   (501) staff       (20)      127 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/gunicorn/app/__init__.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     7150 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/gunicorn/app/base.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     2038 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/gunicorn/app/pasterapp.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1926 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/gunicorn/app/wsgiapp.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)    20869 2023-06-13 23:21:02.000000 squad-gunicorn-121.0.4/gunicorn/arbiter.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)    58155 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/gunicorn/config.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     2289 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/gunicorn/debug.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      919 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/gunicorn/errors.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)    14913 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/gunicorn/glogging.py
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.400454 squad-gunicorn-121.0.4/gunicorn/http/
--rw-r--r--   0 vineetgupta   (501) staff       (20)      277 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/gunicorn/http/__init__.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     7297 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/gunicorn/http/body.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     2850 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/gunicorn/http/errors.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)    12481 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/gunicorn/http/message.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1294 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/gunicorn/http/parser.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1943 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/gunicorn/http/unreader.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)    12328 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/gunicorn/http/wsgi.py
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.400687 squad-gunicorn-121.0.4/gunicorn/instrument/
--rw-r--r--   0 vineetgupta   (501) staff       (20)        0 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/gunicorn/instrument/__init__.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     4633 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/gunicorn/instrument/statsd.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     2367 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/gunicorn/pidfile.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     3777 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/gunicorn/reloader.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     6110 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/gunicorn/sock.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     2511 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/gunicorn/systemd.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)    18516 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/gunicorn/util.py
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.402311 squad-gunicorn-121.0.4/gunicorn/workers/
--rw-r--r--   0 vineetgupta   (501) staff       (20)      594 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/gunicorn/workers/__init__.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     9199 2023-06-13 08:54:51.000000 squad-gunicorn-121.0.4/gunicorn/workers/base.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     5555 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/gunicorn/workers/base_async.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     5713 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/gunicorn/workers/geventlet.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     5733 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/gunicorn/workers/ggevent.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)    12049 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/gunicorn/workers/gthread.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     5902 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/gunicorn/workers/gtornado.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     7264 2023-06-13 08:54:51.000000 squad-gunicorn-121.0.4/gunicorn/workers/sync.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1649 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/gunicorn/workers/workertmp.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       50 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/requirements_dev.txt
--rw-r--r--   0 vineetgupta   (501) staff       (20)       58 2023-06-13 08:54:51.000000 squad-gunicorn-121.0.4/requirements_test.txt
--rw-r--r--   0 vineetgupta   (501) staff       (20)      203 2023-06-13 23:48:56.434710 squad-gunicorn-121.0.4/setup.cfg
--rw-r--r--   0 vineetgupta   (501) staff       (20)     3622 2023-06-13 23:35:15.000000 squad-gunicorn-121.0.4/setup.py
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.403293 squad-gunicorn-121.0.4/squad_gunicorn.egg-info/
--rw-r--r--   0 vineetgupta   (501) staff       (20)     3481 2023-06-13 23:48:56.000000 squad-gunicorn-121.0.4/squad_gunicorn.egg-info/PKG-INFO
--rw-r--r--   0 vineetgupta   (501) staff       (20)     9001 2023-06-13 23:48:56.000000 squad-gunicorn-121.0.4/squad_gunicorn.egg-info/SOURCES.txt
--rw-r--r--   0 vineetgupta   (501) staff       (20)        1 2023-06-13 23:48:56.000000 squad-gunicorn-121.0.4/squad_gunicorn.egg-info/dependency_links.txt
--rw-r--r--   0 vineetgupta   (501) staff       (20)      113 2023-06-13 23:48:56.000000 squad-gunicorn-121.0.4/squad_gunicorn.egg-info/entry_points.txt
--rw-r--r--   0 vineetgupta   (501) staff       (20)        1 2023-06-11 19:44:32.000000 squad-gunicorn-121.0.4/squad_gunicorn.egg-info/not-zip-safe
--rw-r--r--   0 vineetgupta   (501) staff       (20)      140 2023-06-13 23:48:56.000000 squad-gunicorn-121.0.4/squad_gunicorn.egg-info/requires.txt
--rw-r--r--   0 vineetgupta   (501) staff       (20)        9 2023-06-13 23:48:56.000000 squad-gunicorn-121.0.4/squad_gunicorn.egg-info/top_level.txt
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.407046 squad-gunicorn-121.0.4/tests/
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.407592 squad-gunicorn-121.0.4/tests/config/
--rw-r--r--   0 vineetgupta   (501) staff       (20)        0 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/config/__init__.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       88 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/config/test_cfg.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       24 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/config/test_cfg_alt.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       23 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/config/test_cfg_with_wsgi_app.py
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.371116 squad-gunicorn-121.0.4/tests/requests/
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.415577 squad-gunicorn-121.0.4/tests/requests/invalid/
--rw-r--r--   0 vineetgupta   (501) staff       (20)       29 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/001.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)       64 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/001.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       21 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/002.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)       81 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/002.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       30 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/003.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)       84 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/003.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       25 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/004.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)       80 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/004.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       41 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/005.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)       78 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/005.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     4122 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/006.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)       77 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/006.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     8358 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/007.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)       83 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/007.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)    12418 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/008.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)       83 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/008.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1829 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/009.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)       83 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/009.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       44 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/010.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      174 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/010.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      169 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/011.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      169 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/011.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      169 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/012.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      174 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/012.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       49 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/013.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      174 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/013.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       78 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/014.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)       72 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/014.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       88 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/015.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)       72 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/015.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       33 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/016.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)       82 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/016.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     8222 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/017.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      134 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/017.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       48 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/018.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)       81 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/018.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       82 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/019.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      172 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/019.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       69 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/020.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      130 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/020.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       90 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/021.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      122 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/021.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       37 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/pp_01.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      161 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/pp_01.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       53 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/pp_02.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      161 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/invalid/pp_02.py
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.433915 squad-gunicorn-121.0.4/tests/requests/valid/
--rw-r--r--   0 vineetgupta   (501) staff       (20)      149 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/001.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      275 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/001.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      168 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/002.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      296 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/002.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      394 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/003.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      577 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/003.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       57 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/004.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      164 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/004.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       62 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/005.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      153 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/005.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       51 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/006.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      142 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/006.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       61 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/007.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      167 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/007.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       73 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/008.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      178 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/008.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      137 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/009.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      264 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/009.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      134 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/010.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      218 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/010.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      125 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/011.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      196 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/011.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      166 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/012.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      285 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/012.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      159 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/013.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      192 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/013.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       46 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/014.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      137 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/014.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       98 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/015.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      226 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/015.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     2234 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/016.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)     2376 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/016.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       91 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/017.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      207 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/017.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       58 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/018.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      258 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/018.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       58 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/019.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      119 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/019.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       81 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/020.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      171 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/020.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       80 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/021.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      142 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/021.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       85 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/022.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      286 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/022.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      155 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/023.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      335 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/023.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)    16408 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/024.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)    16639 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/024.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      364 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/025.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      476 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/025.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     8233 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/026.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)     8463 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/026.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       30 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/027.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      130 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/027.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       68 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/028.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      261 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/028.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      129 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/029.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      278 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/029.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      129 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/030.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      278 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/030.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     9909 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/099.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)     9135 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/099.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)       41 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/100.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      131 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/100.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      199 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/pp_01.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      359 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/pp_01.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      361 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/pp_02.http
--rw-r--r--   0 vineetgupta   (501) staff       (20)      639 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/requests/valid/pp_02.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1745 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/support.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1608 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/tests/t.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     6113 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/tests/test_arbiter.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)    14482 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/tests/test_config.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     6856 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/tests/test_http.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      597 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/test_invalid_requests.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     3140 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/test_logger.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1525 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/tests/test_pidfile.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1851 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/test_reload.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     1878 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/tests/test_sock.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     2277 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/tests/test_ssl.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     4449 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/tests/test_statsd.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     2052 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/tests/test_systemd.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     4367 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/test_util.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      608 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/test_valid_requests.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)     9422 2023-06-12 05:53:24.000000 squad-gunicorn-121.0.4/tests/treq.py
-drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-13 23:48:56.434267 squad-gunicorn-121.0.4/tests/workers/
--rw-r--r--   0 vineetgupta   (501) staff       (20)        0 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/workers/__init__.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      192 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/workers/test_geventlet.py
--rw-r--r--   0 vineetgupta   (501) staff       (20)      190 2023-06-07 09:12:42.000000 squad-gunicorn-121.0.4/tests/workers/test_ggevent.py
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.387071 squad-gunicorn-20.0.4/
+-rwxr-xr-x   0 vineetgupta   (501) staff       (20)      267 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/.gitignore
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1136 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/LICENSE
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      324 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/MANIFEST.in
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     3777 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/NOTICE
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     3480 2023-06-12 07:21:07.387182 squad-gunicorn-20.0.4/PKG-INFO
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1762 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/README.rst
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     6638 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/THANKS
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.330821 squad-gunicorn-20.0.4/docs/
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     5791 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/Makefile
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      288 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/README.rst
+-rwxr-xr-x   0 vineetgupta   (501) staff       (20)     2853 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/docs/gunicorn_ext.py
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.331289 squad-gunicorn-20.0.4/docs/logo/
+-rw-r--r--   0 vineetgupta   (501) staff       (20)    21550 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/logo/gunicorn.png
+-rw-r--r--   0 vineetgupta   (501) staff       (20)    12798 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/logo/gunicorn.svg
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     5109 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/make.bat
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.334016 squad-gunicorn-20.0.4/docs/site/
+-rw-r--r--   0 vineetgupta   (501) staff       (20)        0 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/.nojekyll
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       13 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/CNAME
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      340 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/community.html
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      304 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/configuration.html
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      300 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/configure.html
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.334148 squad-gunicorn-20.0.4/docs/site/css/
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     6671 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/css/style.css
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      343 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/deploy.html
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      342 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/deployment.html
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      297 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/design.html
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      294 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/faq.html
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.337209 squad-gunicorn-20.0.4/docs/site/images/
+-rw-r--r--   0 vineetgupta   (501) staff       (20)    17551 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/images/about.jpg
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      408 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/images/arrow.png
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      611 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/images/banner-bg.jpg
+-rw-r--r--   0 vineetgupta   (501) staff       (20)    15593 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/images/community.jpg
+-rw-r--r--   0 vineetgupta   (501) staff       (20)    17566 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/images/documents.jpg
+-rw-r--r--   0 vineetgupta   (501) staff       (20)    15962 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/images/downloads.jpg
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1771 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/images/favicon.png
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      255 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/images/footer-arrow.png
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     2499 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/images/footer-logo.jpg
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      335 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/images/greenbutton.jpg
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1553 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/images/gunicorn.png
+-rw-r--r--   0 vineetgupta   (501) staff       (20)    21956 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/images/large_gunicorn.png
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     3145 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/images/logo-bottom.png
+-rw-r--r--   0 vineetgupta   (501) staff       (20)    10238 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/images/logo.jpg
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     7343 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/images/logo.png
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      577 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/images/redbutton.jpg
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      440 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/images/separator.jpg
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     3450 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/images/title.png
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     2184 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/images/user1.jpg
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     7854 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/docs/site/index.html
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      298 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/install.html
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      298 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/installation.html
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.337372 squad-gunicorn-20.0.4/docs/site/js/
+-rwxr-xr-x   0 vineetgupta   (501) staff       (20)     1479 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/js/main.js
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      295 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/news.html
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      294 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/run.html
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1990 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/sitemap.xml
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      294 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/tuning.html
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      294 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/site/usage.html
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     2088 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/sitemap_gen.py
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.343155 squad-gunicorn-20.0.4/docs/source/
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     6643 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/source/2010-news.rst
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     2092 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/source/2011-news.rst
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     4183 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/docs/source/2012-news.rst
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     3270 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/docs/source/2013-news.rst
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     6834 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/docs/source/2014-news.rst
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     5702 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/source/2015-news.rst
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     2911 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/source/2016-news.rst
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     2100 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/source/2017-news.rst
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     2956 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/source/2018-news.rst
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.343295 squad-gunicorn-20.0.4/docs/source/_static/
+-rw-r--r--   0 vineetgupta   (501) staff       (20)    14398 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/source/_static/gunicorn.png
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1375 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/docs/source/community.rst
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1755 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/source/conf.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     3849 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/docs/source/configure.rst
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1933 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/docs/source/custom.rst
+-rw-r--r--   0 vineetgupta   (501) staff       (20)    11588 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/docs/source/deploy.rst
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     6453 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/docs/source/design.rst
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     8402 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/docs/source/faq.rst
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1040 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/docs/source/index.rst
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     5204 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/docs/source/install.rst
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1325 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/source/instrumentation.rst
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     4870 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/docs/source/news.rst
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     6485 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/source/run.rst
+-rw-r--r--   0 vineetgupta   (501) staff       (20)    29162 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/docs/source/settings.rst
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     5420 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/docs/source/signals.rst
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.348098 squad-gunicorn-20.0.4/examples/
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      738 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/alt_spec.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      204 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/bad.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      108 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/boot_fail.py
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.348325 squad-gunicorn-20.0.4/examples/deep/
+-rw-r--r--   0 vineetgupta   (501) staff       (20)        0 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/deep/__init__.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      659 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/deep/test.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      676 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/echo.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     6691 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/examples/example_config.py
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.350458 squad-gunicorn-20.0.4/examples/frameworks/
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      198 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/cherryapp.py
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.350863 squad-gunicorn-20.0.4/examples/frameworks/django/
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       60 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/django/README
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.351019 squad-gunicorn-20.0.4/examples/frameworks/django/testing/
+-rwxr-xr-x   0 vineetgupta   (501) staff       (20)      244 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/django/testing/manage.py
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.351593 squad-gunicorn-20.0.4/examples/frameworks/django/testing/testing/
+-rw-r--r--   0 vineetgupta   (501) staff       (20)        0 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/django/testing/testing/__init__.py
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.351748 squad-gunicorn-20.0.4/examples/frameworks/django/testing/testing/apps/
+-rw-r--r--   0 vineetgupta   (501) staff       (20)        0 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/django/testing/testing/apps/__init__.py
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.352572 squad-gunicorn-20.0.4/examples/frameworks/django/testing/testing/apps/someapp/
+-rwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/django/testing/testing/apps/someapp/__init__.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      627 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/django/testing/testing/apps/someapp/middleware.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)        0 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/django/testing/testing/apps/someapp/models.py
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.352854 squad-gunicorn-20.0.4/examples/frameworks/django/testing/testing/apps/someapp/templates/
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      759 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/django/testing/testing/apps/someapp/templates/base.html
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      471 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/django/testing/testing/apps/someapp/templates/home.html
+-rwxr-xr-x   0 vineetgupta   (501) staff       (20)      513 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/examples/frameworks/django/testing/testing/apps/someapp/tests.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      133 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/django/testing/testing/apps/someapp/urls.py
+-rwxr-xr-x   0 vineetgupta   (501) staff       (20)     1548 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/django/testing/testing/apps/someapp/views.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     5730 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/django/testing/testing/settings.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      577 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/django/testing/testing/urls.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1359 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/django/testing/testing/wsgi.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      291 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/flask_sendfile.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      147 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/flaskapp.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      501 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/flaskapp_aiohttp_wsgi.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      338 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/pyramidapp.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      150 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/requirements.txt
+-rw-r--r--   0 vineetgupta   (501) staff       (20)        9 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/requirements_cherryapp.txt
+-rw-r--r--   0 vineetgupta   (501) staff       (20)        6 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/requirements_flaskapp.txt
+-rw-r--r--   0 vineetgupta   (501) staff       (20)        8 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/requirements_pyramidapp.txt
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       10 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/requirements_tornadoapp.txt
+-rw-r--r--   0 vineetgupta   (501) staff       (20)        7 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/requirements_webpyapp.txt
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      873 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/tornadoapp.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      197 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/frameworks/webpyapp.py
+-rwxr-xr-x   0 vineetgupta   (501) staff       (20)      215 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/gunicorn_rc
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       13 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/hello.txt
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      448 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/log_app.ini
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      372 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/log_app.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      841 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/logging.conf
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      737 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/longpoll.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1470 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/multiapp.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      993 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/multidomainapp.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1980 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/nginx.conf
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      403 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/read_django_settings.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1015 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/readline_app.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      584 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/sendfile.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1257 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/server.crt
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1679 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/server.key
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      604 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/slowclient.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1339 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/standalone_app.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      182 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/supervisor.conf
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      659 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/test.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      620 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/timeout.py
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.353289 squad-gunicorn-20.0.4/examples/websocket/
+-rw-r--r--   0 vineetgupta   (501) staff       (20)    15684 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/websocket/gevent_websocket.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1320 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/websocket/websocket.html
+-rw-r--r--   0 vineetgupta   (501) staff       (20)    15729 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/websocket/websocket.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1020 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/examples/when_ready.conf.py
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.356043 squad-gunicorn-20.0.4/gunicorn/
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      279 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/gunicorn/__init__.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      171 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/gunicorn/__main__.py
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.356682 squad-gunicorn-20.0.4/gunicorn/app/
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      127 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/gunicorn/app/__init__.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     7150 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/gunicorn/app/base.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     2038 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/gunicorn/app/pasterapp.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1926 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/gunicorn/app/wsgiapp.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)    21018 2023-06-12 06:14:00.000000 squad-gunicorn-20.0.4/gunicorn/arbiter.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)    58155 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/gunicorn/config.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     2289 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/gunicorn/debug.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      919 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/gunicorn/errors.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)    14913 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/gunicorn/glogging.py
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.357658 squad-gunicorn-20.0.4/gunicorn/http/
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      277 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/gunicorn/http/__init__.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     7297 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/gunicorn/http/body.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     2850 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/gunicorn/http/errors.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)    12481 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/gunicorn/http/message.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1294 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/gunicorn/http/parser.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1943 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/gunicorn/http/unreader.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)    12328 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/gunicorn/http/wsgi.py
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.357895 squad-gunicorn-20.0.4/gunicorn/instrument/
+-rw-r--r--   0 vineetgupta   (501) staff       (20)        0 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/gunicorn/instrument/__init__.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     4633 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/gunicorn/instrument/statsd.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     2367 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/gunicorn/pidfile.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     3777 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/gunicorn/reloader.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     6110 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/gunicorn/sock.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     2511 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/gunicorn/systemd.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)    18516 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/gunicorn/util.py
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.359112 squad-gunicorn-20.0.4/gunicorn/workers/
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      594 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/gunicorn/workers/__init__.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     9199 2023-06-12 06:14:00.000000 squad-gunicorn-20.0.4/gunicorn/workers/base.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     5555 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/gunicorn/workers/base_async.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     5713 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/gunicorn/workers/geventlet.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     5733 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/gunicorn/workers/ggevent.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)    12049 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/gunicorn/workers/gthread.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     5902 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/gunicorn/workers/gtornado.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     7264 2023-06-12 06:14:00.000000 squad-gunicorn-20.0.4/gunicorn/workers/sync.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1649 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/gunicorn/workers/workertmp.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       50 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/requirements_dev.txt
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       58 2023-06-12 06:56:44.000000 squad-gunicorn-20.0.4/requirements_test.txt
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      203 2023-06-12 07:21:07.387961 squad-gunicorn-20.0.4/setup.cfg
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     3625 2023-06-12 07:20:57.000000 squad-gunicorn-20.0.4/setup.py
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.360039 squad-gunicorn-20.0.4/squad_gunicorn.egg-info/
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     3480 2023-06-12 07:21:07.000000 squad-gunicorn-20.0.4/squad_gunicorn.egg-info/PKG-INFO
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     9001 2023-06-12 07:21:07.000000 squad-gunicorn-20.0.4/squad_gunicorn.egg-info/SOURCES.txt
+-rw-r--r--   0 vineetgupta   (501) staff       (20)        1 2023-06-12 07:21:07.000000 squad-gunicorn-20.0.4/squad_gunicorn.egg-info/dependency_links.txt
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      113 2023-06-12 07:21:07.000000 squad-gunicorn-20.0.4/squad_gunicorn.egg-info/entry_points.txt
+-rw-r--r--   0 vineetgupta   (501) staff       (20)        1 2023-06-11 19:44:32.000000 squad-gunicorn-20.0.4/squad_gunicorn.egg-info/not-zip-safe
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      140 2023-06-12 07:21:07.000000 squad-gunicorn-20.0.4/squad_gunicorn.egg-info/requires.txt
+-rw-r--r--   0 vineetgupta   (501) staff       (20)        9 2023-06-12 07:21:07.000000 squad-gunicorn-20.0.4/squad_gunicorn.egg-info/top_level.txt
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.363059 squad-gunicorn-20.0.4/tests/
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.364008 squad-gunicorn-20.0.4/tests/config/
+-rw-r--r--   0 vineetgupta   (501) staff       (20)        0 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/config/__init__.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       88 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/config/test_cfg.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       24 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/config/test_cfg_alt.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       23 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/config/test_cfg_with_wsgi_app.py
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.327553 squad-gunicorn-20.0.4/tests/requests/
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.375686 squad-gunicorn-20.0.4/tests/requests/invalid/
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       29 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/001.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       64 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/001.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       21 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/002.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       81 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/002.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       30 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/003.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       84 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/003.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       25 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/004.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       80 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/004.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       41 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/005.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       78 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/005.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     4122 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/006.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       77 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/006.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     8358 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/007.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       83 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/007.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)    12418 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/008.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       83 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/008.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1829 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/009.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       83 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/009.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       44 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/010.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      174 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/010.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      169 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/011.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      169 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/011.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      169 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/012.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      174 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/012.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       49 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/013.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      174 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/013.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       78 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/014.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       72 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/014.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       88 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/015.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       72 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/015.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       33 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/016.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       82 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/016.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     8222 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/017.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      134 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/017.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       48 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/018.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       81 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/018.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       82 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/019.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      172 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/019.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       69 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/020.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      130 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/020.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       90 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/021.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      122 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/021.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       37 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/pp_01.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      161 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/pp_01.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       53 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/pp_02.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      161 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/invalid/pp_02.py
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.386542 squad-gunicorn-20.0.4/tests/requests/valid/
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      149 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/001.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      275 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/001.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      168 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/002.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      296 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/002.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      394 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/003.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      577 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/003.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       57 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/004.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      164 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/004.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       62 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/005.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      153 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/005.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       51 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/006.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      142 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/006.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       61 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/007.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      167 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/007.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       73 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/008.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      178 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/008.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      137 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/009.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      264 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/009.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      134 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/010.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      218 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/010.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      125 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/011.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      196 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/011.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      166 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/012.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      285 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/012.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      159 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/013.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      192 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/013.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       46 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/014.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      137 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/014.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       98 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/015.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      226 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/015.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     2234 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/016.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     2376 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/016.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       91 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/017.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      207 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/017.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       58 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/018.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      258 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/018.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       58 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/019.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      119 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/019.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       81 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/020.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      171 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/020.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       80 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/021.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      142 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/021.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       85 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/022.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      286 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/022.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      155 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/023.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      335 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/023.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)    16408 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/024.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)    16639 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/024.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      364 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/025.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      476 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/025.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     8233 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/026.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     8463 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/026.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       30 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/027.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      130 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/027.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       68 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/028.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      261 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/028.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      129 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/029.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      278 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/029.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      129 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/030.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      278 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/030.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     9909 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/099.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     9135 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/099.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)       41 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/100.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      131 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/100.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      199 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/pp_01.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      359 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/pp_01.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      361 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/pp_02.http
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      639 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/requests/valid/pp_02.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1745 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/support.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1608 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/tests/t.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     6113 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/tests/test_arbiter.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)    14482 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/tests/test_config.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     6856 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/tests/test_http.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      597 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/test_invalid_requests.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     3140 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/test_logger.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1525 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/tests/test_pidfile.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1851 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/test_reload.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     1878 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/tests/test_sock.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     2277 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/tests/test_ssl.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     4449 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/tests/test_statsd.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     2052 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/tests/test_systemd.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     4367 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/test_util.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      608 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/test_valid_requests.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)     9422 2023-06-12 05:53:24.000000 squad-gunicorn-20.0.4/tests/treq.py
+drwxr-xr-x   0 vineetgupta   (501) staff       (20)        0 2023-06-12 07:21:07.386928 squad-gunicorn-20.0.4/tests/workers/
+-rw-r--r--   0 vineetgupta   (501) staff       (20)        0 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/workers/__init__.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      192 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/workers/test_geventlet.py
+-rw-r--r--   0 vineetgupta   (501) staff       (20)      190 2023-06-07 09:12:42.000000 squad-gunicorn-20.0.4/tests/workers/test_ggevent.py
```

### Comparing `squad-gunicorn-121.0.4/LICENSE` & `squad-gunicorn-20.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/NOTICE` & `squad-gunicorn-20.0.4/NOTICE`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/PKG-INFO` & `squad-gunicorn-20.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squad-gunicorn
-Version: 121.0.4
+Version: 20.0.4
 Summary: WSGI HTTP Server for UNIX
 Home-page: https://gunicorn.org
 Author: Benoit Chesneau
 Author-email: benoitc@e-engura.com
 License: MIT
 Project-URL: Documentation, https://docs.gunicorn.org
 Project-URL: Homepage, https://gunicorn.org
```

### Comparing `squad-gunicorn-121.0.4/README.rst` & `squad-gunicorn-20.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/THANKS` & `squad-gunicorn-20.0.4/THANKS`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/Makefile` & `squad-gunicorn-20.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/gunicorn_ext.py` & `squad-gunicorn-20.0.4/docs/gunicorn_ext.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/logo/gunicorn.png` & `squad-gunicorn-20.0.4/docs/logo/gunicorn.png`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/logo/gunicorn.svg` & `squad-gunicorn-20.0.4/docs/logo/gunicorn.svg`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/make.bat` & `squad-gunicorn-20.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/site/css/style.css` & `squad-gunicorn-20.0.4/docs/site/css/style.css`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/site/images/about.jpg` & `squad-gunicorn-20.0.4/docs/site/images/about.jpg`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/site/images/banner-bg.jpg` & `squad-gunicorn-20.0.4/docs/site/images/banner-bg.jpg`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/site/images/community.jpg` & `squad-gunicorn-20.0.4/docs/site/images/community.jpg`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/site/images/documents.jpg` & `squad-gunicorn-20.0.4/docs/site/images/documents.jpg`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/site/images/downloads.jpg` & `squad-gunicorn-20.0.4/docs/site/images/downloads.jpg`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/site/images/favicon.png` & `squad-gunicorn-20.0.4/docs/site/images/favicon.png`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/site/images/footer-logo.jpg` & `squad-gunicorn-20.0.4/docs/site/images/footer-logo.jpg`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/site/images/gunicorn.png` & `squad-gunicorn-20.0.4/docs/site/images/gunicorn.png`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/site/images/large_gunicorn.png` & `squad-gunicorn-20.0.4/docs/site/images/large_gunicorn.png`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/site/images/logo-bottom.png` & `squad-gunicorn-20.0.4/docs/site/images/logo-bottom.png`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/site/images/logo.jpg` & `squad-gunicorn-20.0.4/docs/site/images/logo.jpg`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/site/images/logo.png` & `squad-gunicorn-20.0.4/docs/site/images/logo.png`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/site/images/redbutton.jpg` & `squad-gunicorn-20.0.4/docs/site/images/redbutton.jpg`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/site/images/title.png` & `squad-gunicorn-20.0.4/docs/site/images/title.png`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/site/images/user1.jpg` & `squad-gunicorn-20.0.4/docs/site/images/user1.jpg`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/site/index.html` & `squad-gunicorn-20.0.4/docs/site/index.html`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/site/js/main.js` & `squad-gunicorn-20.0.4/docs/site/js/main.js`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/site/sitemap.xml` & `squad-gunicorn-20.0.4/docs/site/sitemap.xml`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/sitemap_gen.py` & `squad-gunicorn-20.0.4/docs/sitemap_gen.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/source/2010-news.rst` & `squad-gunicorn-20.0.4/docs/source/2010-news.rst`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/source/2011-news.rst` & `squad-gunicorn-20.0.4/docs/source/2011-news.rst`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/source/2012-news.rst` & `squad-gunicorn-20.0.4/docs/source/2012-news.rst`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/source/2013-news.rst` & `squad-gunicorn-20.0.4/docs/source/2013-news.rst`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/source/2014-news.rst` & `squad-gunicorn-20.0.4/docs/source/2014-news.rst`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/source/2015-news.rst` & `squad-gunicorn-20.0.4/docs/source/2015-news.rst`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/source/2016-news.rst` & `squad-gunicorn-20.0.4/docs/source/2016-news.rst`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/source/2017-news.rst` & `squad-gunicorn-20.0.4/docs/source/2017-news.rst`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/source/2018-news.rst` & `squad-gunicorn-20.0.4/docs/source/2018-news.rst`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/source/_static/gunicorn.png` & `squad-gunicorn-20.0.4/docs/source/_static/gunicorn.png`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/source/community.rst` & `squad-gunicorn-20.0.4/docs/source/community.rst`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/source/conf.py` & `squad-gunicorn-20.0.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/source/configure.rst` & `squad-gunicorn-20.0.4/docs/source/configure.rst`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/source/custom.rst` & `squad-gunicorn-20.0.4/docs/source/custom.rst`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/source/deploy.rst` & `squad-gunicorn-20.0.4/docs/source/deploy.rst`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/source/design.rst` & `squad-gunicorn-20.0.4/docs/source/design.rst`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/source/faq.rst` & `squad-gunicorn-20.0.4/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/source/index.rst` & `squad-gunicorn-20.0.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/source/install.rst` & `squad-gunicorn-20.0.4/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/source/instrumentation.rst` & `squad-gunicorn-20.0.4/docs/source/instrumentation.rst`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/source/news.rst` & `squad-gunicorn-20.0.4/docs/source/news.rst`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/source/run.rst` & `squad-gunicorn-20.0.4/docs/source/run.rst`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/source/settings.rst` & `squad-gunicorn-20.0.4/docs/source/settings.rst`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/docs/source/signals.rst` & `squad-gunicorn-20.0.4/docs/source/signals.rst`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/alt_spec.py` & `squad-gunicorn-20.0.4/examples/alt_spec.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/deep/test.py` & `squad-gunicorn-20.0.4/examples/deep/test.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/echo.py` & `squad-gunicorn-20.0.4/examples/echo.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/example_config.py` & `squad-gunicorn-20.0.4/examples/example_config.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/frameworks/django/testing/testing/apps/someapp/middleware.py` & `squad-gunicorn-20.0.4/examples/frameworks/django/testing/testing/apps/someapp/middleware.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/frameworks/django/testing/testing/apps/someapp/templates/base.html` & `squad-gunicorn-20.0.4/examples/frameworks/django/testing/testing/apps/someapp/templates/base.html`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/frameworks/django/testing/testing/apps/someapp/tests.py` & `squad-gunicorn-20.0.4/examples/frameworks/django/testing/testing/apps/someapp/tests.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/frameworks/django/testing/testing/apps/someapp/views.py` & `squad-gunicorn-20.0.4/examples/frameworks/django/testing/testing/apps/someapp/views.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/frameworks/django/testing/testing/settings.py` & `squad-gunicorn-20.0.4/examples/frameworks/django/testing/testing/settings.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/frameworks/django/testing/testing/urls.py` & `squad-gunicorn-20.0.4/examples/frameworks/django/testing/testing/urls.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/frameworks/django/testing/testing/wsgi.py` & `squad-gunicorn-20.0.4/examples/frameworks/django/testing/testing/wsgi.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/frameworks/tornadoapp.py` & `squad-gunicorn-20.0.4/examples/frameworks/tornadoapp.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/logging.conf` & `squad-gunicorn-20.0.4/examples/logging.conf`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/longpoll.py` & `squad-gunicorn-20.0.4/examples/longpoll.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/multiapp.py` & `squad-gunicorn-20.0.4/examples/multiapp.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/multidomainapp.py` & `squad-gunicorn-20.0.4/examples/multidomainapp.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/nginx.conf` & `squad-gunicorn-20.0.4/examples/nginx.conf`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/readline_app.py` & `squad-gunicorn-20.0.4/examples/readline_app.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/sendfile.py` & `squad-gunicorn-20.0.4/examples/sendfile.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/server.crt` & `squad-gunicorn-20.0.4/examples/server.crt`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/server.key` & `squad-gunicorn-20.0.4/examples/server.key`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/slowclient.py` & `squad-gunicorn-20.0.4/examples/slowclient.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/standalone_app.py` & `squad-gunicorn-20.0.4/examples/standalone_app.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/test.py` & `squad-gunicorn-20.0.4/examples/test.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/timeout.py` & `squad-gunicorn-20.0.4/examples/timeout.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/websocket/gevent_websocket.py` & `squad-gunicorn-20.0.4/examples/websocket/gevent_websocket.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/websocket/websocket.html` & `squad-gunicorn-20.0.4/examples/websocket/websocket.html`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/websocket/websocket.py` & `squad-gunicorn-20.0.4/examples/websocket/websocket.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/examples/when_ready.conf.py` & `squad-gunicorn-20.0.4/examples/when_ready.conf.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/app/base.py` & `squad-gunicorn-20.0.4/gunicorn/app/base.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/app/pasterapp.py` & `squad-gunicorn-20.0.4/gunicorn/app/pasterapp.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/app/wsgiapp.py` & `squad-gunicorn-20.0.4/gunicorn/app/wsgiapp.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/arbiter.py` & `squad-gunicorn-20.0.4/gunicorn/arbiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -566,19 +566,21 @@
                     process_info.append({
                         "pid": pid,
                         "rss": memory_info.rss,
                         "vms": memory_info.vms,
                     })
                 except (psutil.NoSuchProcess, psutil.AccessDenied):
                     continue
-            self.log.info("Process Info: {0}".format(process_info))
-
-            if self.cfg.statsd_host:
-                self.log.gauge("gunicorn.workers", active_worker_count)
-                self.log.gauge("gunicorn.busy_workers", busy_workers)
+            
+            self.log.debug("Process Info: {0}".format(process_info),
+                            extra={"metric": "gunicorn.processes",
+                                    "value": process_info,
+                                    "mtype": "gauge"})
+            self.log.gauge("gunicorn.workers", active_worker_count)
+            self.log.gauge("gunicorn.busy_workers", busy_workers)
 
 
     def spawn_worker(self):
         self.worker_age += 1
         worker = self.worker_class(self.worker_age, self.pid, self.LISTENERS,
                                    self.app, self.timeout / 2.0,
                                    self.cfg, self.log)
```

### Comparing `squad-gunicorn-121.0.4/gunicorn/config.py` & `squad-gunicorn-20.0.4/gunicorn/config.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/debug.py` & `squad-gunicorn-20.0.4/gunicorn/debug.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/errors.py` & `squad-gunicorn-20.0.4/gunicorn/errors.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/glogging.py` & `squad-gunicorn-20.0.4/gunicorn/glogging.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/http/body.py` & `squad-gunicorn-20.0.4/gunicorn/http/body.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/http/errors.py` & `squad-gunicorn-20.0.4/gunicorn/http/errors.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/http/message.py` & `squad-gunicorn-20.0.4/gunicorn/http/message.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/http/parser.py` & `squad-gunicorn-20.0.4/gunicorn/http/parser.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/http/unreader.py` & `squad-gunicorn-20.0.4/gunicorn/http/unreader.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/http/wsgi.py` & `squad-gunicorn-20.0.4/gunicorn/http/wsgi.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/instrument/statsd.py` & `squad-gunicorn-20.0.4/gunicorn/instrument/statsd.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/pidfile.py` & `squad-gunicorn-20.0.4/gunicorn/pidfile.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/reloader.py` & `squad-gunicorn-20.0.4/gunicorn/reloader.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/sock.py` & `squad-gunicorn-20.0.4/gunicorn/sock.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/systemd.py` & `squad-gunicorn-20.0.4/gunicorn/systemd.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/util.py` & `squad-gunicorn-20.0.4/gunicorn/util.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/workers/__init__.py` & `squad-gunicorn-20.0.4/gunicorn/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/workers/base.py` & `squad-gunicorn-20.0.4/gunicorn/workers/base.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/workers/base_async.py` & `squad-gunicorn-20.0.4/gunicorn/workers/base_async.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/workers/geventlet.py` & `squad-gunicorn-20.0.4/gunicorn/workers/geventlet.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/workers/ggevent.py` & `squad-gunicorn-20.0.4/gunicorn/workers/ggevent.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/workers/gthread.py` & `squad-gunicorn-20.0.4/gunicorn/workers/gthread.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/workers/gtornado.py` & `squad-gunicorn-20.0.4/gunicorn/workers/gtornado.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/workers/sync.py` & `squad-gunicorn-20.0.4/gunicorn/workers/sync.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/gunicorn/workers/workertmp.py` & `squad-gunicorn-20.0.4/gunicorn/workers/workertmp.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/setup.py` & `squad-gunicorn-20.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     'tornado': ['tornado>=0.2'],
     'gthread': [],
     'setproctitle': ['setproctitle'],
 }
 
 setup(
     name='squad-gunicorn',
-    version='121.0.4',
+    version=__version__,
 
     description='WSGI HTTP Server for UNIX',
     long_description=long_description,
     author='Benoit Chesneau',
     author_email='benoitc@e-engura.com',
     license='MIT',
     url='https://gunicorn.org',
@@ -115,8 +115,8 @@
     [console_scripts]
     gunicorn=gunicorn.app.wsgiapp:run
 
     [paste.server_runner]
     main=gunicorn.app.pasterapp:serve
     """,
     extras_require=extras_require,
-)
+)
```

### Comparing `squad-gunicorn-121.0.4/squad_gunicorn.egg-info/PKG-INFO` & `squad-gunicorn-20.0.4/squad_gunicorn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squad-gunicorn
-Version: 121.0.4
+Version: 20.0.4
 Summary: WSGI HTTP Server for UNIX
 Home-page: https://gunicorn.org
 Author: Benoit Chesneau
 Author-email: benoitc@e-engura.com
 License: MIT
 Project-URL: Documentation, https://docs.gunicorn.org
 Project-URL: Homepage, https://gunicorn.org
```

### Comparing `squad-gunicorn-121.0.4/squad_gunicorn.egg-info/SOURCES.txt` & `squad-gunicorn-20.0.4/squad_gunicorn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/requests/invalid/006.http` & `squad-gunicorn-20.0.4/tests/requests/invalid/006.http`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/requests/invalid/007.http` & `squad-gunicorn-20.0.4/tests/requests/invalid/007.http`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/requests/invalid/008.http` & `squad-gunicorn-20.0.4/tests/requests/invalid/008.http`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/requests/invalid/009.http` & `squad-gunicorn-20.0.4/tests/requests/invalid/009.http`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/requests/invalid/017.http` & `squad-gunicorn-20.0.4/tests/requests/invalid/017.http`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/requests/valid/003.py` & `squad-gunicorn-20.0.4/tests/requests/valid/003.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/requests/valid/016.http` & `squad-gunicorn-20.0.4/tests/requests/valid/016.http`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/requests/valid/016.py` & `squad-gunicorn-20.0.4/tests/requests/valid/016.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/requests/valid/024.http` & `squad-gunicorn-20.0.4/tests/requests/valid/024.http`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/requests/valid/024.py` & `squad-gunicorn-20.0.4/tests/requests/valid/024.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/requests/valid/026.http` & `squad-gunicorn-20.0.4/tests/requests/valid/026.http`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/requests/valid/026.py` & `squad-gunicorn-20.0.4/tests/requests/valid/026.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/requests/valid/099.http` & `squad-gunicorn-20.0.4/tests/requests/valid/099.http`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/requests/valid/099.py` & `squad-gunicorn-20.0.4/tests/requests/valid/099.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/requests/valid/pp_02.py` & `squad-gunicorn-20.0.4/tests/requests/valid/pp_02.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/support.py` & `squad-gunicorn-20.0.4/tests/support.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/t.py` & `squad-gunicorn-20.0.4/tests/t.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/test_arbiter.py` & `squad-gunicorn-20.0.4/tests/test_arbiter.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/test_config.py` & `squad-gunicorn-20.0.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/test_http.py` & `squad-gunicorn-20.0.4/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/test_invalid_requests.py` & `squad-gunicorn-20.0.4/tests/test_invalid_requests.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/test_logger.py` & `squad-gunicorn-20.0.4/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/test_pidfile.py` & `squad-gunicorn-20.0.4/tests/test_pidfile.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/test_reload.py` & `squad-gunicorn-20.0.4/tests/test_reload.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/test_sock.py` & `squad-gunicorn-20.0.4/tests/test_sock.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/test_ssl.py` & `squad-gunicorn-20.0.4/tests/test_ssl.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/test_statsd.py` & `squad-gunicorn-20.0.4/tests/test_statsd.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/test_systemd.py` & `squad-gunicorn-20.0.4/tests/test_systemd.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/test_util.py` & `squad-gunicorn-20.0.4/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/test_valid_requests.py` & `squad-gunicorn-20.0.4/tests/test_valid_requests.py`

 * *Files identical despite different names*

### Comparing `squad-gunicorn-121.0.4/tests/treq.py` & `squad-gunicorn-20.0.4/tests/treq.py`

 * *Files identical despite different names*

