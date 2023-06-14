# Comparing `tmp/seaplane-0.3.8.tar.gz` & `tmp/seaplane-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaplane-0.3.8.tar", max compression
+gzip compressed data, was "seaplane-0.3.9.tar", max compression
```

## Comparing `seaplane-0.3.8.tar` & `seaplane-0.3.9.tar`

### file list

```diff
@@ -1,67 +1,68 @@
--rw-r--r--   0        0        0     1538 2023-05-10 16:05:26.809759 seaplane-0.3.8/README.md
--rw-r--r--   0        0        0     2682 2023-06-08 16:25:39.765711 seaplane-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     1178 2023-06-08 15:19:56.475350 seaplane-0.3.8/src/seaplane/__init__.py
--rw-r--r--   0        0        0      106 2023-06-07 13:57:55.120996 seaplane-0.3.8/src/seaplane/api/__init__.py
--rw-r--r--   0        0        0      527 2023-05-10 16:07:33.887179 seaplane-0.3.8/src/seaplane/api/api_http.py
--rw-r--r--   0        0        0     2558 2023-06-07 11:17:31.773475 seaplane-0.3.8/src/seaplane/api/api_request.py
--rw-r--r--   0        0        0     2987 2023-06-07 11:17:31.773747 seaplane-0.3.8/src/seaplane/api/compute_api.py
--rw-r--r--   0        0        0     3158 2023-06-07 11:17:31.774043 seaplane-0.3.8/src/seaplane/api/formation_configuration_api.py
--rw-r--r--   0        0        0     7410 2023-06-07 11:17:31.774348 seaplane-0.3.8/src/seaplane/api/lock_api.py
--rw-r--r--   0        0        0     5806 2023-06-07 11:17:31.774586 seaplane-0.3.8/src/seaplane/api/metadata_api.py
--rw-r--r--   0        0        0     7724 2023-06-07 11:17:31.774882 seaplane-0.3.8/src/seaplane/api/restrict_api.py
--rw-r--r--   0        0        0     1552 2023-06-07 11:17:31.775138 seaplane-0.3.8/src/seaplane/api/sql_api.py
--rw-r--r--   0        0        0     3141 2023-05-10 16:07:33.888286 seaplane-0.3.8/src/seaplane/api/token_api.py
--rw-r--r--   0        0        0       57 2023-06-08 15:27:56.714791 seaplane-0.3.8/src/seaplane/carrier/__init__.py
--rw-r--r--   0        0        0     2401 2023-06-08 15:27:17.021086 seaplane-0.3.8/src/seaplane/carrier/processor.py
--rw-r--r--   0        0        0     8148 2023-06-08 16:06:32.018960 seaplane-0.3.8/src/seaplane/configuration.py
--rw-r--r--   0        0        0     1818 2023-06-05 16:13:40.927293 seaplane-0.3.8/src/seaplane/logging/__init__.py
--rw-r--r--   0        0        0      334 2023-06-07 13:57:55.121524 seaplane-0.3.8/src/seaplane/model/__init__.py
--rw-r--r--   0        0        0     1310 2023-05-10 16:07:33.888946 seaplane-0.3.8/src/seaplane/model/compute/__init__.py
--rw-r--r--   0        0        0     1539 2023-05-10 16:07:33.889076 seaplane-0.3.8/src/seaplane/model/compute/formation_configuration.py
--rw-r--r--   0        0        0      129 2023-05-10 16:07:33.889214 seaplane-0.3.8/src/seaplane/model/compute/formation_metadata.py
--rw-r--r--   0        0        0      436 2023-05-10 16:07:33.889338 seaplane-0.3.8/src/seaplane/model/errors.py
--rw-r--r--   0        0        0     3077 2023-06-07 11:17:31.775418 seaplane-0.3.8/src/seaplane/model/locks/__init__.py
--rw-r--r--   0        0        0     3560 2023-06-07 11:17:31.775652 seaplane-0.3.8/src/seaplane/model/metadata/__init__.py
--rw-r--r--   0        0        0      422 2023-05-10 16:07:33.889804 seaplane-0.3.8/src/seaplane/model/provider.py
--rw-r--r--   0        0        0      478 2023-05-10 16:07:33.889921 seaplane-0.3.8/src/seaplane/model/region.py
--rw-r--r--   0        0        0     4221 2023-06-07 11:17:31.775895 seaplane-0.3.8/src/seaplane/model/restrict/__init__.py
--rw-r--r--   0        0        0      530 2023-05-10 16:07:33.890271 seaplane-0.3.8/src/seaplane/model/sql/__init__.py
--rw-r--r--   0        0        0      313 2023-06-08 15:19:30.007796 seaplane-0.3.8/src/seaplane/smartpipes/__init__.py
--rw-r--r--   0        0        0     1521 2023-06-08 15:18:22.874342 seaplane-0.3.8/src/seaplane/smartpipes/build.py
--rw-r--r--   0        0        0     2756 2023-06-07 14:00:21.738111 seaplane-0.3.8/src/seaplane/smartpipes/coprocessor.py
--rw-r--r--   0        0        0      166 2023-06-07 13:57:55.122029 seaplane-0.3.8/src/seaplane/smartpipes/coprocessors/__init__.py
--rw-r--r--   0        0        0     1827 2023-06-07 13:57:55.122241 seaplane-0.3.8/src/seaplane/smartpipes/coprocessors/bloom.py
--rw-r--r--   0        0        0     3242 2023-06-07 13:57:55.122396 seaplane-0.3.8/src/seaplane/smartpipes/coprocessors/openai.py
--rw-r--r--   0        0        0     4054 2023-06-07 13:57:55.122622 seaplane-0.3.8/src/seaplane/smartpipes/coprocessors/pinecone.py
--rw-r--r--   0        0        0     3164 2023-06-07 13:57:55.122771 seaplane-0.3.8/src/seaplane/smartpipes/coprocessors/replicate.py
--rw-r--r--   0        0        0     7131 2023-06-08 06:15:04.301952 seaplane-0.3.8/src/seaplane/smartpipes/decorators.py
--rw-r--r--   0        0        0     6081 2023-06-08 16:19:46.270911 seaplane-0.3.8/src/seaplane/smartpipes/deploy.py
--rw-r--r--   0        0        0     2364 2023-06-07 14:02:48.693793 seaplane-0.3.8/src/seaplane/smartpipes/event_handler.py
--rw-r--r--   0        0        0     1639 2023-06-07 14:17:11.058070 seaplane-0.3.8/src/seaplane/smartpipes/executor.py
--rw-r--r--   0        0        0     3231 2023-06-08 15:31:47.495475 seaplane-0.3.8/src/seaplane/smartpipes/smartapi.py
--rw-r--r--   0        0        0     2090 2023-06-07 13:59:40.996093 seaplane-0.3.8/src/seaplane/smartpipes/smartpipe.py
--rw-r--r--   0        0        0       33 2023-06-05 16:13:40.929884 seaplane-0.3.8/src/seaplane/smartpipes/website/.gitignore
--rw-r--r--   0        0        0     1750 2023-06-05 16:13:40.930353 seaplane-0.3.8/src/seaplane/smartpipes/website/README.md
--rw-r--r--   0        0        0       77 2023-06-05 16:13:40.930859 seaplane-0.3.8/src/seaplane/smartpipes/website/jsconfig.json
--rw-r--r--   0        0        0      118 2023-06-05 16:13:40.931524 seaplane-0.3.8/src/seaplane/smartpipes/website/next.config.js
--rw-r--r--   0        0        0      650 2023-06-05 16:13:40.932082 seaplane-0.3.8/src/seaplane/smartpipes/website/package.json
--rw-r--r--   0        0        0       82 2023-06-05 16:13:40.932489 seaplane-0.3.8/src/seaplane/smartpipes/website/postcss.config.js
--rw-r--r--   0        0        0      717 2023-06-05 16:13:40.933215 seaplane-0.3.8/src/seaplane/smartpipes/website/public/favicon.ico
--rw-r--r--   0        0        0     1375 2023-06-05 16:13:40.933596 seaplane-0.3.8/src/seaplane/smartpipes/website/public/next.svg
--rw-r--r--   0        0        0    39147 2023-06-05 16:13:40.934215 seaplane-0.3.8/src/seaplane/smartpipes/website/public/openai.png
--rw-r--r--   0        0        0    11580 2023-06-05 16:13:40.934926 seaplane-0.3.8/src/seaplane/smartpipes/website/public/seaplane_logo.svg
--rw-r--r--   0        0        0     2296 2023-06-05 16:13:40.935333 seaplane-0.3.8/src/seaplane/smartpipes/website/public/seaplane_logo_mark.svg
--rw-r--r--   0        0        0   195272 2023-06-05 16:13:40.938647 seaplane-0.3.8/src/seaplane/smartpipes/website/public/stabilityai.png
--rw-r--r--   0        0        0      629 2023-06-05 16:13:40.939528 seaplane-0.3.8/src/seaplane/smartpipes/website/public/vercel.svg
--rw-r--r--   0        0        0     3691 2023-06-05 16:13:40.943187 seaplane-0.3.8/src/seaplane/smartpipes/website/src/components/Header.jsx
--rw-r--r--   0        0        0    10990 2023-06-05 16:13:40.944429 seaplane-0.3.8/src/seaplane/smartpipes/website/src/components/SmartPipe.jsx
--rw-r--r--   0        0        0     4317 2023-06-07 13:59:40.996261 seaplane-0.3.8/src/seaplane/smartpipes/website/src/components/SmartPipesList.jsx
--rw-r--r--   0        0        0      127 2023-06-05 16:13:40.945730 seaplane-0.3.8/src/seaplane/smartpipes/website/src/pages/_app.js
--rw-r--r--   0        0        0      231 2023-06-05 16:13:40.946888 seaplane-0.3.8/src/seaplane/smartpipes/website/src/pages/_document.js
--rw-r--r--   0        0        0     1962 2023-06-05 16:13:40.947276 seaplane-0.3.8/src/seaplane/smartpipes/website/src/pages/index.js
--rw-r--r--   0        0        0     2643 2023-06-07 13:57:55.123829 seaplane-0.3.8/src/seaplane/smartpipes/website/src/pages/tutorial.js
--rw-r--r--   0        0        0      228 2023-06-05 16:13:40.947900 seaplane-0.3.8/src/seaplane/smartpipes/website/src/styles/globals.css
--rw-r--r--   0        0        0      528 2023-06-05 16:13:40.948083 seaplane-0.3.8/src/seaplane/smartpipes/website/tailwind.config.js
--rw-r--r--   0        0        0      424 2023-05-10 16:07:33.896564 seaplane-0.3.8/src/seaplane/util/__init__.py
--rw-r--r--   0        0        0      318 2023-05-10 16:07:33.896679 seaplane-0.3.8/src/seaplane/util/base64url.py
--rw-r--r--   0        0        0     3233 1970-01-01 00:00:00.000000 seaplane-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1538 2023-05-10 16:05:26.809759 seaplane-0.3.9/README.md
+-rw-r--r--   0        0        0     2682 2023-06-08 16:33:33.572139 seaplane-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1178 2023-06-08 15:19:56.475350 seaplane-0.3.9/src/seaplane/__init__.py
+-rw-r--r--   0        0        0      106 2023-06-07 13:57:55.120996 seaplane-0.3.9/src/seaplane/api/__init__.py
+-rw-r--r--   0        0        0      527 2023-05-10 16:07:33.887179 seaplane-0.3.9/src/seaplane/api/api_http.py
+-rw-r--r--   0        0        0     2558 2023-06-07 11:17:31.773475 seaplane-0.3.9/src/seaplane/api/api_request.py
+-rw-r--r--   0        0        0     2987 2023-06-07 11:17:31.773747 seaplane-0.3.9/src/seaplane/api/compute_api.py
+-rw-r--r--   0        0        0     3158 2023-06-07 11:17:31.774043 seaplane-0.3.9/src/seaplane/api/formation_configuration_api.py
+-rw-r--r--   0        0        0     7410 2023-06-07 11:17:31.774348 seaplane-0.3.9/src/seaplane/api/lock_api.py
+-rw-r--r--   0        0        0     5806 2023-06-07 11:17:31.774586 seaplane-0.3.9/src/seaplane/api/metadata_api.py
+-rw-r--r--   0        0        0     7724 2023-06-07 11:17:31.774882 seaplane-0.3.9/src/seaplane/api/restrict_api.py
+-rw-r--r--   0        0        0     1552 2023-06-07 11:17:31.775138 seaplane-0.3.9/src/seaplane/api/sql_api.py
+-rw-r--r--   0        0        0     3141 2023-05-10 16:07:33.888286 seaplane-0.3.9/src/seaplane/api/token_api.py
+-rw-r--r--   0        0        0       57 2023-06-08 15:27:56.714791 seaplane-0.3.9/src/seaplane/carrier/__init__.py
+-rw-r--r--   0        0        0     2401 2023-06-08 15:27:17.021086 seaplane-0.3.9/src/seaplane/carrier/processor.py
+-rw-r--r--   0        0        0     8148 2023-06-08 16:06:32.018960 seaplane-0.3.9/src/seaplane/configuration.py
+-rw-r--r--   0        0        0     1818 2023-06-05 16:13:40.927293 seaplane-0.3.9/src/seaplane/logging/__init__.py
+-rw-r--r--   0        0        0      334 2023-06-07 13:57:55.121524 seaplane-0.3.9/src/seaplane/model/__init__.py
+-rw-r--r--   0        0        0     1310 2023-05-10 16:07:33.888946 seaplane-0.3.9/src/seaplane/model/compute/__init__.py
+-rw-r--r--   0        0        0     1539 2023-05-10 16:07:33.889076 seaplane-0.3.9/src/seaplane/model/compute/formation_configuration.py
+-rw-r--r--   0        0        0      129 2023-05-10 16:07:33.889214 seaplane-0.3.9/src/seaplane/model/compute/formation_metadata.py
+-rw-r--r--   0        0        0      436 2023-05-10 16:07:33.889338 seaplane-0.3.9/src/seaplane/model/errors.py
+-rw-r--r--   0        0        0     3077 2023-06-07 11:17:31.775418 seaplane-0.3.9/src/seaplane/model/locks/__init__.py
+-rw-r--r--   0        0        0     3560 2023-06-07 11:17:31.775652 seaplane-0.3.9/src/seaplane/model/metadata/__init__.py
+-rw-r--r--   0        0        0      422 2023-05-10 16:07:33.889804 seaplane-0.3.9/src/seaplane/model/provider.py
+-rw-r--r--   0        0        0      478 2023-05-10 16:07:33.889921 seaplane-0.3.9/src/seaplane/model/region.py
+-rw-r--r--   0        0        0     4221 2023-06-07 11:17:31.775895 seaplane-0.3.9/src/seaplane/model/restrict/__init__.py
+-rw-r--r--   0        0        0      530 2023-05-10 16:07:33.890271 seaplane-0.3.9/src/seaplane/model/sql/__init__.py
+-rw-r--r--   0        0        0      313 2023-06-08 15:19:30.007796 seaplane-0.3.9/src/seaplane/smartpipes/__init__.py
+-rw-r--r--   0        0        0     1521 2023-06-08 15:18:22.874342 seaplane-0.3.9/src/seaplane/smartpipes/build.py
+-rw-r--r--   0        0        0     2756 2023-06-07 14:00:21.738111 seaplane-0.3.9/src/seaplane/smartpipes/coprocessor.py
+-rw-r--r--   0        0        0      166 2023-06-07 13:57:55.122029 seaplane-0.3.9/src/seaplane/smartpipes/coprocessors/__init__.py
+-rw-r--r--   0        0        0     1827 2023-06-07 13:57:55.122241 seaplane-0.3.9/src/seaplane/smartpipes/coprocessors/bloom.py
+-rw-r--r--   0        0        0     3242 2023-06-07 13:57:55.122396 seaplane-0.3.9/src/seaplane/smartpipes/coprocessors/openai.py
+-rw-r--r--   0        0        0     4054 2023-06-07 13:57:55.122622 seaplane-0.3.9/src/seaplane/smartpipes/coprocessors/pinecone.py
+-rw-r--r--   0        0        0     3164 2023-06-07 13:57:55.122771 seaplane-0.3.9/src/seaplane/smartpipes/coprocessors/replicate.py
+-rw-r--r--   0        0        0     7131 2023-06-08 06:15:04.301952 seaplane-0.3.9/src/seaplane/smartpipes/decorators.py
+-rw-r--r--   0        0        0     6081 2023-06-08 16:19:46.270911 seaplane-0.3.9/src/seaplane/smartpipes/deploy.py
+-rw-r--r--   0        0        0     2364 2023-06-07 14:02:48.693793 seaplane-0.3.9/src/seaplane/smartpipes/event_handler.py
+-rw-r--r--   0        0        0     1639 2023-06-07 14:17:11.058070 seaplane-0.3.9/src/seaplane/smartpipes/executor.py
+-rw-r--r--   0        0        0     3495 2023-06-08 16:33:17.244291 seaplane-0.3.9/src/seaplane/smartpipes/smartapi.py
+-rw-r--r--   0        0        0     2090 2023-06-07 13:59:40.996093 seaplane-0.3.9/src/seaplane/smartpipes/smartpipe.py
+-rw-r--r--   0        0        0       33 2023-06-05 16:13:40.929884 seaplane-0.3.9/src/seaplane/smartpipes/website/.gitignore
+-rw-r--r--   0        0        0     1750 2023-06-05 16:13:40.930353 seaplane-0.3.9/src/seaplane/smartpipes/website/README.md
+-rw-r--r--   0        0        0       77 2023-06-05 16:13:40.930859 seaplane-0.3.9/src/seaplane/smartpipes/website/jsconfig.json
+-rw-r--r--   0        0        0      118 2023-06-05 16:13:40.931524 seaplane-0.3.9/src/seaplane/smartpipes/website/next.config.js
+-rw-r--r--   0        0        0      650 2023-06-05 16:13:40.932082 seaplane-0.3.9/src/seaplane/smartpipes/website/package.json
+-rw-r--r--   0        0        0       82 2023-06-05 16:13:40.932489 seaplane-0.3.9/src/seaplane/smartpipes/website/postcss.config.js
+-rw-r--r--   0        0        0      717 2023-06-05 16:13:40.933215 seaplane-0.3.9/src/seaplane/smartpipes/website/public/favicon.ico
+-rw-r--r--   0        0        0     1375 2023-06-05 16:13:40.933596 seaplane-0.3.9/src/seaplane/smartpipes/website/public/next.svg
+-rw-r--r--   0        0        0    39147 2023-06-05 16:13:40.934215 seaplane-0.3.9/src/seaplane/smartpipes/website/public/openai.png
+-rw-r--r--   0        0        0    11580 2023-06-05 16:13:40.934926 seaplane-0.3.9/src/seaplane/smartpipes/website/public/seaplane_logo.svg
+-rw-r--r--   0        0        0     2296 2023-06-05 16:13:40.935333 seaplane-0.3.9/src/seaplane/smartpipes/website/public/seaplane_logo_mark.svg
+-rw-r--r--   0        0        0   195272 2023-06-05 16:13:40.938647 seaplane-0.3.9/src/seaplane/smartpipes/website/public/stabilityai.png
+-rw-r--r--   0        0        0      629 2023-06-05 16:13:40.939528 seaplane-0.3.9/src/seaplane/smartpipes/website/public/vercel.svg
+-rw-r--r--   0        0        0     3691 2023-06-05 16:13:40.943187 seaplane-0.3.9/src/seaplane/smartpipes/website/src/components/Header.jsx
+-rw-r--r--   0        0        0    10990 2023-06-05 16:13:40.944429 seaplane-0.3.9/src/seaplane/smartpipes/website/src/components/SmartPipe.jsx
+-rw-r--r--   0        0        0     4317 2023-06-07 13:59:40.996261 seaplane-0.3.9/src/seaplane/smartpipes/website/src/components/SmartPipesList.jsx
+-rw-r--r--   0        0        0      127 2023-06-05 16:13:40.945730 seaplane-0.3.9/src/seaplane/smartpipes/website/src/pages/_app.js
+-rw-r--r--   0        0        0      231 2023-06-05 16:13:40.946888 seaplane-0.3.9/src/seaplane/smartpipes/website/src/pages/_document.js
+-rw-r--r--   0        0        0     1962 2023-06-05 16:13:40.947276 seaplane-0.3.9/src/seaplane/smartpipes/website/src/pages/index.js
+-rw-r--r--   0        0        0     2643 2023-06-07 13:57:55.123829 seaplane-0.3.9/src/seaplane/smartpipes/website/src/pages/tutorial.js
+-rw-r--r--   0        0        0      228 2023-06-05 16:13:40.947900 seaplane-0.3.9/src/seaplane/smartpipes/website/src/styles/globals.css
+-rw-r--r--   0        0        0      528 2023-06-05 16:13:40.948083 seaplane-0.3.9/src/seaplane/smartpipes/website/tailwind.config.js
+-rw-r--r--   0        0        0      424 2023-05-10 16:07:33.896564 seaplane-0.3.9/src/seaplane/util/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-10 16:07:33.896679 seaplane-0.3.9/src/seaplane/util/base64url.py
+-rw-r--r--   0        0        0     5883 2023-06-08 16:34:11.748651 seaplane-0.3.9/setup.py
+-rw-r--r--   0        0        0     3182 2023-06-08 16:34:11.748974 seaplane-0.3.9/PKG-INFO
```

### Comparing `seaplane-0.3.8/README.md` & `seaplane-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/pyproject.toml` & `seaplane-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seaplane"
-version = "0.3.8"
+version = "0.3.9"
 description = "Seaplane Python SDK"
 authors = ["Seaplane IO, Inc."]
 license = "Apache License"
 readme = "README.md"
 repository = "https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python"
 documentation = "https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python"
```

### Comparing `seaplane-0.3.8/src/seaplane/__init__.py` & `seaplane-0.3.9/src/seaplane/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/api/api_http.py` & `seaplane-0.3.9/src/seaplane/api/api_http.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/api/api_request.py` & `seaplane-0.3.9/src/seaplane/api/api_request.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/api/compute_api.py` & `seaplane-0.3.9/src/seaplane/api/compute_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/api/formation_configuration_api.py` & `seaplane-0.3.9/src/seaplane/api/formation_configuration_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/api/lock_api.py` & `seaplane-0.3.9/src/seaplane/api/lock_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/api/metadata_api.py` & `seaplane-0.3.9/src/seaplane/api/metadata_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/api/restrict_api.py` & `seaplane-0.3.9/src/seaplane/api/restrict_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/api/sql_api.py` & `seaplane-0.3.9/src/seaplane/api/sql_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/api/token_api.py` & `seaplane-0.3.9/src/seaplane/api/token_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/carrier/processor.py` & `seaplane-0.3.9/src/seaplane/carrier/processor.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/configuration.py` & `seaplane-0.3.9/src/seaplane/configuration.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/logging/__init__.py` & `seaplane-0.3.9/src/seaplane/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/model/compute/__init__.py` & `seaplane-0.3.9/src/seaplane/model/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/model/compute/formation_configuration.py` & `seaplane-0.3.9/src/seaplane/model/compute/formation_configuration.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/model/locks/__init__.py` & `seaplane-0.3.9/src/seaplane/model/locks/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/model/metadata/__init__.py` & `seaplane-0.3.9/src/seaplane/model/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/model/restrict/__init__.py` & `seaplane-0.3.9/src/seaplane/model/restrict/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/model/sql/__init__.py` & `seaplane-0.3.9/src/seaplane/model/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/build.py` & `seaplane-0.3.9/src/seaplane/smartpipes/build.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/coprocessor.py` & `seaplane-0.3.9/src/seaplane/smartpipes/coprocessor.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/coprocessors/bloom.py` & `seaplane-0.3.9/src/seaplane/smartpipes/coprocessors/bloom.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/coprocessors/openai.py` & `seaplane-0.3.9/src/seaplane/smartpipes/coprocessors/openai.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/coprocessors/pinecone.py` & `seaplane-0.3.9/src/seaplane/smartpipes/coprocessors/pinecone.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/coprocessors/replicate.py` & `seaplane-0.3.9/src/seaplane/smartpipes/coprocessors/replicate.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/decorators.py` & `seaplane-0.3.9/src/seaplane/smartpipes/decorators.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/deploy.py` & `seaplane-0.3.9/src/seaplane/smartpipes/deploy.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/event_handler.py` & `seaplane-0.3.9/src/seaplane/smartpipes/event_handler.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/executor.py` & `seaplane-0.3.9/src/seaplane/smartpipes/executor.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/smartapi.py` & `seaplane-0.3.9/src/seaplane/smartpipes/smartapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import functools
 import os
-import json
+import sys
 from typing import Any, Optional
 
 from flask import Flask, request
 from flask_cors import CORS
 from flask_socketio import SocketIO, emit
 
 from ..configuration import config
 from ..logging import log
 from .decorators import context, smart_pipes_json
 from .smartpipe import SmartPipe
 from ..model.errors import SeaplaneError
 from ..carrier import processor
+from .build import build
+from .deploy import deploy
 
 SMARTPIPES_CORS = list(os.getenv("SMARTPIPES_CORS", "http://localhost:3000").split(" "))
 AUTH_TOKEN = os.getenv("SMARTPIPES_AUTH_TOKEN")
 
 app = Flask(__name__)
 sio = SocketIO(app, cors_allowed_origins=SMARTPIPES_CORS, async_mode="threading")
 CORS(app, origins=SMARTPIPES_CORS)
@@ -97,14 +99,24 @@
     while True:        
         print(f" Coprocessor {coprocessor.id}  waiting for getting data...")
         message = processor.read()
         print(f"  RECEIVED! {message}")
 
 
 def start() -> Optional[Flask]:
+    if len(sys.argv) > 1:
+        command = sys.argv[0]
+
+        if command == "build":
+            build()
+            return None
+        elif command == "deploy": 
+            deploy()
+            return None
+
     coprocessor_id = os.getenv("COPROCESSOR_ID")
 
     if not coprocessor_id:
         log.info("Starting API Entry Point...")
         return https_api_start()
     else:
         log.info(f"Starting Coprocessor {coprocessor_id} ...")
```

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/smartpipe.py` & `seaplane-0.3.9/src/seaplane/smartpipes/smartpipe.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/website/README.md` & `seaplane-0.3.9/src/seaplane/smartpipes/website/README.md`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/website/package.json` & `seaplane-0.3.9/src/seaplane/smartpipes/website/package.json`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/website/public/favicon.ico` & `seaplane-0.3.9/src/seaplane/smartpipes/website/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/website/public/next.svg` & `seaplane-0.3.9/src/seaplane/smartpipes/website/public/next.svg`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/website/public/openai.png` & `seaplane-0.3.9/src/seaplane/smartpipes/website/public/openai.png`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/website/public/seaplane_logo.svg` & `seaplane-0.3.9/src/seaplane/smartpipes/website/public/seaplane_logo.svg`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/website/public/seaplane_logo_mark.svg` & `seaplane-0.3.9/src/seaplane/smartpipes/website/public/seaplane_logo_mark.svg`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/website/public/stabilityai.png` & `seaplane-0.3.9/src/seaplane/smartpipes/website/public/stabilityai.png`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/website/public/vercel.svg` & `seaplane-0.3.9/src/seaplane/smartpipes/website/public/vercel.svg`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/website/src/components/Header.jsx` & `seaplane-0.3.9/src/seaplane/smartpipes/website/src/components/Header.jsx`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/website/src/components/SmartPipe.jsx` & `seaplane-0.3.9/src/seaplane/smartpipes/website/src/components/SmartPipe.jsx`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/website/src/components/SmartPipesList.jsx` & `seaplane-0.3.9/src/seaplane/smartpipes/website/src/components/SmartPipesList.jsx`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/website/src/pages/index.js` & `seaplane-0.3.9/src/seaplane/smartpipes/website/src/pages/index.js`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/website/src/pages/tutorial.js` & `seaplane-0.3.9/src/seaplane/smartpipes/website/src/pages/tutorial.js`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/src/seaplane/smartpipes/website/tailwind.config.js` & `seaplane-0.3.9/src/seaplane/smartpipes/website/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.8/PKG-INFO` & `seaplane-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: seaplane
-Version: 0.3.8
+Version: 0.3.9
 Summary: Seaplane Python SDK
 Home-page: https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python
 License: Apache License
 Author: Seaplane IO, Inc.
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Flask-Cors (>=3.0.10,<4.0.0)
 Requires-Dist: Flask-SocketIO (>=5.3.4,<6.0.0)
 Requires-Dist: attrs (==21.4.0)
 Requires-Dist: boto3 (>=1.26.142,<2.0.0)
 Requires-Dist: certifi (==2022.6.15)
 Requires-Dist: charset-normalizer (==2.1.0)
 Requires-Dist: idna (==3.3)
```

