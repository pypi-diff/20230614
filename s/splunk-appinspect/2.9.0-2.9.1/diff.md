# Comparing `tmp/splunk-appinspect-2.9.0.tar.gz` & `tmp/splunk-appinspect-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/splunk-appinspect-2.9.0.tar", last modified: Tue Aug 31 23:48:32 2021, max compression
+gzip compressed data, was "dist/splunk-appinspect-2.9.1.tar", last modified: Thu Sep  2 23:09:26 2021, max compression
```

## Comparing `splunk-appinspect-2.9.0.tar` & `splunk-appinspect-2.9.1.tar`

### file list

```diff
@@ -1,426 +1,426 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:32.000000 splunk-appinspect-2.9.0/
--rw-rw-rw-   0 root         (0) root         (0)      270 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1332 2021-08-31 23:48:32.000000 splunk-appinspect-2.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2625 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      214 2021-08-31 23:48:32.000000 splunk-appinspect-2.9.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3857 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/
--rw-rw-rw-   0 root         (0) root         (0)     1325 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11304 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/alert_actions.py
--rw-rw-rw-   0 root         (0) root         (0)      364 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/alert_actions_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)    41844 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/app.py
--rw-rw-rw-   0 root         (0) root         (0)      413 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/app_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)    48715 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/app_package_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     2713 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/app_util.py
--rw-rw-rw-   0 root         (0) root         (0)      368 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/authentication_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)      353 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/authorize_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/banned_wordlist.txt
--rw-rw-rw-   0 root         (0) root         (0)     1668 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/bias.py
--rw-rw-rw-   0 root         (0) root         (0)       32 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/bias_wordlist.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/check_routine/
--rw-rw-rw-   0 root         (0) root         (0)     4766 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/check_routine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1541 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/check_routine/find_endpoint_usage.py
--rw-rw-rw-   0 root         (0) root         (0)     2626 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/check_routine/find_spl_command_usage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/check_routine/python_ast_searcher/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/check_routine/python_ast_searcher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4243 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/check_routine/python_ast_searcher/ast_searcher.py
--rw-rw-rw-   0 root         (0) root         (0)      294 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/check_routine/python_ast_searcher/node_filters.py
--rw-rw-rw-   0 root         (0) root         (0)     7241 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/check_routine/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/
--rw-rw-rw-   0 root         (0) root         (0)    11174 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_alert_actions_config.py
--rw-rw-rw-   0 root         (0) root         (0)    19522 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_app_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)     8529 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_application_content.py
--rw-rw-rw-   0 root         (0) root         (0)    10593 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_application_structure.py
--rw-rw-rw-   0 root         (0) root         (0)     7091 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_authentication_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)     1935 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_authorize_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)     1243 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_bias_language.py
--rw-rw-rw-   0 root         (0) root         (0)    94581 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_cloud_simple_app.py
--rw-rw-rw-   0 root         (0) root         (0)     9915 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_configuration_files.py
--rw-rw-rw-   0 root         (0) root         (0)    14365 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_custom_commands.py
--rw-rw-rw-   0 root         (0) root         (0)    37993 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_custom_visualizations.py
--rw-rw-rw-   0 root         (0) root         (0)     5603 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_data_models_config.py
--rw-rw-rw-   0 root         (0) root         (0)     3989 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_documentation_for_sensitive_functionality.py
--rw-rw-rw-   0 root         (0) root         (0)     7743 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_documentation_standards.py
--rw-rw-rw-   0 root         (0) root         (0)      581 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_external_data_sources.py
--rw-rw-rw-   0 root         (0) root         (0)     9939 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_indexes_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)      919 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_intellectual_property.py
--rw-rw-rw-   0 root         (0) root         (0)     6629 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_itsi_module_file_structure.py
--rw-rw-rw-   0 root         (0) root         (0)    11886 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_javascript_files.py
--rw-rw-rw-   0 root         (0) root         (0)     3138 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_jquery_standards.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_json_files.py
--rw-rw-rw-   0 root         (0) root         (0)     1254 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_limits_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)     4096 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_lookup_files.py
--rw-rw-rw-   0 root         (0) root         (0)     4680 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_malware.py
--rw-rw-rw-   0 root         (0) root         (0)     2083 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_meta_files.py
--rw-rw-rw-   0 root         (0) root         (0)    13054 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_modular_inputs.py
--rw-rw-rw-   0 root         (0) root         (0)     2841 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_outputs_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)    18574 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_packaging_standards.py
--rw-rw-rw-   0 root         (0) root         (0)     5288 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_potentially_harmful_operations.py
--rw-rw-rw-   0 root         (0) root         (0)    25787 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_props_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)    37368 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_python_files.py
--rw-rw-rw-   0 root         (0) root         (0)     1566 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_readme_spec_files.py
--rw-rw-rw-   0 root         (0) root         (0)     4940 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_rest_endpoints.py
--rw-rw-rw-   0 root         (0) root         (0)    16598 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_saved_searches.py
--rwxrwxrwx   0 root         (0) root         (0)    16806 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_security.py
--rw-rw-rw-   0 root         (0) root         (0)     3223 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_server_configuration_file.py
--rwxrwxrwx   0 root         (0) root         (0)    13821 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_source_and_binaries.py
--rw-rw-rw-   0 root         (0) root         (0)     2311 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_splunk_5_0_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)     2064 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_splunk_6_0_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)     1306 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_splunk_6_1_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)     4153 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_splunk_6_2_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)     8682 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_splunk_6_3_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)     9961 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_splunk_6_4_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)     3233 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_splunk_6_5_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)     4292 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_splunk_6_6_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)     1647 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_splunk_7_1_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)     1115 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_splunk_7_2_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)     1581 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_splunk_7_3_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)    12324 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_splunk_8_0_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)     7388 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_support_and_installation_standards.py
--rw-rw-rw-   0 root         (0) root         (0)     1076 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_support_requirements.py
--rw-rw-rw-   0 root         (0) root         (0)     5012 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_transforms_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)     9889 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_web_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)     4249 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_workflow_actions.py
--rw-rw-rw-   0 root         (0) root         (0)     5197 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/check_xml_files.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks/disabled_check_splunk_future_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)    34008 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/checks.py
--rw-rw-rw-   0 root         (0) root         (0)      436 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/collections_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)     5577 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/command_line_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)      350 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/commands_configuration_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      290 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/common/file_hash.py
--rw-rw-rw-   0 root         (0) root         (0)     4901 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)     5240 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/configuration_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2842 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/cron_expression.py
--rw-rw-rw-   0 root         (0) root         (0)    11077 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/custom_commands.py
--rw-rw-rw-   0 root         (0) root         (0)     4584 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/custom_visualizations.py
--rw-rw-rw-   0 root         (0) root         (0)     1413 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/distsearch_configuration_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/documentation/
--rw-rw-rw-   0 root         (0) root         (0)      181 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/documentation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2950 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/documentation/criteria_generator.py
--rw-rw-rw-   0 root         (0) root         (0)      747 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/documentation/splunk_docs.py
--rw-rw-rw-   0 root         (0) root         (0)     3120 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/documentation/tag_reference_generator.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/environment_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     3353 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/feedback_file_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     1003 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/file_resource.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/formatters/
--rw-rw-rw-   0 root         (0) root         (0)      315 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/formatters/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      473 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/formatters/date_time_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)      429 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/formatters/validation_report_formatter.py
--rw-rw-rw-   0 root         (0) root         (0)     5811 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/formatters/validation_report_json_formatter.py
--rw-rw-rw-   0 root         (0) root         (0)     8276 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/formatters/validation_report_junitxml_formatter.py
--rw-rw-rw-   0 root         (0) root         (0)      689 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/image_resource.py
--rw-rw-rw-   0 root         (0) root         (0)      439 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/indexes_configuration_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/infra/
--rw-rw-rw-   0 root         (0) root         (0)      949 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/infra/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1198 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/infra/log_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/inputs_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/inputs_specification_file.py
--rw-rw-rw-   0 root         (0) root         (0)     7277 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/inspected_file.py
--rw-rw-rw-   0 root         (0) root         (0)      521 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/iter_ext.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/listeners/
--rw-rw-rw-   0 root         (0) root         (0)      184 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/listeners/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3692 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/listeners/cert_status_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     3550 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/listeners/dot_status_listener.py
--rw-rw-rw-   0 root         (0) root         (0)      455 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/listeners/listener.py
--rw-rw-rw-   0 root         (0) root         (0)     5761 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/lookup.py
--rwxrwxrwx   0 root         (0) root         (0)    23916 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/main.py
--rw-rw-rw-   0 root         (0) root         (0)    15726 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/modular_inputs.py
--rw-rw-rw-   0 root         (0) root         (0)     2172 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/offense.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/outputs_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/props_configuration_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/
--rw-rw-rw-   0 root         (0) root         (0)      240 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   114348 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/ast_analyzer.py
--rw-rw-rw-   0 root         (0) root         (0)    11260 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/ast_info_query.py
--rw-rw-rw-   0 root         (0) root         (0)     2331 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/ast_info_store.py
--rw-rw-rw-   0 root         (0) root         (0)    23917 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/ast_types.py
--rw-rw-rw-   0 root         (0) root         (0)    11083 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/client.py
--rw-rw-rw-   0 root         (0) root         (0)    18452 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/file_dep_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/trustedlibs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/trustedlibs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/trustedlibs/lib_files/
--rw-r--r--   0 root         (0) root         (0)  4147312 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/trustedlibs/lib_files/trusted_file_hashes.csv
--rw-r--r--   0 root         (0) root         (0)       22 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/trustedlibs/lib_files/untrusted_file_hashes.csv
--rw-rw-rw-   0 root         (0) root         (0)     2426 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/trustedlibs/trusted_data_collector.py
--rw-rw-rw-   0 root         (0) root         (0)     1253 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/trustedlibs/trusted_libs_manager.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/trustedlibs/utilities.py
--rw-rw-rw-   0 root         (0) root         (0)    14860 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/BaseHTTPServer/
--rw-rw-rw-   0 root         (0) root         (0)      484 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/BaseHTTPServer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/ConfigParser/
--rw-rw-rw-   0 root         (0) root         (0)      958 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/ConfigParser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/DocXMLRPCServer/
--rw-rw-rw-   0 root         (0) root         (0)      548 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/DocXMLRPCServer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/MimeWriter/
--rw-rw-rw-   0 root         (0) root         (0)      632 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/MimeWriter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/SimpleXMLRPCServer/
--rw-rw-rw-   0 root         (0) root         (0)      537 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/SimpleXMLRPCServer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/SocketServer/
--rw-rw-rw-   0 root         (0) root         (0)      655 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/SocketServer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/___configparser/
--rw-rw-rw-   0 root         (0) root         (0)      958 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/___configparser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/___socketserver/
--rw-rw-rw-   0 root         (0) root         (0)      695 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/___socketserver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/_thread/
--rw-rw-rw-   0 root         (0) root         (0)      386 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/_thread/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/aifc/
--rw-rw-rw-   0 root         (0) root         (0)      473 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/aifc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/anydbm/
--rw-rw-rw-   0 root         (0) root         (0)      424 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/anydbm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/argparse/
--rw-rw-rw-   0 root         (0) root         (0)      505 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/argparse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/asynchat/
--rw-rw-rw-   0 root         (0) root         (0)      559 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/asynchat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/asyncore/
--rw-rw-rw-   0 root         (0) root         (0)     1121 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/asyncore/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/base64/
--rw-rw-rw-   0 root         (0) root         (0)      738 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/base64/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/binhex/
--rw-rw-rw-   0 root         (0) root         (0)      618 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/binhex/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/bz2/
--rw-rw-rw-   0 root         (0) root         (0)      373 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/bz2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/cPickle/
--rw-rw-rw-   0 root         (0) root         (0)      766 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/cPickle/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/chunk/
--rw-rw-rw-   0 root         (0) root         (0)      495 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/chunk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/cmd/
--rw-rw-rw-   0 root         (0) root         (0)      423 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/cmd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/code/
--rw-rw-rw-   0 root         (0) root         (0)      952 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/code/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/commands/
--rw-rw-rw-   0 root         (0) root         (0)      782 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/crypt/
--rw-rw-rw-   0 root         (0) root         (0)      410 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/crypt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/csv/
--rw-rw-rw-   0 root         (0) root         (0)      680 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/csv/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/dbm/
--rw-rw-rw-   0 root         (0) root         (0)      442 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/dbm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/dbm/dumb/
--rw-rw-rw-   0 root         (0) root         (0)      440 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/dbm/dumb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/dbm/gnu/
--rw-rw-rw-   0 root         (0) root         (0)      394 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/dbm/gnu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/dbm/ndbm/
--rw-rw-rw-   0 root         (0) root         (0)      400 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/dbm/ndbm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/dircache/
--rw-rw-rw-   0 root         (0) root         (0)       42 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/dircache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/dl/
--rw-rw-rw-   0 root         (0) root         (0)      538 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/dl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/dumbdbm/
--rw-rw-rw-   0 root         (0) root         (0)      432 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/dumbdbm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/email/
--rw-rw-rw-   0 root         (0) root         (0)      544 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/email/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/ftplib/
--rw-rw-rw-   0 root         (0) root         (0)      542 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/ftplib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/gc/
--rw-rw-rw-   0 root         (0) root         (0)      445 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/gc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/gdbm/
--rw-rw-rw-   0 root         (0) root         (0)      434 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/gdbm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/getpass/
--rw-rw-rw-   0 root         (0) root         (0)      365 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/getpass/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/gzip/
--rw-rw-rw-   0 root         (0) root         (0)      570 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/gzip/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/http/
--rw-rw-rw-   0 root         (0) root         (0)      112 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/http/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/http/client/
--rw-rw-rw-   0 root         (0) root         (0)      466 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/http/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/http/server/
--rw-rw-rw-   0 root         (0) root         (0)      685 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/http/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/httplib/
--rw-rw-rw-   0 root         (0) root         (0)      329 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/httplib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/httplib2/
--rw-rw-rw-   0 root         (0) root         (0)      353 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/httplib2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/imaplib/
--rw-rw-rw-   0 root         (0) root         (0)      764 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/imaplib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/imp/
--rw-rw-rw-   0 root         (0) root         (0)      525 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/imp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/importlib/
--rw-rw-rw-   0 root         (0) root         (0)      555 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/importlib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/imputil/
--rw-rw-rw-   0 root         (0) root         (0)      916 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/imputil/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/inspect/
--rw-rw-rw-   0 root         (0) root         (0)      915 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/inspect/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/io/
--rw-rw-rw-   0 root         (0) root         (0)     3701 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/io/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/json/
--rw-rw-rw-   0 root         (0) root         (0)      567 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/json/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/linecache/
--rw-rw-rw-   0 root         (0) root         (0)      833 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/linecache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/logging/
--rw-rw-rw-   0 root         (0) root         (0)      586 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/logging/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/logging/config/
--rw-rw-rw-   0 root         (0) root         (0)      593 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/logging/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/logging/handlers/
--rw-rw-rw-   0 root         (0) root         (0)     2057 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/logging/handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/marshal/
--rw-rw-rw-   0 root         (0) root         (0)      523 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/marshal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/mimetools/
--rw-rw-rw-   0 root         (0) root         (0)      844 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/mimetools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/mimetypes/
--rw-rw-rw-   0 root         (0) root         (0)     1038 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/mimetypes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/mimify/
--rw-rw-rw-   0 root         (0) root         (0)      683 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/mimify/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/mmap/
--rw-rw-rw-   0 root         (0) root         (0)      443 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/mmap/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/modulefinder/
--rw-rw-rw-   0 root         (0) root         (0)      814 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/modulefinder/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/multifile/
--rw-rw-rw-   0 root         (0) root         (0)     1179 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/multifile/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/multiprocessing/
--rw-rw-rw-   0 root         (0) root         (0)      603 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/multiprocessing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/nntplib/
--rw-rw-rw-   0 root         (0) root         (0)      386 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/nntplib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/os/
--rw-rw-rw-   0 root         (0) root         (0)     4828 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/os/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/os/path/
--rw-rw-rw-   0 root         (0) root         (0)      931 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/os/path/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/pickle/
--rw-rw-rw-   0 root         (0) root         (0)      692 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/pickle/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/pipes/
--rw-rw-rw-   0 root         (0) root         (0)      547 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/pipes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/pkgutil/
--rw-rw-rw-   0 root         (0) root         (0)      805 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/pkgutil/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/plistlib/
--rw-rw-rw-   0 root         (0) root         (0)      732 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/plistlib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/poplib/
--rw-rw-rw-   0 root         (0) root         (0)      359 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/poplib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/posix/
--rw-rw-rw-   0 root         (0) root         (0)     2264 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/posix/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/posixfile/
--rw-rw-rw-   0 root         (0) root         (0)      533 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/posixfile/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/pty/
--rw-rw-rw-   0 root         (0) root         (0)      665 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/pty/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/quopri/
--rw-rw-rw-   0 root         (0) root         (0)      768 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/quopri/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/requests/
--rw-rw-rw-   0 root         (0) root         (0)     1993 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/requests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/runpy/
--rw-rw-rw-   0 root         (0) root         (0)      725 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/runpy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/shelve/
--rw-rw-rw-   0 root         (0) root         (0)      353 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/shelve/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/shutil/
--rw-rw-rw-   0 root         (0) root         (0)     1529 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/shutil/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/smtplib/
--rw-rw-rw-   0 root         (0) root         (0)      847 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/smtplib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/socket/
--rw-rw-rw-   0 root         (0) root         (0)      745 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/socket/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/sqlite3/
--rw-rw-rw-   0 root         (0) root         (0)      540 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/sqlite3/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/subprocess/
--rw-rw-rw-   0 root         (0) root         (0)     1712 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/subprocess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/sunau/
--rw-rw-rw-   0 root         (0) root         (0)      678 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/sunau/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/syslog/
--rw-rw-rw-   0 root         (0) root         (0)      549 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/syslog/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/tarfile/
--rw-rw-rw-   0 root         (0) root         (0)      616 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/tarfile/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/telnetlib/
--rw-rw-rw-   0 root         (0) root         (0)      595 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/telnetlib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/tempfile/
--rw-rw-rw-   0 root         (0) root         (0)     1051 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/tempfile/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/termios/
--rw-rw-rw-   0 root         (0) root         (0)      459 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/termios/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/thread/
--rw-rw-rw-   0 root         (0) root         (0)      324 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/thread/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/threading/
--rw-rw-rw-   0 root         (0) root         (0)      541 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/threading/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/trace/
--rw-rw-rw-   0 root         (0) root         (0)     1135 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/trace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/tty/
--rw-rw-rw-   0 root         (0) root         (0)      574 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/tty/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/urllib/
--rw-rw-rw-   0 root         (0) root         (0)     1679 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/urllib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/urllib/request/
--rw-rw-rw-   0 root         (0) root         (0)     1461 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/urllib/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/urllib2/
--rw-rw-rw-   0 root         (0) root         (0)      426 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/urllib2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/uu/
--rw-rw-rw-   0 root         (0) root         (0)      729 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/uu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/wave/
--rw-rw-rw-   0 root         (0) root         (0)      684 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/wave/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/wsgiref/
--rw-rw-rw-   0 root         (0) root         (0)      167 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/wsgiref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/wsgiref/simple_server/
--rw-rw-rw-   0 root         (0) root         (0)      611 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/wsgiref/simple_server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/xml/
--rw-rw-rw-   0 root         (0) root         (0)       84 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/xml/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/xml/dom/
--rw-rw-rw-   0 root         (0) root         (0)       76 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/xml/dom/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      580 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/xml/dom/minidom.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/xml/dom/pulldom.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/xml/etree/
--rw-rw-rw-   0 root         (0) root         (0)     1080 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/xml/etree/ElementTree.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/xml/etree/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/xml/sax/
--rw-rw-rw-   0 root         (0) root         (0)      352 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/xml/sax/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/xml/sax/xmlreader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/
--rw-rw-rw-   0 root         (0) root         (0)      124 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/client/
--rw-rw-rw-   0 root         (0) root         (0)      433 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/server/
--rw-rw-rw-   0 root         (0) root         (0)      648 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpclib/
--rw-rw-rw-   0 root         (0) root         (0)      404 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpclib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/zipfile/
--rw-rw-rw-   0 root         (0) root         (0)      463 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/zipfile/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/zipimport/
--rw-rw-rw-   0 root         (0) root         (0)      635 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/zipimport/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:32.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata_common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata_common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3721 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata_common/metadata_consts.py
--rw-rw-rw-   0 root         (0) root         (0)      178 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata_common/metadata_decorator.py
--rw-rw-rw-   0 root         (0) root         (0)       96 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata_common/metadata_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5998 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata_common/metadata_types.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata_importer.py
--rw-rw-rw-   0 root         (0) root         (0)    14789 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/python_modules_metadata_store.py
--rw-rw-rw-   0 root         (0) root         (0)    23756 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/reflected_xss_detector.py
--rw-rw-rw-   0 root         (0) root         (0)    13297 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/regex_matcher.py
--rw-rw-rw-   0 root         (0) root         (0)    12670 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/reporter.py
--rw-rw-rw-   0 root         (0) root         (0)     2448 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/resource_manager.py
--rw-rw-rw-   0 root         (0) root         (0)    10212 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/rest_map.py
--rw-rw-rw-   0 root         (0) root         (0)      419 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/rest_map_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)     3773 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/saved_searches.py
--rw-rw-rw-   0 root         (0) root         (0)      443 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/saved_searches_configuration_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:32.000000 splunk-appinspect-2.9.0/splunk_appinspect/splunk/
--rw-rw-rw-   0 root         (0) root         (0)     1850 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/splunk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:32.000000 splunk-appinspect-2.9.0/splunk_appinspect/splunk/jquery_checks_data/
--rw-rw-rw-   0 root         (0) root         (0)   194697 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/splunk/jquery_checks_data/disallowed_imports.json
--rw-rw-rw-   0 root         (0) root         (0)     9159 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/splunk/splunk_default_source_type_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:32.000000 splunk-appinspect-2.9.0/splunk_appinspect/splunk/telemetry/
--rw-rw-rw-   0 root         (0) root         (0)       37 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/splunk/telemetry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      466 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/splunk/telemetry/core.py
--rw-rw-rw-   0 root         (0) root         (0)      877 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/splunk/telemetry/list.csv
--rw-rw-rw-   0 root         (0) root         (0)     1930 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/splunk/util.py
--rw-rw-rw-   0 root         (0) root         (0)     9159 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/splunk_default_source_type_list.py
--rw-rw-rw-   0 root         (0) root         (0)     5132 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/splunk_defined_authorize_capability_list.py
--rw-rw-rw-   0 root         (0) root         (0)     3461 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/splunk_defined_conf_file_list.py
--rw-rw-rw-   0 root         (0) root         (0)     3007 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/splunk_pretrained_sourcetypes_list.py
--rw-rw-rw-   0 root         (0) root         (0)      579 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/telemetry_configuration_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:32.000000 splunk-appinspect-2.9.0/splunk_appinspect/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2776 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/templates/html_criteria.html
--rw-rw-rw-   0 root         (0) root         (0)     1727 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/templates/tag_reference.html
--rw-rw-rw-   0 root         (0) root         (0)      431 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/transforms_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)     8714 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/validation_report.py
--rw-rw-rw-   0 root         (0) root         (0)    17838 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:32.000000 splunk-appinspect-2.9.0/splunk_appinspect/version/
--rw-rw-rw-   0 root         (0) root         (0)        6 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/version/VERSION.txt
--rw-rw-rw-   0 root         (0) root         (0)      106 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/version/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      557 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/version/version.py
--rw-rw-rw-   0 root         (0) root         (0)      367 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/visualizations_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/web_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)     1438 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/workflow_actions.py
--rw-rw-rw-   0 root         (0) root         (0)      452 2021-08-31 23:48:02.000000 splunk-appinspect-2.9.0/splunk_appinspect/workflow_actions_configuration_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1332 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17115 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      402 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2021-08-31 23:48:31.000000 splunk-appinspect-2.9.0/splunk_appinspect.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)      270 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1332 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      214 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3857 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/
+-rw-rw-rw-   0 root         (0) root         (0)     1325 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11304 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/alert_actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      364 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/alert_actions_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)    41844 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/app.py
+-rw-rw-rw-   0 root         (0) root         (0)      413 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/app_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)    48715 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/app_package_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     2713 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/app_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      368 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/authentication_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      353 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/authorize_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/banned_wordlist.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1668 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/bias.py
+-rw-rw-rw-   0 root         (0) root         (0)       32 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/bias_wordlist.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/check_routine/
+-rw-rw-rw-   0 root         (0) root         (0)     4766 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/check_routine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/check_routine/find_endpoint_usage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2626 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/check_routine/find_spl_command_usage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/check_routine/python_ast_searcher/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/check_routine/python_ast_searcher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4243 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/check_routine/python_ast_searcher/ast_searcher.py
+-rw-rw-rw-   0 root         (0) root         (0)      294 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/check_routine/python_ast_searcher/node_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     7248 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/check_routine/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/
+-rw-rw-rw-   0 root         (0) root         (0)    11174 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_alert_actions_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    19522 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_app_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     8529 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_application_content.py
+-rw-rw-rw-   0 root         (0) root         (0)    10593 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_application_structure.py
+-rw-rw-rw-   0 root         (0) root         (0)     7091 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_authentication_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1935 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_authorize_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1243 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_bias_language.py
+-rw-rw-rw-   0 root         (0) root         (0)    94581 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_cloud_simple_app.py
+-rw-rw-rw-   0 root         (0) root         (0)     9915 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_configuration_files.py
+-rw-rw-rw-   0 root         (0) root         (0)    14365 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_custom_commands.py
+-rw-rw-rw-   0 root         (0) root         (0)    37993 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_custom_visualizations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5603 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_data_models_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3989 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_documentation_for_sensitive_functionality.py
+-rw-rw-rw-   0 root         (0) root         (0)     7743 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_documentation_standards.py
+-rw-rw-rw-   0 root         (0) root         (0)      581 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_external_data_sources.py
+-rw-rw-rw-   0 root         (0) root         (0)     9939 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_indexes_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      919 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_intellectual_property.py
+-rw-rw-rw-   0 root         (0) root         (0)     6629 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_itsi_module_file_structure.py
+-rw-rw-rw-   0 root         (0) root         (0)    11886 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_javascript_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     6697 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_jquery_standards.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_json_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     1254 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_limits_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     4096 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_lookup_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     4680 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_malware.py
+-rw-rw-rw-   0 root         (0) root         (0)     2083 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_meta_files.py
+-rw-rw-rw-   0 root         (0) root         (0)    13054 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_modular_inputs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2841 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_outputs_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)    18574 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_packaging_standards.py
+-rw-rw-rw-   0 root         (0) root         (0)     5288 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_potentially_harmful_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)    25787 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_props_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)    37368 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_python_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_readme_spec_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     4940 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_rest_endpoints.py
+-rw-rw-rw-   0 root         (0) root         (0)    16598 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_saved_searches.py
+-rwxrwxrwx   0 root         (0) root         (0)    16806 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_security.py
+-rw-rw-rw-   0 root         (0) root         (0)     3223 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_server_configuration_file.py
+-rwxrwxrwx   0 root         (0) root         (0)    13821 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_source_and_binaries.py
+-rw-rw-rw-   0 root         (0) root         (0)     2311 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_splunk_5_0_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_splunk_6_0_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     1306 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_splunk_6_1_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     4153 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_splunk_6_2_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     8682 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_splunk_6_3_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     9961 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_splunk_6_4_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     3233 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_splunk_6_5_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     4292 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_splunk_6_6_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     1647 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_splunk_7_1_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_splunk_7_2_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_splunk_7_3_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)    12324 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_splunk_8_0_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     7388 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_support_and_installation_standards.py
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_support_requirements.py
+-rw-rw-rw-   0 root         (0) root         (0)     5012 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_transforms_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     9889 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_web_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     4249 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_workflow_actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5197 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/check_xml_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks/disabled_check_splunk_future_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)    34008 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/checks.py
+-rw-rw-rw-   0 root         (0) root         (0)      436 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/collections_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     5577 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/command_line_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)      350 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/commands_configuration_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      290 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/common/file_hash.py
+-rw-rw-rw-   0 root         (0) root         (0)     4901 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     5240 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/configuration_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2842 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/cron_expression.py
+-rw-rw-rw-   0 root         (0) root         (0)    11077 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/custom_commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     4584 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/custom_visualizations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1413 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/distsearch_configuration_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/documentation/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/documentation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2950 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/documentation/criteria_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)      747 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/documentation/splunk_docs.py
+-rw-rw-rw-   0 root         (0) root         (0)     3120 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/documentation/tag_reference_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/environment_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3353 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/feedback_file_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/file_resource.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/formatters/
+-rw-rw-rw-   0 root         (0) root         (0)      315 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/formatters/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      473 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/formatters/date_time_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)      429 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/formatters/validation_report_formatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     5811 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/formatters/validation_report_json_formatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     8276 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/formatters/validation_report_junitxml_formatter.py
+-rw-rw-rw-   0 root         (0) root         (0)      689 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/image_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)      439 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/indexes_configuration_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/infra/
+-rw-rw-rw-   0 root         (0) root         (0)      949 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/infra/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/infra/log_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/inputs_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/inputs_specification_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     7277 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/inspected_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      521 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/iter_ext.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/listeners/
+-rw-rw-rw-   0 root         (0) root         (0)      184 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/listeners/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3692 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/listeners/cert_status_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     3550 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/listeners/dot_status_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)      455 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/listeners/listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     5761 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/lookup.py
+-rwxrwxrwx   0 root         (0) root         (0)    23916 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/main.py
+-rw-rw-rw-   0 root         (0) root         (0)    15726 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/modular_inputs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2172 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/offense.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/outputs_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/props_configuration_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/
+-rw-rw-rw-   0 root         (0) root         (0)      240 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   114348 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/ast_analyzer.py
+-rw-rw-rw-   0 root         (0) root         (0)    11260 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/ast_info_query.py
+-rw-rw-rw-   0 root         (0) root         (0)     2331 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/ast_info_store.py
+-rw-rw-rw-   0 root         (0) root         (0)    23917 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/ast_types.py
+-rw-rw-rw-   0 root         (0) root         (0)    11083 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/client.py
+-rw-rw-rw-   0 root         (0) root         (0)    18452 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/file_dep_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/trustedlibs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/trustedlibs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/trustedlibs/lib_files/
+-rw-r--r--   0 root         (0) root         (0)  4147312 2021-09-02 23:09:25.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/trustedlibs/lib_files/trusted_file_hashes.csv
+-rw-r--r--   0 root         (0) root         (0)       22 2021-09-02 23:09:25.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/trustedlibs/lib_files/untrusted_file_hashes.csv
+-rw-rw-rw-   0 root         (0) root         (0)     2426 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/trustedlibs/trusted_data_collector.py
+-rw-rw-rw-   0 root         (0) root         (0)     1253 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/trustedlibs/trusted_libs_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/trustedlibs/utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    14860 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/BaseHTTPServer/
+-rw-rw-rw-   0 root         (0) root         (0)      484 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/BaseHTTPServer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/ConfigParser/
+-rw-rw-rw-   0 root         (0) root         (0)      958 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/ConfigParser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/DocXMLRPCServer/
+-rw-rw-rw-   0 root         (0) root         (0)      548 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/DocXMLRPCServer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/MimeWriter/
+-rw-rw-rw-   0 root         (0) root         (0)      632 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/MimeWriter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/SimpleXMLRPCServer/
+-rw-rw-rw-   0 root         (0) root         (0)      537 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/SimpleXMLRPCServer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/SocketServer/
+-rw-rw-rw-   0 root         (0) root         (0)      655 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/SocketServer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/___configparser/
+-rw-rw-rw-   0 root         (0) root         (0)      958 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/___configparser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/___socketserver/
+-rw-rw-rw-   0 root         (0) root         (0)      695 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/___socketserver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      247 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/_thread/
+-rw-rw-rw-   0 root         (0) root         (0)      386 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/_thread/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/aifc/
+-rw-rw-rw-   0 root         (0) root         (0)      473 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/aifc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/anydbm/
+-rw-rw-rw-   0 root         (0) root         (0)      424 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/anydbm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/argparse/
+-rw-rw-rw-   0 root         (0) root         (0)      505 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/argparse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/asynchat/
+-rw-rw-rw-   0 root         (0) root         (0)      559 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/asynchat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/asyncore/
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/asyncore/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/base64/
+-rw-rw-rw-   0 root         (0) root         (0)      738 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/base64/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/binhex/
+-rw-rw-rw-   0 root         (0) root         (0)      618 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/binhex/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/bz2/
+-rw-rw-rw-   0 root         (0) root         (0)      373 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/bz2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/cPickle/
+-rw-rw-rw-   0 root         (0) root         (0)      766 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/cPickle/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/chunk/
+-rw-rw-rw-   0 root         (0) root         (0)      495 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/chunk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/cmd/
+-rw-rw-rw-   0 root         (0) root         (0)      423 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/cmd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/code/
+-rw-rw-rw-   0 root         (0) root         (0)      952 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/code/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/commands/
+-rw-rw-rw-   0 root         (0) root         (0)      782 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/crypt/
+-rw-rw-rw-   0 root         (0) root         (0)      410 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/crypt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/csv/
+-rw-rw-rw-   0 root         (0) root         (0)      680 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/csv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/dbm/
+-rw-rw-rw-   0 root         (0) root         (0)      442 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/dbm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/dbm/dumb/
+-rw-rw-rw-   0 root         (0) root         (0)      440 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/dbm/dumb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/dbm/gnu/
+-rw-rw-rw-   0 root         (0) root         (0)      394 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/dbm/gnu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/dbm/ndbm/
+-rw-rw-rw-   0 root         (0) root         (0)      400 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/dbm/ndbm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/dircache/
+-rw-rw-rw-   0 root         (0) root         (0)       42 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/dircache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/dl/
+-rw-rw-rw-   0 root         (0) root         (0)      538 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/dl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/dumbdbm/
+-rw-rw-rw-   0 root         (0) root         (0)      432 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/dumbdbm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/email/
+-rw-rw-rw-   0 root         (0) root         (0)      544 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/email/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/ftplib/
+-rw-rw-rw-   0 root         (0) root         (0)      542 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/ftplib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/gc/
+-rw-rw-rw-   0 root         (0) root         (0)      445 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/gc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/gdbm/
+-rw-rw-rw-   0 root         (0) root         (0)      434 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/gdbm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/getpass/
+-rw-rw-rw-   0 root         (0) root         (0)      365 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/getpass/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/gzip/
+-rw-rw-rw-   0 root         (0) root         (0)      570 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/gzip/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/http/
+-rw-rw-rw-   0 root         (0) root         (0)      112 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/http/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/http/client/
+-rw-rw-rw-   0 root         (0) root         (0)      466 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/http/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/http/server/
+-rw-rw-rw-   0 root         (0) root         (0)      685 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/http/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/httplib/
+-rw-rw-rw-   0 root         (0) root         (0)      329 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/httplib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/httplib2/
+-rw-rw-rw-   0 root         (0) root         (0)      353 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/httplib2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/imaplib/
+-rw-rw-rw-   0 root         (0) root         (0)      764 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/imaplib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/imp/
+-rw-rw-rw-   0 root         (0) root         (0)      525 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/imp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/importlib/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/importlib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/imputil/
+-rw-rw-rw-   0 root         (0) root         (0)      916 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/imputil/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/inspect/
+-rw-rw-rw-   0 root         (0) root         (0)      915 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/inspect/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/io/
+-rw-rw-rw-   0 root         (0) root         (0)     3701 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/json/
+-rw-rw-rw-   0 root         (0) root         (0)      567 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/json/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/linecache/
+-rw-rw-rw-   0 root         (0) root         (0)      833 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/linecache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/logging/
+-rw-rw-rw-   0 root         (0) root         (0)      586 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/logging/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/logging/config/
+-rw-rw-rw-   0 root         (0) root         (0)      593 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/logging/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/logging/handlers/
+-rw-rw-rw-   0 root         (0) root         (0)     2057 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/logging/handlers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/marshal/
+-rw-rw-rw-   0 root         (0) root         (0)      523 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/marshal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/mimetools/
+-rw-rw-rw-   0 root         (0) root         (0)      844 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/mimetools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/mimetypes/
+-rw-rw-rw-   0 root         (0) root         (0)     1038 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/mimetypes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/mimify/
+-rw-rw-rw-   0 root         (0) root         (0)      683 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/mimify/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/mmap/
+-rw-rw-rw-   0 root         (0) root         (0)      443 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/mmap/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/modulefinder/
+-rw-rw-rw-   0 root         (0) root         (0)      814 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/modulefinder/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/multifile/
+-rw-rw-rw-   0 root         (0) root         (0)     1179 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/multifile/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/multiprocessing/
+-rw-rw-rw-   0 root         (0) root         (0)      603 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/multiprocessing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/nntplib/
+-rw-rw-rw-   0 root         (0) root         (0)      386 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/nntplib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/os/
+-rw-rw-rw-   0 root         (0) root         (0)     4828 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/os/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/os/path/
+-rw-rw-rw-   0 root         (0) root         (0)      931 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/os/path/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/pickle/
+-rw-rw-rw-   0 root         (0) root         (0)      692 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/pickle/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/pipes/
+-rw-rw-rw-   0 root         (0) root         (0)      547 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/pipes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/pkgutil/
+-rw-rw-rw-   0 root         (0) root         (0)      805 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/pkgutil/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/plistlib/
+-rw-rw-rw-   0 root         (0) root         (0)      732 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/plistlib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/poplib/
+-rw-rw-rw-   0 root         (0) root         (0)      359 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/poplib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/posix/
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/posix/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/posixfile/
+-rw-rw-rw-   0 root         (0) root         (0)      533 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/posixfile/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/pty/
+-rw-rw-rw-   0 root         (0) root         (0)      665 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/pty/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/quopri/
+-rw-rw-rw-   0 root         (0) root         (0)      768 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/quopri/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/requests/
+-rw-rw-rw-   0 root         (0) root         (0)     1993 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/requests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/runpy/
+-rw-rw-rw-   0 root         (0) root         (0)      725 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/runpy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/shelve/
+-rw-rw-rw-   0 root         (0) root         (0)      353 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/shelve/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/shutil/
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/shutil/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/smtplib/
+-rw-rw-rw-   0 root         (0) root         (0)      847 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/smtplib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/socket/
+-rw-rw-rw-   0 root         (0) root         (0)      745 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/socket/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/sqlite3/
+-rw-rw-rw-   0 root         (0) root         (0)      540 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/sqlite3/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/subprocess/
+-rw-rw-rw-   0 root         (0) root         (0)     1712 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/subprocess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/sunau/
+-rw-rw-rw-   0 root         (0) root         (0)      678 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/sunau/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/syslog/
+-rw-rw-rw-   0 root         (0) root         (0)      549 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/syslog/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/tarfile/
+-rw-rw-rw-   0 root         (0) root         (0)      616 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/tarfile/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/telnetlib/
+-rw-rw-rw-   0 root         (0) root         (0)      595 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/telnetlib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/tempfile/
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/tempfile/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/termios/
+-rw-rw-rw-   0 root         (0) root         (0)      459 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/termios/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/thread/
+-rw-rw-rw-   0 root         (0) root         (0)      324 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/thread/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/threading/
+-rw-rw-rw-   0 root         (0) root         (0)      541 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/threading/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/trace/
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/trace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/tty/
+-rw-rw-rw-   0 root         (0) root         (0)      574 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/tty/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/urllib/
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/urllib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/urllib/request/
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/urllib/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/urllib2/
+-rw-rw-rw-   0 root         (0) root         (0)      426 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/urllib2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/uu/
+-rw-rw-rw-   0 root         (0) root         (0)      729 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/uu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/wave/
+-rw-rw-rw-   0 root         (0) root         (0)      684 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/wave/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/wsgiref/
+-rw-rw-rw-   0 root         (0) root         (0)      167 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/wsgiref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/wsgiref/simple_server/
+-rw-rw-rw-   0 root         (0) root         (0)      611 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/wsgiref/simple_server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/xml/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/xml/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/xml/dom/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/xml/dom/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      580 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/xml/dom/minidom.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/xml/dom/pulldom.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/xml/etree/
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/xml/etree/ElementTree.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/xml/etree/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/xml/sax/
+-rw-rw-rw-   0 root         (0) root         (0)      352 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/xml/sax/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/xml/sax/xmlreader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/
+-rw-rw-rw-   0 root         (0) root         (0)      124 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/client/
+-rw-rw-rw-   0 root         (0) root         (0)      433 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/server/
+-rw-rw-rw-   0 root         (0) root         (0)      648 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/xmlrpclib/
+-rw-rw-rw-   0 root         (0) root         (0)      404 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/xmlrpclib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/zipfile/
+-rw-rw-rw-   0 root         (0) root         (0)      463 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/zipfile/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/zipimport/
+-rw-rw-rw-   0 root         (0) root         (0)      635 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/zipimport/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata_common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata_common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3721 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata_common/metadata_consts.py
+-rw-rw-rw-   0 root         (0) root         (0)      178 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata_common/metadata_decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)       96 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata_common/metadata_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5998 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata_common/metadata_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      826 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata_importer.py
+-rw-rw-rw-   0 root         (0) root         (0)    14789 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/python_modules_metadata_store.py
+-rw-rw-rw-   0 root         (0) root         (0)    23756 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/reflected_xss_detector.py
+-rw-rw-rw-   0 root         (0) root         (0)    13297 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/regex_matcher.py
+-rw-rw-rw-   0 root         (0) root         (0)    12670 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/reporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2448 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/resource_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    10212 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/rest_map.py
+-rw-rw-rw-   0 root         (0) root         (0)      419 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/rest_map_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     3773 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/saved_searches.py
+-rw-rw-rw-   0 root         (0) root         (0)      443 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/saved_searches_configuration_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/splunk/
+-rw-rw-rw-   0 root         (0) root         (0)     1850 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/splunk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/splunk/jquery_checks_data/
+-rw-rw-rw-   0 root         (0) root         (0)     3421 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/splunk/jquery_checks_data/supported_modules.json
+-rw-rw-rw-   0 root         (0) root         (0)     9159 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/splunk/splunk_default_source_type_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/splunk/telemetry/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/splunk/telemetry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      466 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/splunk/telemetry/core.py
+-rw-rw-rw-   0 root         (0) root         (0)      877 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/splunk/telemetry/list.csv
+-rw-rw-rw-   0 root         (0) root         (0)     1930 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/splunk/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     9159 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/splunk_default_source_type_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     5132 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/splunk_defined_authorize_capability_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     3461 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/splunk_defined_conf_file_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     3007 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/splunk_pretrained_sourcetypes_list.py
+-rw-rw-rw-   0 root         (0) root         (0)      579 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/telemetry_configuration_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2776 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/templates/html_criteria.html
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/templates/tag_reference.html
+-rw-rw-rw-   0 root         (0) root         (0)      431 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/transforms_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     8714 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/validation_report.py
+-rw-rw-rw-   0 root         (0) root         (0)    17838 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect/version/
+-rw-rw-rw-   0 root         (0) root         (0)        6 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/version/VERSION.txt
+-rw-rw-rw-   0 root         (0) root         (0)      106 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/version/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      557 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/version/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      367 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/visualizations_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/web_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1438 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/workflow_actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      452 2021-09-02 23:08:56.000000 splunk-appinspect-2.9.1/splunk_appinspect/workflow_actions_configuration_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-02 23:09:26.000000 splunk-appinspect-2.9.1/splunk_appinspect.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1332 2021-09-02 23:09:25.000000 splunk-appinspect-2.9.1/splunk_appinspect.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17114 2021-09-02 23:09:25.000000 splunk-appinspect-2.9.1/splunk_appinspect.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-09-02 23:09:25.000000 splunk-appinspect-2.9.1/splunk_appinspect.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2021-09-02 23:09:25.000000 splunk-appinspect-2.9.1/splunk_appinspect.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      402 2021-09-02 23:09:25.000000 splunk-appinspect-2.9.1/splunk_appinspect.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2021-09-02 23:09:25.000000 splunk-appinspect-2.9.1/splunk_appinspect.egg-info/top_level.txt
```

### Comparing `splunk-appinspect-2.9.0/PKG-INFO` & `splunk-appinspect-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: splunk-appinspect
-Version: 2.9.0
+Version: 2.9.1
 Summary: Automatic validation checks for Splunk Apps
 Home-page: https://splunk.com
 Author: Splunk
 Author-email: appinspect@splunk.com
 License: Other/Proprietary License
 Download-URL: http://dev.splunk.com/goto/appinspectdownload
 Description: AppInspect is a tool for assessing a Splunk App's compliance with Splunk recommended development practices, by using static analysis. AppInspect is open for extension, allowing other teams to compose checks that meet their domain specific needs for semi- or fully-automated analysis and validation of Splunk Apps.
```

### Comparing `splunk-appinspect-2.9.0/README.md` & `splunk-appinspect-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/setup.py` & `splunk-appinspect-2.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/alert_actions.py` & `splunk-appinspect-2.9.1/splunk_appinspect/alert_actions.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/app.py` & `splunk-appinspect-2.9.1/splunk_appinspect/app.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/app_package_handler.py` & `splunk-appinspect-2.9.1/splunk_appinspect/app_package_handler.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/app_util.py` & `splunk-appinspect-2.9.1/splunk_appinspect/app_util.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/bias.py` & `splunk-appinspect-2.9.1/splunk_appinspect/bias.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/check_routine/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/check_routine/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/check_routine/find_endpoint_usage.py` & `splunk-appinspect-2.9.1/splunk_appinspect/check_routine/find_endpoint_usage.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/check_routine/find_spl_command_usage.py` & `splunk-appinspect-2.9.1/splunk_appinspect/check_routine/find_spl_command_usage.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/check_routine/python_ast_searcher/ast_searcher.py` & `splunk-appinspect-2.9.1/splunk_appinspect/check_routine/python_ast_searcher/ast_searcher.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/check_routine/util.py` & `splunk-appinspect-2.9.1/splunk_appinspect/check_routine/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     for a, b in paths_tuple:
         absolute_paths.append(b)
 
     return absolute_paths
 
 
 def validate_imports(files, allowed_imports_set):
-    """ This function returns paths of files which have require/define statements present in the allowed imports set
+    """This function returns paths of files which have require/define statements not present in the allowed imports set
 
     @param:
     files <Array>: Array of file paths
     allowed_imports_set <Set>: Set of file path imports
 
     returns
 
@@ -101,15 +101,15 @@
     improper_files = []
     try:
         for filepath in files:
             with open(filepath, "r", encoding="utf-8") as my_file:
                 matches = get_imported_matches(my_file.read())
                 bad_imports_in_file = []
                 for match in matches:
-                    if match in allowed_imports_set:
+                    if match not in allowed_imports_set:
                         bad_imports_in_file.append(match)
                 if bad_imports_in_file:
                     improper_files.append({filepath: bad_imports_in_file})
     except Exception as exception:
         print("Exception while validating imports {}".format(exception))
 
     return improper_files
```

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_alert_actions_config.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_alert_actions_config.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_app_configuration_file.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_app_configuration_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_application_content.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_application_content.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_application_structure.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_application_structure.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_authentication_configuration_file.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_authentication_configuration_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_authorize_configuration_file.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_authorize_configuration_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_bias_language.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_bias_language.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_cloud_simple_app.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_cloud_simple_app.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_configuration_files.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_configuration_files.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_custom_commands.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_custom_commands.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_custom_visualizations.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_custom_visualizations.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_data_models_config.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_data_models_config.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_documentation_for_sensitive_functionality.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_documentation_for_sensitive_functionality.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_documentation_standards.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_documentation_standards.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_external_data_sources.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_external_data_sources.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_indexes_configuration_file.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_indexes_configuration_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_intellectual_property.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_intellectual_property.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_itsi_module_file_structure.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_itsi_module_file_structure.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_javascript_files.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_javascript_files.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_json_files.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_json_files.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_limits_configuration_file.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_limits_configuration_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_lookup_files.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_lookup_files.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_malware.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_malware.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_meta_files.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_meta_files.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_modular_inputs.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_modular_inputs.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_outputs_configuration_file.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_outputs_configuration_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_packaging_standards.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_packaging_standards.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_potentially_harmful_operations.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_potentially_harmful_operations.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_props_configuration_file.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_props_configuration_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_python_files.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_python_files.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_readme_spec_files.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_readme_spec_files.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_rest_endpoints.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_rest_endpoints.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_saved_searches.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_saved_searches.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_security.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_security.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_server_configuration_file.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_server_configuration_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_source_and_binaries.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_source_and_binaries.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_splunk_5_0_deprecated_features.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_splunk_5_0_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_splunk_6_0_deprecated_features.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_splunk_6_0_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_splunk_6_1_deprecated_features.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_splunk_6_1_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_splunk_6_2_deprecated_features.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_splunk_6_2_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_splunk_6_3_deprecated_features.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_splunk_6_3_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_splunk_6_4_deprecated_features.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_splunk_6_4_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_splunk_6_5_deprecated_features.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_splunk_6_5_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_splunk_6_6_deprecated_features.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_splunk_6_6_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_splunk_7_1_deprecated_features.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_splunk_7_1_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_splunk_7_2_deprecated_features.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_splunk_7_2_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_splunk_7_3_deprecated_features.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_splunk_7_3_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_splunk_8_0_deprecated_features.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_splunk_8_0_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_support_and_installation_standards.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_support_and_installation_standards.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_support_requirements.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_support_requirements.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_transforms_configuration_file.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_transforms_configuration_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_web_configuration_file.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_web_configuration_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_workflow_actions.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_workflow_actions.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/check_xml_files.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/check_xml_files.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks/disabled_check_splunk_future_deprecated_features.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks/disabled_check_splunk_future_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/checks.py` & `splunk-appinspect-2.9.1/splunk_appinspect/checks.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/command_line_helpers.py` & `splunk-appinspect-2.9.1/splunk_appinspect/command_line_helpers.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/configuration_file.py` & `splunk-appinspect-2.9.1/splunk_appinspect/configuration_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/configuration_parser.py` & `splunk-appinspect-2.9.1/splunk_appinspect/configuration_parser.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/cron_expression.py` & `splunk-appinspect-2.9.1/splunk_appinspect/cron_expression.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/custom_commands.py` & `splunk-appinspect-2.9.1/splunk_appinspect/custom_commands.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/custom_visualizations.py` & `splunk-appinspect-2.9.1/splunk_appinspect/custom_visualizations.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/decorators.py` & `splunk-appinspect-2.9.1/splunk_appinspect/decorators.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/documentation/criteria_generator.py` & `splunk-appinspect-2.9.1/splunk_appinspect/documentation/criteria_generator.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/documentation/splunk_docs.py` & `splunk-appinspect-2.9.1/splunk_appinspect/documentation/splunk_docs.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/documentation/tag_reference_generator.py` & `splunk-appinspect-2.9.1/splunk_appinspect/documentation/tag_reference_generator.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/feedback_file_generator.py` & `splunk-appinspect-2.9.1/splunk_appinspect/feedback_file_generator.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/file_resource.py` & `splunk-appinspect-2.9.1/splunk_appinspect/file_resource.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/formatters/validation_report_json_formatter.py` & `splunk-appinspect-2.9.1/splunk_appinspect/formatters/validation_report_json_formatter.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/formatters/validation_report_junitxml_formatter.py` & `splunk-appinspect-2.9.1/splunk_appinspect/formatters/validation_report_junitxml_formatter.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/image_resource.py` & `splunk-appinspect-2.9.1/splunk_appinspect/image_resource.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/infra/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/infra/log_utils.py` & `splunk-appinspect-2.9.1/splunk_appinspect/infra/log_utils.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/inspected_file.py` & `splunk-appinspect-2.9.1/splunk_appinspect/inspected_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/iter_ext.py` & `splunk-appinspect-2.9.1/splunk_appinspect/iter_ext.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/listeners/cert_status_listener.py` & `splunk-appinspect-2.9.1/splunk_appinspect/listeners/cert_status_listener.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/listeners/dot_status_listener.py` & `splunk-appinspect-2.9.1/splunk_appinspect/listeners/dot_status_listener.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/lookup.py` & `splunk-appinspect-2.9.1/splunk_appinspect/lookup.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/main.py` & `splunk-appinspect-2.9.1/splunk_appinspect/main.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/modular_inputs.py` & `splunk-appinspect-2.9.1/splunk_appinspect/modular_inputs.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/offense.py` & `splunk-appinspect-2.9.1/splunk_appinspect/offense.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/ast_analyzer.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/ast_analyzer.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/ast_info_query.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/ast_info_query.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/ast_info_store.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/ast_info_store.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/ast_types.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/ast_types.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/client.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/client.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/file_dep_manager.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/file_dep_manager.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/trustedlibs/lib_files/trusted_file_hashes.csv` & `splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/trustedlibs/lib_files/trusted_file_hashes.csv`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/trustedlibs/trusted_data_collector.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/trustedlibs/trusted_data_collector.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/trustedlibs/trusted_libs_manager.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/trustedlibs/trusted_libs_manager.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_analyzer/utilities.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_analyzer/utilities.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/ConfigParser/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/ConfigParser/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/DocXMLRPCServer/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/DocXMLRPCServer/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/MimeWriter/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/MimeWriter/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/SimpleXMLRPCServer/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/SimpleXMLRPCServer/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/SocketServer/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/SocketServer/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/___configparser/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/___configparser/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/___socketserver/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/___socketserver/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/asynchat/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/asynchat/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/asyncore/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/asyncore/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/base64/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/base64/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/binhex/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/binhex/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/cPickle/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/cPickle/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/code/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/code/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/commands/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/csv/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/dl/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/dl/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/email/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/email/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/ftplib/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/ftplib/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/gzip/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/gzip/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/http/server/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/http/server/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/imaplib/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/imaplib/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/imp/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/imp/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/importlib/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/importlib/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/imputil/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/imputil/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/inspect/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/inspect/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/io/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/io/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/json/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/json/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/linecache/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/linecache/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/logging/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/logging/config/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/logging/config/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/logging/handlers/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/logging/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/marshal/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/marshal/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/mimetools/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/mimetools/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/mimetypes/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/mimetypes/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/mimify/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/mimify/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/modulefinder/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/modulefinder/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/multifile/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/multifile/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/multiprocessing/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/multiprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/os/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/os/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/os/path/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/os/path/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/pickle/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/pickle/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/pipes/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/pkgutil/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/pkgutil/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/plistlib/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/plistlib/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/posix/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/posix/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/posixfile/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/posixfile/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/pty/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/pty/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/quopri/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/quopri/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/requests/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/runpy/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/runpy/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/shutil/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/shutil/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/smtplib/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/smtplib/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/socket/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/socket/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/sqlite3/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/sqlite3/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/subprocess/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/subprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/sunau/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/sunau/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/syslog/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/syslog/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/tarfile/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/tarfile/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/telnetlib/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/telnetlib/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/tempfile/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/tempfile/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/threading/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/trace/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/tty/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/tty/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/urllib/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/urllib/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/urllib/request/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/urllib/request/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/uu/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/uu/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/wave/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/wave/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/wsgiref/simple_server/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/wsgiref/simple_server/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/xml/dom/minidom.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/xml/dom/minidom.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/xml/etree/ElementTree.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/xml/etree/ElementTree.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/server/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/server/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata/zipimport/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata/zipimport/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata_common/metadata_consts.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata_common/metadata_consts.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata_common/metadata_types.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata_common/metadata_types.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/metadata_importer.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/metadata_importer.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/python_modules_metadata/python_modules_metadata_store.py` & `splunk-appinspect-2.9.1/splunk_appinspect/python_modules_metadata/python_modules_metadata_store.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/reflected_xss_detector.py` & `splunk-appinspect-2.9.1/splunk_appinspect/reflected_xss_detector.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/regex_matcher.py` & `splunk-appinspect-2.9.1/splunk_appinspect/regex_matcher.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/reporter.py` & `splunk-appinspect-2.9.1/splunk_appinspect/reporter.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/resource_manager.py` & `splunk-appinspect-2.9.1/splunk_appinspect/resource_manager.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/rest_map.py` & `splunk-appinspect-2.9.1/splunk_appinspect/rest_map.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/saved_searches.py` & `splunk-appinspect-2.9.1/splunk_appinspect/saved_searches.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/splunk/__init__.py` & `splunk-appinspect-2.9.1/splunk_appinspect/splunk/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/splunk/splunk_default_source_type_list.py` & `splunk-appinspect-2.9.1/splunk_appinspect/splunk/splunk_default_source_type_list.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/splunk/telemetry/list.csv` & `splunk-appinspect-2.9.1/splunk_appinspect/splunk/telemetry/list.csv`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/splunk/util.py` & `splunk-appinspect-2.9.1/splunk_appinspect/splunk/util.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/splunk_default_source_type_list.py` & `splunk-appinspect-2.9.1/splunk_appinspect/splunk_default_source_type_list.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/splunk_defined_authorize_capability_list.py` & `splunk-appinspect-2.9.1/splunk_appinspect/splunk_defined_authorize_capability_list.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/splunk_defined_conf_file_list.py` & `splunk-appinspect-2.9.1/splunk_appinspect/splunk_defined_conf_file_list.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/splunk_pretrained_sourcetypes_list.py` & `splunk-appinspect-2.9.1/splunk_appinspect/splunk_pretrained_sourcetypes_list.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/telemetry_configuration_file.py` & `splunk-appinspect-2.9.1/splunk_appinspect/telemetry_configuration_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/templates/html_criteria.html` & `splunk-appinspect-2.9.1/splunk_appinspect/templates/html_criteria.html`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/templates/tag_reference.html` & `splunk-appinspect-2.9.1/splunk_appinspect/templates/tag_reference.html`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/validation_report.py` & `splunk-appinspect-2.9.1/splunk_appinspect/validation_report.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/validator.py` & `splunk-appinspect-2.9.1/splunk_appinspect/validator.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/version/version.py` & `splunk-appinspect-2.9.1/splunk_appinspect/version/version.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect/workflow_actions.py` & `splunk-appinspect-2.9.1/splunk_appinspect/workflow_actions.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect.egg-info/PKG-INFO` & `splunk-appinspect-2.9.1/splunk_appinspect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: splunk-appinspect
-Version: 2.9.0
+Version: 2.9.1
 Summary: Automatic validation checks for Splunk Apps
 Home-page: https://splunk.com
 Author: Splunk
 Author-email: appinspect@splunk.com
 License: Other/Proprietary License
 Download-URL: http://dev.splunk.com/goto/appinspectdownload
 Description: AppInspect is a tool for assessing a Splunk App's compliance with Splunk recommended development practices, by using static analysis. AppInspect is open for extension, allowing other teams to compose checks that meet their domain specific needs for semi- or fully-automated analysis and validation of Splunk Apps.
```

### Comparing `splunk-appinspect-2.9.0/splunk_appinspect.egg-info/SOURCES.txt` & `splunk-appinspect-2.9.1/splunk_appinspect.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -280,15 +280,15 @@
 splunk_appinspect/python_modules_metadata/metadata_common/metadata_consts.py
 splunk_appinspect/python_modules_metadata/metadata_common/metadata_decorator.py
 splunk_appinspect/python_modules_metadata/metadata_common/metadata_exceptions.py
 splunk_appinspect/python_modules_metadata/metadata_common/metadata_types.py
 splunk_appinspect/splunk/__init__.py
 splunk_appinspect/splunk/splunk_default_source_type_list.py
 splunk_appinspect/splunk/util.py
-splunk_appinspect/splunk/jquery_checks_data/disallowed_imports.json
+splunk_appinspect/splunk/jquery_checks_data/supported_modules.json
 splunk_appinspect/splunk/telemetry/__init__.py
 splunk_appinspect/splunk/telemetry/core.py
 splunk_appinspect/splunk/telemetry/list.csv
 splunk_appinspect/templates/html_criteria.html
 splunk_appinspect/templates/tag_reference.html
 splunk_appinspect/version/VERSION.txt
 splunk_appinspect/version/__init__.py
```

