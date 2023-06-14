# Comparing `tmp/oceanumlab-0.4.0.tar.gz` & `tmp/oceanumlab-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oceanumlab-0.4.0.tar", last modified: Tue Feb 28 20:30:40 2023, max compression
+gzip compressed data, was "oceanumlab-0.4.1.tar", last modified: Wed Jun 14 02:06:28 2023, max compression
```

## Comparing `oceanumlab-0.4.0.tar` & `oceanumlab-0.4.1.tar`

### file list

```diff
@@ -1,105 +1,71 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-28 20:30:40.309141 oceanumlab-0.4.0/
--rw-rw-r--   0 dave      (1000) dave      (1000)       86 2022-06-20 01:46:54.000000 oceanumlab-0.4.0/CHANGELOG.md
--rw-rw-r--   0 dave      (1000) dave      (1000)     1515 2022-06-20 01:46:54.000000 oceanumlab-0.4.0/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)      512 2022-06-20 01:46:54.000000 oceanumlab-0.4.0/MANIFEST.in
--rw-rw-r--   0 dave      (1000) dave      (1000)     4980 2023-02-28 20:30:40.309141 oceanumlab-0.4.0/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     3912 2022-06-27 22:21:02.000000 oceanumlab-0.4.0/README.md
--rw-rw-r--   0 dave      (1000) dave      (1000)     1892 2022-06-20 01:46:54.000000 oceanumlab-0.4.0/RELEASE.md
--rw-rw-r--   0 dave      (1000) dave      (1000)       68 2022-06-20 01:46:54.000000 oceanumlab-0.4.0/babel.config.js
--rw-rw-r--   0 dave      (1000) dave      (1000)      197 2022-06-20 01:46:54.000000 oceanumlab-0.4.0/conftest.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      181 2022-06-20 01:46:54.000000 oceanumlab-0.4.0/install.json
--rw-rw-r--   0 dave      (1000) dave      (1000)      864 2022-06-20 01:46:54.000000 oceanumlab-0.4.0/jest.config.js
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-28 20:30:40.189144 oceanumlab-0.4.0/jupyter-config/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-28 20:30:40.201143 oceanumlab-0.4.0/jupyter-config/nb-config/
--rw-rw-r--   0 dave      (1000) dave      (1000)       87 2022-06-20 01:46:54.000000 oceanumlab-0.4.0/jupyter-config/nb-config/oceanumlab.json
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-28 20:30:40.201143 oceanumlab-0.4.0/jupyter-config/server-config/
--rw-rw-r--   0 dave      (1000) dave      (1000)       85 2022-06-20 01:46:54.000000 oceanumlab-0.4.0/jupyter-config/server-config/oceanumlab.json
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-28 20:30:40.205143 oceanumlab-0.4.0/oceanumlab/
--rw-rw-r--   0 dave      (1000) dave      (1000)      926 2022-10-19 02:54:28.000000 oceanumlab-0.4.0/oceanumlab/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1044 2023-02-27 02:23:39.000000 oceanumlab-0.4.0/oceanumlab/handlers.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-28 20:30:40.205143 oceanumlab-0.4.0/oceanumlab/labextension/
--rw-rw-r--   0 dave      (1000) dave      (1000)    21087 2023-02-27 05:32:24.000000 oceanumlab-0.4.0/oceanumlab/labextension/build_log.json
--rw-rw-r--   0 dave      (1000) dave      (1000)      181 2023-02-27 05:32:24.000000 oceanumlab-0.4.0/oceanumlab/labextension/install.json
--rw-rw-r--   0 dave      (1000) dave      (1000)     4014 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/package.json
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-28 20:30:40.189144 oceanumlab-0.4.0/oceanumlab/labextension/schemas/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-28 20:30:40.189144 oceanumlab-0.4.0/oceanumlab/labextension/schemas/@oceanum/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-28 20:30:40.209143 oceanumlab-0.4.0/oceanumlab/labextension/schemas/@oceanum/oceanumlab/
--rw-rw-r--   0 dave      (1000) dave      (1000)     3872 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/schemas/@oceanum/oceanumlab/package.json.orig
--rw-rw-r--   0 dave      (1000) dave      (1000)      670 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/schemas/@oceanum/oceanumlab/plugin.json
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-28 20:30:40.265142 oceanumlab-0.4.0/oceanumlab/labextension/static/
--rw-rw-r--   0 dave      (1000) dave      (1000)    51847 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/lib_index_js.3adc3e3adbb825b0813c.js
--rw-rw-r--   0 dave      (1000) dave      (1000)    43338 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/lib_index_js.3adc3e3adbb825b0813c.js.map
--rw-rw-r--   0 dave      (1000) dave      (1000)    51932 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/lib_index_js.473e8c5ec2c268001788.js
--rw-rw-r--   0 dave      (1000) dave      (1000)    43442 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/lib_index_js.473e8c5ec2c268001788.js.map
--rw-rw-r--   0 dave      (1000) dave      (1000)    51846 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/lib_index_js.4fd8dcb8ffe729a53ddc.js
--rw-rw-r--   0 dave      (1000) dave      (1000)    43337 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/lib_index_js.4fd8dcb8ffe729a53ddc.js.map
--rw-rw-r--   0 dave      (1000) dave      (1000)    51745 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/lib_index_js.538b13d54a42133c68c0.js
--rw-rw-r--   0 dave      (1000) dave      (1000)    43188 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/lib_index_js.538b13d54a42133c68c0.js.map
--rw-rw-r--   0 dave      (1000) dave      (1000)    51845 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/lib_index_js.851145418e6542f82014.js
--rw-rw-r--   0 dave      (1000) dave      (1000)    43336 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/lib_index_js.851145418e6542f82014.js.map
--rw-rw-r--   0 dave      (1000) dave      (1000)    51748 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/lib_index_js.92838fb259e176bb9527.js
--rw-rw-r--   0 dave      (1000) dave      (1000)    43245 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/lib_index_js.92838fb259e176bb9527.js.map
--rw-rw-r--   0 dave      (1000) dave      (1000)    51739 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/lib_index_js.b12ff7c5c15a8d9c265d.js
--rw-rw-r--   0 dave      (1000) dave      (1000)    43236 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/lib_index_js.b12ff7c5c15a8d9c265d.js.map
--rw-rw-r--   0 dave      (1000) dave      (1000)    51739 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/lib_index_js.be8adfeb4c94ba8686c8.js
--rw-rw-r--   0 dave      (1000) dave      (1000)    43182 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/lib_index_js.be8adfeb4c94ba8686c8.js.map
--rw-rw-r--   0 dave      (1000) dave      (1000)    51826 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/lib_index_js.da07780875ebcca6f724.js
--rw-rw-r--   0 dave      (1000) dave      (1000)    43302 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/lib_index_js.da07780875ebcca6f724.js.map
--rw-rw-r--   0 dave      (1000) dave      (1000)    30907 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/remoteEntry.039579f90115b8894e5b.js.map
--rw-rw-r--   0 dave      (1000) dave      (1000)    30907 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/remoteEntry.0f4eb7021e3593ac15a3.js.map
--rw-rw-r--   0 dave      (1000) dave      (1000)    30907 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/remoteEntry.19d15a570a871d78efc6.js.map
--rw-rw-r--   0 dave      (1000) dave      (1000)    30907 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/remoteEntry.243c687e7d95ef4458e6.js.map
--rw-rw-r--   0 dave      (1000) dave      (1000)    32044 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/remoteEntry.2b8a915d2ad9bd538465.js
--rw-rw-r--   0 dave      (1000) dave      (1000)    30907 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/remoteEntry.2b8a915d2ad9bd538465.js.map
--rw-rw-r--   0 dave      (1000) dave      (1000)    30907 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/remoteEntry.5189d61f1388667c141e.js.map
--rw-rw-r--   0 dave      (1000) dave      (1000)    30907 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/remoteEntry.53aebe0538286ac00b28.js.map
--rw-rw-r--   0 dave      (1000) dave      (1000)    30907 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/remoteEntry.5f9bcad802b939a44a41.js.map
--rw-rw-r--   0 dave      (1000) dave      (1000)    30907 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/remoteEntry.d1c87f28f231b1c1be3c.js.map
--rw-rw-r--   0 dave      (1000) dave      (1000)      162 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/style.js
--rw-rw-r--   0 dave      (1000) dave      (1000)     4262 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/style_index_js.8151418af089e70dbdcb.js
--rw-rw-r--   0 dave      (1000) dave      (1000)     1429 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/style_index_js.8151418af089e70dbdcb.js.map
--rw-rw-r--   0 dave      (1000) dave      (1000)    12068 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.327a6668b065315cd9b3.js
--rw-rw-r--   0 dave      (1000) dave      (1000)    13805 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.327a6668b065315cd9b3.js.map
--rw-rw-r--   0 dave      (1000) dave      (1000)  8866191 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/vendors-node_modules_phosphor-react_dist_index_esm_js.13b2cfee43c894540916.js
--rw-rw-r--   0 dave      (1000) dave      (1000)  8189849 2023-02-27 05:32:25.000000 oceanumlab-0.4.0/oceanumlab/labextension/static/vendors-node_modules_phosphor-react_dist_index_esm_js.13b2cfee43c894540916.js.map
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-28 20:30:40.289141 oceanumlab-0.4.0/oceanumlab/tests/
--rw-rw-r--   0 dave      (1000) dave      (1000)       40 2022-06-20 01:46:54.000000 oceanumlab-0.4.0/oceanumlab/tests/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      274 2022-06-20 02:32:13.000000 oceanumlab-0.4.0/oceanumlab/tests/test_handlers.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-28 20:30:40.205143 oceanumlab-0.4.0/oceanumlab.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     4980 2023-02-28 20:30:40.000000 oceanumlab-0.4.0/oceanumlab.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     3906 2023-02-28 20:30:40.000000 oceanumlab-0.4.0/oceanumlab.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-02-28 20:30:40.000000 oceanumlab-0.4.0/oceanumlab.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2022-10-19 03:07:19.000000 oceanumlab-0.4.0/oceanumlab.egg-info/not-zip-safe
--rw-rw-r--   0 dave      (1000) dave      (1000)       98 2023-02-28 20:30:40.000000 oceanumlab-0.4.0/oceanumlab.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       11 2023-02-28 20:30:40.000000 oceanumlab-0.4.0/oceanumlab.egg-info/top_level.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)     3872 2023-02-28 20:30:13.000000 oceanumlab-0.4.0/package.json
--rw-rw-r--   0 dave      (1000) dave      (1000)      575 2022-06-20 01:46:54.000000 oceanumlab-0.4.0/pyproject.toml
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-28 20:30:40.289141 oceanumlab-0.4.0/schema/
--rw-rw-r--   0 dave      (1000) dave      (1000)      736 2023-02-27 02:48:20.000000 oceanumlab-0.4.0/schema/plugin.json
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-02-28 20:30:40.309141 oceanumlab-0.4.0/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)     3424 2022-06-20 05:36:28.000000 oceanumlab-0.4.0/setup.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-28 20:30:40.297141 oceanumlab-0.4.0/src/
--rw-rw-r--   0 dave      (1000) dave      (1000)      335 2022-06-20 20:32:03.000000 oceanumlab-0.4.0/src/DatameshUI.tsx
--rw-rw-r--   0 dave      (1000) dave      (1000)    14244 2023-02-27 05:27:57.000000 oceanumlab-0.4.0/src/DatameshWidget.tsx
--rw-rw-r--   0 dave      (1000) dave      (1000)     3434 2022-06-20 22:56:03.000000 oceanumlab-0.4.0/src/DatasourceItem.tsx
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-28 20:30:40.301141 oceanumlab-0.4.0/src/__tests__/
--rw-rw-r--   0 dave      (1000) dave      (1000)      185 2022-06-20 01:46:54.000000 oceanumlab-0.4.0/src/__tests__/oceanumlab.spec.ts
--rw-rw-r--   0 dave      (1000) dave      (1000)     1110 2022-06-20 04:51:20.000000 oceanumlab-0.4.0/src/handler.ts
--rw-rw-r--   0 dave      (1000) dave      (1000)     3990 2023-02-27 05:25:14.000000 oceanumlab-0.4.0/src/index.ts
--rw-rw-r--   0 dave      (1000) dave      (1000)       74 2022-06-20 01:53:54.000000 oceanumlab-0.4.0/src/svg.d.ts
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-28 20:30:40.301141 oceanumlab-0.4.0/style/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2022-06-20 01:57:06.000000 oceanumlab-0.4.0/style/base.css
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-28 20:30:40.305141 oceanumlab-0.4.0/style/icons/
--rw-rw-r--   0 dave      (1000) dave      (1000)     6719 2022-06-20 01:57:06.000000 oceanumlab-0.4.0/style/icons/oceanum.png
--rw-rw-r--   0 dave      (1000) dave      (1000)     5926 2022-06-20 01:57:06.000000 oceanumlab-0.4.0/style/icons/oceanum.svg
--rw-rw-r--   0 dave      (1000) dave      (1000)     2683 2022-06-30 03:37:56.000000 oceanumlab-0.4.0/style/index.css
--rw-rw-r--   0 dave      (1000) dave      (1000)       21 2022-06-20 01:57:06.000000 oceanumlab-0.4.0/style/index.js
--rw-rw-r--   0 dave      (1000) dave      (1000)      561 2022-06-20 04:30:26.000000 oceanumlab-0.4.0/tsconfig.json
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-28 20:30:40.305141 oceanumlab-0.4.0/ui-tests/
--rw-rw-r--   0 dave      (1000) dave      (1000)     3390 2022-06-20 01:46:54.000000 oceanumlab-0.4.0/ui-tests/README.md
--rw-rw-r--   0 dave      (1000) dave      (1000)      609 2022-06-20 01:46:54.000000 oceanumlab-0.4.0/ui-tests/jupyter_server_test_config.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      322 2022-06-20 01:46:54.000000 oceanumlab-0.4.0/ui-tests/package.json
--rw-rw-r--   0 dave      (1000) dave      (1000)      340 2022-06-20 01:46:54.000000 oceanumlab-0.4.0/ui-tests/playwright.config.js
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-28 20:30:40.305141 oceanumlab-0.4.0/ui-tests/tests/
--rw-rw-r--   0 dave      (1000) dave      (1000)      516 2022-06-21 01:27:55.000000 oceanumlab-0.4.0/ui-tests/tests/oceanumlab.spec.ts
--rw-rw-r--   0 dave      (1000) dave      (1000)      192 2022-09-21 01:49:14.000000 oceanumlab-0.4.0/webpack.config.js
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 02:06:28.176727 oceanumlab-0.4.1/
+-rw-rw-r--   0 dave      (1000) dave      (1000)       86 2022-06-20 01:46:54.000000 oceanumlab-0.4.1/CHANGELOG.md
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1515 2022-06-20 01:46:54.000000 oceanumlab-0.4.1/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)      512 2022-06-20 01:46:54.000000 oceanumlab-0.4.1/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4980 2023-06-14 02:06:28.176727 oceanumlab-0.4.1/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3912 2022-06-27 22:21:02.000000 oceanumlab-0.4.1/README.md
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1892 2022-06-20 01:46:54.000000 oceanumlab-0.4.1/RELEASE.md
+-rw-rw-r--   0 dave      (1000) dave      (1000)       68 2022-06-20 01:46:54.000000 oceanumlab-0.4.1/babel.config.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)      197 2022-06-20 01:46:54.000000 oceanumlab-0.4.1/conftest.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      181 2022-06-20 01:46:54.000000 oceanumlab-0.4.1/install.json
+-rw-rw-r--   0 dave      (1000) dave      (1000)      864 2023-03-01 01:19:27.000000 oceanumlab-0.4.1/jest.config.js
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 02:06:28.156727 oceanumlab-0.4.1/jupyter-config/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 02:06:28.160727 oceanumlab-0.4.1/jupyter-config/nb-config/
+-rw-rw-r--   0 dave      (1000) dave      (1000)       87 2022-06-20 01:46:54.000000 oceanumlab-0.4.1/jupyter-config/nb-config/oceanumlab.json
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 02:06:28.160727 oceanumlab-0.4.1/jupyter-config/server-config/
+-rw-rw-r--   0 dave      (1000) dave      (1000)       85 2022-06-20 01:46:54.000000 oceanumlab-0.4.1/jupyter-config/server-config/oceanumlab.json
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 02:06:28.160727 oceanumlab-0.4.1/oceanumlab/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      926 2022-10-19 02:54:28.000000 oceanumlab-0.4.1/oceanumlab/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1044 2023-02-27 02:23:39.000000 oceanumlab-0.4.1/oceanumlab/handlers.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 02:06:28.164727 oceanumlab-0.4.1/oceanumlab/labextension/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      181 2023-06-14 02:06:14.000000 oceanumlab-0.4.1/oceanumlab/labextension/install.json
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4024 2023-06-14 02:06:14.000000 oceanumlab-0.4.1/oceanumlab/labextension/package.json
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 02:06:28.156727 oceanumlab-0.4.1/oceanumlab/labextension/schemas/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 02:06:28.156727 oceanumlab-0.4.1/oceanumlab/labextension/schemas/@oceanum/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 02:06:28.164727 oceanumlab-0.4.1/oceanumlab/labextension/schemas/@oceanum/oceanumlab/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3882 2023-06-14 02:06:14.000000 oceanumlab-0.4.1/oceanumlab/labextension/schemas/@oceanum/oceanumlab/package.json.orig
+-rw-rw-r--   0 dave      (1000) dave      (1000)      736 2023-06-14 02:06:14.000000 oceanumlab-0.4.1/oceanumlab/labextension/schemas/@oceanum/oceanumlab/plugin.json
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 02:06:28.172727 oceanumlab-0.4.1/oceanumlab/labextension/static/
+-rw-rw-r--   0 dave      (1000) dave      (1000)  4131662 2023-06-14 02:06:14.000000 oceanumlab-0.4.1/oceanumlab/labextension/static/490.7bd4977c6b29fa73fa5d.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6199 2023-06-14 02:06:14.000000 oceanumlab-0.4.1/oceanumlab/labextension/static/549.98d9219eb389c3f2404c.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)    21379 2023-06-14 02:06:14.000000 oceanumlab-0.4.1/oceanumlab/labextension/static/746.d3b024e6eae9ee883ccc.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8116 2023-06-14 02:06:14.000000 oceanumlab-0.4.1/oceanumlab/labextension/static/remoteEntry.8438a14f26699b797d74.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)      163 2023-06-14 02:06:14.000000 oceanumlab-0.4.1/oceanumlab/labextension/static/style.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3675 2023-06-14 02:06:14.000000 oceanumlab-0.4.1/oceanumlab/labextension/static/third-party-licenses.json
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 02:06:28.172727 oceanumlab-0.4.1/oceanumlab/tests/
+-rw-rw-r--   0 dave      (1000) dave      (1000)       40 2022-06-20 01:46:54.000000 oceanumlab-0.4.1/oceanumlab/tests/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      284 2023-03-01 04:13:25.000000 oceanumlab-0.4.1/oceanumlab/tests/test_handlers.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 02:06:28.164727 oceanumlab-0.4.1/oceanumlab.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4980 2023-06-14 02:06:28.000000 oceanumlab-0.4.1/oceanumlab.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1457 2023-06-14 02:06:28.000000 oceanumlab-0.4.1/oceanumlab.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-06-14 02:06:28.000000 oceanumlab-0.4.1/oceanumlab.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-06-14 02:06:08.000000 oceanumlab-0.4.1/oceanumlab.egg-info/not-zip-safe
+-rw-rw-r--   0 dave      (1000) dave      (1000)       98 2023-06-14 02:06:28.000000 oceanumlab-0.4.1/oceanumlab.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       11 2023-06-14 02:06:28.000000 oceanumlab-0.4.1/oceanumlab.egg-info/top_level.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3882 2023-06-14 02:05:23.000000 oceanumlab-0.4.1/package.json
+-rw-rw-r--   0 dave      (1000) dave      (1000)      575 2023-03-01 04:06:02.000000 oceanumlab-0.4.1/pyproject.toml
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 02:06:28.172727 oceanumlab-0.4.1/schema/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      736 2023-02-27 02:48:20.000000 oceanumlab-0.4.1/schema/plugin.json
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-06-14 02:06:28.176727 oceanumlab-0.4.1/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3424 2022-06-20 05:36:28.000000 oceanumlab-0.4.1/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 02:06:28.172727 oceanumlab-0.4.1/src/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      335 2022-06-20 20:32:03.000000 oceanumlab-0.4.1/src/DatameshUI.tsx
+-rw-rw-r--   0 dave      (1000) dave      (1000)    14244 2023-02-27 05:27:57.000000 oceanumlab-0.4.1/src/DatameshWidget.tsx
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3434 2022-06-20 22:56:03.000000 oceanumlab-0.4.1/src/DatasourceItem.tsx
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1110 2022-06-20 04:51:20.000000 oceanumlab-0.4.1/src/handler.ts
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3990 2023-03-01 00:04:26.000000 oceanumlab-0.4.1/src/index.ts
+-rw-rw-r--   0 dave      (1000) dave      (1000)       74 2022-06-20 01:53:54.000000 oceanumlab-0.4.1/src/svg.d.ts
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 02:06:28.172727 oceanumlab-0.4.1/style/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 02:06:28.176727 oceanumlab-0.4.1/style/icons/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6719 2022-06-20 01:57:06.000000 oceanumlab-0.4.1/style/icons/oceanum.png
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5926 2022-06-20 01:57:06.000000 oceanumlab-0.4.1/style/icons/oceanum.svg
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2651 2023-02-28 23:48:07.000000 oceanumlab-0.4.1/style/index.css
+-rw-rw-r--   0 dave      (1000) dave      (1000)      874 2023-03-01 00:23:30.000000 oceanumlab-0.4.1/tsconfig.json
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 02:06:28.176727 oceanumlab-0.4.1/ui-tests/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3390 2022-06-20 01:46:54.000000 oceanumlab-0.4.1/ui-tests/README.md
+-rw-rw-r--   0 dave      (1000) dave      (1000)      609 2022-06-20 01:46:54.000000 oceanumlab-0.4.1/ui-tests/jupyter_server_test_config.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      322 2022-06-20 01:46:54.000000 oceanumlab-0.4.1/ui-tests/package.json
+-rw-rw-r--   0 dave      (1000) dave      (1000)      340 2022-06-20 01:46:54.000000 oceanumlab-0.4.1/ui-tests/playwright.config.js
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 02:06:28.176727 oceanumlab-0.4.1/ui-tests/tests/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      516 2022-06-21 01:27:55.000000 oceanumlab-0.4.1/ui-tests/tests/oceanumlab.spec.ts
+-rw-rw-r--   0 dave      (1000) dave      (1000)      190 2023-02-28 22:52:39.000000 oceanumlab-0.4.1/webpack.config.js
```

### Comparing `oceanumlab-0.4.0/LICENSE` & `oceanumlab-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oceanumlab-0.4.0/MANIFEST.in` & `oceanumlab-0.4.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `oceanumlab-0.4.0/PKG-INFO` & `oceanumlab-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oceanumlab
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Jupyterlab extension to interact with the Oceanum.io platform
 Home-page: https://github.com/oceanum-io/oceanumlab
 Author: Oceanum
 Author-email: developers@oceanum.science
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `oceanumlab-0.4.0/README.md` & `oceanumlab-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `oceanumlab-0.4.0/RELEASE.md` & `oceanumlab-0.4.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `oceanumlab-0.4.0/jest.config.js` & `oceanumlab-0.4.1/jest.config.js`

 * *Files identical despite different names*

### Comparing `oceanumlab-0.4.0/oceanumlab/__init__.py` & `oceanumlab-0.4.1/oceanumlab/__init__.py`

 * *Files identical despite different names*

### Comparing `oceanumlab-0.4.0/oceanumlab/handlers.py` & `oceanumlab-0.4.1/oceanumlab/handlers.py`

 * *Files identical despite different names*

### Comparing `oceanumlab-0.4.0/oceanumlab/labextension/package.json` & `oceanumlab-0.4.1/oceanumlab/labextension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.892120610870611%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^3.6.1', '@jupyterlab/coreutils': '^5.6.1', "*

 * *                   "'@jupyterlab/services': '^6.6.1', '@jupyterlab/settingregistry': '^3.6.1', "*

 * *                   "'@jupyterlab/apputils': '3.6.1'}",*

 * * "'devDependencies'": "{'@babel/core': '^7.21.0', '@babel/preset-env': '^7.20.2', "*

 * *                      "'@jupyterlab/builder': '^3.6.1', '@jupyterlab/testutils': '^3.6.1', "*

 * *                      "'@types/jest': '~26.0.0', '@typescript-eslint/eslint-plugin': '^5 […]*

```diff
@@ -3,43 +3,44 @@
         "email": "developers@oceanum.science",
         "name": "Oceanum"
     },
     "bugs": {
         "url": "https://github.com/oceanum-io/oceanumlab/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.1.0",
-        "@jupyterlab/coreutils": "^5.1.0",
-        "@jupyterlab/services": "^6.1.0",
-        "@jupyterlab/settingregistry": "^3.1.0",
+        "@jupyterlab/application": "^3.6.1",
+        "@jupyterlab/apputils": "3.6.1",
+        "@jupyterlab/coreutils": "^5.6.1",
+        "@jupyterlab/services": "^6.6.1",
+        "@jupyterlab/settingregistry": "^3.6.1",
         "phosphor-react": "^1.4.1"
     },
     "description": "A Jupyterlab extension to interact with the Oceanum.io platform",
     "devDependencies": {
-        "@babel/core": "^7.0.0",
-        "@babel/preset-env": "^7.0.0",
-        "@jupyterlab/builder": "^3.1.0",
-        "@jupyterlab/testutils": "^3.0.0",
-        "@types/jest": "^26.0.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^6.15.0",
-        "eslint-plugin-prettier": "^3.1.4",
-        "jest": "^26.0.0",
-        "mkdirp": "^1.0.3",
+        "@babel/core": "^7.21.0",
+        "@babel/preset-env": "^7.20.2",
+        "@jupyterlab/builder": "^3.6.1",
+        "@jupyterlab/testutils": "^3.6.1",
+        "@types/jest": "~26.0.0",
+        "@typescript-eslint/eslint-plugin": "^5.54.0",
+        "@typescript-eslint/parser": "^5.54.0",
+        "eslint": "^8.35.0",
+        "eslint-config-prettier": "^8.6.0",
+        "eslint-plugin-prettier": "^4.2.1",
+        "jest": "~26.0.0",
+        "mkdirp": "^2.1.3",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
-        "stylelint": "^14.3.0",
-        "stylelint-config-prettier": "^9.0.3",
-        "stylelint-config-recommended": "^6.0.0",
-        "stylelint-config-standard": "~24.0.0",
-        "stylelint-prettier": "^2.0.0",
-        "ts-jest": "^26.0.0",
+        "prettier": "^2.8.4",
+        "rimraf": "^4.1.2",
+        "stylelint": "^15.2.0",
+        "stylelint-config-prettier": "^9.0.5",
+        "stylelint-config-recommended": "^10.0.1",
+        "stylelint-config-standard": "~30.0.1",
+        "stylelint-prettier": "^3.0.0",
+        "ts-jest": "^29.0.5",
         "typescript": "4.1.6"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
@@ -54,15 +55,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.2b8a915d2ad9bd538465.js",
+            "load": "static/remoteEntry.8438a14f26699b797d74.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "oceanumlab"
                 },
@@ -91,15 +92,15 @@
         "type": "git",
         "url": "https://github.com/oceanum-io/oceanumlab.git"
     },
     "scripts": {
         "build": "jlpm build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
-        "build:lib": "tsc",
+        "build:lib": "npx tsc",
         "build:prod": "jlpm clean && jlpm build:lib && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
         "clean:labextension": "rimraf oceanumlab/labextension",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
         "eslint": "jlpm eslint:check --fix",
@@ -108,21 +109,19 @@
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
         "prettier": "jlpm prettier:base --write --list-different",
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "jlpm prettier:base --check",
         "stylelint": "jlpm stylelint:check --fix",
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
-        "test": "jest --coverage",
+        "test": "jest --coverage --passWithNoTests",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
-        "watch:src": "tsc -w"
+        "watch:src": "npx tsc -w"
     },
     "sideEffects": [
-        "style/*.css",
-        "style/index.js"
+        "style/*.css"
     ],
     "style": "style/index.css",
-    "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.4"
+    "version": "0.4.0"
 }
```

### Comparing `oceanumlab-0.4.0/oceanumlab/labextension/schemas/@oceanum/oceanumlab/package.json.orig` & `oceanumlab-0.4.1/oceanumlab/labextension/schemas/@oceanum/oceanumlab/package.json.orig`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8924512987012987%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^3.6.1', '@jupyterlab/coreutils': '^5.6.1', "*

 * *                   "'@jupyterlab/services': '^6.6.1', '@jupyterlab/settingregistry': '^3.6.1', "*

 * *                   "'@jupyterlab/apputils': '3.6.1'}",*

 * * "'devDependencies'": "{'@babel/core': '^7.21.0', '@babel/preset-env': '^7.20.2', "*

 * *                      "'@jupyterlab/builder': '^3.6.1', '@jupyterlab/testutils': '^3.6.1', "*

 * *                      "'@types/jest': '~26.0.0', '@typescript-eslint/eslint-plugin': '^5 […]*

```diff
@@ -3,43 +3,44 @@
         "email": "developers@oceanum.science",
         "name": "Oceanum"
     },
     "bugs": {
         "url": "https://github.com/oceanum-io/oceanumlab/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.1.0",
-        "@jupyterlab/coreutils": "^5.1.0",
-        "@jupyterlab/services": "^6.1.0",
-        "@jupyterlab/settingregistry": "^3.1.0",
+        "@jupyterlab/application": "^3.6.1",
+        "@jupyterlab/apputils": "3.6.1",
+        "@jupyterlab/coreutils": "^5.6.1",
+        "@jupyterlab/services": "^6.6.1",
+        "@jupyterlab/settingregistry": "^3.6.1",
         "phosphor-react": "^1.4.1"
     },
     "description": "A Jupyterlab extension to interact with the Oceanum.io platform",
     "devDependencies": {
-        "@babel/core": "^7.0.0",
-        "@babel/preset-env": "^7.0.0",
-        "@jupyterlab/builder": "^3.1.0",
-        "@jupyterlab/testutils": "^3.0.0",
-        "@types/jest": "^26.0.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^6.15.0",
-        "eslint-plugin-prettier": "^3.1.4",
-        "jest": "^26.0.0",
-        "mkdirp": "^1.0.3",
+        "@babel/core": "^7.21.0",
+        "@babel/preset-env": "^7.20.2",
+        "@jupyterlab/builder": "^3.6.1",
+        "@jupyterlab/testutils": "^3.6.1",
+        "@types/jest": "~26.0.0",
+        "@typescript-eslint/eslint-plugin": "^5.54.0",
+        "@typescript-eslint/parser": "^5.54.0",
+        "eslint": "^8.35.0",
+        "eslint-config-prettier": "^8.6.0",
+        "eslint-plugin-prettier": "^4.2.1",
+        "jest": "~26.0.0",
+        "mkdirp": "^2.1.3",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
-        "stylelint": "^14.3.0",
-        "stylelint-config-prettier": "^9.0.3",
-        "stylelint-config-recommended": "^6.0.0",
-        "stylelint-config-standard": "~24.0.0",
-        "stylelint-prettier": "^2.0.0",
-        "ts-jest": "^26.0.0",
+        "prettier": "^2.8.4",
+        "rimraf": "^4.1.2",
+        "stylelint": "^15.2.0",
+        "stylelint-config-prettier": "^9.0.5",
+        "stylelint-config-recommended": "^10.0.1",
+        "stylelint-config-standard": "~30.0.1",
+        "stylelint-prettier": "^3.0.0",
+        "ts-jest": "^29.0.5",
         "typescript": "4.1.6"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
@@ -86,15 +87,15 @@
         "type": "git",
         "url": "https://github.com/oceanum-io/oceanumlab.git"
     },
     "scripts": {
         "build": "jlpm build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
-        "build:lib": "tsc",
+        "build:lib": "npx tsc",
         "build:prod": "jlpm clean && jlpm build:lib && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
         "clean:labextension": "rimraf oceanumlab/labextension",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
         "eslint": "jlpm eslint:check --fix",
@@ -103,21 +104,19 @@
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
         "prettier": "jlpm prettier:base --write --list-different",
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "jlpm prettier:base --check",
         "stylelint": "jlpm stylelint:check --fix",
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
-        "test": "jest --coverage",
+        "test": "jest --coverage --passWithNoTests",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
-        "watch:src": "tsc -w"
+        "watch:src": "npx tsc -w"
     },
     "sideEffects": [
-        "style/*.css",
-        "style/index.js"
+        "style/*.css"
     ],
     "style": "style/index.css",
-    "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.4"
+    "version": "0.4.0"
 }
```

### Comparing `oceanumlab-0.4.0/oceanumlab/labextension/schemas/@oceanum/oceanumlab/plugin.json` & `oceanumlab-0.4.1/oceanumlab/labextension/schemas/@oceanum/oceanumlab/plugin.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965277777777778%*

 * *Differences: {"'properties'": "{'datameshToken': {'description': 'Enter your Datamesh token here. You can "*

 * *                 'obtain this at https://home.oceanum.io/account. You will need to reset your '*

 * *                 "kernel after changing this setting.'}, 'injectToken': {'description': 'Inject "*

 * *                 "Datamesh token into code.'}}"}*

```diff
@@ -4,21 +4,21 @@
     "icon": "oceanum",
     "jupyter.lab.setting-icon": "oceanum:main",
     "jupyter.lab.setting-icon-label": "Oceanum",
     "jupyter.lab.shortcuts": [],
     "properties": {
         "datameshToken": {
             "default": "",
-            "description": "Enter your Datamesh token here. You can obtain this at https://home.oceanum.io/account",
+            "description": "Enter your Datamesh token here. You can obtain this at https://home.oceanum.io/account. You will need to reset your kernel after changing this setting.",
             "title": "Datamesh token",
             "type": "string"
         },
         "injectToken": {
             "default": false,
-            "description": "Inject Datamesh token into code",
+            "description": "Inject Datamesh token into code.",
             "title": "Inject token",
             "type": "boolean"
         }
     },
     "title": "Oceanum.io",
     "type": "object"
 }
```

### Comparing `oceanumlab-0.4.0/oceanumlab.egg-info/PKG-INFO` & `oceanumlab-0.4.1/oceanumlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oceanumlab
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Jupyterlab extension to interact with the Oceanum.io platform
 Home-page: https://github.com/oceanum-io/oceanumlab
 Author: Oceanum
 Author-email: developers@oceanum.science
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `oceanumlab-0.4.0/package.json` & `oceanumlab-0.4.1/package.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8924512987012987%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^3.6.1', '@jupyterlab/coreutils': '^5.6.1', "*

 * *                   "'@jupyterlab/services': '^6.6.1', '@jupyterlab/settingregistry': '^3.6.1', "*

 * *                   "'@jupyterlab/apputils': '3.6.1'}",*

 * * "'devDependencies'": "{'@babel/core': '^7.21.0', '@babel/preset-env': '^7.20.2', "*

 * *                      "'@jupyterlab/builder': '^3.6.1', '@jupyterlab/testutils': '^3.6.1', "*

 * *                      "'@types/jest': '~26.0.0', '@typescript-eslint/eslint-plugin': '^5 […]*

```diff
@@ -3,43 +3,44 @@
         "email": "developers@oceanum.science",
         "name": "Oceanum"
     },
     "bugs": {
         "url": "https://github.com/oceanum-io/oceanumlab/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.1.0",
-        "@jupyterlab/coreutils": "^5.1.0",
-        "@jupyterlab/services": "^6.1.0",
-        "@jupyterlab/settingregistry": "^3.1.0",
+        "@jupyterlab/application": "^3.6.1",
+        "@jupyterlab/apputils": "3.6.1",
+        "@jupyterlab/coreutils": "^5.6.1",
+        "@jupyterlab/services": "^6.6.1",
+        "@jupyterlab/settingregistry": "^3.6.1",
         "phosphor-react": "^1.4.1"
     },
     "description": "A Jupyterlab extension to interact with the Oceanum.io platform",
     "devDependencies": {
-        "@babel/core": "^7.0.0",
-        "@babel/preset-env": "^7.0.0",
-        "@jupyterlab/builder": "^3.1.0",
-        "@jupyterlab/testutils": "^3.0.0",
-        "@types/jest": "^26.0.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^6.15.0",
-        "eslint-plugin-prettier": "^3.1.4",
-        "jest": "^26.0.0",
-        "mkdirp": "^1.0.3",
+        "@babel/core": "^7.21.0",
+        "@babel/preset-env": "^7.20.2",
+        "@jupyterlab/builder": "^3.6.1",
+        "@jupyterlab/testutils": "^3.6.1",
+        "@types/jest": "~26.0.0",
+        "@typescript-eslint/eslint-plugin": "^5.54.0",
+        "@typescript-eslint/parser": "^5.54.0",
+        "eslint": "^8.35.0",
+        "eslint-config-prettier": "^8.6.0",
+        "eslint-plugin-prettier": "^4.2.1",
+        "jest": "~26.0.0",
+        "mkdirp": "^2.1.3",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
-        "stylelint": "^14.3.0",
-        "stylelint-config-prettier": "^9.0.3",
-        "stylelint-config-recommended": "^6.0.0",
-        "stylelint-config-standard": "~24.0.0",
-        "stylelint-prettier": "^2.0.0",
-        "ts-jest": "^26.0.0",
+        "prettier": "^2.8.4",
+        "rimraf": "^4.1.2",
+        "stylelint": "^15.2.0",
+        "stylelint-config-prettier": "^9.0.5",
+        "stylelint-config-recommended": "^10.0.1",
+        "stylelint-config-standard": "~30.0.1",
+        "stylelint-prettier": "^3.0.0",
+        "ts-jest": "^29.0.5",
         "typescript": "4.1.6"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
@@ -86,15 +87,15 @@
         "type": "git",
         "url": "https://github.com/oceanum-io/oceanumlab.git"
     },
     "scripts": {
         "build": "jlpm build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
-        "build:lib": "tsc",
+        "build:lib": "npx tsc",
         "build:prod": "jlpm clean && jlpm build:lib && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
         "clean:labextension": "rimraf oceanumlab/labextension",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
         "eslint": "jlpm eslint:check --fix",
@@ -103,21 +104,19 @@
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
         "prettier": "jlpm prettier:base --write --list-different",
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "jlpm prettier:base --check",
         "stylelint": "jlpm stylelint:check --fix",
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
-        "test": "jest --coverage",
+        "test": "jest --coverage --passWithNoTests",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
-        "watch:src": "tsc -w"
+        "watch:src": "npx tsc -w"
     },
     "sideEffects": [
-        "style/*.css",
-        "style/index.js"
+        "style/*.css"
     ],
     "style": "style/index.css",
-    "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.4.0"
+    "version": "0.4.1"
 }
```

### Comparing `oceanumlab-0.4.0/pyproject.toml` & `oceanumlab-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["jupyter_packaging~=0.10,<2", "jupyterlab~=3.1"]
+requires = ["jupyter_packaging~=0.10,<2", "jupyterlab>=3.1"]
 build-backend = "jupyter_packaging.build_api"
 
 [tool.jupyter-packaging.options]
 skip-if-exists = ["oceanumlab/labextension/static/style.js"]
 ensured-targets = ["oceanumlab/labextension/static/style.js", "oceanumlab/labextension/package.json"]
 
 [tool.jupyter-packaging.builder]
```

### Comparing `oceanumlab-0.4.0/schema/plugin.json` & `oceanumlab-0.4.1/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `oceanumlab-0.4.0/setup.py` & `oceanumlab-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `oceanumlab-0.4.0/src/DatameshWidget.tsx` & `oceanumlab-0.4.1/src/DatameshWidget.tsx`

 * *Files identical despite different names*

### Comparing `oceanumlab-0.4.0/src/DatasourceItem.tsx` & `oceanumlab-0.4.1/src/DatasourceItem.tsx`

 * *Files identical despite different names*

### Comparing `oceanumlab-0.4.0/src/handler.ts` & `oceanumlab-0.4.1/src/handler.ts`

 * *Files identical despite different names*

### Comparing `oceanumlab-0.4.0/src/index.ts` & `oceanumlab-0.4.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `oceanumlab-0.4.0/style/icons/oceanum.png` & `oceanumlab-0.4.1/style/icons/oceanum.png`

 * *Files identical despite different names*

### Comparing `oceanumlab-0.4.0/style/icons/oceanum.svg` & `oceanumlab-0.4.1/style/icons/oceanum.svg`

 * *Files identical despite different names*

### Comparing `oceanumlab-0.4.0/style/index.css` & `oceanumlab-0.4.1/style/index.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-@import url('base.css');
-
 .datasource-drag-image {
   border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
   width: var(--jp-private-notebook-dragImage-width);
   height: var(--jp-private-notebook-dragImage-height);
   color: var(--jp-ui-font-color1);
   background: var(--jp-layout-color1);
 }
@@ -57,16 +55,16 @@
 
 .datamesh-workspace-name {
   flex: 0 0 auto;
   font-weight: 600;
   text-transform: uppercase;
   letter-spacing: 1px;
   padding: 8px 8px 8px 12px;
-  margin: 0px;
-  margin-left: 0px;
+  margin: 0;
+  margin-left: 0;
   margin-bottom: 10px;
   font-size: var(--jp-ui-font-size1);
 }
 
 .datasource-item-expand,
 .datasource-item-action,
 .datasource-item-expand.jp-mod-styled {
@@ -101,34 +99,34 @@
   display: inline-flex;
   align-self: flex-end;
   align-items: center;
   height: 100%;
   border: none;
 }
 
-.datasource-item-action:hover,
-.datasource-item-name:hover {
-  cursor: pointer;
-}
-
 .datasource-item-name {
   flex-grow: 1;
   font-size: var(--jp-ui-font-size1);
   white-space: nowrap;
   overflow: hidden;
   text-overflow: ellipsis;
   padding: 4px 0 4px 2px;
   line-height: 28px;
 }
 
+.datasource-item-action:hover,
+.datasource-item-name:hover {
+  cursor: pointer;
+}
+
 .datasource-item-title {
   align-items: center;
   display: flex;
   flex-direction: row;
-  padding: 0px 4px;
+  padding: 0 4px;
   height: 36px;
 }
 
 .datasource-item-title:hover {
   background-color: var(--jp-layout-color2);
 }
```

### Comparing `oceanumlab-0.4.0/ui-tests/README.md` & `oceanumlab-0.4.1/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `oceanumlab-0.4.0/ui-tests/jupyter_server_test_config.py` & `oceanumlab-0.4.1/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `oceanumlab-0.4.0/ui-tests/tests/oceanumlab.spec.ts` & `oceanumlab-0.4.1/ui-tests/tests/oceanumlab.spec.ts`

 * *Files identical despite different names*

