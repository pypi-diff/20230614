# Comparing `tmp/mlc-tools-0.4.674.tar.gz` & `tmp/mlc-tools-0.4.675.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mlc-tools-0.4.674.tar", last modified: Sun Dec 22 05:34:44 2019, max compression
+gzip compressed data, was "dist/mlc-tools-0.4.675.tar", last modified: Sun Dec 22 07:13:36 2019, max compression
```

## Comparing `mlc-tools-0.4.674.tar` & `mlc-tools-0.4.675.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-22 05:34:44.339167 mlc-tools-0.4.674/
--rw-r--r--   0 runner    (1001) docker     (115)       17 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (115)     3563 2019-12-22 05:34:44.339167 mlc-tools-0.4.674/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     2561 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/README.md
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-22 05:34:44.315167 mlc-tools-0.4.674/mlc_tools/
--rw-r--r--   0 runner    (1001) docker     (115)       71 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-22 05:34:44.319167 mlc-tools-0.4.674/mlc_tools/base/
--rw-r--r--   0 runner    (1001) docker     (115)      227 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     1034 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/base/circular_reference.py
--rw-r--r--   0 runner    (1001) docker     (115)     5282 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/base/data_parser.py
--rw-r--r--   0 runner    (1001) docker     (115)      328 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/base/generator.py
--rw-r--r--   0 runner    (1001) docker     (115)     5184 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/base/generator_data_storage_base.py
--rw-r--r--   0 runner    (1001) docker     (115)     2618 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/base/generator_operator_equals.py
--rw-r--r--   0 runner    (1001) docker     (115)     7275 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/base/generator_unit_tests_interface.py
--rw-r--r--   0 runner    (1001) docker     (115)     5240 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/base/generator_visitor.py
--rw-r--r--   0 runner    (1001) docker     (115)     1135 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/base/language.py
--rw-r--r--   0 runner    (1001) docker     (115)     5123 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/base/linker.py
--rw-r--r--   0 runner    (1001) docker     (115)     2680 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/base/model.py
--rw-r--r--   0 runner    (1001) docker     (115)    13469 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/base/parser.py
--rw-r--r--   0 runner    (1001) docker     (115)     2899 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/base/save_plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (115)     5735 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/base/serializer_base.py
--rw-r--r--   0 runner    (1001) docker     (115)     3364 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/base/translator_base.py
--rw-r--r--   0 runner    (1001) docker     (115)     1099 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/base/validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     5885 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/base/writer_base.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-22 05:34:44.319167 mlc-tools-0.4.674/mlc_tools/console/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     4234 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/console/arguments.py
--rw-r--r--   0 runner    (1001) docker     (115)     1706 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/console/config.py
--rw-r--r--   0 runner    (1001) docker     (115)     7360 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/console/console.py
--rw-r--r--   0 runner    (1001) docker     (115)     1371 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/console/files.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-22 05:34:44.323167 mlc-tools-0.4.674/mlc_tools/core/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     8112 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/core/class_.py
--rw-r--r--   0 runner    (1001) docker     (115)     2908 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/core/function.py
--rw-r--r--   0 runner    (1001) docker     (115)      680 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/core/modifiers.py
--rw-r--r--   0 runner    (1001) docker     (115)     4625 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/core/object.py
--rw-r--r--   0 runner    (1001) docker     (115)     1313 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/main.py
--rw-r--r--   0 runner    (1001) docker     (115)     6651 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/mlc_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-22 05:34:44.323167 mlc-tools-0.4.674/mlc_tools/module_cpp/
--rw-r--r--   0 runner    (1001) docker     (115)      166 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_cpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)    23375 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_cpp/cpp_extension.py
--rw-r--r--   0 runner    (1001) docker     (115)      745 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_cpp/generator.py
--rw-r--r--   0 runner    (1001) docker     (115)     2221 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_cpp/generator_data_storage.py
--rw-r--r--   0 runner    (1001) docker     (115)     4833 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_cpp/generator_observer.py
--rw-r--r--   0 runner    (1001) docker     (115)      815 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_cpp/generator_operator_equals.py
--rw-r--r--   0 runner    (1001) docker     (115)     1811 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_cpp/generator_predefined_files.py
--rw-r--r--   0 runner    (1001) docker     (115)    10172 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_cpp/protocols.py
--rw-r--r--   0 runner    (1001) docker     (115)     1531 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_cpp/regex.py
--rw-r--r--   0 runner    (1001) docker     (115)     1405 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_cpp/registrar.py
--rw-r--r--   0 runner    (1001) docker     (115)      258 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_cpp/save_plugin.py
--rw-r--r--   0 runner    (1001) docker     (115)     7947 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_cpp/serializer.py
--rw-r--r--   0 runner    (1001) docker     (115)     7671 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_cpp/translator.py
--rw-r--r--   0 runner    (1001) docker     (115)    22342 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_cpp/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-22 05:34:44.327167 mlc-tools-0.4.674/mlc_tools/module_js/
--rw-r--r--   0 runner    (1001) docker     (115)      166 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_js/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)      908 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_js/generator.py
--rw-r--r--   0 runner    (1001) docker     (115)      779 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_js/generator_config.py
--rw-r--r--   0 runner    (1001) docker     (115)      679 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_js/generator_data_storage.py
--rw-r--r--   0 runner    (1001) docker     (115)     1060 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_js/generator_factory.py
--rw-r--r--   0 runner    (1001) docker     (115)      390 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_js/generator_functions.py
--rw-r--r--   0 runner    (1001) docker     (115)     1405 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_js/generator_observer.py
--rw-r--r--   0 runner    (1001) docker     (115)      638 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_js/generator_operator_value_of.py
--rw-r--r--   0 runner    (1001) docker     (115)     3896 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_js/protocols.py
--rw-r--r--   0 runner    (1001) docker     (115)     8433 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_js/regex.py
--rw-r--r--   0 runner    (1001) docker     (115)      529 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_js/save_plugin.py
--rw-r--r--   0 runner    (1001) docker     (115)     3651 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_js/serializer.py
--rw-r--r--   0 runner    (1001) docker     (115)      645 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_js/translator.py
--rw-r--r--   0 runner    (1001) docker     (115)     3829 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_js/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-22 05:34:44.331167 mlc-tools-0.4.674/mlc_tools/module_php/
--rw-r--r--   0 runner    (1001) docker     (115)      166 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_php/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)      696 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_php/generator.py
--rw-r--r--   0 runner    (1001) docker     (115)      652 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_php/generator_config.py
--rw-r--r--   0 runner    (1001) docker     (115)     6507 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_php/generator_data_storage.py
--rw-r--r--   0 runner    (1001) docker     (115)     3247 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_php/generator_factory.py
--rw-r--r--   0 runner    (1001) docker     (115)     1493 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_php/generator_observer.py
--rw-r--r--   0 runner    (1001) docker     (115)     8302 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_php/protocols.py
--rw-r--r--   0 runner    (1001) docker     (115)     6988 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_php/regex.py
--rw-r--r--   0 runner    (1001) docker     (115)      646 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_php/save_plugin.py
--rw-r--r--   0 runner    (1001) docker     (115)     4209 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_php/serializer.py
--rw-r--r--   0 runner    (1001) docker     (115)     2327 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_php/translator.py
--rw-r--r--   0 runner    (1001) docker     (115)     5014 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_php/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-22 05:34:44.335167 mlc-tools-0.4.674/mlc_tools/module_python/
--rw-r--r--   0 runner    (1001) docker     (115)      166 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     2749 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_python/constants.py
--rw-r--r--   0 runner    (1001) docker     (115)      812 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_python/generator.py
--rw-r--r--   0 runner    (1001) docker     (115)      982 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_python/generator_data_storage.py
--rw-r--r--   0 runner    (1001) docker     (115)      590 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_python/generator_factory.py
--rw-r--r--   0 runner    (1001) docker     (115)     2201 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_python/generator_observer.py
--rw-r--r--   0 runner    (1001) docker     (115)      881 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_python/generator_operator_equals.py
--rw-r--r--   0 runner    (1001) docker     (115)      631 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_python/generator_package.py
--rw-r--r--   0 runner    (1001) docker     (115)    10660 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_python/protocols.py
--rw-r--r--   0 runner    (1001) docker     (115)     7051 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_python/regex.py
--rw-r--r--   0 runner    (1001) docker     (115)      762 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_python/save_plugin.py
--rw-r--r--   0 runner    (1001) docker     (115)     4090 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_python/serializer.py
--rw-r--r--   0 runner    (1001) docker     (115)     3966 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_python/translator.py
--rw-r--r--   0 runner    (1001) docker     (115)     5508 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/module_python/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-22 05:34:44.339167 mlc-tools-0.4.674/mlc_tools/utils/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     3662 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (115)     3684 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (115)     2763 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/mlc_tools/utils/fileutils.py
--rw-r--r--   0 runner    (1001) docker     (115)       21 2019-12-22 05:34:43.000000 mlc-tools-0.4.674/mlc_tools/version.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-22 05:34:44.315167 mlc-tools-0.4.674/mlc_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)     3563 2019-12-22 05:34:44.000000 mlc-tools-0.4.674/mlc_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     3484 2019-12-22 05:34:44.000000 mlc-tools-0.4.674/mlc_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2019-12-22 05:34:44.000000 mlc-tools-0.4.674/mlc_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)       56 2019-12-22 05:34:44.000000 mlc-tools-0.4.674/mlc_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (115)       21 2019-12-22 05:34:44.000000 mlc-tools-0.4.674/mlc_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (115)       38 2019-12-22 05:34:44.339167 mlc-tools-0.4.674/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (115)      852 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-22 05:34:44.339167 mlc-tools-0.4.674/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)    12518 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/unit_tests/test_base_parser.py
--rw-r--r--   0 runner    (1001) docker     (115)     2956 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/unit_tests/test_core_function_parse.py
--rw-r--r--   0 runner    (1001) docker     (115)     6817 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/unit_tests/test_core_object_parse.py
--rw-r--r--   0 runner    (1001) docker     (115)     9620 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/unit_tests/test_module_writer.py
--rw-r--r--   0 runner    (1001) docker     (115)      569 2019-12-22 05:34:31.000000 mlc-tools-0.4.674/unit_tests/test_utils_common.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-22 07:13:36.675385 mlc-tools-0.4.675/
+-rw-r--r--   0 runner    (1001) docker     (115)       17 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (115)     3563 2019-12-22 07:13:36.675385 mlc-tools-0.4.675/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)     2561 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/README.md
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-22 07:13:36.659385 mlc-tools-0.4.675/mlc_tools/
+-rw-r--r--   0 runner    (1001) docker     (115)       71 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-22 07:13:36.663385 mlc-tools-0.4.675/mlc_tools/base/
+-rw-r--r--   0 runner    (1001) docker     (115)      227 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1034 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/base/circular_reference.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5282 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/base/data_parser.py
+-rw-r--r--   0 runner    (1001) docker     (115)      328 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/base/generator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5184 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/base/generator_data_storage_base.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2618 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/base/generator_operator_equals.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7275 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/base/generator_unit_tests_interface.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5240 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/base/generator_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1135 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/base/language.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5123 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/base/linker.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2680 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/base/model.py
+-rw-r--r--   0 runner    (1001) docker     (115)    13469 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/base/parser.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2899 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/base/save_plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5735 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/base/serializer_base.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3364 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/base/translator_base.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1099 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/base/validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5885 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/base/writer_base.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-22 07:13:36.667385 mlc-tools-0.4.675/mlc_tools/console/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4234 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/console/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1706 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/console/config.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7360 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/console/console.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1371 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/console/files.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-22 07:13:36.667385 mlc-tools-0.4.675/mlc_tools/core/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     8112 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/core/class_.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2908 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/core/function.py
+-rw-r--r--   0 runner    (1001) docker     (115)      680 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/core/modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4625 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/core/object.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1313 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/main.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6651 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/mlc_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-22 07:13:36.667385 mlc-tools-0.4.675/mlc_tools/module_cpp/
+-rw-r--r--   0 runner    (1001) docker     (115)      166 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_cpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)    23375 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_cpp/cpp_extension.py
+-rw-r--r--   0 runner    (1001) docker     (115)      745 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_cpp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2221 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_cpp/generator_data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4833 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_cpp/generator_observer.py
+-rw-r--r--   0 runner    (1001) docker     (115)      815 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_cpp/generator_operator_equals.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1811 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_cpp/generator_predefined_files.py
+-rw-r--r--   0 runner    (1001) docker     (115)    10172 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_cpp/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1531 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_cpp/regex.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1405 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_cpp/registrar.py
+-rw-r--r--   0 runner    (1001) docker     (115)      258 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_cpp/save_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7947 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_cpp/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7671 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_cpp/translator.py
+-rw-r--r--   0 runner    (1001) docker     (115)    22342 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_cpp/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-22 07:13:36.671385 mlc-tools-0.4.675/mlc_tools/module_js/
+-rw-r--r--   0 runner    (1001) docker     (115)      166 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_js/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)      908 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_js/generator.py
+-rw-r--r--   0 runner    (1001) docker     (115)      779 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_js/generator_config.py
+-rw-r--r--   0 runner    (1001) docker     (115)      679 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_js/generator_data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1060 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_js/generator_factory.py
+-rw-r--r--   0 runner    (1001) docker     (115)      390 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_js/generator_functions.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1405 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_js/generator_observer.py
+-rw-r--r--   0 runner    (1001) docker     (115)      638 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_js/generator_operator_value_of.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3896 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_js/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (115)     8433 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_js/regex.py
+-rw-r--r--   0 runner    (1001) docker     (115)      529 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_js/save_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3651 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_js/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (115)      645 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_js/translator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3829 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_js/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-22 07:13:36.671385 mlc-tools-0.4.675/mlc_tools/module_php/
+-rw-r--r--   0 runner    (1001) docker     (115)      166 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_php/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)      696 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_php/generator.py
+-rw-r--r--   0 runner    (1001) docker     (115)      652 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_php/generator_config.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6507 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_php/generator_data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3247 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_php/generator_factory.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1493 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_php/generator_observer.py
+-rw-r--r--   0 runner    (1001) docker     (115)     8302 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_php/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6988 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_php/regex.py
+-rw-r--r--   0 runner    (1001) docker     (115)      646 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_php/save_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4209 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_php/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2327 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_php/translator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5014 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_php/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-22 07:13:36.675385 mlc-tools-0.4.675/mlc_tools/module_python/
+-rw-r--r--   0 runner    (1001) docker     (115)      166 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2749 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_python/constants.py
+-rw-r--r--   0 runner    (1001) docker     (115)      812 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_python/generator.py
+-rw-r--r--   0 runner    (1001) docker     (115)      982 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_python/generator_data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (115)      590 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_python/generator_factory.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2201 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_python/generator_observer.py
+-rw-r--r--   0 runner    (1001) docker     (115)      881 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_python/generator_operator_equals.py
+-rw-r--r--   0 runner    (1001) docker     (115)      631 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_python/generator_package.py
+-rw-r--r--   0 runner    (1001) docker     (115)    10660 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_python/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7051 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_python/regex.py
+-rw-r--r--   0 runner    (1001) docker     (115)      762 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_python/save_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4090 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_python/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3966 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_python/translator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5508 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/module_python/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-22 07:13:36.675385 mlc-tools-0.4.675/mlc_tools/utils/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3662 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3684 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2763 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/mlc_tools/utils/fileutils.py
+-rw-r--r--   0 runner    (1001) docker     (115)       21 2019-12-22 07:13:36.000000 mlc-tools-0.4.675/mlc_tools/version.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-22 07:13:36.663385 mlc-tools-0.4.675/mlc_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (115)     3563 2019-12-22 07:13:36.000000 mlc-tools-0.4.675/mlc_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)     3484 2019-12-22 07:13:36.000000 mlc-tools-0.4.675/mlc_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        1 2019-12-22 07:13:36.000000 mlc-tools-0.4.675/mlc_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       56 2019-12-22 07:13:36.000000 mlc-tools-0.4.675/mlc_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       21 2019-12-22 07:13:36.000000 mlc-tools-0.4.675/mlc_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       38 2019-12-22 07:13:36.675385 mlc-tools-0.4.675/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (115)      852 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-22 07:13:36.675385 mlc-tools-0.4.675/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)    12518 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/unit_tests/test_base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2956 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/unit_tests/test_core_function_parse.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6817 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/unit_tests/test_core_object_parse.py
+-rw-r--r--   0 runner    (1001) docker     (115)     9620 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/unit_tests/test_module_writer.py
+-rw-r--r--   0 runner    (1001) docker     (115)      569 2019-12-22 07:13:24.000000 mlc-tools-0.4.675/unit_tests/test_utils_common.py
```

### Comparing `mlc-tools-0.4.674/PKG-INFO` & `mlc-tools-0.4.675/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlc-tools
-Version: 0.4.674
+Version: 0.4.675
 Summary: A tool to generate and translate C++ code to other languages from one code-base.
 Home-page: https://github.com/mlc-tools/mlc-tools
 Author: Vladimir Tolmachev
 Author-email: tolm_vl@hotmail.com
 License: UNKNOWN
 Description: | ci       | Status                                                                                                                                      |
         |----------|---------------------------------------------------------------------------------------------------------------------------------------------|
```

### Comparing `mlc-tools-0.4.674/README.md` & `mlc-tools-0.4.675/README.md`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/base/circular_reference.py` & `mlc-tools-0.4.675/mlc_tools/base/circular_reference.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/base/data_parser.py` & `mlc-tools-0.4.675/mlc_tools/base/data_parser.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/base/generator_data_storage_base.py` & `mlc-tools-0.4.675/mlc_tools/base/generator_data_storage_base.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/base/generator_operator_equals.py` & `mlc-tools-0.4.675/mlc_tools/base/generator_operator_equals.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/base/generator_unit_tests_interface.py` & `mlc-tools-0.4.675/mlc_tools/base/generator_unit_tests_interface.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/base/generator_visitor.py` & `mlc-tools-0.4.675/mlc_tools/base/generator_visitor.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/base/language.py` & `mlc-tools-0.4.675/mlc_tools/base/language.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/base/linker.py` & `mlc-tools-0.4.675/mlc_tools/base/linker.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/base/model.py` & `mlc-tools-0.4.675/mlc_tools/base/model.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/base/parser.py` & `mlc-tools-0.4.675/mlc_tools/base/parser.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/base/save_plugin_base.py` & `mlc-tools-0.4.675/mlc_tools/base/save_plugin_base.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/base/serializer_base.py` & `mlc-tools-0.4.675/mlc_tools/base/serializer_base.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/base/translator_base.py` & `mlc-tools-0.4.675/mlc_tools/base/translator_base.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/base/validator.py` & `mlc-tools-0.4.675/mlc_tools/base/validator.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/base/writer_base.py` & `mlc-tools-0.4.675/mlc_tools/base/writer_base.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/console/arguments.py` & `mlc-tools-0.4.675/mlc_tools/console/arguments.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/console/config.py` & `mlc-tools-0.4.675/mlc_tools/console/config.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/console/console.py` & `mlc-tools-0.4.675/mlc_tools/console/console.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/console/files.py` & `mlc-tools-0.4.675/mlc_tools/console/files.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/core/class_.py` & `mlc-tools-0.4.675/mlc_tools/core/class_.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/core/function.py` & `mlc-tools-0.4.675/mlc_tools/core/function.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/core/modifiers.py` & `mlc-tools-0.4.675/mlc_tools/core/modifiers.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/core/object.py` & `mlc-tools-0.4.675/mlc_tools/core/object.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/main.py` & `mlc-tools-0.4.675/mlc_tools/main.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/mlc_tools.py` & `mlc-tools-0.4.675/mlc_tools/mlc_tools.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_cpp/cpp_extension.py` & `mlc-tools-0.4.675/mlc_tools/module_cpp/cpp_extension.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_cpp/generator.py` & `mlc-tools-0.4.675/mlc_tools/module_cpp/generator.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_cpp/generator_data_storage.py` & `mlc-tools-0.4.675/mlc_tools/module_cpp/generator_data_storage.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_cpp/generator_observer.py` & `mlc-tools-0.4.675/mlc_tools/module_cpp/generator_observer.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_cpp/generator_operator_equals.py` & `mlc-tools-0.4.675/mlc_tools/module_cpp/generator_operator_equals.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_cpp/generator_predefined_files.py` & `mlc-tools-0.4.675/mlc_tools/module_cpp/generator_predefined_files.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_cpp/protocols.py` & `mlc-tools-0.4.675/mlc_tools/module_cpp/protocols.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_cpp/regex.py` & `mlc-tools-0.4.675/mlc_tools/module_cpp/regex.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_cpp/registrar.py` & `mlc-tools-0.4.675/mlc_tools/module_cpp/registrar.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_cpp/serializer.py` & `mlc-tools-0.4.675/mlc_tools/module_cpp/serializer.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_cpp/translator.py` & `mlc-tools-0.4.675/mlc_tools/module_cpp/translator.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_cpp/writer.py` & `mlc-tools-0.4.675/mlc_tools/module_cpp/writer.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_js/generator.py` & `mlc-tools-0.4.675/mlc_tools/module_js/generator.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_js/generator_config.py` & `mlc-tools-0.4.675/mlc_tools/module_js/generator_config.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_js/generator_data_storage.py` & `mlc-tools-0.4.675/mlc_tools/module_js/generator_data_storage.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_js/generator_factory.py` & `mlc-tools-0.4.675/mlc_tools/module_js/generator_factory.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_js/generator_observer.py` & `mlc-tools-0.4.675/mlc_tools/module_js/generator_observer.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_js/generator_operator_value_of.py` & `mlc-tools-0.4.675/mlc_tools/module_js/generator_operator_value_of.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_js/protocols.py` & `mlc-tools-0.4.675/mlc_tools/module_js/protocols.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_js/regex.py` & `mlc-tools-0.4.675/mlc_tools/module_js/regex.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_js/save_plugin.py` & `mlc-tools-0.4.675/mlc_tools/module_js/save_plugin.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_js/serializer.py` & `mlc-tools-0.4.675/mlc_tools/module_js/serializer.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_js/translator.py` & `mlc-tools-0.4.675/mlc_tools/module_js/translator.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_js/writer.py` & `mlc-tools-0.4.675/mlc_tools/module_js/writer.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_php/generator.py` & `mlc-tools-0.4.675/mlc_tools/module_php/generator.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_php/generator_config.py` & `mlc-tools-0.4.675/mlc_tools/module_php/generator_config.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_php/generator_data_storage.py` & `mlc-tools-0.4.675/mlc_tools/module_php/generator_data_storage.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_php/generator_factory.py` & `mlc-tools-0.4.675/mlc_tools/module_php/generator_factory.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_php/generator_observer.py` & `mlc-tools-0.4.675/mlc_tools/module_php/generator_observer.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_php/protocols.py` & `mlc-tools-0.4.675/mlc_tools/module_php/protocols.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_php/regex.py` & `mlc-tools-0.4.675/mlc_tools/module_php/regex.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_php/save_plugin.py` & `mlc-tools-0.4.675/mlc_tools/module_php/save_plugin.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_php/serializer.py` & `mlc-tools-0.4.675/mlc_tools/module_php/serializer.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_php/translator.py` & `mlc-tools-0.4.675/mlc_tools/module_php/translator.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_php/writer.py` & `mlc-tools-0.4.675/mlc_tools/module_php/writer.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_python/constants.py` & `mlc-tools-0.4.675/mlc_tools/module_python/constants.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_python/generator.py` & `mlc-tools-0.4.675/mlc_tools/module_python/generator.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_python/generator_data_storage.py` & `mlc-tools-0.4.675/mlc_tools/module_python/generator_data_storage.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_python/generator_factory.py` & `mlc-tools-0.4.675/mlc_tools/module_python/generator_factory.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_python/generator_observer.py` & `mlc-tools-0.4.675/mlc_tools/module_python/generator_observer.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_python/generator_operator_equals.py` & `mlc-tools-0.4.675/mlc_tools/module_python/generator_operator_equals.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_python/generator_package.py` & `mlc-tools-0.4.675/mlc_tools/module_python/generator_package.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_python/protocols.py` & `mlc-tools-0.4.675/mlc_tools/module_python/protocols.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_python/regex.py` & `mlc-tools-0.4.675/mlc_tools/module_python/regex.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_python/save_plugin.py` & `mlc-tools-0.4.675/mlc_tools/module_python/save_plugin.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_python/serializer.py` & `mlc-tools-0.4.675/mlc_tools/module_python/serializer.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_python/translator.py` & `mlc-tools-0.4.675/mlc_tools/module_python/translator.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/module_python/writer.py` & `mlc-tools-0.4.675/mlc_tools/module_python/writer.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/utils/common.py` & `mlc-tools-0.4.675/mlc_tools/utils/common.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/utils/error.py` & `mlc-tools-0.4.675/mlc_tools/utils/error.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools/utils/fileutils.py` & `mlc-tools-0.4.675/mlc_tools/utils/fileutils.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/mlc_tools.egg-info/PKG-INFO` & `mlc-tools-0.4.675/mlc_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlc-tools
-Version: 0.4.674
+Version: 0.4.675
 Summary: A tool to generate and translate C++ code to other languages from one code-base.
 Home-page: https://github.com/mlc-tools/mlc-tools
 Author: Vladimir Tolmachev
 Author-email: tolm_vl@hotmail.com
 License: UNKNOWN
 Description: | ci       | Status                                                                                                                                      |
         |----------|---------------------------------------------------------------------------------------------------------------------------------------------|
```

### Comparing `mlc-tools-0.4.674/mlc_tools.egg-info/SOURCES.txt` & `mlc-tools-0.4.675/mlc_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/setup.py` & `mlc-tools-0.4.675/setup.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/unit_tests/test_base_parser.py` & `mlc-tools-0.4.675/unit_tests/test_base_parser.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/unit_tests/test_core_function_parse.py` & `mlc-tools-0.4.675/unit_tests/test_core_function_parse.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/unit_tests/test_core_object_parse.py` & `mlc-tools-0.4.675/unit_tests/test_core_object_parse.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/unit_tests/test_module_writer.py` & `mlc-tools-0.4.675/unit_tests/test_module_writer.py`

 * *Files identical despite different names*

### Comparing `mlc-tools-0.4.674/unit_tests/test_utils_common.py` & `mlc-tools-0.4.675/unit_tests/test_utils_common.py`

 * *Files identical despite different names*

