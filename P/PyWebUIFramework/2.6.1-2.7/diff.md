# Comparing `tmp/PyWebUIFramework-2.6.1.tar.gz` & `tmp/PyWebUIFramework-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyWebUIFramework-2.6.1.tar", last modified: Wed Jun 14 17:26:33 2023, max compression
+gzip compressed data, was "dist\PyWebUIFramework-2.7.tar", last modified: Wed Jun 14 17:28:13 2023, max compression
```

## Comparing `PyWebUIFramework-2.6.1.tar` & `PyWebUIFramework-2.7.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/
--rw-rw-rw-   0        0        0       38 2023-06-13 22:20:29.000000 PyWebUIFramework-2.6.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4355 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     3222 2023-06-13 22:15:22.000000 PyWebUIFramework-2.6.1/README.md
--rw-rw-rw-   0        0        0      115 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1397 2023-06-14 17:26:31.000000 PyWebUIFramework-2.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/PyWebUIFramework.egg-info/
--rw-rw-rw-   0        0        0     4355 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/PyWebUIFramework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4824 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/PyWebUIFramework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/PyWebUIFramework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      198 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/PyWebUIFramework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/PyWebUIFramework.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/browser/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/browser/__init__.py
--rw-rw-rw-   0        0        0      140 2023-06-07 13:55:32.000000 PyWebUIFramework-2.6.1/src/browser/alert_actions.py
--rw-rw-rw-   0        0        0     2152 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6.1/src/browser/base_browser_factory.py
--rw-rw-rw-   0        0        0     8174 2023-06-10 12:55:40.000000 PyWebUIFramework-2.6.1/src/browser/browser.py
--rw-rw-rw-   0        0        0     1123 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6.1/src/browser/browser_module.py
--rw-rw-rw-   0        0        0      200 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/browser/browser_name.py
--rw-rw-rw-   0        0        0     3121 2023-06-01 18:36:29.000000 PyWebUIFramework-2.6.1/src/browser/browser_tab_navigation.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/browser/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/browser/interfaces/__init__.py
--rw-rw-rw-   0        0        0      563 2023-06-07 13:56:57.000000 PyWebUIFramework-2.6.1/src/browser/interfaces/browser_factory_interface.py
--rw-rw-rw-   0        0        0      778 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6.1/src/browser/java_script.py
--rw-rw-rw-   0        0        0     2621 2023-06-02 19:04:26.000000 PyWebUIFramework-2.6.1/src/browser/local_browser_factory.py
--rw-rw-rw-   0        0        0     5002 2023-06-07 14:03:45.000000 PyWebUIFramework-2.6.1/src/browser/py_quality_services.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/configuration/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/configuration/__init__.py
--rw-rw-rw-   0        0        0     2859 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6.1/src/configuration/browser_profile.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/configuration/driver_settings/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/configuration/driver_settings/__init__.py
--rw-rw-rw-   0        0        0     4307 2023-06-01 18:27:00.000000 PyWebUIFramework-2.6.1/src/configuration/driver_settings/base_driver_settings.py
--rw-rw-rw-   0        0        0      968 2023-06-01 18:27:00.000000 PyWebUIFramework-2.6.1/src/configuration/driver_settings/chrome_settings.py
--rw-rw-rw-   0        0        0     1022 2023-06-01 18:27:00.000000 PyWebUIFramework-2.6.1/src/configuration/driver_settings/edge_settings.py
--rw-rw-rw-   0        0        0     1032 2023-06-01 18:27:00.000000 PyWebUIFramework-2.6.1/src/configuration/driver_settings/firefox_settings.py
--rw-rw-rw-   0        0        0      736 2023-06-01 18:27:00.000000 PyWebUIFramework-2.6.1/src/configuration/driver_settings/iexplorer_settings.py
--rw-rw-rw-   0        0        0      142 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/configuration/timeout.py
--rw-rw-rw-   0        0        0     1388 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6.1/src/configuration/timeout_configuration.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/core/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/core/applications/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/applications/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/core/applications/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/applications/interfaces/__init__.py
--rw-rw-rw-   0        0        0      331 2023-06-07 13:19:23.000000 PyWebUIFramework-2.6.1/src/core/applications/interfaces/application_interface.py
--rw-rw-rw-   0        0        0     3301 2023-06-01 18:27:00.000000 PyWebUIFramework-2.6.1/src/core/applications/quality_module.py
--rw-rw-rw-   0        0        0     2255 2023-06-07 12:34:08.000000 PyWebUIFramework-2.6.1/src/core/applications/quality_services.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/core/configurations/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/configurations/__init__.py
--rw-rw-rw-   0        0        0     1587 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6.1/src/core/configurations/configuration_module.py
--rw-rw-rw-   0        0        0      526 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6.1/src/core/configurations/element_cache_configuration.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/core/configurations/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/configurations/interfaces/__init__.py
--rw-rw-rw-   0        0        0     1681 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6.1/src/core/configurations/interfaces/browser_profile_interface.py
--rw-rw-rw-   0        0        0      549 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/configurations/interfaces/retry_configuration_interface.py
--rw-rw-rw-   0        0        0     1667 2023-06-10 12:45:38.000000 PyWebUIFramework-2.6.1/src/core/configurations/interfaces/timeout_configuration_interface.py
--rw-rw-rw-   0        0        0      874 2023-06-07 13:58:03.000000 PyWebUIFramework-2.6.1/src/core/configurations/retry_configuration.py
--rw-rw-rw-   0        0        0     1190 2023-06-07 13:56:36.000000 PyWebUIFramework-2.6.1/src/core/configurations/timeout_configuration.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/core/elements/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/elements/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/core/elements/actions/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/elements/actions/__init__.py
--rw-rw-rw-   0        0        0     2906 2023-06-10 12:57:02.000000 PyWebUIFramework-2.6.1/src/core/elements/actions/js_actions.py
--rw-rw-rw-   0        0        0    11790 2023-06-07 13:03:03.000000 PyWebUIFramework-2.6.1/src/core/elements/base_element.py
--rw-rw-rw-   0        0        0     1866 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6.1/src/core/elements/base_element_cache_handler.py
--rw-rw-rw-   0        0        0     5701 2023-06-07 13:03:03.000000 PyWebUIFramework-2.6.1/src/core/elements/base_element_factory.py
--rw-rw-rw-   0        0        0     2566 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6.1/src/core/elements/base_parent_element.py
--rw-rw-rw-   0        0        0      795 2023-06-07 13:55:20.000000 PyWebUIFramework-2.6.1/src/core/elements/element_cache_handler.py
--rw-rw-rw-   0        0        0     8552 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6.1/src/core/elements/element_factory.py
--rw-rw-rw-   0        0        0     3985 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6.1/src/core/elements/element_finder.py
--rw-rw-rw-   0        0        0     2504 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6.1/src/core/elements/element_finder_interface.py
--rw-rw-rw-   0        0        0      147 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/elements/highlight_state.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/core/elements/states/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/elements/states/__init__.py
--rw-rw-rw-   0        0        0     4304 2023-06-07 13:55:13.000000 PyWebUIFramework-2.6.1/src/core/elements/states/base_element_state_provider.py
--rw-rw-rw-   0        0        0     6787 2023-06-01 18:36:29.000000 PyWebUIFramework-2.6.1/src/core/elements/states/cached_element_state_provider.py
--rw-rw-rw-   0        0        0     1008 2023-06-01 18:36:29.000000 PyWebUIFramework-2.6.1/src/core/elements/states/desired_state.py
--rw-rw-rw-   0        0        0      105 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/elements/states/element_count.py
--rw-rw-rw-   0        0        0      614 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/elements/states/element_state.py
--rw-rw-rw-   0        0        0     2720 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6.1/src/core/elements/states/element_state_provider.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/core/localization/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/localization/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/core/localization/configurations/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/localization/configurations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/core/localization/configurations/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/localization/configurations/interfaces/__init__.py
--rw-rw-rw-   0        0        0      559 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/localization/configurations/interfaces/logger_configuration_interface.py
--rw-rw-rw-   0        0        0      989 2023-06-07 13:55:09.000000 PyWebUIFramework-2.6.1/src/core/localization/configurations/logger_configuration.py
--rw-rw-rw-   0        0        0      921 2023-06-01 18:36:29.000000 PyWebUIFramework-2.6.1/src/core/localization/localization_module.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/core/localization/loggers/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/localization/loggers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/core/localization/loggers/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/localization/loggers/interfaces/__init__.py
--rw-rw-rw-   0        0        0     3696 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6.1/src/core/localization/loggers/interfaces/localized_logger_interface.py
--rw-rw-rw-   0        0        0     3889 2023-06-07 13:54:24.000000 PyWebUIFramework-2.6.1/src/core/localization/loggers/localized_logger.py
--rw-rw-rw-   0        0        0      332 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/localization/loggers/logger_config.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/core/localization/managers/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/localization/managers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/core/localization/managers/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/localization/managers/interfaces/__init__.py
--rw-rw-rw-   0        0        0      508 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/localization/managers/interfaces/localization_interface.py
--rw-rw-rw-   0        0        0     2258 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6.1/src/core/localization/managers/localization_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/core/resources/
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/core/resources/js/
--rw-rw-rw-   0        0        0       42 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6.1/src/core/resources/js/borderElement.js
--rw-rw-rw-   0        0        0       21 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6.1/src/core/resources/js/clickElement.js
--rw-rw-rw-   0        0        0       75 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6.1/src/core/resources/js/getCheckBoxState.js
--rw-rw-rw-   0        0        0       31 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6.1/src/core/resources/js/getElementText.js
--rw-rw-rw-   0        0        0       26 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6.1/src/core/resources/js/openInNewTab.js
--rw-rw-rw-   0        0        0       14 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6.1/src/core/resources/js/openNewTab.js
--rw-rw-rw-   0        0        0       73 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6.1/src/core/resources/js/pageLoaded.js
--rw-rw-rw-   0        0        0       48 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6.1/src/core/resources/js/scrollBy.js
--rw-rw-rw-   0        0        0       42 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6.1/src/core/resources/js/scrollWindowBy.js
--rw-rw-rw-   0        0        0       31 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6.1/src/core/resources/js/setValue.js
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/core/resources/localization/
--rw-rw-rw-   0        0        0     6717 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6.1/src/core/resources/localization/be.json
--rw-rw-rw-   0        0        0     4495 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6.1/src/core/resources/localization/en.json
--rw-rw-rw-   0        0        0     6771 2023-06-02 16:56:53.000000 PyWebUIFramework-2.6.1/src/core/resources/localization/ru.json
--rw-rw-rw-   0        0        0     2445 2023-06-10 12:57:35.000000 PyWebUIFramework-2.6.1/src/core/resources/settings.json
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/core/utilities/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/utilities/__init__.py
--rw-rw-rw-   0        0        0     1675 2023-06-07 13:56:12.000000 PyWebUIFramework-2.6.1/src/core/utilities/action_repeater.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/core/utilities/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/utilities/interfaces/__init__.py
--rw-rw-rw-   0        0        0      571 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/utilities/interfaces/action_repeater_interface.py
--rw-rw-rw-   0        0        0     1619 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/utilities/interfaces/settings_file_interface.py
--rw-rw-rw-   0        0        0     3387 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6.1/src/core/utilities/json_settings_file.py
--rw-rw-rw-   0        0        0     3034 2023-06-02 17:00:05.000000 PyWebUIFramework-2.6.1/src/core/utilities/resource_file.py
--rw-rw-rw-   0        0        0      391 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6.1/src/core/utilities/utilities_module.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/core/waitings/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/waitings/__init__.py
--rw-rw-rw-   0        0        0     5521 2023-06-07 13:03:39.000000 PyWebUIFramework-2.6.1/src/core/waitings/conditional_wait.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/core/waitings/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/waitings/interfaces/__init__.py
--rw-rw-rw-   0        0        0     2722 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/core/waitings/interfaces/conditional_wait_interface.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/elements/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/elements/__init__.py
--rw-rw-rw-   0        0        0      222 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/elements/attributes.py
--rw-rw-rw-   0        0        0      215 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6.1/src/elements/button.py
--rw-rw-rw-   0        0        0      516 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6.1/src/elements/check_box.py
--rw-rw-rw-   0        0        0      436 2023-06-01 18:36:29.000000 PyWebUIFramework-2.6.1/src/elements/checkable_element.py
--rw-rw-rw-   0        0        0      297 2023-06-07 13:55:00.000000 PyWebUIFramework-2.6.1/src/elements/combo_box.py
--rw-rw-rw-   0        0        0     1694 2023-06-01 18:36:29.000000 PyWebUIFramework-2.6.1/src/elements/element_factory.py
--rw-rw-rw-   0        0        0      213 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6.1/src/elements/label.py
--rw-rw-rw-   0        0        0      292 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6.1/src/elements/link.py
--rw-rw-rw-   0        0        0      229 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6.1/src/elements/radio_button.py
--rw-rw-rw-   0        0        0     1780 2023-06-01 18:36:30.000000 PyWebUIFramework-2.6.1/src/elements/text_box.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:26:33.000000 PyWebUIFramework-2.6.1/src/forms/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.6.1/src/forms/__init__.py
--rw-rw-rw-   0        0        0     1050 2023-06-10 13:04:02.000000 PyWebUIFramework-2.6.1/src/forms/base_form.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/
+-rw-rw-rw-   0        0        0       38 2023-06-13 22:20:29.000000 PyWebUIFramework-2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4353 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3222 2023-06-13 22:15:22.000000 PyWebUIFramework-2.7/README.md
+-rw-rw-rw-   0        0        0      115 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1395 2023-06-14 17:27:15.000000 PyWebUIFramework-2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/PyWebUIFramework.egg-info/
+-rw-rw-rw-   0        0        0     4353 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/PyWebUIFramework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4824 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/PyWebUIFramework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/PyWebUIFramework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      198 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/PyWebUIFramework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/PyWebUIFramework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/browser/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/browser/__init__.py
+-rw-rw-rw-   0        0        0      140 2023-06-07 13:55:32.000000 PyWebUIFramework-2.7/src/browser/alert_actions.py
+-rw-rw-rw-   0        0        0     2152 2023-06-01 18:36:30.000000 PyWebUIFramework-2.7/src/browser/base_browser_factory.py
+-rw-rw-rw-   0        0        0     8174 2023-06-10 12:55:40.000000 PyWebUIFramework-2.7/src/browser/browser.py
+-rw-rw-rw-   0        0        0     1123 2023-06-01 18:36:30.000000 PyWebUIFramework-2.7/src/browser/browser_module.py
+-rw-rw-rw-   0        0        0      200 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/browser/browser_name.py
+-rw-rw-rw-   0        0        0     3121 2023-06-01 18:36:29.000000 PyWebUIFramework-2.7/src/browser/browser_tab_navigation.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/browser/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/browser/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      563 2023-06-07 13:56:57.000000 PyWebUIFramework-2.7/src/browser/interfaces/browser_factory_interface.py
+-rw-rw-rw-   0        0        0      778 2023-06-01 18:36:30.000000 PyWebUIFramework-2.7/src/browser/java_script.py
+-rw-rw-rw-   0        0        0     2621 2023-06-02 19:04:26.000000 PyWebUIFramework-2.7/src/browser/local_browser_factory.py
+-rw-rw-rw-   0        0        0     5002 2023-06-07 14:03:45.000000 PyWebUIFramework-2.7/src/browser/py_quality_services.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/configuration/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/configuration/__init__.py
+-rw-rw-rw-   0        0        0     2859 2023-06-01 18:36:30.000000 PyWebUIFramework-2.7/src/configuration/browser_profile.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/configuration/driver_settings/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/configuration/driver_settings/__init__.py
+-rw-rw-rw-   0        0        0     4307 2023-06-01 18:27:00.000000 PyWebUIFramework-2.7/src/configuration/driver_settings/base_driver_settings.py
+-rw-rw-rw-   0        0        0      968 2023-06-01 18:27:00.000000 PyWebUIFramework-2.7/src/configuration/driver_settings/chrome_settings.py
+-rw-rw-rw-   0        0        0     1022 2023-06-01 18:27:00.000000 PyWebUIFramework-2.7/src/configuration/driver_settings/edge_settings.py
+-rw-rw-rw-   0        0        0     1032 2023-06-01 18:27:00.000000 PyWebUIFramework-2.7/src/configuration/driver_settings/firefox_settings.py
+-rw-rw-rw-   0        0        0      736 2023-06-01 18:27:00.000000 PyWebUIFramework-2.7/src/configuration/driver_settings/iexplorer_settings.py
+-rw-rw-rw-   0        0        0      142 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/configuration/timeout.py
+-rw-rw-rw-   0        0        0     1388 2023-06-01 18:36:30.000000 PyWebUIFramework-2.7/src/configuration/timeout_configuration.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/core/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/core/applications/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/applications/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/core/applications/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/applications/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      331 2023-06-07 13:19:23.000000 PyWebUIFramework-2.7/src/core/applications/interfaces/application_interface.py
+-rw-rw-rw-   0        0        0     3301 2023-06-01 18:27:00.000000 PyWebUIFramework-2.7/src/core/applications/quality_module.py
+-rw-rw-rw-   0        0        0     2255 2023-06-07 12:34:08.000000 PyWebUIFramework-2.7/src/core/applications/quality_services.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/core/configurations/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/configurations/__init__.py
+-rw-rw-rw-   0        0        0     1587 2023-06-01 18:36:30.000000 PyWebUIFramework-2.7/src/core/configurations/configuration_module.py
+-rw-rw-rw-   0        0        0      526 2023-06-01 18:36:30.000000 PyWebUIFramework-2.7/src/core/configurations/element_cache_configuration.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/core/configurations/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/configurations/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     1681 2023-06-01 18:36:30.000000 PyWebUIFramework-2.7/src/core/configurations/interfaces/browser_profile_interface.py
+-rw-rw-rw-   0        0        0      549 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/configurations/interfaces/retry_configuration_interface.py
+-rw-rw-rw-   0        0        0     1667 2023-06-10 12:45:38.000000 PyWebUIFramework-2.7/src/core/configurations/interfaces/timeout_configuration_interface.py
+-rw-rw-rw-   0        0        0      874 2023-06-07 13:58:03.000000 PyWebUIFramework-2.7/src/core/configurations/retry_configuration.py
+-rw-rw-rw-   0        0        0     1190 2023-06-07 13:56:36.000000 PyWebUIFramework-2.7/src/core/configurations/timeout_configuration.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/core/elements/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/elements/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/core/elements/actions/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/elements/actions/__init__.py
+-rw-rw-rw-   0        0        0     2906 2023-06-10 12:57:02.000000 PyWebUIFramework-2.7/src/core/elements/actions/js_actions.py
+-rw-rw-rw-   0        0        0    11790 2023-06-07 13:03:03.000000 PyWebUIFramework-2.7/src/core/elements/base_element.py
+-rw-rw-rw-   0        0        0     1866 2023-06-01 18:36:30.000000 PyWebUIFramework-2.7/src/core/elements/base_element_cache_handler.py
+-rw-rw-rw-   0        0        0     5701 2023-06-07 13:03:03.000000 PyWebUIFramework-2.7/src/core/elements/base_element_factory.py
+-rw-rw-rw-   0        0        0     2566 2023-06-01 18:36:30.000000 PyWebUIFramework-2.7/src/core/elements/base_parent_element.py
+-rw-rw-rw-   0        0        0      795 2023-06-07 13:55:20.000000 PyWebUIFramework-2.7/src/core/elements/element_cache_handler.py
+-rw-rw-rw-   0        0        0     8552 2023-06-01 18:36:30.000000 PyWebUIFramework-2.7/src/core/elements/element_factory.py
+-rw-rw-rw-   0        0        0     3985 2023-06-01 18:36:30.000000 PyWebUIFramework-2.7/src/core/elements/element_finder.py
+-rw-rw-rw-   0        0        0     2504 2023-06-01 18:36:30.000000 PyWebUIFramework-2.7/src/core/elements/element_finder_interface.py
+-rw-rw-rw-   0        0        0      147 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/elements/highlight_state.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/core/elements/states/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/elements/states/__init__.py
+-rw-rw-rw-   0        0        0     4304 2023-06-07 13:55:13.000000 PyWebUIFramework-2.7/src/core/elements/states/base_element_state_provider.py
+-rw-rw-rw-   0        0        0     6787 2023-06-01 18:36:29.000000 PyWebUIFramework-2.7/src/core/elements/states/cached_element_state_provider.py
+-rw-rw-rw-   0        0        0     1008 2023-06-01 18:36:29.000000 PyWebUIFramework-2.7/src/core/elements/states/desired_state.py
+-rw-rw-rw-   0        0        0      105 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/elements/states/element_count.py
+-rw-rw-rw-   0        0        0      614 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/elements/states/element_state.py
+-rw-rw-rw-   0        0        0     2720 2023-06-01 18:36:30.000000 PyWebUIFramework-2.7/src/core/elements/states/element_state_provider.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/core/localization/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/localization/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/core/localization/configurations/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/localization/configurations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/core/localization/configurations/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/localization/configurations/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      559 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/localization/configurations/interfaces/logger_configuration_interface.py
+-rw-rw-rw-   0        0        0      989 2023-06-07 13:55:09.000000 PyWebUIFramework-2.7/src/core/localization/configurations/logger_configuration.py
+-rw-rw-rw-   0        0        0      921 2023-06-01 18:36:29.000000 PyWebUIFramework-2.7/src/core/localization/localization_module.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/core/localization/loggers/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/localization/loggers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/core/localization/loggers/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/localization/loggers/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     3696 2023-06-01 18:36:30.000000 PyWebUIFramework-2.7/src/core/localization/loggers/interfaces/localized_logger_interface.py
+-rw-rw-rw-   0        0        0     3889 2023-06-07 13:54:24.000000 PyWebUIFramework-2.7/src/core/localization/loggers/localized_logger.py
+-rw-rw-rw-   0        0        0      332 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/localization/loggers/logger_config.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/core/localization/managers/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/localization/managers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/core/localization/managers/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/localization/managers/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/localization/managers/interfaces/localization_interface.py
+-rw-rw-rw-   0        0        0     2258 2023-06-01 18:36:30.000000 PyWebUIFramework-2.7/src/core/localization/managers/localization_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/core/resources/
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/core/resources/js/
+-rw-rw-rw-   0        0        0       42 2023-06-02 16:56:53.000000 PyWebUIFramework-2.7/src/core/resources/js/borderElement.js
+-rw-rw-rw-   0        0        0       21 2023-06-02 16:56:53.000000 PyWebUIFramework-2.7/src/core/resources/js/clickElement.js
+-rw-rw-rw-   0        0        0       75 2023-06-02 16:56:53.000000 PyWebUIFramework-2.7/src/core/resources/js/getCheckBoxState.js
+-rw-rw-rw-   0        0        0       31 2023-06-02 16:56:53.000000 PyWebUIFramework-2.7/src/core/resources/js/getElementText.js
+-rw-rw-rw-   0        0        0       26 2023-06-02 16:56:53.000000 PyWebUIFramework-2.7/src/core/resources/js/openInNewTab.js
+-rw-rw-rw-   0        0        0       14 2023-06-02 16:56:53.000000 PyWebUIFramework-2.7/src/core/resources/js/openNewTab.js
+-rw-rw-rw-   0        0        0       73 2023-06-02 16:56:53.000000 PyWebUIFramework-2.7/src/core/resources/js/pageLoaded.js
+-rw-rw-rw-   0        0        0       48 2023-06-02 16:56:53.000000 PyWebUIFramework-2.7/src/core/resources/js/scrollBy.js
+-rw-rw-rw-   0        0        0       42 2023-06-02 16:56:53.000000 PyWebUIFramework-2.7/src/core/resources/js/scrollWindowBy.js
+-rw-rw-rw-   0        0        0       31 2023-06-02 16:56:53.000000 PyWebUIFramework-2.7/src/core/resources/js/setValue.js
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/core/resources/localization/
+-rw-rw-rw-   0        0        0     6717 2023-06-02 16:56:53.000000 PyWebUIFramework-2.7/src/core/resources/localization/be.json
+-rw-rw-rw-   0        0        0     4495 2023-06-02 16:56:53.000000 PyWebUIFramework-2.7/src/core/resources/localization/en.json
+-rw-rw-rw-   0        0        0     6771 2023-06-02 16:56:53.000000 PyWebUIFramework-2.7/src/core/resources/localization/ru.json
+-rw-rw-rw-   0        0        0     2445 2023-06-10 12:57:35.000000 PyWebUIFramework-2.7/src/core/resources/settings.json
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/core/utilities/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1675 2023-06-07 13:56:12.000000 PyWebUIFramework-2.7/src/core/utilities/action_repeater.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/core/utilities/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/utilities/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      571 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/utilities/interfaces/action_repeater_interface.py
+-rw-rw-rw-   0        0        0     1619 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/utilities/interfaces/settings_file_interface.py
+-rw-rw-rw-   0        0        0     3387 2023-06-01 18:36:30.000000 PyWebUIFramework-2.7/src/core/utilities/json_settings_file.py
+-rw-rw-rw-   0        0        0     3034 2023-06-02 17:00:05.000000 PyWebUIFramework-2.7/src/core/utilities/resource_file.py
+-rw-rw-rw-   0        0        0      391 2023-06-01 18:36:30.000000 PyWebUIFramework-2.7/src/core/utilities/utilities_module.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/core/waitings/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/waitings/__init__.py
+-rw-rw-rw-   0        0        0     5521 2023-06-07 13:03:39.000000 PyWebUIFramework-2.7/src/core/waitings/conditional_wait.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/core/waitings/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/waitings/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     2722 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/core/waitings/interfaces/conditional_wait_interface.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/elements/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/elements/__init__.py
+-rw-rw-rw-   0        0        0      222 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/elements/attributes.py
+-rw-rw-rw-   0        0        0      215 2023-06-01 18:36:30.000000 PyWebUIFramework-2.7/src/elements/button.py
+-rw-rw-rw-   0        0        0      516 2023-06-01 18:36:30.000000 PyWebUIFramework-2.7/src/elements/check_box.py
+-rw-rw-rw-   0        0        0      436 2023-06-01 18:36:29.000000 PyWebUIFramework-2.7/src/elements/checkable_element.py
+-rw-rw-rw-   0        0        0      297 2023-06-07 13:55:00.000000 PyWebUIFramework-2.7/src/elements/combo_box.py
+-rw-rw-rw-   0        0        0     1694 2023-06-01 18:36:29.000000 PyWebUIFramework-2.7/src/elements/element_factory.py
+-rw-rw-rw-   0        0        0      213 2023-06-01 18:36:30.000000 PyWebUIFramework-2.7/src/elements/label.py
+-rw-rw-rw-   0        0        0      292 2023-06-01 18:36:30.000000 PyWebUIFramework-2.7/src/elements/link.py
+-rw-rw-rw-   0        0        0      229 2023-06-01 18:36:30.000000 PyWebUIFramework-2.7/src/elements/radio_button.py
+-rw-rw-rw-   0        0        0     1780 2023-06-01 18:36:30.000000 PyWebUIFramework-2.7/src/elements/text_box.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:28:13.000000 PyWebUIFramework-2.7/src/forms/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-2.7/src/forms/__init__.py
+-rw-rw-rw-   0        0        0     1050 2023-06-10 13:04:02.000000 PyWebUIFramework-2.7/src/forms/base_form.py
```

### Comparing `PyWebUIFramework-2.6.1/PKG-INFO` & `PyWebUIFramework-2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyWebUIFramework
-Version: 2.6.1
+Version: 2.7
 Summary: UNKNOWN
 Home-page: https://github.com/philip136/PyWebUIFramework
 Author: Philip Vasilevsky
 Author-email: fil13698@gmail.com
 License: MIT
 Description: # PyWebUIFramework
         This framework is needed for simple work with Selenium.
```

### Comparing `PyWebUIFramework-2.6.1/README.md` & `PyWebUIFramework-2.7/README.md`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/setup.py` & `PyWebUIFramework-2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # PATH VARIABLES
 SOURCE_NAME = "src"
 FRAMEWORK_NAME = "PyWebUIFramework"
 PATH_TO_RESOURCES = os.path.join(SOURCE_NAME, "core", "resources.*")
 
 # PROJECT VARIABLES
-CURRENT_VERSION = "2.6.1"
+CURRENT_VERSION = "2.7"
 LICENSE_TYPE = "MIT"
 
 # AUTHOR VARIABLES
 AUTHOR_FULL_NAME = "Philip Vasilevsky"
 AUTHOR_EMAIL = "fil13698@gmail.com"
 LINK_TO_REPO = "https://github.com/philip136/PyWebUIFramework"
```

### Comparing `PyWebUIFramework-2.6.1/src/PyWebUIFramework.egg-info/PKG-INFO` & `PyWebUIFramework-2.7/src/PyWebUIFramework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyWebUIFramework
-Version: 2.6.1
+Version: 2.7
 Summary: UNKNOWN
 Home-page: https://github.com/philip136/PyWebUIFramework
 Author: Philip Vasilevsky
 Author-email: fil13698@gmail.com
 License: MIT
 Description: # PyWebUIFramework
         This framework is needed for simple work with Selenium.
```

### Comparing `PyWebUIFramework-2.6.1/src/PyWebUIFramework.egg-info/SOURCES.txt` & `PyWebUIFramework-2.7/src/PyWebUIFramework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/browser/base_browser_factory.py` & `PyWebUIFramework-2.7/src/browser/base_browser_factory.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/browser/browser.py` & `PyWebUIFramework-2.7/src/browser/browser.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/browser/browser_module.py` & `PyWebUIFramework-2.7/src/browser/browser_module.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/browser/browser_tab_navigation.py` & `PyWebUIFramework-2.7/src/browser/browser_tab_navigation.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/browser/interfaces/browser_factory_interface.py` & `PyWebUIFramework-2.7/src/browser/interfaces/browser_factory_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/browser/java_script.py` & `PyWebUIFramework-2.7/src/browser/java_script.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/browser/local_browser_factory.py` & `PyWebUIFramework-2.7/src/browser/local_browser_factory.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/browser/py_quality_services.py` & `PyWebUIFramework-2.7/src/browser/py_quality_services.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/configuration/browser_profile.py` & `PyWebUIFramework-2.7/src/configuration/browser_profile.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/configuration/driver_settings/base_driver_settings.py` & `PyWebUIFramework-2.7/src/configuration/driver_settings/base_driver_settings.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/configuration/driver_settings/chrome_settings.py` & `PyWebUIFramework-2.7/src/configuration/driver_settings/chrome_settings.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/configuration/driver_settings/edge_settings.py` & `PyWebUIFramework-2.7/src/configuration/driver_settings/edge_settings.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/configuration/driver_settings/firefox_settings.py` & `PyWebUIFramework-2.7/src/configuration/driver_settings/firefox_settings.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/configuration/driver_settings/iexplorer_settings.py` & `PyWebUIFramework-2.7/src/configuration/driver_settings/iexplorer_settings.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/configuration/timeout_configuration.py` & `PyWebUIFramework-2.7/src/configuration/timeout_configuration.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/applications/quality_module.py` & `PyWebUIFramework-2.7/src/core/applications/quality_module.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/applications/quality_services.py` & `PyWebUIFramework-2.7/src/core/applications/quality_services.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/configurations/configuration_module.py` & `PyWebUIFramework-2.7/src/core/configurations/configuration_module.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/configurations/element_cache_configuration.py` & `PyWebUIFramework-2.7/src/core/configurations/element_cache_configuration.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/configurations/interfaces/browser_profile_interface.py` & `PyWebUIFramework-2.7/src/core/configurations/interfaces/browser_profile_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/configurations/interfaces/retry_configuration_interface.py` & `PyWebUIFramework-2.7/src/core/configurations/interfaces/retry_configuration_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/configurations/interfaces/timeout_configuration_interface.py` & `PyWebUIFramework-2.7/src/core/configurations/interfaces/timeout_configuration_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/configurations/retry_configuration.py` & `PyWebUIFramework-2.7/src/core/configurations/retry_configuration.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/configurations/timeout_configuration.py` & `PyWebUIFramework-2.7/src/core/configurations/timeout_configuration.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/elements/actions/js_actions.py` & `PyWebUIFramework-2.7/src/core/elements/actions/js_actions.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/elements/base_element.py` & `PyWebUIFramework-2.7/src/core/elements/base_element.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/elements/base_element_cache_handler.py` & `PyWebUIFramework-2.7/src/core/elements/base_element_cache_handler.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/elements/base_element_factory.py` & `PyWebUIFramework-2.7/src/core/elements/base_element_factory.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/elements/base_parent_element.py` & `PyWebUIFramework-2.7/src/core/elements/base_parent_element.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/elements/element_cache_handler.py` & `PyWebUIFramework-2.7/src/core/elements/element_cache_handler.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/elements/element_factory.py` & `PyWebUIFramework-2.7/src/core/elements/element_factory.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/elements/element_finder.py` & `PyWebUIFramework-2.7/src/core/elements/element_finder.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/elements/element_finder_interface.py` & `PyWebUIFramework-2.7/src/core/elements/element_finder_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/elements/states/base_element_state_provider.py` & `PyWebUIFramework-2.7/src/core/elements/states/base_element_state_provider.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/elements/states/cached_element_state_provider.py` & `PyWebUIFramework-2.7/src/core/elements/states/cached_element_state_provider.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/elements/states/desired_state.py` & `PyWebUIFramework-2.7/src/core/elements/states/desired_state.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/elements/states/element_state.py` & `PyWebUIFramework-2.7/src/core/elements/states/element_state.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/elements/states/element_state_provider.py` & `PyWebUIFramework-2.7/src/core/elements/states/element_state_provider.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/localization/configurations/interfaces/logger_configuration_interface.py` & `PyWebUIFramework-2.7/src/core/localization/configurations/interfaces/logger_configuration_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/localization/configurations/logger_configuration.py` & `PyWebUIFramework-2.7/src/core/localization/configurations/logger_configuration.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/localization/localization_module.py` & `PyWebUIFramework-2.7/src/core/localization/localization_module.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/localization/loggers/interfaces/localized_logger_interface.py` & `PyWebUIFramework-2.7/src/core/localization/loggers/interfaces/localized_logger_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/localization/loggers/localized_logger.py` & `PyWebUIFramework-2.7/src/core/localization/loggers/localized_logger.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/localization/managers/localization_manager.py` & `PyWebUIFramework-2.7/src/core/localization/managers/localization_manager.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/resources/localization/be.json` & `PyWebUIFramework-2.7/src/core/resources/localization/be.json`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/resources/localization/en.json` & `PyWebUIFramework-2.7/src/core/resources/localization/en.json`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/resources/localization/ru.json` & `PyWebUIFramework-2.7/src/core/resources/localization/ru.json`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/resources/settings.json` & `PyWebUIFramework-2.7/src/core/resources/settings.json`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/utilities/action_repeater.py` & `PyWebUIFramework-2.7/src/core/utilities/action_repeater.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/utilities/interfaces/action_repeater_interface.py` & `PyWebUIFramework-2.7/src/core/utilities/interfaces/action_repeater_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/utilities/interfaces/settings_file_interface.py` & `PyWebUIFramework-2.7/src/core/utilities/interfaces/settings_file_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/utilities/json_settings_file.py` & `PyWebUIFramework-2.7/src/core/utilities/json_settings_file.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/utilities/resource_file.py` & `PyWebUIFramework-2.7/src/core/utilities/resource_file.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/waitings/conditional_wait.py` & `PyWebUIFramework-2.7/src/core/waitings/conditional_wait.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/core/waitings/interfaces/conditional_wait_interface.py` & `PyWebUIFramework-2.7/src/core/waitings/interfaces/conditional_wait_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/elements/check_box.py` & `PyWebUIFramework-2.7/src/elements/check_box.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/elements/element_factory.py` & `PyWebUIFramework-2.7/src/elements/element_factory.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/elements/text_box.py` & `PyWebUIFramework-2.7/src/elements/text_box.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-2.6.1/src/forms/base_form.py` & `PyWebUIFramework-2.7/src/forms/base_form.py`

 * *Files identical despite different names*

