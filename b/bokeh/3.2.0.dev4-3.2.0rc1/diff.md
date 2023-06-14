# Comparing `tmp/bokeh-3.2.0.dev4.tar.gz` & `tmp/bokeh-3.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bokeh-3.2.0.dev4.tar", last modified: Fri Jun  9 10:33:29 2023, max compression
+gzip compressed data, was "bokeh-3.2.0rc1.tar", last modified: Wed Jun 14 19:44:22 2023, max compression
```

## Comparing `bokeh-3.2.0.dev4.tar` & `bokeh-3.2.0rc1.tar`

### file list

```diff
@@ -1,1205 +1,1205 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:29.010450 bokeh-3.2.0.dev4/
--rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-06-09 10:22:42.000000 bokeh-3.2.0.dev4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      881 2023-06-09 10:22:42.000000 bokeh-3.2.0.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    12082 2023-06-09 10:33:29.010450 bokeh-3.2.0.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8603 2023-06-09 10:22:42.000000 bokeh-3.2.0.dev4/README.md
--rw-r--r--   0 runner    (1001) docker     (122)    10430 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 10:33:29.010450 bokeh-3.2.0.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     6745 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.822447 bokeh-3.2.0.dev4/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.834447 bokeh-3.2.0.dev4/src/bokeh/
--rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3750 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2136 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    73110 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/_sri.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.834447 bokeh-3.2.0.dev4/src/bokeh/application/
--rw-r--r--   0 runner    (1001) docker     (122)     2145 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11549 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/application.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.838447 bokeh-3.2.0.dev4/src/bokeh/application/handlers/
--rw-r--r--   0 runner    (1001) docker     (122)     2194 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6919 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/code.py
--rw-r--r--   0 runner    (1001) docker     (122)     7818 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/code_runner.py
--rw-r--r--   0 runner    (1001) docker     (122)    10926 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/directory.py
--rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/document_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (122)     4943 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/function.py
--rw-r--r--   0 runner    (1001) docker     (122)     7975 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     4705 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (122)     5180 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/notebook.py
--rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     3348 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/script.py
--rw-r--r--   0 runner    (1001) docker     (122)     5035 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/server_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (122)     4339 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/server_request_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.838447 bokeh-3.2.0.dev4/src/bokeh/client/
--rw-r--r--   0 runner    (1001) docker     (122)     2373 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16199 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (122)    21727 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/client/session.py
--rw-r--r--   0 runner    (1001) docker     (122)     5334 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/client/states.py
--rw-r--r--   0 runner    (1001) docker     (122)     3299 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/client/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     3252 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/client/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.838447 bokeh-3.2.0.dev4/src/bokeh/colors/
--rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14039 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/colors/color.py
--rw-r--r--   0 runner    (1001) docker     (122)     9825 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/colors/groups.py
--rw-r--r--   0 runner    (1001) docker     (122)    13046 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/colors/named.py
--rw-r--r--   0 runner    (1001) docker     (122)     5432 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/colors/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.838447 bokeh-3.2.0.dev4/src/bokeh/command/
--rw-r--r--   0 runner    (1001) docker     (122)      901 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3965 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (122)     5822 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/subcommand.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.838447 bokeh-3.2.0.dev4/src/bokeh/command/subcommands/
--rw-r--r--   0 runner    (1001) docker     (122)     2802 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2567 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/subcommands/build.py
--rw-r--r--   0 runner    (1001) docker     (122)     7336 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/subcommands/file_output.py
--rw-r--r--   0 runner    (1001) docker     (122)     4658 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/subcommands/info.py
--rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/subcommands/init.py
--rw-r--r--   0 runner    (1001) docker     (122)     3592 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/subcommands/json.py
--rw-r--r--   0 runner    (1001) docker     (122)     2564 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/subcommands/sampledata.py
--rw-r--r--   0 runner    (1001) docker     (122)     2775 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/subcommands/secret.py
--rw-r--r--   0 runner    (1001) docker     (122)    37703 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/subcommands/serve.py
--rw-r--r--   0 runner    (1001) docker     (122)     3764 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/subcommands/static.py
--rw-r--r--   0 runner    (1001) docker     (122)     7996 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.842447 bokeh-3.2.0.dev4/src/bokeh/core/
--rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.842447 bokeh-3.2.0.dev4/src/bokeh/core/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/autoload_js.js
--rw-r--r--   0 runner    (1001) docker     (122)     6450 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/autoload_nb_js.js
--rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/autoload_request_tag.html
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/autoload_tag.html
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/css_resources.html
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/doc_js.js
--rw-r--r--   0 runner    (1001) docker     (122)      213 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/doc_nb_js.js
--rw-r--r--   0 runner    (1001) docker     (122)     1634 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/file.html
--rw-r--r--   0 runner    (1001) docker     (122)      586 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/js_resources.html
--rw-r--r--   0 runner    (1001) docker     (122)      158 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/macros.html
--rw-r--r--   0 runner    (1001) docker     (122)     3933 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/notebook_load.html
--rw-r--r--   0 runner    (1001) docker     (122)      356 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/plot_div.html
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/root_div.html
--rw-r--r--   0 runner    (1001) docker     (122)      260 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/script_tag.html
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/try_run.js
--rw-r--r--   0 runner    (1001) docker     (122)    16751 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)    29845 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/has_props.py
--rw-r--r--   0 runner    (1001) docker     (122)     7133 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (122)    11533 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/properties.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.846447 bokeh-3.2.0.dev4/src/bokeh/core/property/
--rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2782 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/_sphinx.py
--rw-r--r--   0 runner    (1001) docker     (122)     3646 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/alias.py
--rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/aliases.py
--rw-r--r--   0 runner    (1001) docker     (122)     3156 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/any.py
--rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/auto.py
--rw-r--r--   0 runner    (1001) docker     (122)    20064 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/bases.py
--rw-r--r--   0 runner    (1001) docker     (122)     6436 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/color.py
--rw-r--r--   0 runner    (1001) docker     (122)    12052 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/container.py
--rw-r--r--   0 runner    (1001) docker     (122)    22696 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/dataspec.py
--rw-r--r--   0 runner    (1001) docker     (122)     6091 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/datetime.py
--rw-r--r--   0 runner    (1001) docker     (122)     5123 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/descriptor_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    35217 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/either.py
--rw-r--r--   0 runner    (1001) docker     (122)     3989 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/enum.py
--rw-r--r--   0 runner    (1001) docker     (122)     3021 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/factors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2879 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/include.py
--rw-r--r--   0 runner    (1001) docker     (122)     6521 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/instance.py
--rw-r--r--   0 runner    (1001) docker     (122)     2743 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/json.py
--rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/nothing.py
--rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/nullable.py
--rw-r--r--   0 runner    (1001) docker     (122)     9631 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/numeric.py
--rw-r--r--   0 runner    (1001) docker     (122)     3458 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/override.py
--rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/pd.py
--rw-r--r--   0 runner    (1001) docker     (122)     7166 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/primitive.py
--rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/readonly.py
--rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/required.py
--rw-r--r--   0 runner    (1001) docker     (122)     2536 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/serialized.py
--rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/singletons.py
--rw-r--r--   0 runner    (1001) docker     (122)     3465 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/string.py
--rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     2481 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/text_like.py
--rw-r--r--   0 runner    (1001) docker     (122)     3378 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/validation.py
--rw-r--r--   0 runner    (1001) docker     (122)     5977 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/vectorization.py
--rw-r--r--   0 runner    (1001) docker     (122)     8905 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/visual.py
--rw-r--r--   0 runner    (1001) docker     (122)    17517 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property_aliases.py
--rw-r--r--   0 runner    (1001) docker     (122)    12260 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property_mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)    10171 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/query.py
--rw-r--r--   0 runner    (1001) docker     (122)    23292 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/serialization.py
--rw-r--r--   0 runner    (1001) docker     (122)     4892 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     3025 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.850448 bokeh-3.2.0.dev4/src/bokeh/core/validation/
--rw-r--r--   0 runner    (1001) docker     (122)     3502 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7168 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/validation/check.py
--rw-r--r--   0 runner    (1001) docker     (122)     6555 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/validation/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     9259 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/validation/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2983 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/validation/issue.py
--rw-r--r--   0 runner    (1001) docker     (122)     3082 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/validation/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.850448 bokeh-3.2.0.dev4/src/bokeh/document/
--rw-r--r--   0 runner    (1001) docker     (122)     2435 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16657 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/document/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)    27922 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/document/document.py
--rw-r--r--   0 runner    (1001) docker     (122)    29934 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/document/events.py
--rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/document/json.py
--rw-r--r--   0 runner    (1001) docker     (122)     4978 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/document/locking.py
--rw-r--r--   0 runner    (1001) docker     (122)     9341 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/document/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     5026 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/document/modules.py
--rw-r--r--   0 runner    (1001) docker     (122)     6344 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/driving.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.850448 bokeh-3.2.0.dev4/src/bokeh/embed/
--rw-r--r--   0 runner    (1001) docker     (122)     2074 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/embed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14666 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/embed/bundle.py
--rw-r--r--   0 runner    (1001) docker     (122)     6464 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/embed/elements.py
--rw-r--r--   0 runner    (1001) docker     (122)     3968 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/embed/notebook.py
--rw-r--r--   0 runner    (1001) docker     (122)    12506 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/embed/server.py
--rw-r--r--   0 runner    (1001) docker     (122)    17807 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/embed/standalone.py
--rw-r--r--   0 runner    (1001) docker     (122)    14837 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/embed/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/embed/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (122)    23182 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/events.py
--rw-r--r--   0 runner    (1001) docker     (122)     3844 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.854447 bokeh-3.2.0.dev4/src/bokeh/io/
--rw-r--r--   0 runner    (1001) docker     (122)     2208 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3375 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/io/doc.py
--rw-r--r--   0 runner    (1001) docker     (122)    19390 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/io/export.py
--rw-r--r--   0 runner    (1001) docker     (122)    21518 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/io/notebook.py
--rw-r--r--   0 runner    (1001) docker     (122)     5047 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/io/output.py
--rw-r--r--   0 runner    (1001) docker     (122)     6261 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/io/saving.py
--rw-r--r--   0 runner    (1001) docker     (122)     8278 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/io/showing.py
--rw-r--r--   0 runner    (1001) docker     (122)     8360 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/io/state.py
--rw-r--r--   0 runner    (1001) docker     (122)     4155 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/io/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     6093 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/io/webdriver.py
--rw-r--r--   0 runner    (1001) docker     (122)    23032 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/layouts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.854447 bokeh-3.2.0.dev4/src/bokeh/model/
--rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/model/data_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     4140 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/model/docs.py
--rw-r--r--   0 runner    (1001) docker     (122)    21302 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/model/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     7839 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/model/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.858448 bokeh-3.2.0.dev4/src/bokeh/models/
--rw-r--r--   0 runner    (1001) docker     (122)     4057 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.858448 bokeh-3.2.0.dev4/src/bokeh/models/annotations/
--rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/annotations/annotation.py
--rw-r--r--   0 runner    (1001) docker     (122)     5564 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/annotations/arrows.py
--rw-r--r--   0 runner    (1001) docker     (122)    13775 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/annotations/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.858448 bokeh-3.2.0.dev4/src/bokeh/models/annotations/html/
--rw-r--r--   0 runner    (1001) docker     (122)     1950 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/annotations/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2265 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/annotations/html/html_annotation.py
--rw-r--r--   0 runner    (1001) docker     (122)    10444 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/annotations/html/labels.py
--rw-r--r--   0 runner    (1001) docker     (122)     2093 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/annotations/html/toolbars.py
--rw-r--r--   0 runner    (1001) docker     (122)     9340 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/annotations/labels.py
--rw-r--r--   0 runner    (1001) docker     (122)    16806 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/annotations/legends.py
--rw-r--r--   0 runner    (1001) docker     (122)    12456 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/axes.py
--rw-r--r--   0 runner    (1001) docker     (122)     7795 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)     2363 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/canvas.py
--rw-r--r--   0 runner    (1001) docker     (122)     3154 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (122)    16739 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/css.py
--rw-r--r--   0 runner    (1001) docker     (122)     6881 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/dom.py
--rw-r--r--   0 runner    (1001) docker     (122)     9495 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/expressions.py
--rw-r--r--   0 runner    (1001) docker     (122)     8487 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)    24509 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/formatters.py
--rw-r--r--   0 runner    (1001) docker     (122)     4197 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/glyph.py
--rw-r--r--   0 runner    (1001) docker     (122)    54279 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/glyphs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/graphics.py
--rw-r--r--   0 runner    (1001) docker     (122)     6435 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/graphs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4263 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/grids.py
--rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/labeling.py
--rw-r--r--   0 runner    (1001) docker     (122)    23128 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/layouts.py
--rw-r--r--   0 runner    (1001) docker     (122)     7304 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/map_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)    12636 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/mappers.py
--rw-r--r--   0 runner    (1001) docker     (122)    33674 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/plots.py
--rw-r--r--   0 runner    (1001) docker     (122)    17571 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/ranges.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.858448 bokeh-3.2.0.dev4/src/bokeh/models/renderers/
--rw-r--r--   0 runner    (1001) docker     (122)     2101 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4996 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/renderers/contour_renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)     8796 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/renderers/glyph_renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/renderers/graph_renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)     4219 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/renderers/renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2613 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/renderers/tile_renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3815 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/scales.py
--rw-r--r--   0 runner    (1001) docker     (122)     4923 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/selections.py
--rw-r--r--   0 runner    (1001) docker     (122)     3711 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/selectors.py
--rw-r--r--   0 runner    (1001) docker     (122)    33223 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/sources.py
--rw-r--r--   0 runner    (1001) docker     (122)     4673 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/text.py
--rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/textures.py
--rw-r--r--   0 runner    (1001) docker     (122)    11476 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/tickers.py
--rw-r--r--   0 runner    (1001) docker     (122)     6596 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/tiles.py
--rw-r--r--   0 runner    (1001) docker     (122)    73516 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/tools.py
--rw-r--r--   0 runner    (1001) docker     (122)     9422 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.862448 bokeh-3.2.0.dev4/src/bokeh/models/ui/
--rw-r--r--   0 runner    (1001) docker     (122)     2153 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2548 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/ui/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2275 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/ui/examiner.py
--rw-r--r--   0 runner    (1001) docker     (122)     4930 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/ui/icons.py
--rw-r--r--   0 runner    (1001) docker     (122)     3706 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/ui/menus.py
--rw-r--r--   0 runner    (1001) docker     (122)     2095 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/ui/panes.py
--rw-r--r--   0 runner    (1001) docker     (122)     3913 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/ui/tooltips.py
--rw-r--r--   0 runner    (1001) docker     (122)     3068 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/ui/ui_element.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.862448 bokeh-3.2.0.dev4/src/bokeh/models/util/
--rw-r--r--   0 runner    (1001) docker     (122)      876 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12432 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/util/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.862448 bokeh-3.2.0.dev4/src/bokeh/models/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7089 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/widgets/buttons.py
--rw-r--r--   0 runner    (1001) docker     (122)     4612 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/widgets/groups.py
--rw-r--r--   0 runner    (1001) docker     (122)    16135 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/widgets/inputs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4680 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/widgets/markups.py
--rw-r--r--   0 runner    (1001) docker     (122)    11229 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/widgets/pickers.py
--rw-r--r--   0 runner    (1001) docker     (122)    10242 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/widgets/sliders.py
--rw-r--r--   0 runner    (1001) docker     (122)    28151 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/widgets/tables.py
--rw-r--r--   0 runner    (1001) docker     (122)     2429 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/widgets/widget.py
--rw-r--r--   0 runner    (1001) docker     (122)   113099 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/palettes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.862448 bokeh-3.2.0.dev4/src/bokeh/plotting/
--rw-r--r--   0 runner    (1001) docker     (122)     2533 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3921 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     8267 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/_docstring.py
--rw-r--r--   0 runner    (1001) docker     (122)    32388 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/_figure.py
--rw-r--r--   0 runner    (1001) docker     (122)     6603 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/_graph.py
--rw-r--r--   0 runner    (1001) docker     (122)     5002 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/_legends.py
--rw-r--r--   0 runner    (1001) docker     (122)     6567 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/_plot.py
--rw-r--r--   0 runner    (1001) docker     (122)    12625 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/_renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3813 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/_stack.py
--rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/_tools.py
--rw-r--r--   0 runner    (1001) docker     (122)    14637 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/contour.py
--rw-r--r--   0 runner    (1001) docker     (122)    27693 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/glyph_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     4939 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/gmap.py
--rw-r--r--   0 runner    (1001) docker     (122)     5836 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.866448 bokeh-3.2.0.dev4/src/bokeh/protocol/
--rw-r--r--   0 runner    (1001) docker     (122)     5428 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2485 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    11813 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/message.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.866448 bokeh-3.2.0.dev4/src/bokeh/protocol/messages/
--rw-r--r--   0 runner    (1001) docker     (122)     2138 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/messages/ack.py
--rw-r--r--   0 runner    (1001) docker     (122)     3307 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/messages/error.py
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/messages/ok.py
--rw-r--r--   0 runner    (1001) docker     (122)     3754 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/messages/patch_doc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3176 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/messages/pull_doc_reply.py
--rw-r--r--   0 runner    (1001) docker     (122)     2334 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/messages/pull_doc_req.py
--rw-r--r--   0 runner    (1001) docker     (122)     2799 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/messages/push_doc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3072 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/messages/server_info_reply.py
--rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/messages/server_info_req.py
--rw-r--r--   0 runner    (1001) docker     (122)     6987 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/receiver.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    24107 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.870448 bokeh-3.2.0.dev4/src/bokeh/sampledata/
--rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.874448 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/
--rw-r--r--   0 runner    (1001) docker     (122)    79935 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/USHolidays.ics
--rw-r--r--   0 runner    (1001) docker     (122)   106201 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/US_Regions_State_Boundaries.csv.gz
--rw-r--r--   0 runner    (1001) docker     (122)    17444 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/auto-mpg.csv
--rw-r--r--   0 runner    (1001) docker     (122)    17345 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/auto-mpg2.csv
--rw-r--r--   0 runner    (1001) docker     (122)     2296 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/browsers_nov_2013.csv
--rw-r--r--   0 runner    (1001) docker     (122)    25491 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/commits.txt.gz
--rw-r--r--   0 runner    (1001) docker     (122)    11342 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/daylight_warsaw_2013.csv
--rw-r--r--   0 runner    (1001) docker     (122)    14487 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/elements.csv
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.874448 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/icons/
--rw-r--r--   0 runner    (1001) docker     (122)     1985 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/icons/chrome_32x32.png
--rw-r--r--   0 runner    (1001) docker     (122)     2443 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/icons/firefox_32x32.png
--rw-r--r--   0 runner    (1001) docker     (122)     2293 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/icons/ie_32x32.png
--rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/icons/opera_32x32.png
--rw-r--r--   0 runner    (1001) docker     (122)     2552 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/icons/safari_32x32.png
--rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/iris.csv
--rw-r--r--   0 runner    (1001) docker     (122)    11536 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/les_mis.json
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/numberly.csv
--rw-r--r--   0 runner    (1001) docker     (122)    33264 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/obiszow_mtb_xcm.csv
--rw-r--r--   0 runner    (1001) docker     (122)     8630 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/olympics2014.json
--rw-r--r--   0 runner    (1001) docker     (122)    13478 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/penguins.csv
--rw-r--r--   0 runner    (1001) docker     (122)     5682 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/percent-bachelors-degrees-women-usa.csv
--rw-r--r--   0 runner    (1001) docker     (122)     2465 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/probly.csv
--rw-r--r--   0 runner    (1001) docker     (122)    14494 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/sample_geojson.geojson
--rw-r--r--   0 runner    (1001) docker     (122)    76453 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/sea_surface_temperature.csv.gz
--rw-r--r--   0 runner    (1001) docker     (122)     5332 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/sprint.csv
--rw-r--r--   0 runner    (1001) docker     (122)     4003 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/unemployment1948.csv
--rw-r--r--   0 runner    (1001) docker     (122)     5387 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/us_marriages_divorces.csv
--rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/airport_routes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2761 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/airports.py
--rw-r--r--   0 runner    (1001) docker     (122)     3122 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/anscombe.py
--rw-r--r--   0 runner    (1001) docker     (122)     3780 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/antibiotics.py
--rw-r--r--   0 runner    (1001) docker     (122)     3038 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/autompg.py
--rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/autompg2.py
--rw-r--r--   0 runner    (1001) docker     (122)     3112 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/browsers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/commits.py
--rw-r--r--   0 runner    (1001) docker     (122)     2648 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/daylight.py
--rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/degrees.py
--rw-r--r--   0 runner    (1001) docker     (122)     4599 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/gapminder.py
--rw-r--r--   0 runner    (1001) docker     (122)     2022 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/glucose.py
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/haar_cascade.py
--rw-r--r--   0 runner    (1001) docker     (122)     2371 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/iris.py
--rw-r--r--   0 runner    (1001) docker     (122)     2367 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/les_mis.py
--rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/movies_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2096 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/mtb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2224 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/olympics2014.py
--rw-r--r--   0 runner    (1001) docker     (122)     2212 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/penguins.py
--rw-r--r--   0 runner    (1001) docker     (122)     2270 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/perceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2041 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/periodic_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     2548 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/population.py
--rw-r--r--   0 runner    (1001) docker     (122)     2071 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/sample_geojson.py
--rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/sample_superstore.py
--rw-r--r--   0 runner    (1001) docker     (122)     2706 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/sea_surface_temperature.py
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/sprint.py
--rw-r--r--   0 runner    (1001) docker     (122)     3520 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/stocks.py
--rw-r--r--   0 runner    (1001) docker     (122)     2777 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/unemployment.py
--rw-r--r--   0 runner    (1001) docker     (122)     2099 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/unemployment1948.py
--rw-r--r--   0 runner    (1001) docker     (122)     2116 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/us_cities.py
--rw-r--r--   0 runner    (1001) docker     (122)     4032 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/us_counties.py
--rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/us_holidays.py
--rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/us_marriages_divorces.py
--rw-r--r--   0 runner    (1001) docker     (122)     3703 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/us_states.py
--rw-r--r--   0 runner    (1001) docker     (122)     2132 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/world_cities.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.874448 bokeh-3.2.0.dev4/src/bokeh/server/
--rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9579 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/auth_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)     6721 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)     3939 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/connection.py
--rw-r--r--   0 runner    (1001) docker     (122)    14606 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/contexts.py
--rw-r--r--   0 runner    (1001) docker     (122)     4096 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/protocol_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)    20849 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/server.py
--rw-r--r--   0 runner    (1001) docker     (122)    11852 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/session.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.830447 bokeh-3.2.0.dev4/src/bokeh/server/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.890448 bokeh-3.2.0.dev4/src/bokeh/server/static/js/
--rw-r--r--   0 runner    (1001) docker     (122)   211364 2023-06-09 10:32:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-api.js
--rw-r--r--   0 runner    (1001) docker     (122)   118620 2023-06-09 10:32:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-api.min.js
--rw-r--r--   0 runner    (1001) docker     (122)   535981 2023-06-09 10:32:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-gl.js
--rw-r--r--   0 runner    (1001) docker     (122)   198524 2023-06-09 10:32:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-gl.min.js
--rw-r--r--   0 runner    (1001) docker     (122)  2750420 2023-06-09 10:32:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-mathjax.js
--rw-r--r--   0 runner    (1001) docker     (122)  1785923 2023-06-09 10:32:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-mathjax.min.js
--rw-r--r--   0 runner    (1001) docker     (122)   949247 2023-06-09 10:32:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-tables.js
--rw-r--r--   0 runner    (1001) docker     (122)   302599 2023-06-09 10:32:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-tables.min.js
--rw-r--r--   0 runner    (1001) docker     (122)   799629 2023-06-09 10:32:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-widgets.js
--rw-r--r--   0 runner    (1001) docker     (122)   301352 2023-06-09 10:32:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-widgets.min.js
--rw-r--r--   0 runner    (1001) docker     (122)  2257234 2023-06-09 10:32:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh.js
--rw-r--r--   0 runner    (1001) docker     (122)   959268 2023-06-09 10:32:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh.min.js
--rw-r--r--   0 runner    (1001) docker     (122) 20427534 2023-06-09 10:32:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/compiler.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.914449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.914449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/
--rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/charts.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      508 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/expr.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4471 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/figure.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    19794 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/glyph_api.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/gridplot.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      448 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      739 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/io.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3346 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/linalg.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/main.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/models.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    63941 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/palettes.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     5394 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/parser.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      206 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/plotting.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/themes.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/base.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      260 2023-06-09 10:31:49.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/bokeh.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.914449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/client/
--rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/client/connection.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1106 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/client/session.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.918449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/
--rw-r--r--   0 runner    (1001) docker     (122)     5846 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/bokeh_events.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      820 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/build_views.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      274 2023-06-09 10:31:32.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/class.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    42976 2023-06-09 10:31:34.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      334 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/diagnostics.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     5953 2023-06-09 10:31:34.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/dom.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/dom_view.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    11975 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/enums.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/geometry.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3638 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/graphics.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     5113 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/has_props.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      966 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/hittest.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     8908 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/kinds.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.918449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/alignments.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/border.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3050 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/grid.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      321 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/layoutable.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/side_panel.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1595 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/types.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/logging.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      861 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/patching.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     9618 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/properties.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     6764 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/property_mixins.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/resolvers.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/selection_manager.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.918449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/serialization/
--rw-r--r--   0 runner    (1001) docker     (122)      409 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/serialization/buffer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2491 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/serialization/deserializer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      201 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/serialization/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2038 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/serialization/reps.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/serialization/serializer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      376 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/settings.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1442 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/signaling.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3051 2023-06-09 10:31:32.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/types.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     6931 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/ui_events.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1746 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/uniforms.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.926449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/
--rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-06-09 10:31:34.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/affine.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      754 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/algorithms.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/array.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4300 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/arrayable.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-06-09 10:31:32.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/assert.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3261 2023-06-09 10:31:34.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/bbox.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-06-09 10:31:32.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/bitset.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      298 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/buffer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-06-09 10:31:34.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/canvas.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      592 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/cloneable.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      918 2023-06-09 10:31:32.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/color.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/defer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-06-09 10:31:32.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/eq.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/flip_step_mode.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/image.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/interpolation.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/iterator.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/math.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      737 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/matrix.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/menus.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/modules.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     6794 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/ndarray.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/object.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/platform.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      865 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/pretty.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1027 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/projections.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      963 2023-06-09 10:31:32.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/ragged_array.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-06-09 10:31:34.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/random.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/refs.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/set.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      507 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/slice.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/spatial.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/string.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    11070 2023-06-09 10:31:34.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/svg.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-06-09 10:31:32.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/svg_colors.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1813 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/templating.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/text.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/throttle.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/typed_array.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1756 2023-06-09 10:31:32.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/types.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/version.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/wheel.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      770 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/zoom.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/vectorization.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2375 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/view.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.926449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/
--rw-r--r--   0 runner    (1001) docker     (122)     1355 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/fill.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2414 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/hatch.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/image.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      959 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1947 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/line.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      472 2023-06-09 10:31:34.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/patterns.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2167 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/text.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/visual.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.926449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/document/
--rw-r--r--   0 runner    (1001) docker     (122)     1161 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/document/defs.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4788 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/document/document.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     6205 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/document/events.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/document/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.926449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/embed/
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/embed/dom.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      843 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/embed/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      482 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/embed/json.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/embed/notebook.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      308 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/embed/server.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/embed/standalone.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      446 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/main.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-06-09 10:31:34.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/model.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.926449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.930449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/
--rw-r--r--   0 runner    (1001) docker     (122)     1133 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/annotation.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/arrow.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/arrow_head.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      900 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/band.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4220 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/base_color_bar.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4135 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/box_annotation.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2099 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/color_bar.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1398 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/contour_color_bar.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/data_annotation.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.930449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/html/
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/html/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/html/label.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2245 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/html/label_set.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1191 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/html/text_annotation.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/html/title.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1004 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/label.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/label_set.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3890 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/legend.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      948 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/legend_item.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3650 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/poly_annotation.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/slope.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/span.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1699 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/text_annotation.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/title.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/toolbar_panel.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/upper_lower.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/whisker.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.934449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/
--rw-r--r--   0 runner    (1001) docker     (122)     5022 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/axis.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2312 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/categorical_axis.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/continuous_axis.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      834 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/datetime_axis.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      350 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      816 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/linear_axis.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      754 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/log_axis.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      823 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/mercator_axis.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.934449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)      982 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/callbacks/callback.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1311 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/callbacks/customjs.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/callbacks/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      696 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/callbacks/open_url.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      604 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/callbacks/set_value.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.934449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/canvas/
--rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/canvas/canvas.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1852 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/canvas/cartesian_frame.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      122 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/canvas/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.934449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/common/
--rw-r--r--   0 runner    (1001) docker     (122)     3477 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/common/kinds.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      256 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/common/painting.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/common/resolve.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.934449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/coordinates/
--rw-r--r--   0 runner    (1001) docker     (122)     2253 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/coordinates/coordinate_mapping.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/coordinates/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.938449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/action.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      932 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/color_ref.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/dom_element.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      605 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/dom_node.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/elements.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      936 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/html.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/index_.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      872 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/placeholder.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    16289 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/styles.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/stylesheets.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/template.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/text.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      902 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/toggle_group.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      729 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/value_of.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/value_ref.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.938449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/
--rw-r--r--   0 runner    (1001) docker     (122)     1972 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/coordinate_transform.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      699 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/cumsum.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/customjs_expr.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/expression.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/maximum.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/minimum.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      850 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/polar.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      652 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/stack.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.938449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/
--rw-r--r--   0 runner    (1001) docker     (122)      607 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/all_indices.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      681 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/boolean_filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      827 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/customjs_filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/difference_filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      571 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/group_filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      599 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/index_filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/intersection_filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      689 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/inversion_filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      758 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/symmetric_difference_filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      659 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/union_filter.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.942449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/
--rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/basic_tick_formatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      631 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/categorical_tick_formatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      813 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/customjs_tick_formatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/datetime_tick_formatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      605 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/log_tick_formatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      729 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/mercator_tick_formatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      820 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/numeral_tick_formatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      642 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/printf_tick_formatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      878 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/tick_formatter.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.946449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/
--rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/annular_wedge.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/annulus.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1757 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/arc.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/area.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/bezier.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/block.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1712 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/center_rotatable.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/circle.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/defs.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1293 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/ellipse.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4094 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/glyph.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/harea.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1747 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/harea_step.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1286 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/hbar.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2711 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/hex_tile.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/hspan.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/hstrip.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1043 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/image.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2979 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/image_base.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      922 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/image_rgba.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1160 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/image_stack.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2425 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/image_url.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/line.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/lrtb.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2220 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/marker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/multi_line.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/multi_polygons.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/patch.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2116 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/patches.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1169 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/quad.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1892 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/quadratic.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/ray.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/rect.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1161 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/scatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2090 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/segment.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/spline.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/step.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2543 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/text.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/utils.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/varea.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1747 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/varea_step.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1284 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/vbar.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/vspan.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/vstrip.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.950449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/
--rw-r--r--   0 runner    (1001) docker     (122)      668 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/annular_wedge.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      595 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/annulus.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      944 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/base.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/base_line.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2179 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/base_marker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1920 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/buffer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/circle.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      552 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/dash_cache.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      472 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/hex_tile.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      438 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      700 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/line_gl.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      825 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/lrtb.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       52 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/main.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/marker.frag.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/marker.vert.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      853 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/multi_marker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      452 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/rect.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/regl_line.frag.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/regl_line.vert.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1310 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/regl_wrap.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      930 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/single_marker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      703 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/step.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/sxsy.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3538 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/types.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.950449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/utils/math.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      697 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/webgl_utils.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      612 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/wedge.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2052 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/wedge.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/xy_glyph.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.950449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphics/
--rw-r--r--   0 runner    (1001) docker     (122)     1123 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphics/decoration.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      115 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphics/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphics/marking.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.950449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphs/
--rw-r--r--   0 runner    (1001) docker     (122)     5351 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphs/graph_hit_test_policy.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphs/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphs/layout_provider.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      933 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphs/static_layout_provider.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.950449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/grids/
--rw-r--r--   0 runner    (1001) docker     (122)     1926 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/grids/grid.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       66 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/grids/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      875 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.954449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/
--rw-r--r--   0 runner    (1001) docker     (122)      636 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/alignments.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      556 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/column.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1190 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/css_grid_box.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/flex_box.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/grid_box.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/group_box.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/hbox.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4125 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/layout_dom.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      523 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/row.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/scroll_box.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/spacer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      618 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/tab_panel.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1288 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/tabs.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/vbox.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/main.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.954449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/
--rw-r--r--   0 runner    (1001) docker     (122)      891 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/categorical_color_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      866 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/categorical_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      977 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/categorical_marker_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1003 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/categorical_pattern_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1659 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/color_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1888 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/continuous_color_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      807 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/eqhist_color_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      726 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/linear_color_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      830 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/log_color_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      668 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      993 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/scanning_color_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/stack_color_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/weighted_stack_color_mapper.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.954449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/action.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      612 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/check_action.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      556 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/divider.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/menu.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      666 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/menu_item.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      605 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/section.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.958449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/
--rw-r--r--   0 runner    (1001) docker     (122)      604 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/figure.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      609 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/gmap.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/gmap_plot.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/gmap_plot_canvas.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/grid_plot.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4499 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/plot.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4933 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/plot_canvas.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/range_manager.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1274 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/state_manager.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.958449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/policies/
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/policies/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2207 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/policies/labeling.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.958449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/random/
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/random/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      630 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/random/park_miller_lcg.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      573 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/random/random_generator.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.958449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ranges/
--rw-r--r--   0 runner    (1001) docker     (122)      553 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ranges/data_range.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2363 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ranges/data_range1d.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3167 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ranges/factor_range.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ranges/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ranges/range.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      826 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ranges/range1d.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.958449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/
--rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/contour_renderer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1306 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/data_renderer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2946 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/glyph_renderer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1809 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/graph_renderer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      687 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/guide_renderer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2714 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/renderer.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.962449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/categorical_scale.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      473 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/continuous_scale.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      337 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/linear_interpolation_scale.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      604 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/linear_scale.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      679 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/log_scale.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1109 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/scale.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.962449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selections/
--rw-r--r--   0 runner    (1001) docker     (122)      114 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selections/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      982 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selections/interaction_policy.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selections/selection.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.962449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selectors/
--rw-r--r--   0 runner    (1001) docker     (122)      459 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selectors/by_class.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selectors/by_css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      438 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selectors/by_id.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      459 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selectors/by_xpath.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selectors/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selectors/selector.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.962449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/
--rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/ajax_data_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/cds_view.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      901 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/column_data_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1541 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/columnar_data_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/data_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/geojson_data_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      464 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      582 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/server_sent_data_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/web_data_source.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.962449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/
--rw-r--r--   0 runner    (1001) docker     (122)      797 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/base_text.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4357 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/math_text.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.962449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/mathjax/
--rw-r--r--   0 runner    (1001) docker     (122)      361 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/mathjax/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       52 2023-06-09 10:31:49.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/mathjax/main.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      666 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/plain_text.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/providers.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/utils.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.966450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/textures/
--rw-r--r--   0 runner    (1001) docker     (122)      719 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/textures/canvas_texture.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      771 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/textures/image_url_texture.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/textures/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      766 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/textures/texture.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.966450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/
--rw-r--r--   0 runner    (1001) docker     (122)      905 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/adaptive_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      465 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/basic_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      817 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/binned_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      797 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/categorical_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/composite_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/continuous_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      490 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/datetime_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      757 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/days_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      959 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/fixed_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      779 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      620 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/log_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      999 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/mercator_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      773 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/months_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1222 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/single_interval_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      623 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      495 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/util.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      787 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/years_ticker.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.966450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/bbox_tile_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2788 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/mercator_tile_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/quadkey_tile_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2434 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/tile_renderer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2277 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/tile_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      486 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/tile_utils.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      557 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/tms_tile_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      564 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/wmts_tile_source.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.970450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.970450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/
--rw-r--r--   0 runner    (1001) docker     (122)      903 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/action_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/copy_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/custom_action.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      867 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/examine_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      686 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/fullscreen_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/help_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      760 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/plot_action_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      680 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/redo_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      661 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/reset_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/save_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      680 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/undo_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/zoom_base_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      552 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/zoom_in_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      766 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/zoom_out_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      748 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/click_button.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.974450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/
--rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/box_edit_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/edit_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/freehand_draw_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      417 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1466 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/line_edit_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/line_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/point_draw_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1621 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/poly_draw_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1574 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/poly_edit_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1288 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/poly_tool.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.974450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/
--rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/box_select_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1944 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/box_zoom_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      928 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/gesture_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      549 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/lasso_select_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/pan_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1900 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/poly_select_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1294 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/range_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1343 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/region_select_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/select_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2003 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/tap_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/wheel_pan_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/wheel_zoom_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      391 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.974450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/inspectors/
--rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/inspectors/crosshair_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      792 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/inspectors/customjs_hover.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4159 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/inspectors/hover_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/inspectors/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/inspectors/inspect_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/on_off_button.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4774 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/tool_button.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/tool_proxy.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4551 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/toolbar.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.974450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/
--rw-r--r--   0 runner    (1001) docker     (122)      978 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/customjs_transform.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      510 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/dodge.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1012 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/interpolator.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/jitter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      537 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/linear_interpolator.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/range_transform.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/step_interpolator.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      628 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/transform.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.978450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/
--rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/dialog.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/examiner.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.978450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/icons/
--rw-r--r--   0 runner    (1001) docker     (122)      905 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/icons/builtin_icon.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      623 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/icons/icon.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/icons/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/icons/svg_icon.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/icons/tabler_icon.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      244 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1107 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/pane.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1754 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/tooltip.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/ui_element.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/util.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.982450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/abstract_button.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2666 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/abstract_slider.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1826 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/autocomplete_input.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/base_date_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1166 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/base_datetime_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      752 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/button.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      946 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/checkbox.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      866 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/checkbox_button_group.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      810 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/checkbox_group.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/color_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      655 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/control.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      798 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/date_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      861 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/date_range_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      952 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/date_range_slider.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      890 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/date_slider.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      904 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/datetime_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      962 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/datetime_range_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      901 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/datetime_range_slider.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/div.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1188 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/dropdown.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/file_input.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/help_button.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1454 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/input_widget.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/main.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      998 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/markup.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1311 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/multi_choice.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      923 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/multiple_date_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/multiple_datetime_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      873 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/multiselect.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/numeric_input.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      732 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/oriented_control.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      563 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/paragraph.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      742 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/password_input.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1246 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/picker_base.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      543 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/pretext.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      810 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/radio_button_group.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      754 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/radio_group.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      820 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/range_slider.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/selectbox.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      758 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/slider.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/spinner.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      833 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/switch.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.986450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/
--rw-r--r--   0 runner    (1001) docker     (122)     6181 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/cell_editors.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4072 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/cell_formatters.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2397 2023-06-09 10:31:49.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/data_cube.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3920 2023-06-09 10:31:49.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/data_table.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/definitions.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-09 10:31:49.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-06-09 10:31:49.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/main.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-06-09 10:31:49.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/row_aggregators.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      980 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/table_column.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      646 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/table_widget.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      859 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/text_input.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/text_like_input.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      834 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/textarea_input.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/time_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      715 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/toggle.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1199 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/toggle_button_group.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      792 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/toggle_input.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      996 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/toggle_input_group.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      853 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/widget.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.986450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/protocol/
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/protocol/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      975 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/protocol/message.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      736 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/protocol/receiver.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/safely.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.986450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/attribution.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/base.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/buttons.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/canvas.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/caret.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/clearfix.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/dialogs.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/dropdown.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/examiner.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/group_box.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2067 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/icons.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/logo.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/menus.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/plots.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      263 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/tabs.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      248 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/tool_button.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      332 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/toolbar.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/tooltips.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/ui.css.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.990450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/widgets/checkbox.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/widgets/choices.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/widgets/flatpickr.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      430 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/widgets/inputs.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/widgets/nouislider.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/widgets/password_input.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/widgets/slickgrid.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/widgets/sliders.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/widgets/switch.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/widgets/tables.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/testing.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/version.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.998450 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/
--rw-r--r--   0 runner    (1001) docker     (122)    12714 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.decorators.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.decorators.legacy.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)   824027 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.dom.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    16886 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.dom.iterable.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.collection.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    21204 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.core.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2552 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.generator.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    14892 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.iterable.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3199 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.promise.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     5251 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.proxy.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     6493 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.reflect.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.symbol.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    10621 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.symbol.wellknown.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4861 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2016.array.include.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      928 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2016.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2016.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1083 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.intl.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2451 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.object.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     6227 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.sharedmemory.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2378 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.string.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.typedarrays.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2687 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.asyncgenerator.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.asynciterable.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3076 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.intl.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.promise.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.regexp.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3173 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.array.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.intl.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.object.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1528 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.string.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.symbol.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    35366 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.bigint.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2955 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.date.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    20994 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.intl.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1587 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.number.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1802 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.promise.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4749 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.sharedmemory.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.string.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.symbol.wellknown.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1036 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2021.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2021.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     8378 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2021.intl.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2259 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2021.promise.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1592 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2021.string.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2739 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2021.weakref.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4258 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.array.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1152 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2337 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.error.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     5563 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.intl.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1085 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.object.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1336 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.regexp.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2081 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.sharedmemory.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.string.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    21108 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2023.array.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      921 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2023.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2023.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)   212834 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es5.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es6.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      920 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.esnext.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.esnext.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.esnext.intl.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     9453 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.scripthost.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)   273794 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.webworker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.webworker.importscripts.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    12132 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.webworker.iterable.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    31831 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/tornado.py
--rw-r--r--   0 runner    (1001) docker     (122)     4014 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     7787 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:29.002450 bokeh-3.2.0.dev4/src/bokeh/server/views/
--rw-r--r--   0 runner    (1001) docker     (122)      331 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7033 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/app_index.html
--rw-r--r--   0 runner    (1001) docker     (122)     3207 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/auth_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     3817 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/autoload_js_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)    15086 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/bokeh-dev.ico
--rw-r--r--   0 runner    (1001) docker     (122)    15086 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/bokeh.ico
--rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/doc_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/ico_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2571 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/metadata_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/multi_root_static_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2840 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/root_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     6493 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/session_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     3205 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/static_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)    13576 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/ws.py
--rw-r--r--   0 runner    (1001) docker     (122)    26423 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:29.006450 bokeh-3.2.0.dev4/src/bokeh/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (122)      929 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:29.006450 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)     2608 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/bokehjs_codepen_init.html
--rw-r--r--   0 runner    (1001) docker     (122)      383 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/bokehjs_content_epilogue.html
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/bokehjs_content_prologue.html
--rw-r--r--   0 runner    (1001) docker     (122)      480 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/bokehjs_html_template.html
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/color_detail.html
--rw-r--r--   0 runner    (1001) docker     (122)      417 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/enum_detail.rst
--rw-r--r--   0 runner    (1001) docker     (122)      230 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/example_metadata.rst
--rw-r--r--   0 runner    (1001) docker     (122)      199 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/gallery_detail.rst
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/gallery_page.rst
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/jinja_detail.rst
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/model_detail.rst
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/options_detail.rst
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/palette_detail.html
--rw-r--r--   0 runner    (1001) docker     (122)      481 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/palette_group_detail.html
--rw-r--r--   0 runner    (1001) docker     (122)      171 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/prop_detail.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1269 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/release_detail.rst
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/settings_detail.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4320 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_autodoc.py
--rw-r--r--   0 runner    (1001) docker     (122)     2912 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_color.py
--rw-r--r--   0 runner    (1001) docker     (122)     3465 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (122)     2725 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_directive.py
--rw-r--r--   0 runner    (1001) docker     (122)     4423 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_enum.py
--rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_example_metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)     6570 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_gallery.py
--rw-r--r--   0 runner    (1001) docker     (122)     3964 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_jinja.py
--rw-r--r--   0 runner    (1001) docker     (122)     6135 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     4828 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_options.py
--rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_palette.py
--rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_palette_group.py
--rw-r--r--   0 runner    (1001) docker     (122)    12661 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     4988 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_prop.py
--rw-r--r--   0 runner    (1001) docker     (122)     3398 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_releases.py
--rw-r--r--   0 runner    (1001) docker     (122)     8083 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_roles.py
--rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_sampledata_xref.py
--rw-r--r--   0 runner    (1001) docker     (122)     4275 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     3791 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_sitemap.py
--rw-r--r--   0 runner    (1001) docker     (122)     9589 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokehjs_content.py
--rw-r--r--   0 runner    (1001) docker     (122)     4630 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/example_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2600 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/sample.py
--rw-r--r--   0 runner    (1001) docker     (122)     3247 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     3004 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:29.006450 bokeh-3.2.0.dev4/src/bokeh/themes/
--rw-r--r--   0 runner    (1001) docker     (122)     2904 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/themes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2243 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/themes/_caliber.py
--rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/themes/_contrast.py
--rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/themes/_dark_minimal.py
--rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/themes/_light_minimal.py
--rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/themes/_night_sky.py
--rw-r--r--   0 runner    (1001) docker     (122)     9267 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/themes/theme.py
--rw-r--r--   0 runner    (1001) docker     (122)     8284 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/tile_providers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:29.010450 bokeh-3.2.0.dev4/src/bokeh/util/
--rw-r--r--   0 runner    (1001) docker     (122)     2528 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4707 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/browser.py
--rw-r--r--   0 runner    (1001) docker     (122)     7856 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/callback_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)    18959 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2711 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (122)     3827 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2924 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2303 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/functions.py
--rw-r--r--   0 runner    (1001) docker     (122)     8426 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/hex.py
--rw-r--r--   0 runner    (1001) docker     (122)     3600 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/logconfig.py
--rw-r--r--   0 runner    (1001) docker     (122)     3043 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/options.py
--rw-r--r--   0 runner    (1001) docker     (122)     4391 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/package.py
--rw-r--r--   0 runner    (1001) docker     (122)     2505 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/paths.py
--rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/sampledata.json
--rw-r--r--   0 runner    (1001) docker     (122)     7969 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/sampledata.py
--rw-r--r--   0 runner    (1001) docker     (122)    11396 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/serialization.py
--rw-r--r--   0 runner    (1001) docker     (122)     5419 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/strings.py
--rw-r--r--   0 runner    (1001) docker     (122)     3646 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/terminal.py
--rw-r--r--   0 runner    (1001) docker     (122)    12872 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/token.py
--rw-r--r--   0 runner    (1001) docker     (122)    11285 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/tornado.py
--rw-r--r--   0 runner    (1001) docker     (122)     2944 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/version.py
--rw-r--r--   0 runner    (1001) docker     (122)     3153 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.834447 bokeh-3.2.0.dev4/src/bokeh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    12082 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    55013 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:29.010450 bokeh-3.2.0.dev4/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/tests/test_bokehjs.py
--rw-r--r--   0 runner    (1001) docker     (122)     6178 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/tests/test_cross.py
--rw-r--r--   0 runner    (1001) docker     (122)     2588 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/tests/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (122)    10468 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.752895 bokeh-3.2.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    12080 2023-06-14 19:44:22.752895 bokeh-3.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8603 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)    10430 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-14 19:44:22.752895 bokeh-3.2.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     6745 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.596896 bokeh-3.2.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.604896 bokeh-3.2.0rc1/src/bokeh/
+-rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3750 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2136 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    73110 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/_sri.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.608896 bokeh-3.2.0rc1/src/bokeh/application/
+-rw-r--r--   0 runner    (1001) docker     (122)     2145 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11549 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/application/application.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.608896 bokeh-3.2.0rc1/src/bokeh/application/handlers/
+-rw-r--r--   0 runner    (1001) docker     (122)     2194 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/application/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6919 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/application/handlers/code.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7818 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/application/handlers/code_runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10926 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/application/handlers/directory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/application/handlers/document_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4943 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/application/handlers/function.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7975 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/application/handlers/handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4705 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/application/handlers/lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5180 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/application/handlers/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/application/handlers/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3348 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/application/handlers/script.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5035 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/application/handlers/server_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4339 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/application/handlers/server_request_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.608896 bokeh-3.2.0rc1/src/bokeh/client/
+-rw-r--r--   0 runner    (1001) docker     (122)     2373 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16199 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21727 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/client/session.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5334 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/client/states.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3299 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/client/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3252 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/client/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.608896 bokeh-3.2.0rc1/src/bokeh/colors/
+-rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14039 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/colors/color.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9825 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/colors/groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13046 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/colors/named.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5432 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/colors/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.608896 bokeh-3.2.0rc1/src/bokeh/command/
+-rw-r--r--   0 runner    (1001) docker     (122)      901 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3965 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/command/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5822 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/command/subcommand.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.612896 bokeh-3.2.0rc1/src/bokeh/command/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (122)     2802 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/command/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2567 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/command/subcommands/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7336 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/command/subcommands/file_output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4658 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/command/subcommands/info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/command/subcommands/init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3592 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/command/subcommands/json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2564 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/command/subcommands/sampledata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2775 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/command/subcommands/secret.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37703 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/command/subcommands/serve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3764 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/command/subcommands/static.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7996 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/command/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.612896 bokeh-3.2.0rc1/src/bokeh/core/
+-rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.612896 bokeh-3.2.0rc1/src/bokeh/core/_templates/
+-rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/_templates/autoload_js.js
+-rw-r--r--   0 runner    (1001) docker     (122)     6450 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/_templates/autoload_nb_js.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/_templates/autoload_request_tag.html
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/_templates/autoload_tag.html
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/_templates/css_resources.html
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/_templates/doc_js.js
+-rw-r--r--   0 runner    (1001) docker     (122)      213 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/_templates/doc_nb_js.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1634 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/_templates/file.html
+-rw-r--r--   0 runner    (1001) docker     (122)      586 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/_templates/js_resources.html
+-rw-r--r--   0 runner    (1001) docker     (122)      158 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/_templates/macros.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3933 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/_templates/notebook_load.html
+-rw-r--r--   0 runner    (1001) docker     (122)      356 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/_templates/plot_div.html
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/_templates/root_div.html
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/_templates/script_tag.html
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/_templates/try_run.js
+-rw-r--r--   0 runner    (1001) docker     (122)    16751 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29845 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/has_props.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7133 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11533 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.616896 bokeh-3.2.0rc1/src/bokeh/core/property/
+-rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2782 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/_sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3646 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/alias.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3156 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/any.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/auto.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20064 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/bases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6436 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/color.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12052 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/container.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22696 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/dataspec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6091 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5123 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/descriptor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35217 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/either.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3989 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/enum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3021 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/factors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2879 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/include.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6521 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/instance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2743 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/nothing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/nullable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9631 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3458 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/override.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/pd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7166 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/primitive.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/readonly.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/required.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2536 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/serialized.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/singletons.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3465 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/string.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2481 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/text_like.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3378 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/validation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5977 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/vectorization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8905 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/visual.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17517 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12260 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/property_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10171 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/query.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23292 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4892 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3025 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.616896 bokeh-3.2.0rc1/src/bokeh/core/validation/
+-rw-r--r--   0 runner    (1001) docker     (122)     3502 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7168 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/validation/check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6555 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/validation/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9259 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/validation/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2983 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/validation/issue.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3082 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/core/validation/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.620895 bokeh-3.2.0rc1/src/bokeh/document/
+-rw-r--r--   0 runner    (1001) docker     (122)     2435 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16657 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/document/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27922 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/document/document.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29934 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/document/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/document/json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4978 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/document/locking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9341 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/document/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5026 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/document/modules.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6344 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/driving.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.620895 bokeh-3.2.0rc1/src/bokeh/embed/
+-rw-r--r--   0 runner    (1001) docker     (122)     2074 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/embed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14666 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/embed/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6464 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/embed/elements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3968 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/embed/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12506 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/embed/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17807 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/embed/standalone.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14837 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/embed/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/embed/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23182 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3844 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.620895 bokeh-3.2.0rc1/src/bokeh/io/
+-rw-r--r--   0 runner    (1001) docker     (122)     2208 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3375 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/io/doc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19390 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/io/export.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21518 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/io/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5047 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/io/output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6261 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/io/saving.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8278 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/io/showing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8360 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/io/state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4155 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/io/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6093 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/io/webdriver.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23032 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/layouts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.620895 bokeh-3.2.0rc1/src/bokeh/model/
+-rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/model/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4140 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/model/docs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21302 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8027 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/model/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.624895 bokeh-3.2.0rc1/src/bokeh/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     4057 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.624895 bokeh-3.2.0rc1/src/bokeh/models/annotations/
+-rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/annotations/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5564 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/annotations/arrows.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13775 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/annotations/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.624895 bokeh-3.2.0rc1/src/bokeh/models/annotations/html/
+-rw-r--r--   0 runner    (1001) docker     (122)     1950 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/annotations/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2265 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/annotations/html/html_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10444 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/annotations/html/labels.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2093 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/annotations/html/toolbars.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9340 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/annotations/labels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16806 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/annotations/legends.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12456 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/axes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7795 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2363 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3154 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16739 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/css.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6881 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/dom.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9495 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8487 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24509 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4197 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (122)    54279 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/glyphs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6435 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4263 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/grids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/labeling.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23128 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/layouts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7304 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/map_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12636 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/mappers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33674 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17571 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/ranges.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.628896 bokeh-3.2.0rc1/src/bokeh/models/renderers/
+-rw-r--r--   0 runner    (1001) docker     (122)     2101 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4996 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/renderers/contour_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8796 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/renderers/glyph_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/renderers/graph_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4219 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/renderers/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2613 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/renderers/tile_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3815 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/scales.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4923 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/selections.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3711 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33223 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/sources.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4673 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/text.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/textures.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11476 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/tickers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6596 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/tiles.py
+-rw-r--r--   0 runner    (1001) docker     (122)    73516 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9422 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.628896 bokeh-3.2.0rc1/src/bokeh/models/ui/
+-rw-r--r--   0 runner    (1001) docker     (122)     2153 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2548 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/ui/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2275 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/ui/examiner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4930 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/ui/icons.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3706 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/ui/menus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2095 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/ui/panes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3913 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/ui/tooltips.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3068 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/ui/ui_element.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.628896 bokeh-3.2.0rc1/src/bokeh/models/util/
+-rw-r--r--   0 runner    (1001) docker     (122)      876 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12432 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/util/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.628896 bokeh-3.2.0rc1/src/bokeh/models/widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7089 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/widgets/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4612 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/widgets/groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16135 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/widgets/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4680 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/widgets/markups.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11229 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/widgets/pickers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10242 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/widgets/sliders.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28151 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/widgets/tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2429 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/models/widgets/widget.py
+-rw-r--r--   0 runner    (1001) docker     (122)   113099 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/palettes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.628896 bokeh-3.2.0rc1/src/bokeh/plotting/
+-rw-r--r--   0 runner    (1001) docker     (122)     2533 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3921 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/plotting/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8267 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/plotting/_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32388 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/plotting/_figure.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6603 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/plotting/_graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5002 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/plotting/_legends.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6567 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/plotting/_plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12625 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/plotting/_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3813 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/plotting/_stack.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/plotting/_tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14637 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/plotting/contour.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27693 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/plotting/glyph_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4939 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/plotting/gmap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5836 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/plotting/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.632896 bokeh-3.2.0rc1/src/bokeh/protocol/
+-rw-r--r--   0 runner    (1001) docker     (122)     5428 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2485 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/protocol/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11813 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/protocol/message.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.632896 bokeh-3.2.0rc1/src/bokeh/protocol/messages/
+-rw-r--r--   0 runner    (1001) docker     (122)     2138 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/protocol/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/protocol/messages/ack.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3307 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/protocol/messages/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/protocol/messages/ok.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3754 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/protocol/messages/patch_doc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3176 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/protocol/messages/pull_doc_reply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2334 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/protocol/messages/pull_doc_req.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2799 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/protocol/messages/push_doc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3072 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/protocol/messages/server_info_reply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/protocol/messages/server_info_req.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6987 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/protocol/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    24107 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.636896 bokeh-3.2.0rc1/src/bokeh/sampledata/
+-rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.636896 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/
+-rw-r--r--   0 runner    (1001) docker     (122)    79935 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/USHolidays.ics
+-rw-r--r--   0 runner    (1001) docker     (122)   106201 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/US_Regions_State_Boundaries.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (122)    17444 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/auto-mpg.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    17345 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/auto-mpg2.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     2296 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/browsers_nov_2013.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    25491 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/commits.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (122)    11342 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/daylight_warsaw_2013.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    14487 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/elements.csv
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.640895 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/icons/
+-rw-r--r--   0 runner    (1001) docker     (122)     1985 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/icons/chrome_32x32.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2443 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/icons/firefox_32x32.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2293 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/icons/ie_32x32.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/icons/opera_32x32.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2552 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/icons/safari_32x32.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/iris.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    11536 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/les_mis.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/numberly.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    33264 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/obiszow_mtb_xcm.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     8630 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/olympics2014.json
+-rw-r--r--   0 runner    (1001) docker     (122)    13478 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/penguins.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     5682 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/percent-bachelors-degrees-women-usa.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     2465 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/probly.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    14494 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/sample_geojson.geojson
+-rw-r--r--   0 runner    (1001) docker     (122)    76453 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/sea_surface_temperature.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (122)     5332 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/sprint.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     4003 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/unemployment1948.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     5387 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/_data/us_marriages_divorces.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/airport_routes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2761 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/airports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3122 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/anscombe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3780 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/antibiotics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3038 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/autompg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/autompg2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3112 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/browsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/commits.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2648 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/daylight.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/degrees.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4599 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/gapminder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2022 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/glucose.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/haar_cascade.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2371 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/iris.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2367 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/les_mis.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/movies_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2096 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/mtb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2224 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/olympics2014.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2212 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/penguins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2270 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/perceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2041 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/periodic_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2548 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/population.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2071 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/sample_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/sample_superstore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2706 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/sea_surface_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3520 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/stocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2777 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/unemployment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2099 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/unemployment1948.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2116 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/us_cities.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4032 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/us_counties.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/us_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/us_marriages_divorces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3703 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/us_states.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2132 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sampledata/world_cities.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.640895 bokeh-3.2.0rc1/src/bokeh/server/
+-rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9579 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/server/auth_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6721 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/server/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3939 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/server/connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14606 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/server/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4096 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/server/protocol_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20849 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11852 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/server/session.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.604896 bokeh-3.2.0rc1/src/bokeh/server/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.652895 bokeh-3.2.0rc1/src/bokeh/server/static/js/
+-rw-r--r--   0 runner    (1001) docker     (122)   211363 2023-06-14 19:43:32.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/bokeh-api.js
+-rw-r--r--   0 runner    (1001) docker     (122)   118619 2023-06-14 19:43:32.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/bokeh-api.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)   535980 2023-06-14 19:43:32.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/bokeh-gl.js
+-rw-r--r--   0 runner    (1001) docker     (122)   198523 2023-06-14 19:43:32.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/bokeh-gl.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)  2750419 2023-06-14 19:43:32.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/bokeh-mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (122)  1785922 2023-06-14 19:43:32.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/bokeh-mathjax.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)   949246 2023-06-14 19:43:32.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/bokeh-tables.js
+-rw-r--r--   0 runner    (1001) docker     (122)   302598 2023-06-14 19:43:32.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/bokeh-tables.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)   799628 2023-06-14 19:43:32.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/bokeh-widgets.js
+-rw-r--r--   0 runner    (1001) docker     (122)   301351 2023-06-14 19:43:32.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/bokeh-widgets.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)  2257233 2023-06-14 19:43:32.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/bokeh.js
+-rw-r--r--   0 runner    (1001) docker     (122)   959267 2023-06-14 19:43:32.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/bokeh.min.js
+-rw-r--r--   0 runner    (1001) docker     (122) 20427534 2023-06-14 19:43:46.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/compiler.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.672895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.672895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/api/
+-rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/api/charts.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      508 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/api/expr.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4471 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/api/figure.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    19794 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/api/glyph_api.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/api/gridplot.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      448 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/api/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      739 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/api/io.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3346 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/api/linalg.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/api/main.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/api/models.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    63941 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/api/palettes.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     5394 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/api/parser.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/api/plotting.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/api/themes.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/base.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-06-14 19:43:00.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/bokeh.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.672895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/client/
+-rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/client/connection.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1106 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/client/session.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.676895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/
+-rw-r--r--   0 runner    (1001) docker     (122)     5846 2023-06-14 19:42:47.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/bokeh_events.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      820 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/build_views.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      274 2023-06-14 19:42:45.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/class.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    42976 2023-06-14 19:42:47.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      334 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/diagnostics.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     5953 2023-06-14 19:42:47.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/dom.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/dom_view.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    11975 2023-06-14 19:42:46.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/enums.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-06-14 19:42:46.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/geometry.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3638 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/graphics.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     5113 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/has_props.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      966 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/hittest.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     8908 2023-06-14 19:42:46.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/kinds.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.676895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/layout/
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/layout/alignments.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-06-14 19:42:52.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/layout/border.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3050 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/layout/grid.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      321 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/layout/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/layout/layoutable.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/layout/side_panel.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1595 2023-06-14 19:42:48.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/layout/types.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-06-14 19:42:46.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/logging.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      861 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/patching.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     9618 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/properties.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     6764 2023-06-14 19:42:48.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/property_mixins.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/resolvers.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/selection_manager.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.676895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/serialization/
+-rw-r--r--   0 runner    (1001) docker     (122)      409 2023-06-14 19:42:46.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/serialization/buffer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2491 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/serialization/deserializer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      201 2023-06-14 19:42:46.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/serialization/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2038 2023-06-14 19:42:46.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/serialization/reps.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-06-14 19:42:46.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/serialization/serializer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      376 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/settings.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1442 2023-06-14 19:42:46.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/signaling.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3051 2023-06-14 19:42:45.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/types.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     6931 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/ui_events.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1746 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/uniforms.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.680895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/
+-rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-06-14 19:42:47.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/affine.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/algorithms.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-06-14 19:42:46.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/array.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4300 2023-06-14 19:42:46.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/arrayable.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-06-14 19:42:45.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/assert.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3261 2023-06-14 19:42:47.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/bbox.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-06-14 19:42:45.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/bitset.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      298 2023-06-14 19:42:46.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/buffer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-06-14 19:42:48.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/canvas.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      592 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/cloneable.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      918 2023-06-14 19:42:46.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/color.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-14 19:42:46.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/defer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-06-14 19:42:45.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/eq.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/flip_step_mode.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/image.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/interpolation.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-06-14 19:42:46.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/iterator.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-06-14 19:42:46.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/math.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      737 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/matrix.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/menus.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/modules.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     6794 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/ndarray.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-06-14 19:42:46.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/object.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-06-14 19:42:46.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/platform.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      865 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/pretty.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1027 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/projections.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      963 2023-06-14 19:42:45.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/ragged_array.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-06-14 19:42:47.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/random.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-06-14 19:42:46.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/refs.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-06-14 19:42:48.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/set.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/slice.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/spatial.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/string.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    11070 2023-06-14 19:42:48.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/svg.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-06-14 19:42:45.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/svg_colors.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1813 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/templating.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/text.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-06-14 19:42:52.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/throttle.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/typed_array.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1756 2023-06-14 19:42:45.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/types.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/version.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/wheel.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/zoom.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/vectorization.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2375 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/view.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.680895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/visuals/
+-rw-r--r--   0 runner    (1001) docker     (122)     1355 2023-06-14 19:42:48.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/visuals/fill.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2414 2023-06-14 19:42:48.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/visuals/hatch.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-06-14 19:42:48.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/visuals/image.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      959 2023-06-14 19:42:48.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/visuals/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1947 2023-06-14 19:42:48.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/visuals/line.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-06-14 19:42:48.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/visuals/patterns.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2167 2023-06-14 19:42:48.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/visuals/text.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-06-14 19:42:48.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/visuals/visual.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.684895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/document/
+-rw-r--r--   0 runner    (1001) docker     (122)     1161 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/document/defs.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4788 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/document/document.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     6205 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/document/events.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/document/index.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.684895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/embed/
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/embed/dom.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/embed/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      482 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/embed/json.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/embed/notebook.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      308 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/embed/server.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/embed/standalone.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      446 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/main.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-06-14 19:42:47.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/model.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.684895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.684895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1133 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/annotation.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/arrow.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/arrow_head.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      900 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/band.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4220 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/base_color_bar.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4135 2023-06-14 19:42:52.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/box_annotation.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2099 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/color_bar.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1398 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/contour_color_bar.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/data_annotation.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.684895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/html/
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/html/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/html/label.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2245 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/html/label_set.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1191 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/html/text_annotation.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/html/title.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1004 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/label.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/label_set.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3890 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/legend.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      948 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/legend_item.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3650 2023-06-14 19:42:52.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/poly_annotation.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/slope.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-06-14 19:42:52.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/span.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1699 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/text_annotation.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/title.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-06-14 19:42:52.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/toolbar_panel.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/upper_lower.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/whisker.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.688895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/axes/
+-rw-r--r--   0 runner    (1001) docker     (122)     5022 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/axes/axis.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2312 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/axes/categorical_axis.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/axes/continuous_axis.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/axes/datetime_axis.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      350 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/axes/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      816 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/axes/linear_axis.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/axes/log_axis.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      823 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/axes/mercator_axis.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.688895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)      982 2023-06-14 19:42:47.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/callbacks/callback.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1311 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/callbacks/customjs.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/callbacks/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      696 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/callbacks/open_url.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      604 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/callbacks/set_value.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.688895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/canvas/
+-rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/canvas/canvas.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1852 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/canvas/cartesian_frame.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/canvas/index.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.688895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/common/
+-rw-r--r--   0 runner    (1001) docker     (122)     3477 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/common/kinds.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-06-14 19:42:52.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/common/painting.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/common/resolve.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.688895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/coordinates/
+-rw-r--r--   0 runner    (1001) docker     (122)     2253 2023-06-14 19:42:52.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/coordinates/coordinate_mapping.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/coordinates/index.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.688895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/action.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      932 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/color_ref.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/dom_element.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      605 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/dom_node.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/elements.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      936 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/html.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/index_.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      872 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/placeholder.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    16289 2023-06-14 19:42:48.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/styles.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-06-14 19:42:48.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/stylesheets.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/template.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/text.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/toggle_group.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      729 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/value_of.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/value_ref.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.692895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/expressions/
+-rw-r--r--   0 runner    (1001) docker     (122)     1972 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/expressions/coordinate_transform.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/expressions/cumsum.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/expressions/customjs_expr.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/expressions/expression.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/expressions/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/expressions/maximum.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/expressions/minimum.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      850 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/expressions/polar.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/expressions/stack.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.692895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      607 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/filters/all_indices.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/filters/boolean_filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      827 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/filters/customjs_filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/filters/difference_filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/filters/filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/filters/group_filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      599 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/filters/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/filters/index_filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/filters/intersection_filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      689 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/filters/inversion_filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/filters/symmetric_difference_filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      659 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/filters/union_filter.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.692895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/formatters/
+-rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/formatters/basic_tick_formatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      631 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/formatters/categorical_tick_formatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      813 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/formatters/customjs_tick_formatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/formatters/datetime_tick_formatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      605 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/formatters/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/formatters/log_tick_formatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      729 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/formatters/mercator_tick_formatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      820 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/formatters/numeral_tick_formatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      642 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/formatters/printf_tick_formatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      878 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/formatters/tick_formatter.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.696895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/annular_wedge.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/annulus.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1757 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/arc.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/area.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/bezier.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/block.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1712 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/center_rotatable.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/circle.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/defs.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1293 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/ellipse.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4094 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/glyph.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/harea.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1747 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/harea_step.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1286 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/hbar.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2711 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/hex_tile.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/hspan.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/hstrip.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1043 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/image.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2979 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/image_base.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      922 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/image_rgba.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1160 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/image_stack.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2425 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/image_url.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/line.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/lrtb.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2220 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/marker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/multi_line.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/multi_polygons.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/patch.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2116 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/patches.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1169 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/quad.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1892 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/quadratic.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/ray.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/rect.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1161 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/scatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2090 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/segment.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/spline.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/step.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2543 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/text.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/utils.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/varea.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1747 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/varea_step.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1284 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/vbar.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/vspan.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/vstrip.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.700895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/annular_wedge.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/annulus.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      944 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/base.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/base_line.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2179 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/base_marker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1920 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/buffer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/circle.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/dash_cache.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/hex_tile.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      700 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/line_gl.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      825 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/lrtb.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/main.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/marker.frag.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/marker.vert.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      853 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/multi_marker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      452 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/rect.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/regl_line.frag.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/regl_line.vert.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1310 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/regl_wrap.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      930 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/single_marker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/step.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/sxsy.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3538 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/types.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.700895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/utils/math.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/webgl_utils.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/wedge.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2052 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/wedge.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/xy_glyph.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.700895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/graphics/
+-rw-r--r--   0 runner    (1001) docker     (122)     1123 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/graphics/decoration.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/graphics/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1239 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/graphics/marking.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.700895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/graphs/
+-rw-r--r--   0 runner    (1001) docker     (122)     5351 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/graphs/graph_hit_test_policy.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/graphs/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/graphs/layout_provider.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      933 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/graphs/static_layout_provider.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.700895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/grids/
+-rw-r--r--   0 runner    (1001) docker     (122)     1926 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/grids/grid.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/grids/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      875 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/index.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.704895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/
+-rw-r--r--   0 runner    (1001) docker     (122)      636 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/alignments.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/column.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1190 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/css_grid_box.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/flex_box.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/grid_box.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/group_box.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/hbox.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4125 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/layout_dom.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      523 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/row.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-06-14 19:42:56.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/scroll_box.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/spacer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      618 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/tab_panel.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1288 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/tabs.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/vbox.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/main.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.704895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/
+-rw-r--r--   0 runner    (1001) docker     (122)      891 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/categorical_color_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/categorical_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      977 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/categorical_marker_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1003 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/categorical_pattern_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1659 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/color_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1888 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/continuous_color_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      807 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/eqhist_color_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      726 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/linear_color_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/log_color_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      993 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/scanning_color_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/stack_color_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/weighted_stack_color_mapper.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.704895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/menus/
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/menus/action.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/menus/check_action.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/menus/divider.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/menus/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/menus/menu.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/menus/menu_item.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      605 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/menus/section.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.708895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)      604 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/plots/figure.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/plots/gmap.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/plots/gmap_plot.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/plots/gmap_plot_canvas.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/plots/grid_plot.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/plots/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4499 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/plots/plot.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4933 2023-06-14 19:42:52.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/plots/plot_canvas.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-06-14 19:42:52.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/plots/range_manager.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1274 2023-06-14 19:42:52.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/plots/state_manager.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.708895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/policies/
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/policies/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2207 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/policies/labeling.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.708895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/random/
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/random/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      630 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/random/park_miller_lcg.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/random/random_generator.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.708895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ranges/
+-rw-r--r--   0 runner    (1001) docker     (122)      553 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ranges/data_range.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2363 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ranges/data_range1d.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3167 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ranges/factor_range.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ranges/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ranges/range.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      826 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ranges/range1d.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.708895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/renderers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/renderers/contour_renderer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1306 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/renderers/data_renderer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2946 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/renderers/glyph_renderer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1809 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/renderers/graph_renderer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      687 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/renderers/guide_renderer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/renderers/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2714 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/renderers/renderer.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.708895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/scales/
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/scales/categorical_scale.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      473 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/scales/continuous_scale.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/scales/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/scales/linear_interpolation_scale.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      604 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/scales/linear_scale.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      679 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/scales/log_scale.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1109 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/scales/scale.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.708895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/selections/
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/selections/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      982 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/selections/interaction_policy.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/selections/selection.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.712895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/selectors/
+-rw-r--r--   0 runner    (1001) docker     (122)      459 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/selectors/by_class.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/selectors/by_css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/selectors/by_id.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      459 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/selectors/by_xpath.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/selectors/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/selectors/selector.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.712895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/sources/ajax_data_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/sources/cds_view.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      901 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/sources/column_data_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1541 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/sources/columnar_data_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      558 2023-06-14 19:42:50.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/sources/data_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/sources/geojson_data_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      464 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/sources/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      582 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/sources/server_sent_data_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/sources/web_data_source.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.712895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/text/
+-rw-r--r--   0 runner    (1001) docker     (122)      797 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/text/base_text.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/text/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4357 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/text/math_text.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.712895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/text/mathjax/
+-rw-r--r--   0 runner    (1001) docker     (122)      361 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/text/mathjax/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-06-14 19:43:00.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/text/mathjax/main.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/text/plain_text.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/text/providers.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/text/utils.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.712895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (122)      719 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/textures/canvas_texture.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      771 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/textures/image_url_texture.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/textures/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      766 2023-06-14 19:42:48.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/textures/texture.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.716895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/
+-rw-r--r--   0 runner    (1001) docker     (122)      905 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/adaptive_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      465 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/basic_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      817 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/binned_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      797 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/categorical_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/composite_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/continuous_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      490 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/datetime_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/days_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      959 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/fixed_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      620 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/log_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      999 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/mercator_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      773 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/months_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1222 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/single_interval_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      495 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/util.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      787 2023-06-14 19:42:54.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/years_ticker.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.716895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tiles/
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tiles/bbox_tile_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tiles/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2788 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tiles/mercator_tile_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tiles/quadkey_tile_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2434 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tiles/tile_renderer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2277 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tiles/tile_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      486 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tiles/tile_utils.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tiles/tms_tile_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      564 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tiles/wmts_tile_source.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.716895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.716895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/
+-rw-r--r--   0 runner    (1001) docker     (122)      903 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/action_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/copy_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/custom_action.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      867 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/examine_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      686 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/fullscreen_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/help_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      760 2023-06-14 19:42:52.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/plot_action_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/redo_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      661 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/reset_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/save_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/undo_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-06-14 19:42:52.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/zoom_base_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-06-14 19:42:52.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/zoom_in_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      766 2023-06-14 19:42:52.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/zoom_out_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      748 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/click_button.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.720895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/edit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/edit/box_edit_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/edit/edit_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/edit/freehand_draw_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/edit/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1466 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/edit/line_edit_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/edit/line_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/edit/point_draw_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1621 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/edit/poly_draw_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1574 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/edit/poly_edit_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1288 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/edit/poly_tool.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.720895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/
+-rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-06-14 19:42:52.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/box_select_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1944 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/box_zoom_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/gesture_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      549 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-06-14 19:42:52.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/lasso_select_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/pan_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1900 2023-06-14 19:42:52.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/poly_select_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1294 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/range_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1343 2023-06-14 19:42:52.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/region_select_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-06-14 19:42:52.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/select_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2003 2023-06-14 19:42:52.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/tap_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/wheel_pan_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/wheel_zoom_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      391 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/index.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.720895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/inspectors/
+-rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-06-14 19:42:52.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/inspectors/crosshair_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      792 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/inspectors/customjs_hover.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4159 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/inspectors/hover_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/inspectors/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/inspectors/inspect_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/on_off_button.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4774 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/tool_button.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/tool_proxy.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4551 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/toolbar.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.720895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/transforms/
+-rw-r--r--   0 runner    (1001) docker     (122)      978 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/transforms/customjs_transform.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/transforms/dodge.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/transforms/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1012 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/transforms/interpolator.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/transforms/jitter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/transforms/linear_interpolator.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/transforms/range_transform.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/transforms/step_interpolator.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      628 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/transforms/transform.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.720895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ui/
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ui/dialog.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ui/examiner.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.724895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ui/icons/
+-rw-r--r--   0 runner    (1001) docker     (122)      905 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ui/icons/builtin_icon.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ui/icons/icon.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ui/icons/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ui/icons/svg_icon.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ui/icons/tabler_icon.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ui/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1107 2023-06-14 19:42:57.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ui/pane.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1754 2023-06-14 19:42:53.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ui/tooltip.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-06-14 19:42:49.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ui/ui_element.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-14 19:42:51.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/util.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.728895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/abstract_button.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2666 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/abstract_slider.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1826 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/autocomplete_input.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/base_date_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1166 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/base_datetime_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      752 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/button.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      946 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/checkbox.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/checkbox_button_group.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      810 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/checkbox_group.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/color_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      655 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/control.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      798 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/date_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      861 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/date_range_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      952 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/date_range_slider.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      890 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/date_slider.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      904 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/datetime_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/datetime_range_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      901 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/datetime_range_slider.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      558 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/div.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1188 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/dropdown.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/file_input.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/help_button.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1454 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/input_widget.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/main.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      998 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/markup.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1311 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/multi_choice.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      923 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/multiple_date_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/multiple_datetime_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      873 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/multiselect.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/numeric_input.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      732 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/oriented_control.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      563 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/paragraph.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/password_input.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1246 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/picker_base.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      543 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/pretext.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      810 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/radio_button_group.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/radio_group.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      820 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/range_slider.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/selectbox.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/slider.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/spinner.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      833 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/switch.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.728895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/tables/
+-rw-r--r--   0 runner    (1001) docker     (122)     6181 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/tables/cell_editors.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4072 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/tables/cell_formatters.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2397 2023-06-14 19:43:00.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/tables/data_cube.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3920 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/tables/data_table.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      355 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/tables/definitions.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-14 19:43:00.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/tables/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-06-14 19:43:00.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/tables/main.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/tables/row_aggregators.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      980 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/tables/table_column.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      646 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/tables/table_widget.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      859 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/text_input.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/text_like_input.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/textarea_input.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/time_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      715 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/toggle.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1199 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/toggle_button_group.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      792 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/toggle_input.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      996 2023-06-14 19:42:59.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/toggle_input_group.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      853 2023-06-14 19:42:58.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/widget.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.728895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/protocol/
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/protocol/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/protocol/message.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      736 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/protocol/receiver.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/safely.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.732895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/attribution.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/base.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/buttons.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/canvas.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/caret.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/clearfix.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/dialogs.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/dropdown.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/examiner.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/group_box.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2067 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/icons.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/logo.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/menus.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/plots.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      263 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/tabs.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      248 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/tool_button.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      332 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/toolbar.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/tooltips.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/ui.css.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.732895 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/widgets/checkbox.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/widgets/choices.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/widgets/flatpickr.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      430 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/widgets/inputs.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/widgets/nouislider.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/widgets/password_input.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/widgets/slickgrid.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/widgets/sliders.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/widgets/switch.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/widgets/tables.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-06-14 19:42:55.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/testing.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-14 19:42:43.000000 bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/version.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.740895 bokeh-3.2.0rc1/src/bokeh/server/static/lib/
+-rw-r--r--   0 runner    (1001) docker     (122)    12714 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.decorators.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.decorators.legacy.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)   824027 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.dom.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    16886 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.dom.iterable.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2015.collection.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    21204 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2015.core.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2015.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2552 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2015.generator.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    14892 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2015.iterable.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3199 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2015.promise.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     5251 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2015.proxy.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     6493 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2015.reflect.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2015.symbol.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    10621 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2015.symbol.wellknown.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4861 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2016.array.include.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2016.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2016.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1083 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2017.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2017.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2017.intl.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2451 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2017.object.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     6227 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2017.sharedmemory.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2378 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2017.string.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2017.typedarrays.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2687 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2018.asyncgenerator.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2018.asynciterable.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2018.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2018.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3076 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2018.intl.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2018.promise.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2018.regexp.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3173 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2019.array.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2019.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2019.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2019.intl.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2019.object.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1528 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2019.string.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2019.symbol.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    35366 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2020.bigint.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2020.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2955 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2020.date.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2020.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    20994 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2020.intl.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1587 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2020.number.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1802 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2020.promise.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4749 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2020.sharedmemory.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2020.string.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2020.symbol.wellknown.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1036 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2021.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2021.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     8378 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2021.intl.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2259 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2021.promise.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1592 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2021.string.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2739 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2021.weakref.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4258 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2022.array.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1152 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2022.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2337 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2022.error.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2022.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     5563 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2022.intl.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1085 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2022.object.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1336 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2022.regexp.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2081 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2022.sharedmemory.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2022.string.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    21108 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2023.array.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2023.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2023.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)   212834 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es5.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es6.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      920 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.esnext.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.esnext.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.esnext.intl.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     9453 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.scripthost.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)   273794 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.webworker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.webworker.importscripts.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    12132 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.webworker.iterable.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    31831 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/server/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4014 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/server/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7787 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/server/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.744895 bokeh-3.2.0rc1/src/bokeh/server/views/
+-rw-r--r--   0 runner    (1001) docker     (122)      331 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/server/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7033 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/server/views/app_index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3207 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/server/views/auth_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3817 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/server/views/autoload_js_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15086 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/server/views/bokeh-dev.ico
+-rw-r--r--   0 runner    (1001) docker     (122)    15086 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/server/views/bokeh.ico
+-rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/server/views/doc_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/server/views/ico_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2571 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/server/views/metadata_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/server/views/multi_root_static_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2840 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/server/views/root_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6493 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/server/views/session_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3205 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/server/views/static_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13576 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/server/views/ws.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26423 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.744895 bokeh-3.2.0rc1/src/bokeh/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (122)      929 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.748895 bokeh-3.2.0rc1/src/bokeh/sphinxext/_templates/
+-rw-r--r--   0 runner    (1001) docker     (122)     2608 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/_templates/bokehjs_codepen_init.html
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/_templates/bokehjs_content_epilogue.html
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/_templates/bokehjs_content_prologue.html
+-rw-r--r--   0 runner    (1001) docker     (122)      480 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/_templates/bokehjs_html_template.html
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/_templates/color_detail.html
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/_templates/enum_detail.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      230 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/_templates/example_metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/_templates/gallery_detail.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/_templates/gallery_page.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/_templates/jinja_detail.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/_templates/model_detail.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/_templates/options_detail.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/_templates/palette_detail.html
+-rw-r--r--   0 runner    (1001) docker     (122)      481 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/_templates/palette_group_detail.html
+-rw-r--r--   0 runner    (1001) docker     (122)      171 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/_templates/prop_detail.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1269 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/_templates/release_detail.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/_templates/settings_detail.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4320 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_autodoc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2912 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_color.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3465 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2725 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_directive.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4423 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_enum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_example_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6570 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3964 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_jinja.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6135 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4828 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_palette.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_palette_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12661 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4988 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_prop.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3398 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_releases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8083 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_roles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_sampledata_xref.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4275 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3791 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_sitemap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9589 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/bokehjs_content.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4630 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/example_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2600 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/sample.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3247 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3004 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/sphinxext/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.748895 bokeh-3.2.0rc1/src/bokeh/themes/
+-rw-r--r--   0 runner    (1001) docker     (122)     2904 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/themes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2243 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/themes/_caliber.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/themes/_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/themes/_dark_minimal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/themes/_light_minimal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/themes/_night_sky.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9348 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/themes/theme.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8284 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/tile_providers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.752895 bokeh-3.2.0rc1/src/bokeh/util/
+-rw-r--r--   0 runner    (1001) docker     (122)     2528 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4707 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/util/browser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7856 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/util/callback_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18959 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/util/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2711 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/util/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3827 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/util/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2924 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/util/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/util/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2303 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/util/functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8426 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/util/hex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3600 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/util/logconfig.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3043 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/util/options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4391 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/util/package.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2505 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/util/paths.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/util/sampledata.json
+-rw-r--r--   0 runner    (1001) docker     (122)     7969 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/util/sampledata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11396 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/util/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5419 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/util/strings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3646 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/util/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12872 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/util/token.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11285 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/util/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2944 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/util/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3153 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/src/bokeh/util/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.604896 bokeh-3.2.0rc1/src/bokeh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    12080 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    55013 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-06-14 19:44:22.000000 bokeh-3.2.0rc1/src/bokeh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:44:22.752895 bokeh-3.2.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/tests/test_bokehjs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6178 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/tests/test_cross.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2588 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/tests/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10468 2023-06-14 19:35:22.000000 bokeh-3.2.0rc1/tests/test_examples.py
```

### Comparing `bokeh-3.2.0.dev4/LICENSE.txt` & `bokeh-3.2.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/MANIFEST.in` & `bokeh-3.2.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/PKG-INFO` & `bokeh-3.2.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bokeh
-Version: 3.2.0.dev4
+Version: 3.2.0rc1
 Summary: Interactive plots and applications in the browser from Python
 Author: Bokeh Team
 Author-email: info@bokeh.org
 License: Copyright (c) 2012 - 2023, Anaconda, Inc., and Bokeh Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
```

### Comparing `bokeh-3.2.0.dev4/README.md` & `bokeh-3.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/pyproject.toml` & `bokeh-3.2.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/setup.py` & `bokeh-3.2.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/LICENSE.txt` & `bokeh-3.2.0rc1/src/bokeh/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/__main__.py` & `bokeh-3.2.0rc1/src/bokeh/__main__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/_sri.json` & `bokeh-3.2.0rc1/src/bokeh/_sri.json`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/application/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/application/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/application/application.py` & `bokeh-3.2.0rc1/src/bokeh/application/application.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/application/handlers/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/application/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/application/handlers/code.py` & `bokeh-3.2.0rc1/src/bokeh/application/handlers/code.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/application/handlers/code_runner.py` & `bokeh-3.2.0rc1/src/bokeh/application/handlers/code_runner.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/application/handlers/directory.py` & `bokeh-3.2.0rc1/src/bokeh/application/handlers/directory.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/application/handlers/document_lifecycle.py` & `bokeh-3.2.0rc1/src/bokeh/application/handlers/document_lifecycle.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/application/handlers/function.py` & `bokeh-3.2.0rc1/src/bokeh/application/handlers/function.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/application/handlers/handler.py` & `bokeh-3.2.0rc1/src/bokeh/application/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/application/handlers/lifecycle.py` & `bokeh-3.2.0rc1/src/bokeh/application/handlers/lifecycle.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/application/handlers/notebook.py` & `bokeh-3.2.0rc1/src/bokeh/application/handlers/notebook.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/application/handlers/request_handler.py` & `bokeh-3.2.0rc1/src/bokeh/application/handlers/request_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/application/handlers/script.py` & `bokeh-3.2.0rc1/src/bokeh/application/handlers/script.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/application/handlers/server_lifecycle.py` & `bokeh-3.2.0rc1/src/bokeh/application/handlers/server_lifecycle.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/application/handlers/server_request_handler.py` & `bokeh-3.2.0rc1/src/bokeh/application/handlers/server_request_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/client/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/client/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/client/connection.py` & `bokeh-3.2.0rc1/src/bokeh/client/connection.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/client/session.py` & `bokeh-3.2.0rc1/src/bokeh/client/session.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/client/states.py` & `bokeh-3.2.0rc1/src/bokeh/client/states.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/client/util.py` & `bokeh-3.2.0rc1/src/bokeh/client/util.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/client/websocket.py` & `bokeh-3.2.0rc1/src/bokeh/client/websocket.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/colors/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/colors/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/colors/color.py` & `bokeh-3.2.0rc1/src/bokeh/colors/color.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/colors/groups.py` & `bokeh-3.2.0rc1/src/bokeh/colors/groups.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/colors/named.py` & `bokeh-3.2.0rc1/src/bokeh/colors/named.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/colors/util.py` & `bokeh-3.2.0rc1/src/bokeh/colors/util.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/command/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/command/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/command/bootstrap.py` & `bokeh-3.2.0rc1/src/bokeh/command/bootstrap.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/command/subcommand.py` & `bokeh-3.2.0rc1/src/bokeh/command/subcommand.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/command/subcommands/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/command/subcommands/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/command/subcommands/build.py` & `bokeh-3.2.0rc1/src/bokeh/command/subcommands/build.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/command/subcommands/file_output.py` & `bokeh-3.2.0rc1/src/bokeh/command/subcommands/file_output.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/command/subcommands/info.py` & `bokeh-3.2.0rc1/src/bokeh/command/subcommands/info.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/command/subcommands/init.py` & `bokeh-3.2.0rc1/src/bokeh/command/subcommands/init.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/command/subcommands/json.py` & `bokeh-3.2.0rc1/src/bokeh/command/subcommands/json.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/command/subcommands/sampledata.py` & `bokeh-3.2.0rc1/src/bokeh/command/subcommands/sampledata.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/command/subcommands/secret.py` & `bokeh-3.2.0rc1/src/bokeh/command/subcommands/secret.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/command/subcommands/serve.py` & `bokeh-3.2.0rc1/src/bokeh/command/subcommands/serve.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/command/subcommands/static.py` & `bokeh-3.2.0rc1/src/bokeh/command/subcommands/static.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/command/util.py` & `bokeh-3.2.0rc1/src/bokeh/command/util.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/core/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/_templates/autoload_js.js` & `bokeh-3.2.0rc1/src/bokeh/core/_templates/autoload_js.js`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/_templates/autoload_nb_js.js` & `bokeh-3.2.0rc1/src/bokeh/core/_templates/autoload_nb_js.js`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/_templates/autoload_request_tag.html` & `bokeh-3.2.0rc1/src/bokeh/core/_templates/autoload_request_tag.html`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/_templates/autoload_tag.html` & `bokeh-3.2.0rc1/src/bokeh/core/_templates/autoload_tag.html`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/_templates/file.html` & `bokeh-3.2.0rc1/src/bokeh/core/_templates/file.html`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/_templates/js_resources.html` & `bokeh-3.2.0rc1/src/bokeh/core/_templates/js_resources.html`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/_templates/notebook_load.html` & `bokeh-3.2.0rc1/src/bokeh/core/_templates/notebook_load.html`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/_templates/try_run.js` & `bokeh-3.2.0rc1/src/bokeh/core/_templates/try_run.js`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/enums.py` & `bokeh-3.2.0rc1/src/bokeh/core/enums.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/has_props.py` & `bokeh-3.2.0rc1/src/bokeh/core/has_props.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/json_encoder.py` & `bokeh-3.2.0rc1/src/bokeh/core/json_encoder.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/properties.py` & `bokeh-3.2.0rc1/src/bokeh/core/properties.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/_sphinx.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/_sphinx.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/alias.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/alias.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/aliases.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/aliases.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/any.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/any.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/auto.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/auto.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/bases.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/bases.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/color.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/color.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/container.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/container.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/dataspec.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/dataspec.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/datetime.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/datetime.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/descriptor_factory.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/descriptor_factory.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/descriptors.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/descriptors.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/either.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/either.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/enum.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/enum.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/factors.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/factors.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/include.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/include.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/instance.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/instance.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/json.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/json.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/nothing.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/nothing.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/nullable.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/nullable.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/numeric.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/numeric.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/override.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/override.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/pd.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/pd.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/primitive.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/primitive.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/readonly.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/readonly.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/required.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/required.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/serialized.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/serialized.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/singletons.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/singletons.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/string.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/string.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/struct.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/struct.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/text_like.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/text_like.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/validation.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/validation.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/vectorization.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/vectorization.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/visual.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/visual.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property/wrappers.py` & `bokeh-3.2.0rc1/src/bokeh/core/property/wrappers.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property_aliases.py` & `bokeh-3.2.0rc1/src/bokeh/core/property_aliases.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/property_mixins.py` & `bokeh-3.2.0rc1/src/bokeh/core/property_mixins.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/query.py` & `bokeh-3.2.0rc1/src/bokeh/core/query.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/serialization.py` & `bokeh-3.2.0rc1/src/bokeh/core/serialization.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/templates.py` & `bokeh-3.2.0rc1/src/bokeh/core/templates.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/types.py` & `bokeh-3.2.0rc1/src/bokeh/core/types.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/validation/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/core/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/validation/check.py` & `bokeh-3.2.0rc1/src/bokeh/core/validation/check.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/validation/decorators.py` & `bokeh-3.2.0rc1/src/bokeh/core/validation/decorators.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/validation/errors.py` & `bokeh-3.2.0rc1/src/bokeh/core/validation/errors.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/validation/issue.py` & `bokeh-3.2.0rc1/src/bokeh/core/validation/issue.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/core/validation/warnings.py` & `bokeh-3.2.0rc1/src/bokeh/core/validation/warnings.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/document/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/document/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/document/callbacks.py` & `bokeh-3.2.0rc1/src/bokeh/document/callbacks.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/document/document.py` & `bokeh-3.2.0rc1/src/bokeh/document/document.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/document/events.py` & `bokeh-3.2.0rc1/src/bokeh/document/events.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/document/json.py` & `bokeh-3.2.0rc1/src/bokeh/document/json.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/document/locking.py` & `bokeh-3.2.0rc1/src/bokeh/document/locking.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/document/models.py` & `bokeh-3.2.0rc1/src/bokeh/document/models.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/document/modules.py` & `bokeh-3.2.0rc1/src/bokeh/document/modules.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/driving.py` & `bokeh-3.2.0rc1/src/bokeh/driving.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/embed/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/embed/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/embed/bundle.py` & `bokeh-3.2.0rc1/src/bokeh/embed/bundle.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/embed/elements.py` & `bokeh-3.2.0rc1/src/bokeh/embed/elements.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/embed/notebook.py` & `bokeh-3.2.0rc1/src/bokeh/embed/notebook.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/embed/server.py` & `bokeh-3.2.0rc1/src/bokeh/embed/server.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/embed/standalone.py` & `bokeh-3.2.0rc1/src/bokeh/embed/standalone.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/embed/util.py` & `bokeh-3.2.0rc1/src/bokeh/embed/util.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/embed/wrappers.py` & `bokeh-3.2.0rc1/src/bokeh/embed/wrappers.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/events.py` & `bokeh-3.2.0rc1/src/bokeh/events.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/ext.py` & `bokeh-3.2.0rc1/src/bokeh/ext.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/io/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/io/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/io/doc.py` & `bokeh-3.2.0rc1/src/bokeh/io/doc.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/io/export.py` & `bokeh-3.2.0rc1/src/bokeh/io/export.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/io/notebook.py` & `bokeh-3.2.0rc1/src/bokeh/io/notebook.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/io/output.py` & `bokeh-3.2.0rc1/src/bokeh/io/output.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/io/saving.py` & `bokeh-3.2.0rc1/src/bokeh/io/saving.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/io/showing.py` & `bokeh-3.2.0rc1/src/bokeh/io/showing.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/io/state.py` & `bokeh-3.2.0rc1/src/bokeh/io/state.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/io/util.py` & `bokeh-3.2.0rc1/src/bokeh/io/util.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/io/webdriver.py` & `bokeh-3.2.0rc1/src/bokeh/io/webdriver.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/layouts.py` & `bokeh-3.2.0rc1/src/bokeh/layouts.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/model/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/model/data_model.py` & `bokeh-3.2.0rc1/src/bokeh/model/data_model.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/model/docs.py` & `bokeh-3.2.0rc1/src/bokeh/model/docs.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/model/model.py` & `bokeh-3.2.0rc1/src/bokeh/model/model.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/model/util.py` & `bokeh-3.2.0rc1/src/bokeh/model/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 #-----------------------------------------------------------------------------
 
 # Standard library imports
 from typing import TYPE_CHECKING, Any, Callable
 
 # Bokeh imports
 from ..core.has_props import HasProps, Qualified
+from ..util.dataclasses import entries, is_dataclass
 
 if TYPE_CHECKING:
     from ..core.types import ID
     from ..document import Document
     from .model import Model
 
 #-----------------------------------------------------------------------------
@@ -212,14 +213,17 @@
             visit_value_and_its_immediate_references(value, visitor)
     elif issubclass(typ, HasProps):
         if issubclass(typ, Model):
             visitor(obj)
         else:
             # this isn't a Model, so recurse into it
             visit_immediate_value_references(obj, visitor)
+    elif is_dataclass(obj):
+        for _, value in entries(obj):
+            visit_value_and_its_immediate_references(value, visitor)
 
 #-----------------------------------------------------------------------------
 # Private API
 #-----------------------------------------------------------------------------
 
 #-----------------------------------------------------------------------------
 # Code
```

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/annotations/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/models/annotations/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/annotations/annotation.py` & `bokeh-3.2.0rc1/src/bokeh/models/annotations/annotation.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/annotations/arrows.py` & `bokeh-3.2.0rc1/src/bokeh/models/annotations/arrows.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/annotations/geometry.py` & `bokeh-3.2.0rc1/src/bokeh/models/annotations/geometry.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/annotations/html/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/models/annotations/html/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/annotations/html/html_annotation.py` & `bokeh-3.2.0rc1/src/bokeh/models/annotations/html/html_annotation.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/annotations/html/labels.py` & `bokeh-3.2.0rc1/src/bokeh/models/annotations/html/labels.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/annotations/html/toolbars.py` & `bokeh-3.2.0rc1/src/bokeh/models/annotations/html/toolbars.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/annotations/labels.py` & `bokeh-3.2.0rc1/src/bokeh/models/annotations/labels.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/annotations/legends.py` & `bokeh-3.2.0rc1/src/bokeh/models/annotations/legends.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/axes.py` & `bokeh-3.2.0rc1/src/bokeh/models/axes.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/callbacks.py` & `bokeh-3.2.0rc1/src/bokeh/models/callbacks.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/canvas.py` & `bokeh-3.2.0rc1/src/bokeh/models/canvas.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/coordinates.py` & `bokeh-3.2.0rc1/src/bokeh/models/coordinates.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/css.py` & `bokeh-3.2.0rc1/src/bokeh/models/css.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/dom.py` & `bokeh-3.2.0rc1/src/bokeh/models/dom.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/expressions.py` & `bokeh-3.2.0rc1/src/bokeh/models/expressions.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/filters.py` & `bokeh-3.2.0rc1/src/bokeh/models/filters.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/formatters.py` & `bokeh-3.2.0rc1/src/bokeh/models/formatters.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/glyph.py` & `bokeh-3.2.0rc1/src/bokeh/models/glyph.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/glyphs.py` & `bokeh-3.2.0rc1/src/bokeh/models/glyphs.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/graphics.py` & `bokeh-3.2.0rc1/src/bokeh/models/graphics.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/graphs.py` & `bokeh-3.2.0rc1/src/bokeh/models/graphs.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/grids.py` & `bokeh-3.2.0rc1/src/bokeh/models/grids.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/labeling.py` & `bokeh-3.2.0rc1/src/bokeh/models/labeling.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/layouts.py` & `bokeh-3.2.0rc1/src/bokeh/models/layouts.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/map_plots.py` & `bokeh-3.2.0rc1/src/bokeh/models/map_plots.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/mappers.py` & `bokeh-3.2.0rc1/src/bokeh/models/mappers.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/plots.py` & `bokeh-3.2.0rc1/src/bokeh/models/plots.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/ranges.py` & `bokeh-3.2.0rc1/src/bokeh/models/ranges.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/renderers/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/models/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/renderers/contour_renderer.py` & `bokeh-3.2.0rc1/src/bokeh/models/renderers/contour_renderer.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/renderers/glyph_renderer.py` & `bokeh-3.2.0rc1/src/bokeh/models/renderers/glyph_renderer.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/renderers/graph_renderer.py` & `bokeh-3.2.0rc1/src/bokeh/models/renderers/graph_renderer.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/renderers/renderer.py` & `bokeh-3.2.0rc1/src/bokeh/models/renderers/renderer.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/renderers/tile_renderer.py` & `bokeh-3.2.0rc1/src/bokeh/models/renderers/tile_renderer.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/scales.py` & `bokeh-3.2.0rc1/src/bokeh/models/scales.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/selections.py` & `bokeh-3.2.0rc1/src/bokeh/models/selections.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/selectors.py` & `bokeh-3.2.0rc1/src/bokeh/models/selectors.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/sources.py` & `bokeh-3.2.0rc1/src/bokeh/models/sources.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/text.py` & `bokeh-3.2.0rc1/src/bokeh/models/text.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/textures.py` & `bokeh-3.2.0rc1/src/bokeh/models/textures.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/tickers.py` & `bokeh-3.2.0rc1/src/bokeh/models/tickers.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/tiles.py` & `bokeh-3.2.0rc1/src/bokeh/models/tiles.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/tools.py` & `bokeh-3.2.0rc1/src/bokeh/models/tools.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/transforms.py` & `bokeh-3.2.0rc1/src/bokeh/models/transforms.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/ui/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/models/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/ui/dialogs.py` & `bokeh-3.2.0rc1/src/bokeh/models/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/ui/examiner.py` & `bokeh-3.2.0rc1/src/bokeh/models/ui/examiner.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/ui/icons.py` & `bokeh-3.2.0rc1/src/bokeh/models/ui/icons.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/ui/menus.py` & `bokeh-3.2.0rc1/src/bokeh/models/ui/menus.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/ui/panes.py` & `bokeh-3.2.0rc1/src/bokeh/models/ui/panes.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/ui/tooltips.py` & `bokeh-3.2.0rc1/src/bokeh/models/ui/tooltips.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/ui/ui_element.py` & `bokeh-3.2.0rc1/src/bokeh/models/ui/ui_element.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/util/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/models/util/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/util/structure.py` & `bokeh-3.2.0rc1/src/bokeh/models/util/structure.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/widgets/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/models/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/widgets/buttons.py` & `bokeh-3.2.0rc1/src/bokeh/models/widgets/buttons.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/widgets/groups.py` & `bokeh-3.2.0rc1/src/bokeh/models/widgets/groups.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/widgets/inputs.py` & `bokeh-3.2.0rc1/src/bokeh/models/widgets/inputs.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/widgets/markups.py` & `bokeh-3.2.0rc1/src/bokeh/models/widgets/markups.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/widgets/pickers.py` & `bokeh-3.2.0rc1/src/bokeh/models/widgets/pickers.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/widgets/sliders.py` & `bokeh-3.2.0rc1/src/bokeh/models/widgets/sliders.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/widgets/tables.py` & `bokeh-3.2.0rc1/src/bokeh/models/widgets/tables.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/models/widgets/widget.py` & `bokeh-3.2.0rc1/src/bokeh/models/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/palettes.py` & `bokeh-3.2.0rc1/src/bokeh/palettes.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/plotting/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/plotting/_decorators.py` & `bokeh-3.2.0rc1/src/bokeh/plotting/_decorators.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/plotting/_docstring.py` & `bokeh-3.2.0rc1/src/bokeh/plotting/_docstring.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/plotting/_figure.py` & `bokeh-3.2.0rc1/src/bokeh/plotting/_figure.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/plotting/_graph.py` & `bokeh-3.2.0rc1/src/bokeh/plotting/_graph.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/plotting/_legends.py` & `bokeh-3.2.0rc1/src/bokeh/plotting/_legends.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/plotting/_plot.py` & `bokeh-3.2.0rc1/src/bokeh/plotting/_plot.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/plotting/_renderer.py` & `bokeh-3.2.0rc1/src/bokeh/plotting/_renderer.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/plotting/_stack.py` & `bokeh-3.2.0rc1/src/bokeh/plotting/_stack.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/plotting/_tools.py` & `bokeh-3.2.0rc1/src/bokeh/plotting/_tools.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/plotting/contour.py` & `bokeh-3.2.0rc1/src/bokeh/plotting/contour.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/plotting/glyph_api.py` & `bokeh-3.2.0rc1/src/bokeh/plotting/glyph_api.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/plotting/gmap.py` & `bokeh-3.2.0rc1/src/bokeh/plotting/gmap.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/plotting/graph.py` & `bokeh-3.2.0rc1/src/bokeh/plotting/graph.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/protocol/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/protocol/exceptions.py` & `bokeh-3.2.0rc1/src/bokeh/protocol/exceptions.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/protocol/message.py` & `bokeh-3.2.0rc1/src/bokeh/protocol/message.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/protocol/messages/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/protocol/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/protocol/messages/ack.py` & `bokeh-3.2.0rc1/src/bokeh/protocol/messages/ack.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/protocol/messages/error.py` & `bokeh-3.2.0rc1/src/bokeh/protocol/messages/error.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/protocol/messages/ok.py` & `bokeh-3.2.0rc1/src/bokeh/protocol/messages/ok.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/protocol/messages/patch_doc.py` & `bokeh-3.2.0rc1/src/bokeh/protocol/messages/patch_doc.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/protocol/messages/pull_doc_reply.py` & `bokeh-3.2.0rc1/src/bokeh/protocol/messages/pull_doc_reply.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/protocol/messages/pull_doc_req.py` & `bokeh-3.2.0rc1/src/bokeh/protocol/messages/pull_doc_req.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/protocol/messages/push_doc.py` & `bokeh-3.2.0rc1/src/bokeh/protocol/messages/push_doc.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/protocol/messages/server_info_reply.py` & `bokeh-3.2.0rc1/src/bokeh/protocol/messages/server_info_reply.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/protocol/messages/server_info_req.py` & `bokeh-3.2.0rc1/src/bokeh/protocol/messages/server_info_req.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/protocol/receiver.py` & `bokeh-3.2.0rc1/src/bokeh/protocol/receiver.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/resources.py` & `bokeh-3.2.0rc1/src/bokeh/resources.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/USHolidays.ics` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/USHolidays.ics`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/US_Regions_State_Boundaries.csv.gz` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/US_Regions_State_Boundaries.csv.gz`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/auto-mpg.csv` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/auto-mpg.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/auto-mpg2.csv` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/auto-mpg2.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/browsers_nov_2013.csv` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/browsers_nov_2013.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/commits.txt.gz` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/commits.txt.gz`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/daylight_warsaw_2013.csv` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/daylight_warsaw_2013.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/elements.csv` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/elements.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/icons/chrome_32x32.png` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/icons/chrome_32x32.png`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/icons/firefox_32x32.png` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/icons/firefox_32x32.png`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/icons/ie_32x32.png` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/icons/ie_32x32.png`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/icons/opera_32x32.png` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/icons/opera_32x32.png`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/icons/safari_32x32.png` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/icons/safari_32x32.png`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/iris.csv` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/iris.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/les_mis.json` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/les_mis.json`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/numberly.csv` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/numberly.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/obiszow_mtb_xcm.csv` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/obiszow_mtb_xcm.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/olympics2014.json` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/olympics2014.json`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/penguins.csv` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/penguins.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/percent-bachelors-degrees-women-usa.csv` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/percent-bachelors-degrees-women-usa.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/probly.csv` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/probly.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/sample_geojson.geojson` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/sample_geojson.geojson`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/sea_surface_temperature.csv.gz` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/sea_surface_temperature.csv.gz`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/sprint.csv` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/sprint.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/unemployment1948.csv` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/unemployment1948.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/us_marriages_divorces.csv` & `bokeh-3.2.0rc1/src/bokeh/sampledata/_data/us_marriages_divorces.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/airport_routes.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/airport_routes.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/airports.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/airports.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/anscombe.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/anscombe.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/antibiotics.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/antibiotics.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/autompg.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/autompg.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/autompg2.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/autompg2.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/browsers.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/browsers.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/commits.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/commits.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/daylight.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/daylight.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/degrees.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/degrees.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/gapminder.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/gapminder.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/glucose.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/glucose.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/haar_cascade.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/haar_cascade.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/iris.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/iris.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/les_mis.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/les_mis.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/movies_data.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/movies_data.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/mtb.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/mtb.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/olympics2014.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/olympics2014.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/penguins.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/penguins.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/perceptions.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/perceptions.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/periodic_table.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/periodic_table.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/population.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/population.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/sample_geojson.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/sample_geojson.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/sample_superstore.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/sample_superstore.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/sea_surface_temperature.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/sea_surface_temperature.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/sprint.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/sprint.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/stocks.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/stocks.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/unemployment.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/unemployment.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/unemployment1948.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/unemployment1948.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/us_cities.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/us_cities.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/us_counties.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/us_counties.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/us_holidays.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/us_holidays.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/us_marriages_divorces.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/us_marriages_divorces.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/us_states.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/us_states.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sampledata/world_cities.py` & `bokeh-3.2.0rc1/src/bokeh/sampledata/world_cities.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/server/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/auth_provider.py` & `bokeh-3.2.0rc1/src/bokeh/server/auth_provider.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/callbacks.py` & `bokeh-3.2.0rc1/src/bokeh/server/callbacks.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/connection.py` & `bokeh-3.2.0rc1/src/bokeh/server/connection.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/contexts.py` & `bokeh-3.2.0rc1/src/bokeh/server/contexts.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/protocol_handler.py` & `bokeh-3.2.0rc1/src/bokeh/server/protocol_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/server.py` & `bokeh-3.2.0rc1/src/bokeh/server/server.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/session.py` & `bokeh-3.2.0rc1/src/bokeh/server/session.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-api.js` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/bokeh-api.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.0-dev.4");
+    factory(root["Bokeh"], "3.2.0-rc.1");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
```

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-api.min.js` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/bokeh-api.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.0-dev.4");
+    factory(root["Bokeh"], "3.2.0-rc.1");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
```

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-gl.js` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/bokeh-gl.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.0-dev.4");
+    factory(root["Bokeh"], "3.2.0-rc.1");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
```

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-gl.min.js` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/bokeh-gl.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.0-dev.4");
+    factory(root["Bokeh"], "3.2.0-rc.1");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
```

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-mathjax.js` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/bokeh-mathjax.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.0-dev.4");
+    factory(root["Bokeh"], "3.2.0-rc.1");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
```

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-mathjax.min.js` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/bokeh-mathjax.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.0-dev.4");
+    factory(root["Bokeh"], "3.2.0-rc.1");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
```

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-tables.js` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/bokeh-tables.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.0-dev.4");
+    factory(root["Bokeh"], "3.2.0-rc.1");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
```

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-tables.min.js` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/bokeh-tables.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.0-dev.4");
+    factory(root["Bokeh"], "3.2.0-rc.1");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
```

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-widgets.js` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/bokeh-widgets.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.0-dev.4");
+    factory(root["Bokeh"], "3.2.0-rc.1");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
```

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-widgets.min.js` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/bokeh-widgets.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.0-dev.4");
+    factory(root["Bokeh"], "3.2.0-rc.1");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
```

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh.js` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/bokeh.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -748,15 +748,15 @@
                 __esExport("documents", document_1.documents);
                 var safely_1 = require(69) /* ./safely */ ;
                 __esExport("safely", safely_1.safely);
             },
             /* version.js */
             function _(require, module, exports, __esModule, __esExport) {
                 __esModule();
-                exports.version = "3.2.0-dev.4";
+                exports.version = "3.2.0-rc.1";
             },
             /* embed/index.js */
             function _(require, module, exports, __esModule, __esExport) {
                 __esModule();
                 const document_1 = require(5) /* ../document */ ;
                 const settings_1 = require(28) /* ../core/settings */ ;
                 const logging_1 = require(18) /* ../core/logging */ ;
```

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh.min.js` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/bokeh.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -532,16 +532,16 @@
             function _(e, t, o, s, l) {
                 s();
                 const r = e(1);
                 l("version", e(3).version), l("index", e(4).index), o.embed = r.__importStar(e(4)), o.protocol = r.__importStar(e(67)), o._testing = r.__importStar(e(68));
                 var _ = e(18);
                 l("logger", _.logger), l("set_log_level", _.set_log_level), l("settings", e(28).settings), l("Models", e(7).default_resolver), l("documents", e(5).documents), l("safely", e(69).safely)
             },
-            function _(n, e, i, o, v) {
-                o(), i.version = "3.2.0-dev.4"
+            function _(n, c, i, o, r) {
+                o(), i.version = "3.2.0-rc.1"
             },
             function _(e, o, t, n, r) {
                 n();
                 const s = e(5),
                     d = e(28),
                     i = e(18),
                     _ = e(38),
```

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/compiler.js` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/compiler.js`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/charts.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/api/charts.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/figure.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/api/figure.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/glyph_api.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/api/glyph_api.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/gridplot.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/api/gridplot.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/io.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/api/io.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/linalg.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/api/linalg.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/palettes.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/api/palettes.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/parser.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/api/parser.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/themes.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/api/themes.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/client/connection.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/client/connection.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/client/session.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/client/session.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/bokeh_events.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/bokeh_events.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/build_views.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/build_views.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/css.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/css.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/dom.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/dom.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/dom_view.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/dom_view.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/enums.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/enums.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/geometry.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/geometry.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/graphics.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/graphics.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/has_props.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/has_props.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/hittest.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/hittest.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/kinds.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/kinds.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/alignments.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/layout/alignments.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/border.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/layout/border.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/grid.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/layout/grid.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/layoutable.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/layout/layoutable.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/side_panel.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/layout/side_panel.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/types.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/layout/types.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/logging.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/logging.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/patching.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/patching.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/properties.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/properties.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/property_mixins.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/property_mixins.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/selection_manager.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/selection_manager.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/serialization/deserializer.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/serialization/deserializer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/serialization/reps.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/serialization/reps.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/serialization/serializer.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/serialization/serializer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/signaling.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/signaling.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/types.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/types.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/ui_events.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/ui_events.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/uniforms.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/uniforms.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/affine.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/affine.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/algorithms.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/algorithms.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/array.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/array.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/arrayable.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/arrayable.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/bbox.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/bbox.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/bitset.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/bitset.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/canvas.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/canvas.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/cloneable.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/cloneable.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/color.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/color.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/eq.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/eq.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/image.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/image.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/iterator.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/iterator.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/math.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/math.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/matrix.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/matrix.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/menus.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/menus.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/ndarray.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/ndarray.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/object.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/object.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/pretty.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/pretty.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/projections.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/projections.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/ragged_array.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/ragged_array.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/random.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/random.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/svg.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/svg.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/svg_colors.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/svg_colors.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/templating.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/templating.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/text.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/text.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/types.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/types.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/zoom.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/util/zoom.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/vectorization.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/vectorization.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/view.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/view.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/fill.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/visuals/fill.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/hatch.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/visuals/hatch.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/image.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/visuals/image.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/index.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/visuals/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/line.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/visuals/line.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/text.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/visuals/text.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/visual.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/core/visuals/visual.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/document/defs.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/document/defs.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/document/document.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/document/document.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/document/events.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/document/events.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/embed/index.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/embed/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/model.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/model.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/annotation.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/annotation.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/arrow.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/arrow.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/arrow_head.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/arrow_head.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/band.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/band.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/base_color_bar.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/base_color_bar.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/box_annotation.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/box_annotation.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/color_bar.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/color_bar.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/contour_color_bar.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/contour_color_bar.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/data_annotation.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/data_annotation.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/html/label.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/html/label.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/html/label_set.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/html/label_set.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/html/text_annotation.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/html/text_annotation.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/html/title.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/html/title.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/index.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/label.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/label.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/label_set.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/label_set.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/legend.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/legend.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/legend_item.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/legend_item.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/poly_annotation.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/poly_annotation.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/slope.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/slope.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/span.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/span.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/text_annotation.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/text_annotation.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/title.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/title.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/toolbar_panel.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/toolbar_panel.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/upper_lower.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/upper_lower.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/whisker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/annotations/whisker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/axis.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/axes/axis.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/categorical_axis.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/axes/categorical_axis.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/continuous_axis.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/axes/continuous_axis.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/datetime_axis.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/axes/datetime_axis.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/linear_axis.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/axes/linear_axis.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/log_axis.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/axes/log_axis.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/mercator_axis.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/axes/mercator_axis.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/callbacks/callback.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/callbacks/callback.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/callbacks/customjs.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/callbacks/customjs.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/callbacks/open_url.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/callbacks/open_url.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/callbacks/set_value.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/callbacks/set_value.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/canvas/canvas.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/canvas/canvas.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/canvas/cartesian_frame.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/canvas/cartesian_frame.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/common/kinds.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/common/kinds.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/common/resolve.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/common/resolve.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/coordinates/coordinate_mapping.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/coordinates/coordinate_mapping.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/action.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/action.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/color_ref.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/color_ref.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/dom_element.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/dom_element.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/dom_node.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/dom_node.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/elements.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/elements.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/html.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/html.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/index.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/index_.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/index_.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/placeholder.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/placeholder.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/styles.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/styles.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/stylesheets.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/stylesheets.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/template.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/template.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/text.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/text.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/toggle_group.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/toggle_group.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/value_of.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/value_of.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/value_ref.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/dom/value_ref.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/coordinate_transform.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/expressions/coordinate_transform.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/cumsum.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/expressions/cumsum.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/customjs_expr.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/expressions/customjs_expr.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/expression.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/expressions/expression.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/maximum.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/expressions/maximum.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/minimum.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/expressions/minimum.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/polar.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/expressions/polar.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/stack.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/expressions/stack.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/all_indices.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/filters/all_indices.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/boolean_filter.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/filters/boolean_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/customjs_filter.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/filters/customjs_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/difference_filter.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/filters/difference_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/filter.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/filters/filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/group_filter.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/filters/group_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/index.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/filters/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/index_filter.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/filters/index_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/intersection_filter.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/filters/intersection_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/inversion_filter.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/filters/inversion_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/symmetric_difference_filter.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/filters/symmetric_difference_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/union_filter.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/filters/union_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/basic_tick_formatter.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/formatters/basic_tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/categorical_tick_formatter.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/formatters/categorical_tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/customjs_tick_formatter.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/formatters/customjs_tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/datetime_tick_formatter.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/formatters/datetime_tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/index.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/formatters/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/log_tick_formatter.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/formatters/log_tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/mercator_tick_formatter.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/formatters/mercator_tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/numeral_tick_formatter.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/formatters/numeral_tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/printf_tick_formatter.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/formatters/printf_tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/tick_formatter.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/formatters/tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/annular_wedge.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/annular_wedge.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/annulus.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/annulus.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/arc.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/arc.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/area.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/area.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/bezier.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/bezier.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/block.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/block.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/center_rotatable.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/center_rotatable.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/circle.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/circle.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/ellipse.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/ellipse.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/glyph.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/glyph.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/harea.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/harea.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/harea_step.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/harea_step.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/hbar.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/hbar.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/hex_tile.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/hex_tile.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/hspan.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/hspan.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/hstrip.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/hstrip.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/image.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/image.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/image_base.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/image_base.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/image_rgba.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/image_rgba.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/image_stack.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/image_stack.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/image_url.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/image_url.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/index.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/line.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/line.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/lrtb.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/lrtb.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/marker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/marker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/multi_line.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/multi_line.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/multi_polygons.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/multi_polygons.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/patch.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/patch.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/patches.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/patches.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/quad.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/quad.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/quadratic.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/quadratic.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/ray.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/ray.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/rect.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/rect.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/scatter.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/scatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/segment.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/segment.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/spline.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/spline.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/step.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/step.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/text.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/text.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/utils.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/utils.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/varea.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/varea.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/varea_step.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/varea_step.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/vbar.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/vbar.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/vspan.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/vspan.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/vstrip.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/vstrip.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/annular_wedge.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/annular_wedge.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/annulus.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/annulus.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/base.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/base.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/base_line.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/base_line.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/base_marker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/base_marker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/buffer.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/buffer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/circle.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/circle.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/dash_cache.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/dash_cache.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/line_gl.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/line_gl.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/lrtb.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/lrtb.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/multi_marker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/multi_marker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/regl_wrap.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/regl_wrap.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/single_marker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/single_marker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/step.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/step.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/sxsy.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/sxsy.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/types.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/types.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/webgl_utils.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/webgl_utils.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/wedge.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/webgl/wedge.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/wedge.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/wedge.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/xy_glyph.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/glyphs/xy_glyph.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphics/decoration.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/graphics/decoration.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphics/marking.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/graphics/marking.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphs/graph_hit_test_policy.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/graphs/graph_hit_test_policy.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphs/layout_provider.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/graphs/layout_provider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphs/static_layout_provider.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/graphs/static_layout_provider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/grids/grid.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/grids/grid.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/index.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/alignments.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/alignments.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/column.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/column.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/css_grid_box.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/css_grid_box.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/flex_box.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/flex_box.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/grid_box.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/grid_box.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/group_box.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/group_box.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/hbox.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/hbox.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/layout_dom.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/layout_dom.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/row.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/row.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/scroll_box.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/scroll_box.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/spacer.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/spacer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/tab_panel.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/tab_panel.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/tabs.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/tabs.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/vbox.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/layouts/vbox.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/categorical_color_mapper.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/categorical_color_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/categorical_mapper.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/categorical_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/categorical_marker_mapper.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/categorical_marker_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/categorical_pattern_mapper.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/categorical_pattern_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/color_mapper.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/color_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/continuous_color_mapper.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/continuous_color_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/eqhist_color_mapper.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/eqhist_color_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/index.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/linear_color_mapper.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/linear_color_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/log_color_mapper.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/log_color_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/mapper.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/scanning_color_mapper.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/scanning_color_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/weighted_stack_color_mapper.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/mappers/weighted_stack_color_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/action.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/menus/action.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/check_action.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/menus/check_action.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/divider.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/menus/divider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/menu.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/menus/menu.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/menu_item.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/menus/menu_item.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/section.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/menus/section.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/figure.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/plots/figure.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/gmap.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/plots/gmap.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/gmap_plot.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/plots/gmap_plot.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/gmap_plot_canvas.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/plots/gmap_plot_canvas.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/grid_plot.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/plots/grid_plot.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/plot.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/plots/plot.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/plot_canvas.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/plots/plot_canvas.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/range_manager.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/plots/range_manager.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/state_manager.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/plots/state_manager.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/policies/labeling.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/policies/labeling.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/random/park_miller_lcg.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/random/park_miller_lcg.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/random/random_generator.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/random/random_generator.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ranges/data_range.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ranges/data_range.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ranges/data_range1d.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ranges/data_range1d.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ranges/factor_range.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ranges/factor_range.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ranges/range.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ranges/range.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ranges/range1d.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ranges/range1d.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/contour_renderer.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/renderers/contour_renderer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/data_renderer.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/renderers/data_renderer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/glyph_renderer.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/renderers/glyph_renderer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/graph_renderer.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/renderers/graph_renderer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/guide_renderer.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/renderers/guide_renderer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/renderer.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/renderers/renderer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/categorical_scale.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/scales/categorical_scale.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/linear_interpolation_scale.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/scales/linear_interpolation_scale.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/linear_scale.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/scales/linear_scale.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/log_scale.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/scales/log_scale.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/scale.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/scales/scale.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selections/interaction_policy.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/selections/interaction_policy.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selections/selection.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/selections/selection.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selectors/selector.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/selectors/selector.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/ajax_data_source.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/sources/ajax_data_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/cds_view.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/sources/cds_view.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/column_data_source.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/sources/column_data_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/columnar_data_source.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/sources/columnar_data_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/data_source.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/sources/data_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/geojson_data_source.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/sources/geojson_data_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/server_sent_data_source.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/sources/server_sent_data_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/web_data_source.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/sources/web_data_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/base_text.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/text/base_text.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/math_text.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/text/math_text.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/plain_text.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/text/plain_text.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/providers.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/text/providers.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/textures/canvas_texture.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/textures/canvas_texture.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/textures/image_url_texture.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/textures/image_url_texture.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/textures/texture.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/textures/texture.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/adaptive_ticker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/adaptive_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/binned_ticker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/binned_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/categorical_ticker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/categorical_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/composite_ticker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/composite_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/continuous_ticker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/continuous_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/days_ticker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/days_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/fixed_ticker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/fixed_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/index.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/log_ticker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/log_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/mercator_ticker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/mercator_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/months_ticker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/months_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/single_interval_ticker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/single_interval_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/ticker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/years_ticker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tickers/years_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/bbox_tile_source.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tiles/bbox_tile_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/mercator_tile_source.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tiles/mercator_tile_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/quadkey_tile_source.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tiles/quadkey_tile_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/tile_renderer.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tiles/tile_renderer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/tile_source.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tiles/tile_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/tms_tile_source.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tiles/tms_tile_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/wmts_tile_source.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tiles/wmts_tile_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/action_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/action_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/copy_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/copy_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/custom_action.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/custom_action.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/examine_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/examine_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/fullscreen_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/fullscreen_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/help_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/help_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/index.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/plot_action_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/plot_action_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/redo_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/redo_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/reset_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/reset_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/save_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/save_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/undo_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/undo_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/zoom_base_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/zoom_base_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/zoom_in_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/zoom_in_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/zoom_out_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/actions/zoom_out_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/click_button.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/click_button.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/box_edit_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/edit/box_edit_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/edit_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/edit/edit_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/freehand_draw_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/edit/freehand_draw_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/line_edit_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/edit/line_edit_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/line_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/edit/line_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/point_draw_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/edit/point_draw_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/poly_draw_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/edit/poly_draw_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/poly_edit_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/edit/poly_edit_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/poly_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/edit/poly_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/box_select_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/box_select_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/box_zoom_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/box_zoom_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/gesture_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/gesture_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/index.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/lasso_select_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/lasso_select_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/pan_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/pan_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/poly_select_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/poly_select_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/range_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/range_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/region_select_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/region_select_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/select_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/select_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/tap_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/tap_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/wheel_pan_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/wheel_pan_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/wheel_zoom_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/gestures/wheel_zoom_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/inspectors/crosshair_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/inspectors/crosshair_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/inspectors/customjs_hover.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/inspectors/customjs_hover.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/inspectors/hover_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/inspectors/hover_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/inspectors/inspect_tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/inspectors/inspect_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/on_off_button.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/on_off_button.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/tool.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/tool_button.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/tool_button.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/tool_proxy.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/tool_proxy.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/toolbar.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/tools/toolbar.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/customjs_transform.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/transforms/customjs_transform.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/interpolator.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/transforms/interpolator.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/jitter.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/transforms/jitter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/linear_interpolator.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/transforms/linear_interpolator.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/range_transform.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/transforms/range_transform.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/step_interpolator.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/transforms/step_interpolator.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/transform.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/transforms/transform.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/dialog.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ui/dialog.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/examiner.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ui/examiner.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/icons/builtin_icon.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ui/icons/builtin_icon.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/icons/icon.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ui/icons/icon.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/icons/svg_icon.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ui/icons/svg_icon.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/icons/tabler_icon.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ui/icons/tabler_icon.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/pane.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ui/pane.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/tooltip.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ui/tooltip.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/ui_element.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/ui/ui_element.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/abstract_button.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/abstract_button.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/abstract_slider.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/abstract_slider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/autocomplete_input.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/autocomplete_input.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/base_date_picker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/base_date_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/base_datetime_picker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/base_datetime_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/button.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/button.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/checkbox.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/checkbox.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/checkbox_button_group.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/checkbox_button_group.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/checkbox_group.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/checkbox_group.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/color_picker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/color_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/control.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/control.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/date_picker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/date_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/date_range_picker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/date_range_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/date_range_slider.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/date_range_slider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/date_slider.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/date_slider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/datetime_picker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/datetime_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/datetime_range_picker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/datetime_range_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/datetime_range_slider.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/datetime_range_slider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/div.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/div.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/dropdown.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/dropdown.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/file_input.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/file_input.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/help_button.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/help_button.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/index.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/input_widget.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/input_widget.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/markup.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/markup.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/multi_choice.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/multi_choice.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/multiple_date_picker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/multiple_date_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/multiple_datetime_picker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/multiple_datetime_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/multiselect.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/multiselect.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/numeric_input.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/numeric_input.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/oriented_control.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/oriented_control.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/paragraph.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/paragraph.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/password_input.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/password_input.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/picker_base.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/picker_base.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/pretext.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/pretext.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/radio_button_group.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/radio_button_group.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/radio_group.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/radio_group.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/range_slider.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/range_slider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/selectbox.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/selectbox.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/slider.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/slider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/spinner.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/spinner.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/switch.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/switch.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/cell_editors.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/tables/cell_editors.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/cell_formatters.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/tables/cell_formatters.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/data_cube.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/tables/data_cube.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/data_table.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/tables/data_table.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/row_aggregators.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/tables/row_aggregators.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/table_column.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/tables/table_column.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/table_widget.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/tables/table_widget.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/text_input.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/text_input.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/text_like_input.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/text_like_input.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/textarea_input.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/textarea_input.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/time_picker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/time_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/toggle.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/toggle.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/toggle_button_group.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/toggle_button_group.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/toggle_input.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/toggle_input.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/toggle_input_group.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/toggle_input_group.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/widget.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/models/widgets/widget.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/protocol/message.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/protocol/message.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/protocol/receiver.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/protocol/receiver.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/icons.css.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/js/lib/styles/icons.css.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.decorators.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.decorators.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.decorators.legacy.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.decorators.legacy.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.dom.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.dom.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.dom.iterable.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.dom.iterable.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.collection.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2015.collection.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.core.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2015.core.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2015.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.generator.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2015.generator.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.iterable.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2015.iterable.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.promise.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2015.promise.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.proxy.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2015.proxy.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.reflect.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2015.reflect.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.symbol.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2015.symbol.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.symbol.wellknown.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2015.symbol.wellknown.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2016.array.include.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2016.array.include.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2016.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2016.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2016.full.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2016.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2017.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.full.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2017.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.intl.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2017.intl.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.object.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2017.object.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.sharedmemory.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2017.sharedmemory.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.string.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2017.string.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.typedarrays.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2017.typedarrays.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.asyncgenerator.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2018.asyncgenerator.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.asynciterable.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2018.asynciterable.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2018.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.full.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2018.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.intl.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2018.intl.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.promise.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2018.promise.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.regexp.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2018.regexp.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.array.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2019.array.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2019.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.full.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2019.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.intl.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2019.intl.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.object.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2019.object.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.string.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2019.string.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.symbol.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2019.symbol.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.bigint.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2020.bigint.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2020.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.date.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2020.date.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.full.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2020.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.intl.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2020.intl.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.number.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2020.number.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.promise.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2020.promise.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.sharedmemory.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2020.sharedmemory.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.string.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2020.string.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.symbol.wellknown.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2020.symbol.wellknown.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2021.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2021.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2021.full.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2021.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2021.intl.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2021.intl.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2021.promise.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2021.promise.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2021.string.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2021.string.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2021.weakref.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2021.weakref.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.array.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2022.array.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2022.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.error.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2022.error.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.full.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2022.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.intl.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2022.intl.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.object.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2022.object.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.regexp.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2022.regexp.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.sharedmemory.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2022.sharedmemory.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.string.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2022.string.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2023.array.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2023.array.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2023.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2023.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2023.full.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es2023.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es5.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es5.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es6.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.es6.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.esnext.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.esnext.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.esnext.full.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.esnext.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.esnext.intl.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.esnext.intl.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.scripthost.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.scripthost.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.webworker.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.webworker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.webworker.importscripts.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.webworker.importscripts.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.webworker.iterable.d.ts` & `bokeh-3.2.0rc1/src/bokeh/server/static/lib/lib.webworker.iterable.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/tornado.py` & `bokeh-3.2.0rc1/src/bokeh/server/tornado.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/urls.py` & `bokeh-3.2.0rc1/src/bokeh/server/urls.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/util.py` & `bokeh-3.2.0rc1/src/bokeh/server/util.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/views/app_index.html` & `bokeh-3.2.0rc1/src/bokeh/server/views/app_index.html`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/views/auth_request_handler.py` & `bokeh-3.2.0rc1/src/bokeh/server/views/auth_request_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/views/autoload_js_handler.py` & `bokeh-3.2.0rc1/src/bokeh/server/views/autoload_js_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/views/bokeh-dev.ico` & `bokeh-3.2.0rc1/src/bokeh/server/views/bokeh-dev.ico`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/views/bokeh.ico` & `bokeh-3.2.0rc1/src/bokeh/server/views/bokeh.ico`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/views/doc_handler.py` & `bokeh-3.2.0rc1/src/bokeh/server/views/doc_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/views/ico_handler.py` & `bokeh-3.2.0rc1/src/bokeh/server/views/ico_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/views/metadata_handler.py` & `bokeh-3.2.0rc1/src/bokeh/server/views/metadata_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/views/multi_root_static_handler.py` & `bokeh-3.2.0rc1/src/bokeh/server/views/multi_root_static_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/views/root_handler.py` & `bokeh-3.2.0rc1/src/bokeh/server/views/root_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/views/session_handler.py` & `bokeh-3.2.0rc1/src/bokeh/server/views/session_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/views/static_handler.py` & `bokeh-3.2.0rc1/src/bokeh/server/views/static_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/server/views/ws.py` & `bokeh-3.2.0rc1/src/bokeh/server/views/ws.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/settings.py` & `bokeh-3.2.0rc1/src/bokeh/settings.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/bokehjs_codepen_init.html` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/_templates/bokehjs_codepen_init.html`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/gallery_page.rst` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/_templates/gallery_page.rst`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/release_detail.rst` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/_templates/release_detail.rst`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_autodoc.py` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_autodoc.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_color.py` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_color.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_dataframe.py` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_dataframe.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_directive.py` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_directive.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_enum.py` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_enum.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_example_metadata.py` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_example_metadata.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_gallery.py` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_gallery.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_jinja.py` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_jinja.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_model.py` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_model.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_options.py` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_options.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_palette.py` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_palette.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_palette_group.py` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_palette_group.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_plot.py` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_plot.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_prop.py` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_prop.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_releases.py` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_releases.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_roles.py` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_roles.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_sampledata_xref.py` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_sampledata_xref.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_settings.py` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_settings.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_sitemap.py` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/bokeh_sitemap.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokehjs_content.py` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/bokehjs_content.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/example_handler.py` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/example_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/sample.py` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/sample.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/templates.py` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/templates.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/sphinxext/util.py` & `bokeh-3.2.0rc1/src/bokeh/sphinxext/util.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/themes/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/themes/_caliber.py` & `bokeh-3.2.0rc1/src/bokeh/themes/_caliber.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/themes/_contrast.py` & `bokeh-3.2.0rc1/src/bokeh/themes/_contrast.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/themes/_dark_minimal.py` & `bokeh-3.2.0rc1/src/bokeh/themes/_dark_minimal.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/themes/_light_minimal.py` & `bokeh-3.2.0rc1/src/bokeh/themes/_light_minimal.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/themes/_night_sky.py` & `bokeh-3.2.0rc1/src/bokeh/themes/_night_sky.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/themes/theme.py` & `bokeh-3.2.0rc1/src/bokeh/themes/theme.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,29 +115,30 @@
                     text_color: "white"
 
         Here is the same theme, in JSON format:
 
         .. code-block:: python
 
             {
-            'attrs' : {
-                'Plot': {
-                    'background_fill_color': '#2F2F2F',
-                    'border_fill_color': '#2F2F2F',
-                    'outline_line_color': '#444444',
-                },
-                'Axis': {
-                    'axis_line_color': null,
-                },
-                'Grid': {
-                    'grid_line_dash': [6, 4]',
-                    'grid_line_alpha': .3,
-                },
-                'Title': {
-                    'text_color': 'white'
+                'attrs' : {
+                    'Plot': {
+                        'background_fill_color': '#2F2F2F',
+                        'border_fill_color': '#2F2F2F',
+                        'outline_line_color': '#444444',
+                    },
+                    'Axis': {
+                        'axis_line_color': None,
+                    },
+                    'Grid': {
+                        'grid_line_dash': [6, 4],
+                        'grid_line_alpha': .3,
+                    },
+                    'Title': {
+                        'text_color': 'white'
+                    }
                 }
             }
 
     '''
 
     _by_class_cache: dict[str, dict[str, Any]]
```

### Comparing `bokeh-3.2.0.dev4/src/bokeh/tile_providers.py` & `bokeh-3.2.0rc1/src/bokeh/tile_providers.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/transform.py` & `bokeh-3.2.0rc1/src/bokeh/transform.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/util/__init__.py` & `bokeh-3.2.0rc1/src/bokeh/util/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/util/browser.py` & `bokeh-3.2.0rc1/src/bokeh/util/browser.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/util/callback_manager.py` & `bokeh-3.2.0rc1/src/bokeh/util/callback_manager.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/util/compiler.py` & `bokeh-3.2.0rc1/src/bokeh/util/compiler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/util/dataclasses.py` & `bokeh-3.2.0rc1/src/bokeh/util/dataclasses.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/util/datatypes.py` & `bokeh-3.2.0rc1/src/bokeh/util/datatypes.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/util/dependencies.py` & `bokeh-3.2.0rc1/src/bokeh/util/dependencies.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/util/deprecation.py` & `bokeh-3.2.0rc1/src/bokeh/util/deprecation.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/util/functions.py` & `bokeh-3.2.0rc1/src/bokeh/util/functions.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/util/hex.py` & `bokeh-3.2.0rc1/src/bokeh/util/hex.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/util/logconfig.py` & `bokeh-3.2.0rc1/src/bokeh/util/logconfig.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/util/options.py` & `bokeh-3.2.0rc1/src/bokeh/util/options.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/util/package.py` & `bokeh-3.2.0rc1/src/bokeh/util/package.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/util/paths.py` & `bokeh-3.2.0rc1/src/bokeh/util/paths.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/util/sampledata.json` & `bokeh-3.2.0rc1/src/bokeh/util/sampledata.json`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/util/sampledata.py` & `bokeh-3.2.0rc1/src/bokeh/util/sampledata.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/util/serialization.py` & `bokeh-3.2.0rc1/src/bokeh/util/serialization.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/util/strings.py` & `bokeh-3.2.0rc1/src/bokeh/util/strings.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/util/terminal.py` & `bokeh-3.2.0rc1/src/bokeh/util/terminal.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/util/token.py` & `bokeh-3.2.0rc1/src/bokeh/util/token.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/util/tornado.py` & `bokeh-3.2.0rc1/src/bokeh/util/tornado.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/util/version.py` & `bokeh-3.2.0rc1/src/bokeh/util/version.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh/util/warnings.py` & `bokeh-3.2.0rc1/src/bokeh/util/warnings.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/src/bokeh.egg-info/PKG-INFO` & `bokeh-3.2.0rc1/src/bokeh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bokeh
-Version: 3.2.0.dev4
+Version: 3.2.0rc1
 Summary: Interactive plots and applications in the browser from Python
 Author: Bokeh Team
 Author-email: info@bokeh.org
 License: Copyright (c) 2012 - 2023, Anaconda, Inc., and Bokeh Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
```

### Comparing `bokeh-3.2.0.dev4/src/bokeh.egg-info/SOURCES.txt` & `bokeh-3.2.0rc1/src/bokeh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/tests/test_bokehjs.py` & `bokeh-3.2.0rc1/tests/test_bokehjs.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/tests/test_cross.py` & `bokeh-3.2.0rc1/tests/test_cross.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/tests/test_defaults.py` & `bokeh-3.2.0rc1/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev4/tests/test_examples.py` & `bokeh-3.2.0rc1/tests/test_examples.py`

 * *Files identical despite different names*

