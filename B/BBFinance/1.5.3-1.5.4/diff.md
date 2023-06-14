# Comparing `tmp/BBFinance-1.5.3.tar.gz` & `tmp/BBFinance-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BBFinance-1.5.3.tar", last modified: Wed Jun 14 00:35:46 2023, max compression
+gzip compressed data, was "BBFinance-1.5.4.tar", last modified: Wed Jun 14 00:45:54 2023, max compression
```

## Comparing `BBFinance-1.5.3.tar` & `BBFinance-1.5.4.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 00:35:46.541077 BBFinance-1.5.3/
-drwxrwxrwx   0        0        0        0 2023-06-14 00:35:46.404078 BBFinance-1.5.3/BBFdocs/
-drwxrwxrwx   0        0        0        0 2023-06-14 00:35:46.405076 BBFinance-1.5.3/BBFdocs/docs/
--rw-rw-rw-   0        0        0     4250 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/docs/index.md
--rw-rw-rw-   0        0        0       84 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/mkdocs.yml
-drwxrwxrwx   0        0        0        0 2023-06-14 00:35:46.411079 BBFinance-1.5.3/BBFdocs/site/
--rw-rw-rw-   0        0        0     6276 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/404.html
-drwxrwxrwx   0        0        0        0 2023-06-14 00:35:46.426082 BBFinance-1.5.3/BBFdocs/site/css/
--rw-rw-rw-   0        0        0     5924 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/css/base.css
--rw-rw-rw-   0        0        0     3488 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/css/base.min.css
--rw-rw-rw-   0        0        0   137774 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/css/bootstrap-custom.css
--rw-rw-rw-   0        0        0   109469 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/css/bootstrap-custom.min.css
--rw-rw-rw-   0        0        0     2219 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/css/cinder.css
--rw-rw-rw-   0        0        0     1638 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/css/cinder.min.css
--rw-rw-rw-   0        0        0     1247 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/css/highlight.css
--rw-rw-rw-   0        0        0      867 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/css/highlight.min.css
-drwxrwxrwx   0        0        0        0 2023-06-14 00:35:46.437079 BBFinance-1.5.3/BBFdocs/site/fonts/
--rw-rw-rw-   0        0        0    38205 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   202561 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0    80652 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    44432 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/fonts/fontawesome-webfont.woff
-drwxrwxrwx   0        0        0        0 2023-06-14 00:35:46.476078 BBFinance-1.5.3/BBFdocs/site/img/
--rw-rw-rw-   0        0        0     1150 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/img/favicon.ico
--rw-rw-rw-   0        0        0      251 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/img/grid1.png
--rw-rw-rw-   0        0        0      495 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/img/grid10.png
--rw-rw-rw-   0        0        0      253 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/img/grid11.png
--rw-rw-rw-   0        0        0      260 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/img/grid12.png
--rw-rw-rw-   0        0        0      266 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/img/grid13.png
--rw-rw-rw-   0        0        0      240 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/img/grid14.png
--rw-rw-rw-   0        0        0      442 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/img/grid15.png
--rw-rw-rw-   0        0        0      442 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/img/grid16.png
--rw-rw-rw-   0        0        0      442 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/img/grid17.png
--rw-rw-rw-   0        0        0      457 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/img/grid18.png
--rw-rw-rw-   0        0        0      427 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/img/grid19.png
--rw-rw-rw-   0        0        0      271 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/img/grid2.png
--rw-rw-rw-   0        0        0      493 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/img/grid20.png
--rw-rw-rw-   0        0        0      266 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/img/grid3.png
--rw-rw-rw-   0        0        0      244 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/img/grid4.png
--rw-rw-rw-   0        0        0      442 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/img/grid5.png
--rw-rw-rw-   0        0        0      460 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/img/grid6.png
--rw-rw-rw-   0        0        0      442 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/img/grid7.png
--rw-rw-rw-   0        0        0      457 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/img/grid8.png
--rw-rw-rw-   0        0        0      456 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/img/grid9.png
--rw-rw-rw-   0        0        0    11523 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/index.html
-drwxrwxrwx   0        0        0        0 2023-06-14 00:35:46.482080 BBFinance-1.5.3/BBFdocs/site/js/
--rw-rw-rw-   0        0        0     6136 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/js/base.js
--rw-rw-rw-   0        0        0    27828 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/js/bootstrap-3.0.3.min.js
--rw-rw-rw-   0        0        0    54609 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/js/highlight.pack.js
-drwxrwxrwx   0        0        0        0 2023-06-14 00:35:46.492085 BBFinance-1.5.3/BBFdocs/site/search/
--rw-rw-rw-   0        0        0   103280 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/search/lunr.js
--rw-rw-rw-   0        0        0     3315 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/search/main.js
--rw-rw-rw-   0        0        0     9063 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/search/search_index.json
--rw-rw-rw-   0        0        0     3857 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/search/worker.js
--rw-rw-rw-   0        0        0      241 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/sitemap.xml
--rw-rw-rw-   0        0        0      189 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFdocs/site/sitemap.xml.gz
-drwxrwxrwx   0        0        0        0 2023-06-14 00:35:46.502077 BBFinance-1.5.3/BBFinance/
--rw-rw-rw-   0        0        0      239 2023-06-14 00:28:46.000000 BBFinance-1.5.3/BBFinance/Apresentacao.py
--rw-rw-rw-   0        0        0    45408 2023-06-14 00:26:40.000000 BBFinance-1.5.3/BBFinance/BBFinance.py
--rw-rw-rw-   0        0        0      340 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFinance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 00:35:46.535079 BBFinance-1.5.3/BBFinance/__pycache__/
--rw-rw-rw-   0        0        0    49899 2023-06-14 00:26:45.000000 BBFinance-1.5.3/BBFinance/__pycache__/BBFinance.cpython-311.pyc
--rw-rw-rw-   0        0        0    26937 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFinance/__pycache__/BBFinance.cpython-39.pyc
--rw-rw-rw-   0        0        0      481 2023-04-19 01:37:03.000000 BBFinance-1.5.3/BBFinance/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      446 2023-04-19 01:01:27.000000 BBFinance-1.5.3/BBFinance/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-06-14 00:35:46.528078 BBFinance-1.5.3/BBFinance.egg-info/
--rw-rw-rw-   0        0        0     5167 2023-06-14 00:35:46.000000 BBFinance-1.5.3/BBFinance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1925 2023-06-14 00:35:46.000000 BBFinance-1.5.3/BBFinance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 00:35:46.000000 BBFinance-1.5.3/BBFinance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      302 2023-06-14 00:35:46.000000 BBFinance-1.5.3/BBFinance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-14 00:35:46.000000 BBFinance-1.5.3/BBFinance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      589 2023-04-19 01:01:27.000000 BBFinance-1.5.3/LICENSE.txt
--rw-rw-rw-   0        0        0     5167 2023-06-14 00:35:46.540078 BBFinance-1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     4542 2023-06-13 23:46:21.000000 BBFinance-1.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 00:35:46.538078 BBFinance-1.5.3/__pycache__/
--rw-rw-rw-   0        0        0      301 2023-04-19 01:01:27.000000 BBFinance-1.5.3/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     8340 2023-04-19 01:01:27.000000 BBFinance-1.5.3/__pycache__/main.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-06-14 00:35:46.539077 BBFinance-1.5.3/docs/
--rw-rw-rw-   0        0        0       17 2023-04-19 01:01:27.000000 BBFinance-1.5.3/docs/CNAME
--rw-rw-rw-   0        0        0     1430 2023-06-14 00:32:49.000000 BBFinance-1.5.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 00:35:46.542077 BBFinance-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1395 2023-06-14 00:33:19.000000 BBFinance-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:45:54.055667 BBFinance-1.5.4/
+drwxrwxrwx   0        0        0        0 2023-06-14 00:45:53.926667 BBFinance-1.5.4/BBFdocs/
+drwxrwxrwx   0        0        0        0 2023-06-14 00:45:53.928669 BBFinance-1.5.4/BBFdocs/docs/
+-rw-rw-rw-   0        0        0     4250 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/docs/index.md
+-rw-rw-rw-   0        0        0       84 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/mkdocs.yml
+drwxrwxrwx   0        0        0        0 2023-06-14 00:45:53.936669 BBFinance-1.5.4/BBFdocs/site/
+-rw-rw-rw-   0        0        0     6276 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/404.html
+drwxrwxrwx   0        0        0        0 2023-06-14 00:45:53.954667 BBFinance-1.5.4/BBFdocs/site/css/
+-rw-rw-rw-   0        0        0     5924 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/css/base.css
+-rw-rw-rw-   0        0        0     3488 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/css/base.min.css
+-rw-rw-rw-   0        0        0   137774 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/css/bootstrap-custom.css
+-rw-rw-rw-   0        0        0   109469 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/css/bootstrap-custom.min.css
+-rw-rw-rw-   0        0        0     2219 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/css/cinder.css
+-rw-rw-rw-   0        0        0     1638 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/css/cinder.min.css
+-rw-rw-rw-   0        0        0     1247 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/css/highlight.css
+-rw-rw-rw-   0        0        0      867 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/css/highlight.min.css
+drwxrwxrwx   0        0        0        0 2023-06-14 00:45:53.961667 BBFinance-1.5.4/BBFdocs/site/fonts/
+-rw-rw-rw-   0        0        0    38205 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   202561 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0    80652 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    44432 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/fonts/fontawesome-webfont.woff
+drwxrwxrwx   0        0        0        0 2023-06-14 00:45:53.995667 BBFinance-1.5.4/BBFdocs/site/img/
+-rw-rw-rw-   0        0        0     1150 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/img/favicon.ico
+-rw-rw-rw-   0        0        0      251 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/img/grid1.png
+-rw-rw-rw-   0        0        0      495 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/img/grid10.png
+-rw-rw-rw-   0        0        0      253 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/img/grid11.png
+-rw-rw-rw-   0        0        0      260 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/img/grid12.png
+-rw-rw-rw-   0        0        0      266 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/img/grid13.png
+-rw-rw-rw-   0        0        0      240 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/img/grid14.png
+-rw-rw-rw-   0        0        0      442 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/img/grid15.png
+-rw-rw-rw-   0        0        0      442 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/img/grid16.png
+-rw-rw-rw-   0        0        0      442 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/img/grid17.png
+-rw-rw-rw-   0        0        0      457 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/img/grid18.png
+-rw-rw-rw-   0        0        0      427 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/img/grid19.png
+-rw-rw-rw-   0        0        0      271 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/img/grid2.png
+-rw-rw-rw-   0        0        0      493 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/img/grid20.png
+-rw-rw-rw-   0        0        0      266 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/img/grid3.png
+-rw-rw-rw-   0        0        0      244 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/img/grid4.png
+-rw-rw-rw-   0        0        0      442 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/img/grid5.png
+-rw-rw-rw-   0        0        0      460 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/img/grid6.png
+-rw-rw-rw-   0        0        0      442 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/img/grid7.png
+-rw-rw-rw-   0        0        0      457 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/img/grid8.png
+-rw-rw-rw-   0        0        0      456 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/img/grid9.png
+-rw-rw-rw-   0        0        0    11523 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/index.html
+drwxrwxrwx   0        0        0        0 2023-06-14 00:45:53.999668 BBFinance-1.5.4/BBFdocs/site/js/
+-rw-rw-rw-   0        0        0     6136 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/js/base.js
+-rw-rw-rw-   0        0        0    27828 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/js/bootstrap-3.0.3.min.js
+-rw-rw-rw-   0        0        0    54609 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/js/highlight.pack.js
+drwxrwxrwx   0        0        0        0 2023-06-14 00:45:54.007667 BBFinance-1.5.4/BBFdocs/site/search/
+-rw-rw-rw-   0        0        0   103280 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/search/lunr.js
+-rw-rw-rw-   0        0        0     3315 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/search/main.js
+-rw-rw-rw-   0        0        0     9063 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/search/search_index.json
+-rw-rw-rw-   0        0        0     3857 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/search/worker.js
+-rw-rw-rw-   0        0        0      241 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/sitemap.xml
+-rw-rw-rw-   0        0        0      189 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFdocs/site/sitemap.xml.gz
+drwxrwxrwx   0        0        0        0 2023-06-14 00:45:54.011667 BBFinance-1.5.4/BBFinance/
+-rw-rw-rw-   0        0        0      249 2023-06-14 00:39:17.000000 BBFinance-1.5.4/BBFinance/Apresentacao.py
+-rw-rw-rw-   0        0        0    45408 2023-06-14 00:26:40.000000 BBFinance-1.5.4/BBFinance/BBFinance.py
+-rw-rw-rw-   0        0        0      340 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFinance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:45:54.049668 BBFinance-1.5.4/BBFinance/__pycache__/
+-rw-rw-rw-   0        0        0    49899 2023-06-14 00:26:45.000000 BBFinance-1.5.4/BBFinance/__pycache__/BBFinance.cpython-311.pyc
+-rw-rw-rw-   0        0        0    26937 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFinance/__pycache__/BBFinance.cpython-39.pyc
+-rw-rw-rw-   0        0        0      481 2023-04-19 01:37:03.000000 BBFinance-1.5.4/BBFinance/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      446 2023-04-19 01:01:27.000000 BBFinance-1.5.4/BBFinance/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-06-14 00:45:54.041666 BBFinance-1.5.4/BBFinance.egg-info/
+-rw-rw-rw-   0        0        0     5167 2023-06-14 00:45:53.000000 BBFinance-1.5.4/BBFinance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1925 2023-06-14 00:45:53.000000 BBFinance-1.5.4/BBFinance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 00:45:53.000000 BBFinance-1.5.4/BBFinance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      302 2023-06-14 00:45:53.000000 BBFinance-1.5.4/BBFinance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-14 00:45:53.000000 BBFinance-1.5.4/BBFinance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      589 2023-04-19 01:01:27.000000 BBFinance-1.5.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     5167 2023-06-14 00:45:54.055667 BBFinance-1.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4542 2023-06-13 23:46:21.000000 BBFinance-1.5.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 00:45:54.052667 BBFinance-1.5.4/__pycache__/
+-rw-rw-rw-   0        0        0      301 2023-04-19 01:01:27.000000 BBFinance-1.5.4/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8340 2023-04-19 01:01:27.000000 BBFinance-1.5.4/__pycache__/main.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-06-14 00:45:54.053666 BBFinance-1.5.4/docs/
+-rw-rw-rw-   0        0        0       17 2023-04-19 01:01:27.000000 BBFinance-1.5.4/docs/CNAME
+-rw-rw-rw-   0        0        0     1430 2023-06-14 00:45:06.000000 BBFinance-1.5.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 00:45:54.056668 BBFinance-1.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     1395 2023-06-14 00:45:26.000000 BBFinance-1.5.4/setup.py
```

### Comparing `BBFinance-1.5.3/BBFdocs/docs/index.md` & `BBFinance-1.5.4/BBFdocs/docs/index.md`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFdocs/site/404.html` & `BBFinance-1.5.4/BBFdocs/site/404.html`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFdocs/site/css/base.css` & `BBFinance-1.5.4/BBFdocs/site/css/base.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFdocs/site/css/base.min.css` & `BBFinance-1.5.4/BBFdocs/site/css/base.min.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFdocs/site/css/bootstrap-custom.css` & `BBFinance-1.5.4/BBFdocs/site/css/bootstrap-custom.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFdocs/site/css/bootstrap-custom.min.css` & `BBFinance-1.5.4/BBFdocs/site/css/bootstrap-custom.min.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFdocs/site/css/cinder.css` & `BBFinance-1.5.4/BBFdocs/site/css/cinder.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFdocs/site/css/cinder.min.css` & `BBFinance-1.5.4/BBFdocs/site/css/cinder.min.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFdocs/site/css/highlight.css` & `BBFinance-1.5.4/BBFdocs/site/css/highlight.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFdocs/site/css/highlight.min.css` & `BBFinance-1.5.4/BBFdocs/site/css/highlight.min.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFdocs/site/fonts/fontawesome-webfont.eot` & `BBFinance-1.5.4/BBFdocs/site/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFdocs/site/fonts/fontawesome-webfont.svg` & `BBFinance-1.5.4/BBFdocs/site/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFdocs/site/fonts/fontawesome-webfont.ttf` & `BBFinance-1.5.4/BBFdocs/site/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFdocs/site/fonts/fontawesome-webfont.woff` & `BBFinance-1.5.4/BBFdocs/site/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFdocs/site/img/favicon.ico` & `BBFinance-1.5.4/BBFdocs/site/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFdocs/site/index.html` & `BBFinance-1.5.4/BBFdocs/site/index.html`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFdocs/site/js/base.js` & `BBFinance-1.5.4/BBFdocs/site/js/base.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFdocs/site/js/bootstrap-3.0.3.min.js` & `BBFinance-1.5.4/BBFdocs/site/js/bootstrap-3.0.3.min.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFdocs/site/js/highlight.pack.js` & `BBFinance-1.5.4/BBFdocs/site/js/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFdocs/site/search/lunr.js` & `BBFinance-1.5.4/BBFdocs/site/search/lunr.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFdocs/site/search/main.js` & `BBFinance-1.5.4/BBFdocs/site/search/main.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFdocs/site/search/search_index.json` & `BBFinance-1.5.4/BBFdocs/site/search/search_index.json`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFdocs/site/search/worker.js` & `BBFinance-1.5.4/BBFdocs/site/search/worker.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFinance/BBFinance.py` & `BBFinance-1.5.4/BBFinance/BBFinance.py`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFinance/__pycache__/BBFinance.cpython-311.pyc` & `BBFinance-1.5.4/BBFinance/__pycache__/BBFinance.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFinance/__pycache__/BBFinance.cpython-39.pyc` & `BBFinance-1.5.4/BBFinance/__pycache__/BBFinance.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/BBFinance.egg-info/PKG-INFO` & `BBFinance-1.5.4/BBFinance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BBFinance
-Version: 1.5.3
+Version: 1.5.4
 Summary: Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado
 Home-page: https://github.com/beb0pp/BBFinance
 Author: Luis Abreu
 Author-email: luss.fel@gmail.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `BBFinance-1.5.3/BBFinance.egg-info/SOURCES.txt` & `BBFinance-1.5.4/BBFinance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/LICENSE.txt` & `BBFinance-1.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/PKG-INFO` & `BBFinance-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BBFinance
-Version: 1.5.3
+Version: 1.5.4
 Summary: Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado
 Home-page: https://github.com/beb0pp/BBFinance
 Author: Luis Abreu
 Author-email: luss.fel@gmail.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `BBFinance-1.5.3/README.md` & `BBFinance-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/__pycache__/main.cpython-39.pyc` & `BBFinance-1.5.4/__pycache__/main.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.3/requirements.txt` & `BBFinance-1.5.4/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿yfinance                      0.2.14
+﻿yfinance                      0.2.20
 scipy                         1.9.3
 selenium                      3.141.0
 pandas                        1.5.3
 pandas-datareader             0.10.0
 json5                         0.9.6
 numpy                         1.23.4
 uvicorn                       0.21.1
```

### Comparing `BBFinance-1.5.3/setup.py` & `BBFinance-1.5.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='BBFinance',
-    version='1.5.3',
+    version='1.5.4',
     description='Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado',
     url='https://github.com/beb0pp/BBFinance',
     author='Luis Abreu',
     author_email='luss.fel@gmail.com',
     license='GPLv3',
     packages=['BBFinance'],
     long_description= long_description,
     long_description_content_type='text/markdown',
     install_requires=[
-        'yfinance==0.2.14',
+        'yfinance==0.2.20',
         'selenium>=3.141.0',
         'pandas-datareader>=0.10.0',
         'json5>=0.9.6',
         'numpy>=1.21.6',
         'uvicorn>=0.21.1',
         'fastapi>=0.95.0',
         'scipy>=1.10.1',
```

