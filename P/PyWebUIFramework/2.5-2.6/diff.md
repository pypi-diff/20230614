# Comparing `tmp/PyWebUIFramework-2.5.tar.gz` & `tmp/PyWebUIFramework-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyWebUIFramework-2.5.tar", last modified: Sat Jun  3 01:06:59 2023, max compression
+gzip compressed data, was "dist\PyWebUIFramework-2.6.tar", last modified: Tue Jun 13 22:19:43 2023, max compression
```

## Comparing `PyWebUIFramework-2.5.tar` & `PyWebUIFramework-2.6.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:59.000000 PyWebUIFramework-2.5/
--rw-rw-rw-   0        0        0       38 2023-06-03 01:03:59.000000 PyWebUIFramework-2.5/MANIFEST.in
--rw-rw-rw-   0        0        0      281 2023-06-03 01:06:59.000000 PyWebUIFramework-2.5/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-06-01 17:52:31.000000 PyWebUIFramework-2.5/README.md
--rw-rw-rw-   0        0        0      115 2023-06-03 01:06:59.000000 PyWebUIFramework-2.5/setup.cfg
--rw-rw-rw-   0        0        0     1135 2023-06-03 01:04:55.000000 PyWebUIFramework-2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/PyWebUIFramework.egg-info/
--rw-rw-rw-   0        0        0      281 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/PyWebUIFramework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4824 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/PyWebUIFramework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/PyWebUIFramework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      171 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/PyWebUIFramework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/PyWebUIFramework.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/browser/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/browser/__init__.py
--rw-rw-rw-   0        0        0      144 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/browser/alert_actions.py
--rw-rw-rw-   0        0        0     2152 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/browser/base_browser_factory.py
--rw-rw-rw-   0        0        0     8156 2023-06-02 23:00:37.000000 PyWebUIFramework-2.5/src/browser/browser.py
--rw-rw-rw-   0        0        0     1123 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/browser/browser_module.py
--rw-rw-rw-   0        0        0      200 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/browser/browser_name.py
--rw-rw-rw-   0        0        0     3121 2023-06-01 18:36:29.000000 PyWebUIFramework-2.5/src/browser/browser_tab_navigation.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/browser/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/browser/interfaces/__init__.py
--rw-rw-rw-   0        0        0      567 2023-06-01 18:27:00.000000 PyWebUIFramework-2.5/src/browser/interfaces/browser_factory_interface.py
--rw-rw-rw-   0        0        0      778 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/browser/java_script.py
--rw-rw-rw-   0        0        0     2621 2023-06-02 19:04:26.000000 PyWebUIFramework-2.5/src/browser/local_browser_factory.py
--rw-rw-rw-   0        0        0     4731 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/browser/py_quality_services.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/configuration/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/configuration/__init__.py
--rw-rw-rw-   0        0        0     2859 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/configuration/browser_profile.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/configuration/driver_settings/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/configuration/driver_settings/__init__.py
--rw-rw-rw-   0        0        0     4307 2023-06-01 18:27:00.000000 PyWebUIFramework-2.5/src/configuration/driver_settings/base_driver_settings.py
--rw-rw-rw-   0        0        0      968 2023-06-01 18:27:00.000000 PyWebUIFramework-2.5/src/configuration/driver_settings/chrome_settings.py
--rw-rw-rw-   0        0        0     1022 2023-06-01 18:27:00.000000 PyWebUIFramework-2.5/src/configuration/driver_settings/edge_settings.py
--rw-rw-rw-   0        0        0     1032 2023-06-01 18:27:00.000000 PyWebUIFramework-2.5/src/configuration/driver_settings/firefox_settings.py
--rw-rw-rw-   0        0        0      736 2023-06-01 18:27:00.000000 PyWebUIFramework-2.5/src/configuration/driver_settings/iexplorer_settings.py
--rw-rw-rw-   0        0        0      142 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/configuration/timeout.py
--rw-rw-rw-   0        0        0     1388 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/configuration/timeout_configuration.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/core/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/core/applications/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/applications/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/core/applications/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/applications/interfaces/__init__.py
--rw-rw-rw-   0        0        0      331 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/applications/interfaces/application_interface.py
--rw-rw-rw-   0        0        0     3301 2023-06-01 18:27:00.000000 PyWebUIFramework-2.5/src/core/applications/quality_module.py
--rw-rw-rw-   0        0        0     2255 2023-06-01 18:36:29.000000 PyWebUIFramework-2.5/src/core/applications/quality_services.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/core/configurations/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/configurations/__init__.py
--rw-rw-rw-   0        0        0     1587 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/core/configurations/configuration_module.py
--rw-rw-rw-   0        0        0      526 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/core/configurations/element_cache_configuration.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/core/configurations/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/configurations/interfaces/__init__.py
--rw-rw-rw-   0        0        0     1681 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/core/configurations/interfaces/browser_profile_interface.py
--rw-rw-rw-   0        0        0      549 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/configurations/interfaces/retry_configuration_interface.py
--rw-rw-rw-   0        0        0     1466 2023-06-01 18:27:00.000000 PyWebUIFramework-2.5/src/core/configurations/interfaces/timeout_configuration_interface.py
--rw-rw-rw-   0        0        0      882 2023-06-01 18:27:00.000000 PyWebUIFramework-2.5/src/core/configurations/retry_configuration.py
--rw-rw-rw-   0        0        0     1198 2023-06-01 18:27:00.000000 PyWebUIFramework-2.5/src/core/configurations/timeout_configuration.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/core/elements/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/elements/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/core/elements/actions/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/elements/actions/__init__.py
--rw-rw-rw-   0        0        0     2809 2023-06-01 18:27:00.000000 PyWebUIFramework-2.5/src/core/elements/actions/js_actions.py
--rw-rw-rw-   0        0        0    11790 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/core/elements/base_element.py
--rw-rw-rw-   0        0        0     1866 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/core/elements/base_element_cache_handler.py
--rw-rw-rw-   0        0        0     5701 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/core/elements/base_element_factory.py
--rw-rw-rw-   0        0        0     2566 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/core/elements/base_parent_element.py
--rw-rw-rw-   0        0        0      797 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/core/elements/element_cache_handler.py
--rw-rw-rw-   0        0        0     8552 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/core/elements/element_factory.py
--rw-rw-rw-   0        0        0     3985 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/core/elements/element_finder.py
--rw-rw-rw-   0        0        0     2504 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/core/elements/element_finder_interface.py
--rw-rw-rw-   0        0        0      147 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/elements/highlight_state.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/core/elements/states/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/elements/states/__init__.py
--rw-rw-rw-   0        0        0     4306 2023-06-01 18:36:29.000000 PyWebUIFramework-2.5/src/core/elements/states/base_element_state_provider.py
--rw-rw-rw-   0        0        0     6787 2023-06-01 18:36:29.000000 PyWebUIFramework-2.5/src/core/elements/states/cached_element_state_provider.py
--rw-rw-rw-   0        0        0     1008 2023-06-01 18:36:29.000000 PyWebUIFramework-2.5/src/core/elements/states/desired_state.py
--rw-rw-rw-   0        0        0      105 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/elements/states/element_count.py
--rw-rw-rw-   0        0        0      614 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/elements/states/element_state.py
--rw-rw-rw-   0        0        0     2720 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/core/elements/states/element_state_provider.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/core/localization/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/localization/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/core/localization/configurations/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/localization/configurations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/core/localization/configurations/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/localization/configurations/interfaces/__init__.py
--rw-rw-rw-   0        0        0      559 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/localization/configurations/interfaces/logger_configuration_interface.py
--rw-rw-rw-   0        0        0      991 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/core/localization/configurations/logger_configuration.py
--rw-rw-rw-   0        0        0      921 2023-06-01 18:36:29.000000 PyWebUIFramework-2.5/src/core/localization/localization_module.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/core/localization/loggers/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/localization/loggers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/core/localization/loggers/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/localization/loggers/interfaces/__init__.py
--rw-rw-rw-   0        0        0     3696 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/core/localization/loggers/interfaces/localized_logger_interface.py
--rw-rw-rw-   0        0        0     3895 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/core/localization/loggers/localized_logger.py
--rw-rw-rw-   0        0        0      332 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/localization/loggers/logger_config.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/core/localization/managers/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/localization/managers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/core/localization/managers/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/localization/managers/interfaces/__init__.py
--rw-rw-rw-   0        0        0      508 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/localization/managers/interfaces/localization_interface.py
--rw-rw-rw-   0        0        0     2258 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/core/localization/managers/localization_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/core/resources/
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/core/resources/js/
--rw-rw-rw-   0        0        0       42 2023-06-02 16:56:53.000000 PyWebUIFramework-2.5/src/core/resources/js/borderElement.js
--rw-rw-rw-   0        0        0       21 2023-06-02 16:56:53.000000 PyWebUIFramework-2.5/src/core/resources/js/clickElement.js
--rw-rw-rw-   0        0        0       75 2023-06-02 16:56:53.000000 PyWebUIFramework-2.5/src/core/resources/js/getCheckBoxState.js
--rw-rw-rw-   0        0        0       31 2023-06-02 16:56:53.000000 PyWebUIFramework-2.5/src/core/resources/js/getElementText.js
--rw-rw-rw-   0        0        0       26 2023-06-02 16:56:53.000000 PyWebUIFramework-2.5/src/core/resources/js/openInNewTab.js
--rw-rw-rw-   0        0        0       14 2023-06-02 16:56:53.000000 PyWebUIFramework-2.5/src/core/resources/js/openNewTab.js
--rw-rw-rw-   0        0        0       73 2023-06-02 16:56:53.000000 PyWebUIFramework-2.5/src/core/resources/js/pageLoaded.js
--rw-rw-rw-   0        0        0       48 2023-06-02 16:56:53.000000 PyWebUIFramework-2.5/src/core/resources/js/scrollBy.js
--rw-rw-rw-   0        0        0       42 2023-06-02 16:56:53.000000 PyWebUIFramework-2.5/src/core/resources/js/scrollWindowBy.js
--rw-rw-rw-   0        0        0       31 2023-06-02 16:56:53.000000 PyWebUIFramework-2.5/src/core/resources/js/setValue.js
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/core/resources/localization/
--rw-rw-rw-   0        0        0     6717 2023-06-02 16:56:53.000000 PyWebUIFramework-2.5/src/core/resources/localization/be.json
--rw-rw-rw-   0        0        0     4495 2023-06-02 16:56:53.000000 PyWebUIFramework-2.5/src/core/resources/localization/en.json
--rw-rw-rw-   0        0        0     6771 2023-06-02 16:56:53.000000 PyWebUIFramework-2.5/src/core/resources/localization/ru.json
--rw-rw-rw-   0        0        0     2444 2023-06-02 19:11:28.000000 PyWebUIFramework-2.5/src/core/resources/settings.json
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/core/utilities/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/utilities/__init__.py
--rw-rw-rw-   0        0        0     1683 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/core/utilities/action_repeater.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/core/utilities/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/utilities/interfaces/__init__.py
--rw-rw-rw-   0        0        0      571 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/utilities/interfaces/action_repeater_interface.py
--rw-rw-rw-   0        0        0     1619 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/utilities/interfaces/settings_file_interface.py
--rw-rw-rw-   0        0        0     3387 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/core/utilities/json_settings_file.py
--rw-rw-rw-   0        0        0     3034 2023-06-02 17:00:05.000000 PyWebUIFramework-2.5/src/core/utilities/resource_file.py
--rw-rw-rw-   0        0        0      391 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/core/utilities/utilities_module.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/core/waitings/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/waitings/__init__.py
--rw-rw-rw-   0        0        0     5521 2023-06-02 23:10:44.000000 PyWebUIFramework-2.5/src/core/waitings/conditional_wait.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:58.000000 PyWebUIFramework-2.5/src/core/waitings/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/waitings/interfaces/__init__.py
--rw-rw-rw-   0        0        0     2722 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/core/waitings/interfaces/conditional_wait_interface.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:59.000000 PyWebUIFramework-2.5/src/elements/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/elements/__init__.py
--rw-rw-rw-   0        0        0      222 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/elements/attributes.py
--rw-rw-rw-   0        0        0      215 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/elements/button.py
--rw-rw-rw-   0        0        0      516 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/elements/check_box.py
--rw-rw-rw-   0        0        0      436 2023-06-01 18:36:29.000000 PyWebUIFramework-2.5/src/elements/checkable_element.py
--rw-rw-rw-   0        0        0      295 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/elements/combo_box.py
--rw-rw-rw-   0        0        0     1694 2023-06-01 18:36:29.000000 PyWebUIFramework-2.5/src/elements/element_factory.py
--rw-rw-rw-   0        0        0      213 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/elements/label.py
--rw-rw-rw-   0        0        0      292 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/elements/link.py
--rw-rw-rw-   0        0        0      229 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/elements/radio_button.py
--rw-rw-rw-   0        0        0     1780 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/elements/text_box.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:06:59.000000 PyWebUIFramework-2.5/src/forms/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.5/src/forms/__init__.py
--rw-rw-rw-   0        0        0     1174 2023-06-01 18:36:30.000000 PyWebUIFramework-2.5/src/forms/base_form.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/
+-rw-rw-rw-   0        0        0       67 2023-06-13 22:18:55.000000 PyWebUIFramework-2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      281 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3222 2023-06-13 22:15:22.000000 PyWebUIFramework-2.6/README.md
+-rw-rw-rw-   0        0        0      115 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1174 2023-06-13 22:18:55.000000 PyWebUIFramework-2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:42.000000 PyWebUIFramework-2.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:42.000000 PyWebUIFramework-2.6/src/PyWebUIFramework.egg-info/
+-rw-rw-rw-   0        0        0      281 2023-06-13 22:19:42.000000 PyWebUIFramework-2.6/src/PyWebUIFramework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4824 2023-06-13 22:19:42.000000 PyWebUIFramework-2.6/src/PyWebUIFramework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 22:19:42.000000 PyWebUIFramework-2.6/src/PyWebUIFramework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      198 2023-06-13 22:19:42.000000 PyWebUIFramework-2.6/src/PyWebUIFramework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 22:19:42.000000 PyWebUIFramework-2.6/src/PyWebUIFramework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/browser/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/browser/__init__.py
+-rw-rw-rw-   0        0        0      140 2023-06-07 13:55:32.000000 PyWebUIFramework-2.6/src/browser/alert_actions.py
+-rw-rw-rw-   0        0        0     2152 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6/src/browser/base_browser_factory.py
+-rw-rw-rw-   0        0        0     8174 2023-06-10 12:55:40.000000 PyWebUIFramework-2.6/src/browser/browser.py
+-rw-rw-rw-   0        0        0     1123 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6/src/browser/browser_module.py
+-rw-rw-rw-   0        0        0      200 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/browser/browser_name.py
+-rw-rw-rw-   0        0        0     3121 2023-06-01 18:36:29.000000 PyWebUIFramework-2.6/src/browser/browser_tab_navigation.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/browser/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/browser/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      563 2023-06-07 13:56:57.000000 PyWebUIFramework-2.6/src/browser/interfaces/browser_factory_interface.py
+-rw-rw-rw-   0        0        0      778 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6/src/browser/java_script.py
+-rw-rw-rw-   0        0        0     2621 2023-06-02 19:04:26.000000 PyWebUIFramework-2.6/src/browser/local_browser_factory.py
+-rw-rw-rw-   0        0        0     5002 2023-06-07 14:03:45.000000 PyWebUIFramework-2.6/src/browser/py_quality_services.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/configuration/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/configuration/__init__.py
+-rw-rw-rw-   0        0        0     2859 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6/src/configuration/browser_profile.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/configuration/driver_settings/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/configuration/driver_settings/__init__.py
+-rw-rw-rw-   0        0        0     4307 2023-06-01 18:27:00.000000 PyWebUIFramework-2.6/src/configuration/driver_settings/base_driver_settings.py
+-rw-rw-rw-   0        0        0      968 2023-06-01 18:27:00.000000 PyWebUIFramework-2.6/src/configuration/driver_settings/chrome_settings.py
+-rw-rw-rw-   0        0        0     1022 2023-06-01 18:27:00.000000 PyWebUIFramework-2.6/src/configuration/driver_settings/edge_settings.py
+-rw-rw-rw-   0        0        0     1032 2023-06-01 18:27:00.000000 PyWebUIFramework-2.6/src/configuration/driver_settings/firefox_settings.py
+-rw-rw-rw-   0        0        0      736 2023-06-01 18:27:00.000000 PyWebUIFramework-2.6/src/configuration/driver_settings/iexplorer_settings.py
+-rw-rw-rw-   0        0        0      142 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/configuration/timeout.py
+-rw-rw-rw-   0        0        0     1388 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6/src/configuration/timeout_configuration.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/core/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/core/applications/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/applications/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/core/applications/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/applications/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      331 2023-06-07 13:19:23.000000 PyWebUIFramework-2.6/src/core/applications/interfaces/application_interface.py
+-rw-rw-rw-   0        0        0     3301 2023-06-01 18:27:00.000000 PyWebUIFramework-2.6/src/core/applications/quality_module.py
+-rw-rw-rw-   0        0        0     2255 2023-06-07 12:34:08.000000 PyWebUIFramework-2.6/src/core/applications/quality_services.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/core/configurations/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/configurations/__init__.py
+-rw-rw-rw-   0        0        0     1587 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6/src/core/configurations/configuration_module.py
+-rw-rw-rw-   0        0        0      526 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6/src/core/configurations/element_cache_configuration.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/core/configurations/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/configurations/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     1681 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6/src/core/configurations/interfaces/browser_profile_interface.py
+-rw-rw-rw-   0        0        0      549 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/configurations/interfaces/retry_configuration_interface.py
+-rw-rw-rw-   0        0        0     1667 2023-06-10 12:45:38.000000 PyWebUIFramework-2.6/src/core/configurations/interfaces/timeout_configuration_interface.py
+-rw-rw-rw-   0        0        0      874 2023-06-07 13:58:03.000000 PyWebUIFramework-2.6/src/core/configurations/retry_configuration.py
+-rw-rw-rw-   0        0        0     1190 2023-06-07 13:56:36.000000 PyWebUIFramework-2.6/src/core/configurations/timeout_configuration.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/core/elements/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/elements/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/core/elements/actions/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/elements/actions/__init__.py
+-rw-rw-rw-   0        0        0     2906 2023-06-10 12:57:02.000000 PyWebUIFramework-2.6/src/core/elements/actions/js_actions.py
+-rw-rw-rw-   0        0        0    11790 2023-06-07 13:03:03.000000 PyWebUIFramework-2.6/src/core/elements/base_element.py
+-rw-rw-rw-   0        0        0     1866 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6/src/core/elements/base_element_cache_handler.py
+-rw-rw-rw-   0        0        0     5701 2023-06-07 13:03:03.000000 PyWebUIFramework-2.6/src/core/elements/base_element_factory.py
+-rw-rw-rw-   0        0        0     2566 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6/src/core/elements/base_parent_element.py
+-rw-rw-rw-   0        0        0      795 2023-06-07 13:55:20.000000 PyWebUIFramework-2.6/src/core/elements/element_cache_handler.py
+-rw-rw-rw-   0        0        0     8552 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6/src/core/elements/element_factory.py
+-rw-rw-rw-   0        0        0     3985 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6/src/core/elements/element_finder.py
+-rw-rw-rw-   0        0        0     2504 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6/src/core/elements/element_finder_interface.py
+-rw-rw-rw-   0        0        0      147 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/elements/highlight_state.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/core/elements/states/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/elements/states/__init__.py
+-rw-rw-rw-   0        0        0     4304 2023-06-07 13:55:13.000000 PyWebUIFramework-2.6/src/core/elements/states/base_element_state_provider.py
+-rw-rw-rw-   0        0        0     6787 2023-06-01 18:36:29.000000 PyWebUIFramework-2.6/src/core/elements/states/cached_element_state_provider.py
+-rw-rw-rw-   0        0        0     1008 2023-06-01 18:36:29.000000 PyWebUIFramework-2.6/src/core/elements/states/desired_state.py
+-rw-rw-rw-   0        0        0      105 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/elements/states/element_count.py
+-rw-rw-rw-   0        0        0      614 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/elements/states/element_state.py
+-rw-rw-rw-   0        0        0     2720 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6/src/core/elements/states/element_state_provider.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/core/localization/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/localization/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/core/localization/configurations/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/localization/configurations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/core/localization/configurations/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/localization/configurations/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      559 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/localization/configurations/interfaces/logger_configuration_interface.py
+-rw-rw-rw-   0        0        0      989 2023-06-07 13:55:09.000000 PyWebUIFramework-2.6/src/core/localization/configurations/logger_configuration.py
+-rw-rw-rw-   0        0        0      921 2023-06-01 18:36:29.000000 PyWebUIFramework-2.6/src/core/localization/localization_module.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/core/localization/loggers/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/localization/loggers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/core/localization/loggers/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/localization/loggers/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     3696 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6/src/core/localization/loggers/interfaces/localized_logger_interface.py
+-rw-rw-rw-   0        0        0     3889 2023-06-07 13:54:24.000000 PyWebUIFramework-2.6/src/core/localization/loggers/localized_logger.py
+-rw-rw-rw-   0        0        0      332 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/localization/loggers/logger_config.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/core/localization/managers/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/localization/managers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/core/localization/managers/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/localization/managers/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/localization/managers/interfaces/localization_interface.py
+-rw-rw-rw-   0        0        0     2258 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6/src/core/localization/managers/localization_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/core/resources/
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/core/resources/js/
+-rw-rw-rw-   0        0        0       42 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6/src/core/resources/js/borderElement.js
+-rw-rw-rw-   0        0        0       21 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6/src/core/resources/js/clickElement.js
+-rw-rw-rw-   0        0        0       75 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6/src/core/resources/js/getCheckBoxState.js
+-rw-rw-rw-   0        0        0       31 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6/src/core/resources/js/getElementText.js
+-rw-rw-rw-   0        0        0       26 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6/src/core/resources/js/openInNewTab.js
+-rw-rw-rw-   0        0        0       14 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6/src/core/resources/js/openNewTab.js
+-rw-rw-rw-   0        0        0       73 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6/src/core/resources/js/pageLoaded.js
+-rw-rw-rw-   0        0        0       48 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6/src/core/resources/js/scrollBy.js
+-rw-rw-rw-   0        0        0       42 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6/src/core/resources/js/scrollWindowBy.js
+-rw-rw-rw-   0        0        0       31 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6/src/core/resources/js/setValue.js
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/core/resources/localization/
+-rw-rw-rw-   0        0        0     6717 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6/src/core/resources/localization/be.json
+-rw-rw-rw-   0        0        0     4495 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6/src/core/resources/localization/en.json
+-rw-rw-rw-   0        0        0     6771 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6/src/core/resources/localization/ru.json
+-rw-rw-rw-   0        0        0     2445 2023-06-10 12:57:35.000000 PyWebUIFramework-2.6/src/core/resources/settings.json
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/core/utilities/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1675 2023-06-07 13:56:12.000000 PyWebUIFramework-2.6/src/core/utilities/action_repeater.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/core/utilities/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/utilities/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      571 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/utilities/interfaces/action_repeater_interface.py
+-rw-rw-rw-   0        0        0     1619 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/utilities/interfaces/settings_file_interface.py
+-rw-rw-rw-   0        0        0     3387 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6/src/core/utilities/json_settings_file.py
+-rw-rw-rw-   0        0        0     3034 2023-06-02 17:00:05.000000 PyWebUIFramework-2.6/src/core/utilities/resource_file.py
+-rw-rw-rw-   0        0        0      391 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6/src/core/utilities/utilities_module.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/core/waitings/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/waitings/__init__.py
+-rw-rw-rw-   0        0        0     5521 2023-06-07 13:03:39.000000 PyWebUIFramework-2.6/src/core/waitings/conditional_wait.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/core/waitings/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/waitings/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     2722 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/core/waitings/interfaces/conditional_wait_interface.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/elements/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/elements/__init__.py
+-rw-rw-rw-   0        0        0      222 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/elements/attributes.py
+-rw-rw-rw-   0        0        0      215 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6/src/elements/button.py
+-rw-rw-rw-   0        0        0      516 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6/src/elements/check_box.py
+-rw-rw-rw-   0        0        0      436 2023-06-01 18:36:29.000000 PyWebUIFramework-2.6/src/elements/checkable_element.py
+-rw-rw-rw-   0        0        0      297 2023-06-07 13:55:00.000000 PyWebUIFramework-2.6/src/elements/combo_box.py
+-rw-rw-rw-   0        0        0     1694 2023-06-01 18:36:29.000000 PyWebUIFramework-2.6/src/elements/element_factory.py
+-rw-rw-rw-   0        0        0      213 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6/src/elements/label.py
+-rw-rw-rw-   0        0        0      292 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6/src/elements/link.py
+-rw-rw-rw-   0        0        0      229 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6/src/elements/radio_button.py
+-rw-rw-rw-   0        0        0     1780 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6/src/elements/text_box.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:19:43.000000 PyWebUIFramework-2.6/src/forms/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6/src/forms/__init__.py
+-rw-rw-rw-   0        0        0     1050 2023-06-10 13:04:02.000000 PyWebUIFramework-2.6/src/forms/base_form.py
```

### Comparing `PyWebUIFramework-2.5/setup.py` & `PyWebUIFramework-2.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # PATH VARIABLES
 SOURCE_NAME = "src"
 FRAMEWORK_NAME = "PyWebUIFramework"
 PATH_TO_RESOURCES = os.path.join(SOURCE_NAME, "core", "resources.*")
 
 # PROJECT VARIABLES
-CURRENT_VERSION = "2.5"
+CURRENT_VERSION = "2.6"
 LICENSE_TYPE = "MIT"
 
 # AUTHOR VARIABLES
 AUTHOR_FULL_NAME = "Philip Vasilevsky"
 AUTHOR_EMAIL = "fil13698@gmail.com"
 LINK_TO_REPO = "https://github.com/philip136/PyWebUIFramework"
 
@@ -35,10 +35,11 @@
         'injector==0.18.4',
         'jsonpath-ng==1.5.3',
         'loguru==0.5.3',
         'selenium==4.9.1',
         'typing-extensions==3.10.0.2',
         'webdriver-manager==3.8.6',
         'urllib3==1.26.6',
-        'get-project-root==0.2'
+        'get-project-root==0.2',
+        'importlib-metadata==4.13.0'
     ]
 )
```

### Comparing `PyWebUIFramework-2.5/src/PyWebUIFramework.egg-info/SOURCES.txt` & `PyWebUIFramework-2.6/src/PyWebUIFramework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/browser/base_browser_factory.py` & `PyWebUIFramework-2.6/src/browser/base_browser_factory.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/browser/browser.py` & `PyWebUIFramework-2.6/src/browser/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import typing as ty
 
-from selenium.webdriver.remote.webelement import WebElement
 from selenium.common.exceptions import NoAlertPresentException
 from selenium.webdriver.remote.webdriver import WebDriver
 from core.applications.interfaces.application_interface import IApplication
 from core.configurations.interfaces.browser_profile_interface import IBrowserProfile
 from core.localization.loggers.interfaces.localized_logger_interface import ILocalizedLogger
 from core.configurations.interfaces.timeout_configuration_interface import ITimeoutConfiguration
 from core.waitings.conditional_wait import ConditionalWait
 from browser.browser_tab_navigation import BrowserTabNavigation
 from browser.java_script import JavaScript
 from browser.alert_actions import AlertActions
+from core.elements.base_element import BaseParentElement
 
 WD = ty.TypeVar('WD', bound=WebDriver)
 
 
 class Browser(IApplication):
     def __init__(self, driver: WD, localized_logger: ILocalizedLogger, browser_profile: IBrowserProfile,
                  timeouts: ITimeoutConfiguration) -> None:
@@ -161,19 +161,19 @@
         self.__localized_logger.info('loc.browser.page.wait')
         self.__conditional_wait.wait_for(condition=lambda: self.execute_script(JavaScript.IS_PAGE_LOADED.get_script()),
                                          timeout=self.__timeouts.page_load,
                                          polling_interval=self.__timeouts.polling_interval)
 
         self.__localized_logger.localization_manager.get_localized_message('loc.browser.page.timeout')
 
-    def switch_to_frame(self, element: WebElement) -> None:
+    def switch_to_frame(self, element: BaseParentElement) -> None:
         """Switch to iframe.
         :param element: IFrame element.
         """
-        self.__driver.switch_to.frame(element)
+        self.__driver.switch_to.frame(element.get_element())
 
     @property
     def tabs(self) -> BrowserTabNavigation:
         """Provides interface to manage of browser tabs.
         :return: Instance of BrowserTabNavigation.
         :rtype: BrowserTabNavigation.
         """
```

### Comparing `PyWebUIFramework-2.5/src/browser/browser_module.py` & `PyWebUIFramework-2.6/src/browser/browser_module.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/browser/browser_tab_navigation.py` & `PyWebUIFramework-2.6/src/browser/browser_tab_navigation.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/browser/interfaces/browser_factory_interface.py` & `PyWebUIFramework-2.6/src/browser/interfaces/browser_factory_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     @abstractmethod
     def get_browser(self) -> Browser:
         """Get browser instance
         :return: Browser instance.
         :rtype: Browser.
         """
         pass
-    
+
     @abstractmethod
     def get_driver(self) -> WD:
         """Abstract method for selecting the required driver (Firefox, Chrome and etc).
         :return: WebDriver.
         :rtype: WD.
         """
         pass
```

### Comparing `PyWebUIFramework-2.5/src/browser/java_script.py` & `PyWebUIFramework-2.6/src/browser/java_script.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/browser/local_browser_factory.py` & `PyWebUIFramework-2.6/src/browser/local_browser_factory.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/browser/py_quality_services.py` & `PyWebUIFramework-2.6/src/browser/py_quality_services.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,114 +14,125 @@
 
 T = ty.TypeVar('T', bound=QualityServices)
 BF = ty.TypeVar('BF', bound=BaseBrowserFactory)
 
 LOCAL = local()
 
 
+class classproperty(property):
+    def __get__(self, obj, obj_type=None):
+        return super(classproperty, self).__get__(obj_type)
+
+    def __set__(self, obj, value):
+        super(classproperty, self).__set__(type(obj), value)
+
+    def __delete__(self, obj):
+        super(classproperty, self).__delete__(type(obj))
+
+
 class PyQualityServices(QualityServices):
     def __init__(self) -> None:
         """Create BrowserModule which bound main objects."""
         service_module = BrowserModule(self.get_browser)
         super(PyQualityServices, self).__init__(application_provider=self.get_browser, service_module=service_module)
 
     @classmethod
     def get_browser(cls) -> Browser:
         """Get browser instance.
         :return: Browser instance.
         :rtype: Browser.
         """
-        return cls.get_instance().get_app(cls.__start_browser)
+        return cls.instance.get_app(cls.__start_browser)
 
     @classmethod
     def __start_browser(cls) -> Browser:
         """Choose interface for future browser.
         :return: Browser instance.
         :rtype: Browser.
         """
-        return cls.get_browser_factory().get_browser()
+        return cls.browser_factory.get_browser()
 
-    @classmethod
-    def get_browser_factory(cls) -> BF:
+    @classproperty
+    def browser_factory(cls) -> BaseBrowserFactory:
         """Select a factory for browsers if it does not exist, install it.
         :return: Factory that implements BaseBrowserFactory.
         :rtype: BF.
         """
-        if getattr(cls.get_instance(), 'browser_factory', None) is None:
+        if not getattr(cls.instance, '_browser_factory', None):
             cls.set_default_browser_factory()
-        return cls.get_instance().browser_factory
+        return cls.instance.browser_factory
 
-    @classmethod
-    def set_browser_factory(cls, browser_factory: BF) -> None:
+    @browser_factory.setter
+    def browser_factory(cls, browser_factory: BF) -> None:
         """Set factory in current instance that implements BaseBrowserFactory.
         :param browser_factory: Factory implementing the interface BaseBrowserFactory.
         """
-        setattr(cls.get_instance().__class__, 'browser_factory', browser_factory)
+        setattr(cls.instance.__class__, '_browser_factory', browser_factory)
 
     @classmethod
     def set_default_browser_factory(cls) -> None:
         """Choose interface for browser factory."""
-        browser_factory = cls.get_local_browser_factory()
-        cls.set_browser_factory(browser_factory=browser_factory)
+        browser_factory = cls.local_browser_factory
+        cls.browser_factory = browser_factory
 
-    @classmethod
-    def get_instance(cls) -> T:
+    @classproperty
+    def instance(cls) -> T:
         """Get or create current instance.
         :return: Get or create current class.
         :rtype: T.
         """
         if getattr(LOCAL, '_instance_container', None) is None:
             setattr(LOCAL, '_instance_container', cls())
         return getattr(LOCAL, '_instance_container', None)
 
-    @classmethod
-    def get_service_provider(cls) -> Injector:
+    @classproperty
+    def service_provider(cls) -> Injector:
         """Get injector instance.
         :return: Injector object.
         :rtype: Injector.
         """
-        return cls.get_instance().get_injector()
+        return cls.instance.get_injector()
 
     @classmethod
     def get(cls, clz: ty.Any) -> ty.Any:
         """Get instance from injector instance.
         :param clz: Class that is associated.
         :return: Instance which is registered in injector.
         :rtype: ty.Any.
         """
-        return cls.get_service_provider().get(clz)
+        return cls.service_provider.get(clz)
 
-    @classmethod
-    def get_local_browser_factory(cls) -> LocalBaseBrowserFactory:
+    @classproperty
+    def local_browser_factory(cls) -> LocalBaseBrowserFactory:
         """Get LocalBaseBrowserFactory from injector instance which implements BaseBrowserFactory.
         :return: Get LocalBaseBrowserFactory instance.
         :rtype: LocalBaseBrowserFactory.
         """
         return cls.get(LocalBaseBrowserFactory)
 
-    @classmethod
-    def get_element_factory(cls) -> ElementFactory:
+    @classproperty
+    def element_factory(cls) -> ElementFactory:
         return cls.get(ElementFactory)
 
-    @classmethod
-    def get_browser_profile(cls) -> BrowserProfile:
+    @classproperty
+    def browser_profile(cls) -> BrowserProfile:
         """Get BrowserProfile from injector instance which implements IBrowserProfile.
         :return: Get BrowserProfile instance.
         :rtype: BrowserProfile.
         """
         return cls.get(BrowserProfile)
 
-    @classmethod
-    def get_conditional_wait(cls) -> ConditionalWait:
+    @classproperty
+    def conditional_wait(cls) -> ConditionalWait:
         """Get ConditionalWait from injector instance.
         :return: Get ConditionalWait instance.
         :rtype: ConditionalWait.
         """
         return cls.get(ConditionalWait)
 
-    @classmethod
-    def get_localized_logger(cls) -> ILocalizedLogger:
+    @classproperty
+    def localized_logger(cls) -> ILocalizedLogger:
         """Get LocalizationLogger from injector instance.
         :return: Get LocalizationLogger instance.
         :rtype: LocalizationLogger.
         """
         return cls.get(ILocalizedLogger)
```

### Comparing `PyWebUIFramework-2.5/src/configuration/browser_profile.py` & `PyWebUIFramework-2.6/src/configuration/browser_profile.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/configuration/driver_settings/base_driver_settings.py` & `PyWebUIFramework-2.6/src/configuration/driver_settings/base_driver_settings.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/configuration/driver_settings/chrome_settings.py` & `PyWebUIFramework-2.6/src/configuration/driver_settings/chrome_settings.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/configuration/driver_settings/edge_settings.py` & `PyWebUIFramework-2.6/src/configuration/driver_settings/edge_settings.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/configuration/driver_settings/firefox_settings.py` & `PyWebUIFramework-2.6/src/configuration/driver_settings/firefox_settings.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/configuration/driver_settings/iexplorer_settings.py` & `PyWebUIFramework-2.6/src/configuration/driver_settings/iexplorer_settings.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/configuration/timeout_configuration.py` & `PyWebUIFramework-2.6/src/configuration/timeout_configuration.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/applications/quality_module.py` & `PyWebUIFramework-2.6/src/core/applications/quality_module.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/applications/quality_services.py` & `PyWebUIFramework-2.6/src/core/applications/quality_services.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/configurations/configuration_module.py` & `PyWebUIFramework-2.6/src/core/configurations/configuration_module.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/configurations/element_cache_configuration.py` & `PyWebUIFramework-2.6/src/core/configurations/element_cache_configuration.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/configurations/interfaces/browser_profile_interface.py` & `PyWebUIFramework-2.6/src/core/configurations/interfaces/browser_profile_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/configurations/interfaces/retry_configuration_interface.py` & `PyWebUIFramework-2.6/src/core/configurations/interfaces/retry_configuration_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/configurations/interfaces/timeout_configuration_interface.py` & `PyWebUIFramework-2.6/src/core/configurations/interfaces/timeout_configuration_interface.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,7 +46,15 @@
     @abstractmethod
     def command(self) -> int:
         """Get WebDriver Command timeout.
         :return: Get web driver command timeout as integer.
         :rtype: int.
         """
         pass
+
+    @property
+    @abstractmethod
+    def page_load(self) -> int:
+        """Get the default timeout for page loading.
+        :return: Get timeout for page load
+        :rtype: int
+        """
```

### Comparing `PyWebUIFramework-2.5/src/core/configurations/retry_configuration.py` & `PyWebUIFramework-2.6/src/core/configurations/retry_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from core.configurations.interfaces.retry_configuration_interface import IRetryConfiguration
 
 
 class RetryConfiguration(IRetryConfiguration):
     @inject
     def __init__(self, settings_file: ISettingsFile):
         self._settings_file = settings_file
-        
+
     @property
     def number(self) -> int:
         """Get the number of attempts to retry.
         :return: Number or attempts.
         :rtype: int.
         """
         return int(self._settings_file.get_value('retry.number'))
```

### Comparing `PyWebUIFramework-2.5/src/core/configurations/timeout_configuration.py` & `PyWebUIFramework-2.6/src/core/configurations/timeout_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from core.utilities.interfaces.settings_file_interface import ISettingsFile
 from core.configurations.interfaces.timeout_configuration_interface import ITimeoutConfiguration
 
 
 class TimeoutConfigurationCore(ITimeoutConfiguration):
     """Core class for setting timeouts."""
-    
     @inject
     def __init__(self, settings_file: ISettingsFile):
         """Provides a SettingsFile to select the required configuration settings."""
         self._settings_file = settings_file
 
     @property
     def implicit(self) -> int:
@@ -27,8 +26,7 @@
         """Get ConditionalWait polling interval."""
         return self._get_config_value("timeouts.timeoutPollingInterval")
 
     @property
     def command(self) -> int:
         """Get WebDriver Command timeout."""
         return self._get_config_value("timeouts.timeoutCommand")
-
```

### Comparing `PyWebUIFramework-2.5/src/core/elements/actions/js_actions.py` & `PyWebUIFramework-2.6/src/core/elements/actions/js_actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import typing as ty
 
-from browser.browser import Browser
 from browser.java_script import JavaScript
 from core.elements.highlight_state import HighlightState
+from core.applications.interfaces.application_interface import IApplication
 from core.utilities.interfaces.action_repeater_interface import IActionRepeater
 from core.localization.loggers.interfaces.localized_logger_interface import ILocalizedLogger
 from core.elements.states.element_state import Displayed, ExistsInAnyState
 from core.elements.base_parent_element import BaseParentElement
 
 T = ty.TypeVar('T')
+TBrowser = ty.TypeVar("TBrowser", bound=IApplication)
 
 
 class JsActions:
     def __init__(self, element: BaseParentElement, element_type: ty.Type[ty.Union[Displayed, ExistsInAnyState]],
-                 localized_logger: ILocalizedLogger, action_repeater: IActionRepeater, browser: Browser):
+                 localized_logger: ILocalizedLogger, action_repeater: IActionRepeater, browser: TBrowser):
         self.__element = element.get_element()
         self.__element_type = element_type
         self.__name = element.name
         self.__localized_logger = localized_logger
         self.__action_repeater = action_repeater
         self.__browser = browser
 
     def highlight_element(self, highlight_state: HighlightState = HighlightState.DEFAULT):
-        if (self.__browser.browser_profile.is_element_highlight_enabled or
-                highlight_state.value == HighlightState.HIGHLIGHT.value):
+        if any([self.__browser.browser_profile.is_element_highlight_enabled,
+                highlight_state.value == HighlightState.HIGHLIGHT.value]):
             self.__execute_script(JavaScript.BORDER_ELEMENT.get_script(), self.__element)
 
     def click(self) -> None:
         """Clicking on an item with JS."""
         self.__log_element_action('loc.clicking.js')
         self.__execute_script(JavaScript.CLICK_ELEMENT.get_script(), self.__element)
 
@@ -56,8 +57,7 @@
 
     def __log_element_action(self, message_key, *args):
         """Log action on an element.
         :param message_key: Key in resource file.
         :param args: Arguments, which will be provided to template of localized message.
         """
         return self.__localized_logger.info_element_action(self.__element_type, self.__name, message_key, *args)
-
```

### Comparing `PyWebUIFramework-2.5/src/core/elements/base_element.py` & `PyWebUIFramework-2.6/src/core/elements/base_element.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/elements/base_element_cache_handler.py` & `PyWebUIFramework-2.6/src/core/elements/base_element_cache_handler.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/elements/base_element_factory.py` & `PyWebUIFramework-2.6/src/core/elements/base_element_factory.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/elements/base_parent_element.py` & `PyWebUIFramework-2.6/src/core/elements/base_parent_element.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/elements/element_cache_handler.py` & `PyWebUIFramework-2.6/src/core/elements/element_cache_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,7 @@
         :param custom_state: Element custom state.
         :return: Cached element.
         :rtype: WebElement.
         """
         if self.is_refresh_needed(custom_state):
             self.__remote_element = self.__element_finder.find_element(self._locator, self._state, timeout)
         return self.__remote_element
-
```

### Comparing `PyWebUIFramework-2.5/src/core/elements/element_factory.py` & `PyWebUIFramework-2.6/src/core/elements/element_factory.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/elements/element_finder.py` & `PyWebUIFramework-2.6/src/core/elements/element_finder.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/elements/element_finder_interface.py` & `PyWebUIFramework-2.6/src/core/elements/element_finder_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/elements/states/base_element_state_provider.py` & `PyWebUIFramework-2.6/src/core/elements/states/base_element_state_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,8 +107,7 @@
     def wait_for_clickable(self, timeout: int = 0) -> None:
         """
         Wait for element to become clickable which means element is displayed and enabled.
         :param timeout: Timeout for waiting. Default value is taken from TimeoutConfiguration.
         :raises: WebDriverTimeoutException when timeout exceeded and element is not clickable.
         """
         pass
-
```

### Comparing `PyWebUIFramework-2.5/src/core/elements/states/cached_element_state_provider.py` & `PyWebUIFramework-2.6/src/core/elements/states/cached_element_state_provider.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/elements/states/desired_state.py` & `PyWebUIFramework-2.6/src/core/elements/states/desired_state.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/elements/states/element_state.py` & `PyWebUIFramework-2.6/src/core/elements/states/element_state.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/elements/states/element_state_provider.py` & `PyWebUIFramework-2.6/src/core/elements/states/element_state_provider.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/localization/configurations/interfaces/logger_configuration_interface.py` & `PyWebUIFramework-2.6/src/core/localization/configurations/interfaces/logger_configuration_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/localization/configurations/logger_configuration.py` & `PyWebUIFramework-2.6/src/core/localization/configurations/logger_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,7 @@
     @property
     def log_page_source(self) -> bool:
         """Perform page source logging in case of catastrophic failures or not.
         :return: Perform page source or not.
         :rtype: bool.
         """
         return bool(self._settings_file.get_value_or_default('logger.logPageSource', True))
-
```

### Comparing `PyWebUIFramework-2.5/src/core/localization/localization_module.py` & `PyWebUIFramework-2.6/src/core/localization/localization_module.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/localization/loggers/interfaces/localized_logger_interface.py` & `PyWebUIFramework-2.6/src/core/localization/loggers/interfaces/localized_logger_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/localization/loggers/localized_logger.py` & `PyWebUIFramework-2.6/src/core/localization/loggers/localized_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     @inject
     def __init__(self, localization_manager: ILocalizationManager, logger: Logger,
                  configuration: ILoggerConfiguration) -> None:
         """Initialize with localization manager and logger."""
         self._localization_manager = localization_manager
         self._configuration = configuration
         self._logger = logger
-    
+
     def __localize_message(self, message_key: str, *message_args) -> str:
         """Get localization message from json file.
         :param message_key: Key in resource file.
         :param message_args: Arguments, which will be provided to template of localized message.
         :return: Required message for logging.
         :rtype: str.
         """
@@ -71,8 +71,7 @@
     def fatal(self, message, *message_args, **logger_kwargs) -> None:
         """Log message with level fatal.
         :param message: Message from resource file.
         :param message_args: Additional arguments for message.
         :param logger_kwargs: Additional arguments for logger.
         """
         self._logger.fatal(self.__localize_message(message, *message_args))
-
```

### Comparing `PyWebUIFramework-2.5/src/core/localization/managers/localization_manager.py` & `PyWebUIFramework-2.6/src/core/localization/managers/localization_manager.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/resources/localization/be.json` & `PyWebUIFramework-2.6/src/core/resources/localization/be.json`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/resources/localization/en.json` & `PyWebUIFramework-2.6/src/core/resources/localization/en.json`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/resources/localization/ru.json` & `PyWebUIFramework-2.6/src/core/resources/localization/ru.json`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/resources/settings.json` & `PyWebUIFramework-2.6/src/core/resources/settings.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9953703703703702%*

 * *Differences: {"'timeouts'": "{'timeoutImplicit': 10}"}*

```diff
@@ -63,13 +63,13 @@
     "retry": {
         "number": 2,
         "pollingInterval": 11
     },
     "timeouts": {
         "timeoutCommand": 120,
         "timeoutCondition": 30,
-        "timeoutImplicit": 0,
+        "timeoutImplicit": 10,
         "timeoutPageLoad": 15,
         "timeoutPollingInterval": 300,
         "timeoutScript": 10
     }
 }
```

### Comparing `PyWebUIFramework-2.5/src/core/utilities/action_repeater.py` & `PyWebUIFramework-2.6/src/core/utilities/action_repeater.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class ActionRepeater(IActionRepeater):
     @inject
     def __init__(self, retry_configuration: IRetryConfiguration):
         """Initialize repeater with configuration."""
         self._retry_configuration = retry_configuration
-        
+
     def do_with_retry(self, function: ty.Callable[..., T], handled_exceptions: ty.List[ty.Type[Exception]] = []) -> T:
         """
         Try to execute function repeatedly.
         :param function: Function to retry.
         :param handled_exceptions: Exceptions which will be catches during function execution.
         :return: Result of executed function.
         """
```

### Comparing `PyWebUIFramework-2.5/src/core/utilities/interfaces/action_repeater_interface.py` & `PyWebUIFramework-2.6/src/core/utilities/interfaces/action_repeater_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/utilities/interfaces/settings_file_interface.py` & `PyWebUIFramework-2.6/src/core/utilities/interfaces/settings_file_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/utilities/json_settings_file.py` & `PyWebUIFramework-2.6/src/core/utilities/json_settings_file.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/utilities/resource_file.py` & `PyWebUIFramework-2.6/src/core/utilities/resource_file.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/waitings/conditional_wait.py` & `PyWebUIFramework-2.6/src/core/waitings/conditional_wait.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/core/waitings/interfaces/conditional_wait_interface.py` & `PyWebUIFramework-2.6/src/core/waitings/interfaces/conditional_wait_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/elements/check_box.py` & `PyWebUIFramework-2.6/src/elements/check_box.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/elements/element_factory.py` & `PyWebUIFramework-2.6/src/elements/element_factory.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/elements/text_box.py` & `PyWebUIFramework-2.6/src/elements/text_box.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.5/src/forms/base_form.py` & `PyWebUIFramework-2.6/src/forms/base_form.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,43 +2,38 @@
 from abc import ABC
 
 from selenium.webdriver.common.by import By
 from browser.py_quality_services import PyQualityServices
 
 
 class BaseForm(ABC):
+    _element_factory = PyQualityServices.element_factory
+    _localized_logger = PyQualityServices.localized_logger
+
     def __init__(self, locator: ty.Tuple[By, str], name: str):
         self._locator = locator
         self._name = name
 
     @property
     def locator(self) -> ty.Tuple[By, str]:
         return self._locator
 
     @property
     def name(self) -> str:
         return self._name
 
     def _get_form_label(self):
-        return PyQualityServices.get_element_factory().get_label(self.locator, self.name)
+        return self._element_factory.get_label(self.locator, self.name)
 
     @property
     def state(self):
         return self._get_form_label().state
 
     def is_displayed(self):
         return self.state.wait_for_displayed()
 
     def scroll_by(self, x: int, y: int):
         self._get_form_label().js_action.scroll_by(x, y)
 
     @property
     def size(self):
         return self._get_form_label().get_element().size
-
-    @classmethod
-    def _get_element_factory(cls):
-        return PyQualityServices.get_element_factory()
-
-    @classmethod
-    def _get_localized_logger(cls):
-        return PyQualityServices.get_localized_logger()
```

